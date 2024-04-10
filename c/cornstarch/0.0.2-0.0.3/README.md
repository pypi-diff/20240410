# Comparing `tmp/cornstarch-0.0.2.tar.gz` & `tmp/cornstarch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornstarch-0.0.2.tar", last modified: Wed Apr 10 18:54:26 2024, max compression
+gzip compressed data, was "cornstarch-0.0.3.tar", last modified: Wed Apr 10 19:14:20 2024, max compression
```

## Comparing `cornstarch-0.0.2.tar` & `cornstarch-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.921939 cornstarch-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    11338 2024-03-18 14:10:17.000000 cornstarch-0.0.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    14352 2024-04-10 18:54:26.921939 cornstarch-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      426 2024-04-10 18:36:05.000000 cornstarch-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.920939 cornstarch-0.0.2/cornstarch.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14352 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1336 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.917939 cornstarch-0.0.2/oobleck_colossalai/
--rw-r--r--   0 root         (0) root         (0)      273 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2995 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/pipeline_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.918939 cornstarch-0.0.2/oobleck_colossalai/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-04-06 13:53:20.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     3856 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_module.py
--rw-r--r--   0 root         (0) root         (0)    14670 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_plugin.py
--rw-r--r--   0 root         (0) root         (0)    10621 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/process_group_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.918939 cornstarch-0.0.2/oobleck_colossalai/shardformer/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.919939 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/auto_policy.py
--rw-r--r--   0 root         (0) root         (0)    34146 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/bert.py
--rw-r--r--   0 root         (0) root         (0)    23020 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/gpt2.py
--rw-r--r--   0 root         (0) root         (0)    17991 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/llama.py
--rw-r--r--   0 root         (0) root         (0)    17674 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/opt.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-09 13:57:49.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/utils.py
--rw-r--r--   0 root         (0) root         (0)    14129 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/vit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.919939 cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-09 03:13:36.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/placeholder.py
--rw-r--r--   0 root         (0) root         (0)     7144 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/shardformer.py
--rw-r--r--   0 root         (0) root         (0)     5174 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/stage_manager.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-10 18:54:20.000000 cornstarch-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 18:54:26.921939 cornstarch-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.920939 cornstarch-0.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)    12708 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_heterogeneous_parallel_plugin.py
--rw-r--r--   0 root         (0) root         (0)     3496 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_pipeline_template.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_placeholder.py
--rw-r--r--   0 root         (0) root         (0)     8000 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_process_group_mesh.py
--rw-r--r--   0 root         (0) root         (0)    10440 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_stage_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.468966 cornstarch-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)    11338 2024-03-18 14:10:17.000000 cornstarch-0.0.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    14352 2024-04-10 19:14:20.468966 cornstarch-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      426 2024-04-10 18:36:05.000000 cornstarch-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.461966 cornstarch-0.0.3/cornstarch/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-03-18 14:10:17.000000 cornstarch-0.0.3/cornstarch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/pipeline_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.462966 cornstarch-0.0.3/cornstarch/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.3/cornstarch/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-04-06 13:53:20.000000 cornstarch-0.0.3/cornstarch/plugin/heterogeneous_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/plugin/heterogeneous_parallel_module.py
+-rw-r--r--   0 root         (0) root         (0)    14670 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/plugin/heterogeneous_parallel_plugin.py
+-rw-r--r--   0 root         (0) root         (0)    10621 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/process_group_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.462966 cornstarch-0.0.3/cornstarch/shardformer/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.3/cornstarch/shardformer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.463966 cornstarch-0.0.3/cornstarch/shardformer/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/auto_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34146 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/bert.py
+-rw-r--r--   0 root         (0) root         (0)    23020 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/gpt2.py
+-rw-r--r--   0 root         (0) root         (0)    17991 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/llama.py
+-rw-r--r--   0 root         (0) root         (0)    17674 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/opt.py
+-rw-r--r--   0 root         (0) root         (0)     2479 2024-04-10 18:56:32.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/pipeline_template_policy.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-09 13:57:49.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/utils.py
+-rw-r--r--   0 root         (0) root         (0)    14129 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/shardformer/policies/vit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.464966 cornstarch-0.0.3/cornstarch/shardformer/shard/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-09 03:13:36.000000 cornstarch-0.0.3/cornstarch/shardformer/shard/placeholder.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/shardformer/shard/shardformer.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2024-04-10 18:54:02.000000 cornstarch-0.0.3/cornstarch/stage_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.467966 cornstarch-0.0.3/cornstarch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14352 2024-04-10 19:14:20.000000 cornstarch-0.0.3/cornstarch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-04-10 19:14:20.000000 cornstarch-0.0.3/cornstarch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 19:14:20.000000 cornstarch-0.0.3/cornstarch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-10 19:14:20.000000 cornstarch-0.0.3/cornstarch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-10 19:14:20.000000 cornstarch-0.0.3/cornstarch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.460966 cornstarch-0.0.3/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.460966 cornstarch-0.0.3/dist/whl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.464966 cornstarch-0.0.3/dist/whl/oobleck_colossalai/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-03-18 14:10:16.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/pipeline_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.464966 cornstarch-0.0.3/dist/whl/oobleck_colossalai/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:16.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-04-06 13:53:20.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/plugin/heterogeneous_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/plugin/heterogeneous_parallel_module.py
+-rw-r--r--   0 root         (0) root         (0)    14670 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/plugin/heterogeneous_parallel_plugin.py
+-rw-r--r--   0 root         (0) root         (0)    10621 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/process_group_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.465966 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:16.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.466966 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:16.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/auto_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34146 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/bert.py
+-rw-r--r--   0 root         (0) root         (0)    23020 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/gpt2.py
+-rw-r--r--   0 root         (0) root         (0)    17991 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/llama.py
+-rw-r--r--   0 root         (0) root         (0)    17674 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/opt.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-09 13:57:48.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/utils.py
+-rw-r--r--   0 root         (0) root         (0)    14129 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/vit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.466966 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/shard/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-09 03:13:36.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/shard/placeholder.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/shard/shardformer.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2024-04-10 18:54:02.000000 cornstarch-0.0.3/dist/whl/oobleck_colossalai/stage_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.466966 cornstarch-0.0.3/examples/
+-rw-r--r--   0 root         (0) root         (0)     3057 2024-04-10 18:54:02.000000 cornstarch-0.0.3/examples/data_builder.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2024-04-10 18:54:02.000000 cornstarch-0.0.3/examples/run_bert.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2024-04-10 18:54:02.000000 cornstarch-0.0.3/examples/run_gpt2.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2024-04-10 18:54:02.000000 cornstarch-0.0.3/examples/run_llama.py
+-rw-r--r--   0 root         (0) root         (0)     5403 2024-04-10 18:54:02.000000 cornstarch-0.0.3/examples/run_vit.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-10 19:14:12.000000 cornstarch-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 19:14:20.468966 cornstarch-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:14:20.467966 cornstarch-0.0.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     3612 2024-03-18 14:10:17.000000 cornstarch-0.0.3/tests/data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    12708 2024-04-10 18:54:02.000000 cornstarch-0.0.3/tests/test_heterogeneous_parallel_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2024-04-10 18:54:02.000000 cornstarch-0.0.3/tests/test_pipeline_template.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-10 18:54:02.000000 cornstarch-0.0.3/tests/test_placeholder.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2024-04-10 18:54:02.000000 cornstarch-0.0.3/tests/test_process_group_mesh.py
+-rw-r--r--   0 root         (0) root         (0)    10440 2024-04-10 18:54:02.000000 cornstarch-0.0.3/tests/test_stage_manager.py
```

### Comparing `cornstarch-0.0.2/LICENSE.txt` & `cornstarch-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/PKG-INFO` & `cornstarch-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornstarch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A versatile model toolkit for distributed training.
 Author-email: Insu Jang <insujang@umich.edu>
 Maintainer-email: Insu Jang <insujang@umich.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `cornstarch-0.0.2/cornstarch.egg-info/PKG-INFO` & `cornstarch-0.0.3/cornstarch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornstarch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A versatile model toolkit for distributed training.
 Author-email: Insu Jang <insujang@umich.edu>
 Maintainer-email: Insu Jang <insujang@umich.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `cornstarch-0.0.2/oobleck_colossalai/pipeline_template.py` & `cornstarch-0.0.3/cornstarch/pipeline_template.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_dataloader.py` & `cornstarch-0.0.3/cornstarch/plugin/heterogeneous_dataloader.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_module.py` & `cornstarch-0.0.3/cornstarch/plugin/heterogeneous_parallel_module.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_plugin.py` & `cornstarch-0.0.3/cornstarch/plugin/heterogeneous_parallel_plugin.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/process_group_mesh.py` & `cornstarch-0.0.3/cornstarch/process_group_mesh.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/auto_policy.py` & `cornstarch-0.0.3/cornstarch/shardformer/policies/auto_policy.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/bert.py` & `cornstarch-0.0.3/cornstarch/shardformer/policies/bert.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/gpt2.py` & `cornstarch-0.0.3/cornstarch/shardformer/policies/gpt2.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/llama.py` & `cornstarch-0.0.3/cornstarch/shardformer/policies/llama.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/opt.py` & `cornstarch-0.0.3/cornstarch/shardformer/policies/opt.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py` & `cornstarch-0.0.3/dist/whl/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/utils.py` & `cornstarch-0.0.3/cornstarch/shardformer/policies/utils.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/vit.py` & `cornstarch-0.0.3/cornstarch/shardformer/policies/vit.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/placeholder.py` & `cornstarch-0.0.3/cornstarch/shardformer/shard/placeholder.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/shardformer.py` & `cornstarch-0.0.3/cornstarch/shardformer/shard/shardformer.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/oobleck_colossalai/stage_manager.py` & `cornstarch-0.0.3/cornstarch/stage_manager.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/pyproject.toml` & `cornstarch-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "cornstarch"
 description = "A versatile model toolkit for distributed training."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.10"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Insu Jang", email = "insujang@umich.edu"}
 ]
 maintainers = [
     {name = "Insu Jang", email = "insujang@umich.edu"}
 ]
 classifiers = [
@@ -39,8 +39,11 @@
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
 ignore = ["E501"]
 
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where = ["."]
```

### Comparing `cornstarch-0.0.2/tests/test_heterogeneous_parallel_plugin.py` & `cornstarch-0.0.3/tests/test_heterogeneous_parallel_plugin.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/tests/test_pipeline_template.py` & `cornstarch-0.0.3/tests/test_pipeline_template.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/tests/test_placeholder.py` & `cornstarch-0.0.3/tests/test_placeholder.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/tests/test_process_group_mesh.py` & `cornstarch-0.0.3/tests/test_process_group_mesh.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.2/tests/test_stage_manager.py` & `cornstarch-0.0.3/tests/test_stage_manager.py`

 * *Files identical despite different names*

