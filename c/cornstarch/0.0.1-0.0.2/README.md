# Comparing `tmp/cornstarch-0.0.1.tar.gz` & `tmp/cornstarch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornstarch-0.0.1.tar", last modified: Wed Apr 10 18:37:07 2024, max compression
+gzip compressed data, was "cornstarch-0.0.2.tar", last modified: Wed Apr 10 18:54:26 2024, max compression
```

## Comparing `cornstarch-0.0.1.tar` & `cornstarch-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.430623 cornstarch-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    11338 2024-03-18 14:10:17.000000 cornstarch-0.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    13924 2024-04-10 18:37:07.430623 cornstarch-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.429623 cornstarch-0.0.1/cornstarch.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13924 2024-04-10 18:37:07.000000 cornstarch-0.0.1/cornstarch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1326 2024-04-10 18:37:07.000000 cornstarch-0.0.1/cornstarch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 18:37:07.000000 cornstarch-0.0.1/cornstarch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-10 18:37:07.000000 cornstarch-0.0.1/cornstarch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-10 18:37:07.000000 cornstarch-0.0.1/cornstarch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.427623 cornstarch-0.0.1/oobleck_colossalai/
--rw-r--r--   0 root         (0) root         (0)      273 2024-03-18 14:10:17.000000 cornstarch-0.0.1/oobleck_colossalai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3011 2024-04-01 15:33:29.000000 cornstarch-0.0.1/oobleck_colossalai/pipeline_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.427623 cornstarch-0.0.1/oobleck_colossalai/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.1/oobleck_colossalai/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-04-06 13:53:20.000000 cornstarch-0.0.1/oobleck_colossalai/plugin/heterogeneous_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-04-08 04:04:31.000000 cornstarch-0.0.1/oobleck_colossalai/plugin/heterogeneous_parallel_module.py
--rw-r--r--   0 root         (0) root         (0)    14727 2024-04-08 21:16:34.000000 cornstarch-0.0.1/oobleck_colossalai/plugin/heterogeneous_parallel_plugin.py
--rw-r--r--   0 root         (0) root         (0)    10630 2024-04-07 14:44:42.000000 cornstarch-0.0.1/oobleck_colossalai/process_group_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.427623 cornstarch-0.0.1/oobleck_colossalai/shardformer/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.428623 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1414 2024-03-26 21:55:44.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/auto_policy.py
--rw-r--r--   0 root         (0) root         (0)    34171 2024-04-10 15:09:28.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/bert.py
--rw-r--r--   0 root         (0) root         (0)    23045 2024-04-10 15:09:02.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/gpt2.py
--rw-r--r--   0 root         (0) root         (0)    18016 2024-04-10 15:09:39.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/llama.py
--rw-r--r--   0 root         (0) root         (0)    17699 2024-04-10 15:09:46.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/opt.py
--rw-r--r--   0 root         (0) root         (0)     2509 2024-04-09 03:41:03.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-09 13:57:49.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/utils.py
--rw-r--r--   0 root         (0) root         (0)    14146 2024-04-02 01:04:23.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/vit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.428623 cornstarch-0.0.1/oobleck_colossalai/shardformer/shard/
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-09 03:13:36.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/shard/placeholder.py
--rw-r--r--   0 root         (0) root         (0)     7153 2024-04-09 13:29:40.000000 cornstarch-0.0.1/oobleck_colossalai/shardformer/shard/shardformer.py
--rw-r--r--   0 root         (0) root         (0)     5183 2024-03-27 01:34:07.000000 cornstarch-0.0.1/oobleck_colossalai/stage_manager.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-10 18:37:04.000000 cornstarch-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 18:37:07.430623 cornstarch-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:37:07.429623 cornstarch-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)    12757 2024-03-31 05:23:38.000000 cornstarch-0.0.1/tests/test_heterogeneous_parallel_plugin.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-04-02 01:04:59.000000 cornstarch-0.0.1/tests/test_pipeline_template.py
--rw-r--r--   0 root         (0) root         (0)     1584 2024-03-29 03:14:19.000000 cornstarch-0.0.1/tests/test_placeholder.py
--rw-r--r--   0 root         (0) root         (0)     8017 2024-03-18 18:03:04.000000 cornstarch-0.0.1/tests/test_process_group_mesh.py
--rw-r--r--   0 root         (0) root         (0)    10465 2024-03-27 02:03:44.000000 cornstarch-0.0.1/tests/test_stage_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.921939 cornstarch-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11338 2024-03-18 14:10:17.000000 cornstarch-0.0.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    14352 2024-04-10 18:54:26.921939 cornstarch-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      426 2024-04-10 18:36:05.000000 cornstarch-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.920939 cornstarch-0.0.2/cornstarch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14352 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1336 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-10 18:54:26.000000 cornstarch-0.0.2/cornstarch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.917939 cornstarch-0.0.2/oobleck_colossalai/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/pipeline_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.918939 cornstarch-0.0.2/oobleck_colossalai/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-04-06 13:53:20.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_module.py
+-rw-r--r--   0 root         (0) root         (0)    14670 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_plugin.py
+-rw-r--r--   0 root         (0) root         (0)    10621 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/process_group_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.918939 cornstarch-0.0.2/oobleck_colossalai/shardformer/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.919939 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 14:10:17.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/auto_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34146 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/bert.py
+-rw-r--r--   0 root         (0) root         (0)    23020 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/gpt2.py
+-rw-r--r--   0 root         (0) root         (0)    17991 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/llama.py
+-rw-r--r--   0 root         (0) root         (0)    17674 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/opt.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-09 13:57:49.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/utils.py
+-rw-r--r--   0 root         (0) root         (0)    14129 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/vit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.919939 cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-09 03:13:36.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/placeholder.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/shardformer.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2024-04-10 18:54:02.000000 cornstarch-0.0.2/oobleck_colossalai/stage_manager.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-10 18:54:20.000000 cornstarch-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 18:54:26.921939 cornstarch-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:54:26.920939 cornstarch-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)    12708 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_heterogeneous_parallel_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_pipeline_template.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_placeholder.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_process_group_mesh.py
+-rw-r--r--   0 root         (0) root         (0)    10440 2024-04-10 18:54:02.000000 cornstarch-0.0.2/tests/test_stage_manager.py
```

### Comparing `cornstarch-0.0.1/LICENSE.txt` & `cornstarch-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.1/PKG-INFO` & `cornstarch-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornstarch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A versatile model toolkit for distributed training.
 Author-email: Insu Jang <insujang@umich.edu>
 Maintainer-email: Insu Jang <insujang@umich.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -222,7 +222,17 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black>=23.0; extra == "dev"
 Requires-Dist: isort>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: expecttest; extra == "dev"
 Requires-Dist: accelerate; extra == "dev"
+
+<h1 align="center">Cornstarch<br>
+A Versatile Model Toolkit for Distributed Training</h1>
+
+Cornstarch includes tools that change HuggingFace model shapes for various distributed training.
+Powered by [ColossalAI](https://colossalai.org/) for basic parallelism implementation and training backend, Cornstarch provides more various ways of changing the form of distributed training.
+
+## Run
+
+See [how to run](examples/README.md).
```

### Comparing `cornstarch-0.0.1/cornstarch.egg-info/PKG-INFO` & `cornstarch-0.0.2/cornstarch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornstarch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A versatile model toolkit for distributed training.
 Author-email: Insu Jang <insujang@umich.edu>
 Maintainer-email: Insu Jang <insujang@umich.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -222,7 +222,17 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black>=23.0; extra == "dev"
 Requires-Dist: isort>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: expecttest; extra == "dev"
 Requires-Dist: accelerate; extra == "dev"
+
+<h1 align="center">Cornstarch<br>
+A Versatile Model Toolkit for Distributed Training</h1>
+
+Cornstarch includes tools that change HuggingFace model shapes for various distributed training.
+Powered by [ColossalAI](https://colossalai.org/) for basic parallelism implementation and training backend, Cornstarch provides more various ways of changing the form of distributed training.
+
+## Run
+
+See [how to run](examples/README.md).
```

### Comparing `cornstarch-0.0.1/cornstarch.egg-info/SOURCES.txt` & `cornstarch-0.0.2/cornstarch.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.txt
+README.md
 pyproject.toml
 cornstarch.egg-info/PKG-INFO
 cornstarch.egg-info/SOURCES.txt
 cornstarch.egg-info/dependency_links.txt
 cornstarch.egg-info/requires.txt
 cornstarch.egg-info/top_level.txt
 oobleck_colossalai/__init__.py
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/pipeline_template.py` & `cornstarch-0.0.2/oobleck_colossalai/pipeline_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         """Get the model name from the model."""
         return _fullname(model)
 
     @staticmethod
     def get_modules(model: nn.Module) -> list[str]:
         """Get all modules from the model."""
         # Avoid circular import
-        from oobleck_colossalai.shardformer.policies.auto_policy import (
+        from cornstarch.shardformer.policies.auto_policy import (
             get_policy_type,
         )
-        from oobleck_colossalai.shardformer.policies.pipeline_template_policy import (
+        from cornstarch.shardformer.policies.pipeline_template_policy import (
             PipelineTemplatePolicyBase,
         )
 
         policy: Type[PipelineTemplatePolicyBase] = get_policy_type(
             PipelineTemplate.get_model_name(model)
         )
         assert issubclass(
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/plugin/heterogeneous_dataloader.py` & `cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_dataloader.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.1/oobleck_colossalai/plugin/heterogeneous_parallel_module.py` & `cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from colossalai.booster.plugin.hybrid_parallel_plugin import (
     HybridParallelModule,
     _convert_floating_point,
 )
 from colossalai.interface import ModelWrapper
 from colossalai.shardformer import ShardConfig
 from colossalai.shardformer.policies.base_policy import Policy
-
-from oobleck_colossalai.shardformer.shard.shardformer import ShardFormer
+from cornstarch.shardformer.shard.shardformer import ShardFormer
 
 
 class HeterogeneousParallelModule(HybridParallelModule):
     def __init__(
         self,
         module: torch.nn.Module,
         dp_groups: dict[str, dist.ProcessGroup],
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/plugin/heterogeneous_parallel_plugin.py` & `cornstarch-0.0.2/oobleck_colossalai/plugin/heterogeneous_parallel_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,26 @@
     get_param_info,
 )
 from colossalai.booster.plugin.pp_plugin_base import PipelinePluginBase
 from colossalai.checkpoint_io import CheckpointIO, HybridParallelCheckpointIO
 from colossalai.interface import ModelWrapper, OptimizerWrapper
 from colossalai.pipeline.schedule import OneForwardOneBackwardSchedule
 from colossalai.shardformer import ShardConfig
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.plugin.heterogeneous_dataloader import HeterogeneousDataLoader
+from cornstarch.plugin.heterogeneous_parallel_module import (
+    HeterogeneousParallelModule,
+)
+from cornstarch.process_group_mesh import HeterogeneousProcessGroupMesh
+from cornstarch.shardformer.policies.auto_policy import get_autopolicy
+from cornstarch.stage_manager import HeterogeneousPipelineStageManager
 from torch.optim.lr_scheduler import LRScheduler
 from torch.optim.optimizer import Optimizer
 from torch.utils.data import DataLoader, Dataset
 
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.plugin.heterogeneous_dataloader import HeterogeneousDataLoader
-from oobleck_colossalai.plugin.heterogeneous_parallel_module import (
-    HeterogeneousParallelModule,
-)
-from oobleck_colossalai.process_group_mesh import HeterogeneousProcessGroupMesh
-from oobleck_colossalai.shardformer.policies.auto_policy import get_autopolicy
-from oobleck_colossalai.stage_manager import HeterogeneousPipelineStageManager
-
 
 class HeterogeneousParallelPlugin(HybridParallelPlugin):
     """Plugin for heterogeneous parallel training.
     Tensor parallel, ZeRO, pipeline parallelism, and data parallel are combined in this plugin.
     The size of tp (tp_size) and pp should be passed in by user.
     ZeRO/TP requires a lot of communication, thus should only be done within each node.
     The size of dp is determined by the number of nodes in the given set of pipeline templates.
@@ -334,15 +333,15 @@
                 the batch size, then the last batch will be smaller, defaults to False.
             pin_memory (bool, optional): Whether to pin memory address in CPU memory. Defaults to False.
             num_workers (int, optional): Number of worker threads for this dataloader. Defaults to 0.
             kwargs (dict): optional parameters for ``torch.utils.data.DataLoader``, more details could be found in
                     `DataLoader <https://pytorch.org/docs/stable/_modules/torch/utils/data/dataloader.html#DataLoader>`_.
 
         Returns:
-            :class:`oobleck_colossalai.plugin.heterogeneous_dataloader.HeterogeneousDataLoader`:
+            :class:`cornstarch.plugin.heterogeneous_dataloader.HeterogeneousDataLoader`:
                 A DataLoader used for training or testing.
         """
         _kwargs = kwargs.copy()
         _kwargs.pop("sampler", None)
         _kwargs.pop("batch_sampler", None)
 
         return HeterogeneousDataLoader(
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/process_group_mesh.py` & `cornstarch-0.0.2/oobleck_colossalai/process_group_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import itertools
 from typing import Optional
 
 import numpy as np
 import torch.distributed as dist
 from colossalai.cluster.process_group_mesh import ProcessGroupMesh
+from cornstarch.pipeline_template import PipelineTemplate
 from torch.distributed import ProcessGroup
 from torch.distributed.distributed_c10d import GroupMember
 
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-
 DP_AXIS, PP_AXIS, TP_AXIS = 0, 1, 2
 
 
 class HeterogeneousProcessGroupMesh(ProcessGroupMesh):
     """A helper class to manage the process group mesh.
     Different from original ColossalAI's ProcessGroupMesh, which holds a rank
     per pipeline stage, this HeterogeneousProcessGroupMesh manages ranks per model layer.
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/auto_policy.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/auto_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = ["get_policy_type", "get_autopolicy", "import_policy"]
 
 
 def import_policy(policy_location: PolicyLocation) -> Policy:
     """
     Dynamically import a Policy class based on the policy location.
     """
-    module_name = f"oobleck_colossalai.shardformer.policies.{policy_location.file_name}"
+    module_name = f"cornstarch.shardformer.policies.{policy_location.file_name}"
     module = importlib.import_module(module_name)
     return getattr(module, policy_location.class_name)
 
 
 def get_policy_type(model_name: str) -> Type[Policy]:
     policy_location = _POLICY_LIST.get(model_name, None)
     if policy_location is None:
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/bert.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,25 @@
 )
 from colossalai.shardformer.modeling.jit import get_jit_fused_dropout_add_func
 from colossalai.shardformer.policies.base_policy import (
     ModulePolicyDescription,
     Policy,
     SubModuleReplacementDescription,
 )
-from torch import Tensor
-from torch.nn import Module
-from transformers import BertConfig, PretrainedConfig
-
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.shardformer.policies.pipeline_template_policy import (
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.shardformer.policies.pipeline_template_policy import (
     PipelineTemplatePolicyBase,
 )
-from oobleck_colossalai.shardformer.policies.utils import (
+from cornstarch.shardformer.policies.utils import (
     resize_embeddings,
     resize_lm_head,
 )
+from torch import Tensor
+from torch.nn import Module
+from transformers import BertConfig, PretrainedConfig
 
 __all__ = [
     "BertPolicy",
     "BertModelPolicy",
     "BertForPreTrainingPolicy",
     "BertLMHeadModelPolicy",
     "BertForMaskedLMPolicy",
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/gpt2.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/gpt2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,24 @@
     gpt2_sequence_parallel_forward_fn,
 )
 from colossalai.shardformer.policies.base_policy import (
     ModulePolicyDescription,
     Policy,
     SubModuleReplacementDescription,
 )
-from torch import Tensor, nn
-from transformers import GPT2Config, PretrainedConfig
-
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.shardformer.policies.pipeline_template_policy import (
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.shardformer.policies.pipeline_template_policy import (
     PipelineTemplatePolicyBase,
 )
-from oobleck_colossalai.shardformer.policies.utils import (
+from cornstarch.shardformer.policies.utils import (
     resize_embeddings,
     resize_lm_head,
 )
+from torch import Tensor, nn
+from transformers import GPT2Config, PretrainedConfig
 
 __all__ = [
     "GPT2Policy",
     "GPT2ModelPolicy",
     "GPT2LMHeadModelPolicy",
     "GPT2DoubleHeadsModelPolicy",
     "GPT2ForTokenClassificationPolicy",
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/llama.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,24 @@
     get_lm_forward_with_dist_cross_entropy,
 )
 from colossalai.shardformer.policies.base_policy import (
     ModulePolicyDescription,
     Policy,
     SubModuleReplacementDescription,
 )
-from torch import Tensor, nn
-from transformers import LlamaConfig, PretrainedConfig
-
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.shardformer.policies.pipeline_template_policy import (
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.shardformer.policies.pipeline_template_policy import (
     PipelineTemplatePolicyBase,
 )
-from oobleck_colossalai.shardformer.policies.utils import (
+from cornstarch.shardformer.policies.utils import (
     resize_embeddings,
     resize_lm_head,
 )
+from torch import Tensor, nn
+from transformers import LlamaConfig, PretrainedConfig
 
 __all__ = [
     "LlamaPolicy",
     "LlamaForCausalLMPolicy",
     "LlamaForSequenceClassificationPolicy",
 ]
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/opt.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,24 @@
     get_opt_flash_attention_forward,
 )
 from colossalai.shardformer.policies.base_policy import (
     ModulePolicyDescription,
     Policy,
     SubModuleReplacementDescription,
 )
-from torch import Tensor, nn
-from transformers import OPTConfig, PretrainedConfig
-
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.shardformer.policies.pipeline_template_policy import (
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.shardformer.policies.pipeline_template_policy import (
     PipelineTemplatePolicyBase,
 )
-from oobleck_colossalai.shardformer.policies.utils import (
+from cornstarch.shardformer.policies.utils import (
     resize_embeddings,
     resize_lm_head,
 )
+from torch import Tensor, nn
+from transformers import OPTConfig, PretrainedConfig
 
 __all__ = [
     "OPTPolicy",
     "OPTModelPolicy",
     "OPTForCausalLMPolicy",
     "OPTForSequenceClassificationPolicy",
     "OPTForQuestionAnsweringPolicy",
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/pipeline_template_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
 from abc import ABC, abstractmethod
 
 import numpy as np
+from cornstarch.pipeline_template import PipelineTemplate
 from torch import nn
 from transformers import PretrainedConfig
 
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-
 
 class PipelineTemplatePolicyBase(ABC):
     """A policy base that defines the interface for a pipeline template policy."""
 
     skip_replaced_modules: bool = True
 
     @staticmethod
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/utils.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/utils.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/policies/vit.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/policies/vit.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,19 @@
     get_vit_flash_self_attention_forward,
 )
 from colossalai.shardformer.policies.base_policy import (
     ModulePolicyDescription,
     Policy,
     SubModuleReplacementDescription,
 )
-from transformers import PretrainedConfig, ViTConfig
-
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.shardformer.policies.pipeline_template_policy import (
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.shardformer.policies.pipeline_template_policy import (
     PipelineTemplatePolicyBase,
 )
+from transformers import PretrainedConfig, ViTConfig
 
 __all__ = [
     "ViTPolicy",
     "ViTModelPolicy",
     "ViTForImageClassificationPolicy",
     "ViTForMaskedImageModelingPolicy",
 ]
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/shard/placeholder.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/placeholder.py`

 * *Files identical despite different names*

### Comparing `cornstarch-0.0.1/oobleck_colossalai/shardformer/shard/shardformer.py` & `cornstarch-0.0.2/oobleck_colossalai/shardformer/shard/shardformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from colossalai.shardformer.policies.base_policy import (
     Policy,
     SubModuleReplacementDescription,
 )
 from colossalai.shardformer.shard.sharder import ModelSharder as ColossalModelSharder
 from colossalai.shardformer.shard.shardformer import ShardConfig
 from colossalai.shardformer.shard.shardformer import ShardFormer as ColossalShardFormer
+from cornstarch.shardformer.shard.placeholder import TensorPlaceholder
 from loguru import logger
 from torch import Tensor, nn
 
-from oobleck_colossalai.shardformer.shard.placeholder import TensorPlaceholder
-
 
 class ModelSharder(ColossalModelSharder):
     def shard(self) -> list[dict[int, Tensor]]:
         r"""
         Shard the model according to the policy.
 
         Switch order of _replace_module() and _replace_unheld_layers call
```

### Comparing `cornstarch-0.0.1/oobleck_colossalai/stage_manager.py` & `cornstarch-0.0.2/oobleck_colossalai/stage_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 import torch.distributed as dist
 from colossalai.pipeline.stage_manager import PipelineStageManager
+from cornstarch.process_group_mesh import HeterogeneousProcessGroupMesh
 from torch.distributed.distributed_c10d import GroupMember
 
-from oobleck_colossalai.process_group_mesh import HeterogeneousProcessGroupMesh
-
 
 class HeterogeneousPipelineStageManager(PipelineStageManager):
     """PipelineStageManager is a helper class to manage pipeline stages.
 
     The stage manager is only for a single pipeline, which includes this process rank.
     Thus, self.prev_rank, self.next_rank, and self.p2p_groups might be different across
     different processes.
```

### Comparing `cornstarch-0.0.1/pyproject.toml` & `cornstarch-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "cornstarch"
 description = "A versatile model toolkit for distributed training."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.10"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Insu Jang", email = "insujang@umich.edu"}
 ]
 maintainers = [
     {name = "Insu Jang", email = "insujang@umich.edu"}
 ]
 classifiers = [
```

### Comparing `cornstarch-0.0.1/tests/test_heterogeneous_parallel_plugin.py` & `cornstarch-0.0.2/tests/test_heterogeneous_parallel_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,26 @@
 from unittest.mock import patch
 
 import numpy as np
 import torch
 import torch.distributed as dist
 from colossalai.interface import ModelWrapper, OptimizerWrapper
 from colossalai.shardformer.modeling.gpt2 import GPT2PipelineForwards
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.plugin.heterogeneous_dataloader import HeterogeneousDataLoader
+from cornstarch.plugin.heterogeneous_parallel_module import (
+    HeterogeneousParallelModule,
+)
+from cornstarch.plugin.heterogeneous_parallel_plugin import (
+    HeterogeneousParallelPlugin,
+)
+from cornstarch.shardformer.policies.gpt2 import (
+    GPT2ForSequenceClassificationPolicy,
+)
+from cornstarch.shardformer.shard.placeholder import TensorPlaceholder
 from data_builder import GLUEDataBuilder
 from torch.optim import Adam
 from torch.optim.lr_scheduler import LRScheduler
 from torch.testing._internal.common_distributed import (
     TEST_SKIPS,
     MultiProcessTestCase,
     skip_if_lt_x_gpu,
@@ -25,27 +37,14 @@
 )
 from transformers import (
     GPT2Config,
     GPT2ForSequenceClassification,
     get_linear_schedule_with_warmup,
 )
 
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.plugin.heterogeneous_dataloader import HeterogeneousDataLoader
-from oobleck_colossalai.plugin.heterogeneous_parallel_module import (
-    HeterogeneousParallelModule,
-)
-from oobleck_colossalai.plugin.heterogeneous_parallel_plugin import (
-    HeterogeneousParallelPlugin,
-)
-from oobleck_colossalai.shardformer.policies.gpt2 import (
-    GPT2ForSequenceClassificationPolicy,
-)
-from oobleck_colossalai.shardformer.shard.placeholder import TensorPlaceholder
-
 config: GPT2Config = GPT2Config.from_pretrained("gpt2")
 config.is_decoder = True
 config.n_layer = 4
 config.num_labels = GLUEDataBuilder.glue_task_num_labels["mrpc"]
 
 modules: list[str] = GPT2ForSequenceClassificationPolicy.get_all_modules(config)
 model_name: str = "transformers.models.gpt2.modeling_gpt2.GPT2ForSequenceClassification"
```

### Comparing `cornstarch-0.0.1/tests/test_pipeline_template.py` & `cornstarch-0.0.2/tests/test_pipeline_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from contextlib import nullcontext
 
 import pytest
 from accelerate import init_empty_weights
-from transformers import GPT2Config, GPT2ForSequenceClassification
-
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.shardformer.policies.gpt2 import (
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.shardformer.policies.gpt2 import (
     GPT2ForSequenceClassificationPolicy,
 )
+from transformers import GPT2Config, GPT2ForSequenceClassification
 
 num_layers = 4
 
 
 @pytest.fixture
 def model() -> GPT2ForSequenceClassification:
     config = GPT2Config.from_pretrained("gpt2")
```

### Comparing `cornstarch-0.0.1/tests/test_placeholder.py` & `cornstarch-0.0.2/tests/test_placeholder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 import torch
 from colossalai.accelerator import get_accelerator
-
-from oobleck_colossalai.shardformer.shard.placeholder import TensorPlaceholder
+from cornstarch.shardformer.shard.placeholder import TensorPlaceholder
 
 
 @pytest.mark.skipif(not torch.cuda.is_available(), reason="CUDA is not available")
 @pytest.mark.parametrize(
     "target_device, target_dtype",
     [
         [torch.device("cuda:0"), torch.float32],
```

### Comparing `cornstarch-0.0.1/tests/test_process_group_mesh.py` & `cornstarch-0.0.2/tests/test_process_group_mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import functools
 from collections import defaultdict
 
 import numpy as np
 import pytest
 import torch.distributed as dist
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.process_group_mesh import HeterogeneousProcessGroupMesh
 from pytest_mock import MockerFixture
 from torch.testing._internal.distributed.fake_pg import FakeStore
 
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.process_group_mesh import HeterogeneousProcessGroupMesh
-
 
 @pytest.fixture(autouse=True)
 def init_process_group(request: pytest.FixtureRequest):
     if "noautofixture" in request.keywords:
         yield
     else:
         store = FakeStore()
```

### Comparing `cornstarch-0.0.1/tests/test_stage_manager.py` & `cornstarch-0.0.2/tests/test_stage_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import functools
 from collections import defaultdict
 
 import numpy as np
 import pytest
 import torch.distributed as dist
+from cornstarch.pipeline_template import PipelineTemplate
+from cornstarch.process_group_mesh import HeterogeneousProcessGroupMesh
+from cornstarch.stage_manager import HeterogeneousPipelineStageManager
 from pytest_mock import MockerFixture
 from torch.distributed.distributed_c10d import GroupMember
 from torch.testing._internal.common_distributed import MultiThreadedTestCase
 from torch.testing._internal.common_utils import (
     instantiate_parametrized_tests,
     parametrize,
 )
 from torch.testing._internal.distributed.fake_pg import FakeStore
 
-from oobleck_colossalai.pipeline_template import PipelineTemplate
-from oobleck_colossalai.process_group_mesh import HeterogeneousProcessGroupMesh
-from oobleck_colossalai.stage_manager import HeterogeneousPipelineStageManager
-
 no_tp_templates = [
     PipelineTemplate("fake", [[None, None], [None, None, None, None]]),
     PipelineTemplate("fake", [[None, None], [None, None, None, None]]),
     PipelineTemplate("fake", [[None], [None, None, None], [None, None]]),
 ]
 no_tp_template_ranks = [
     [[0], [0], [1], [1], [1], [1]],
```

