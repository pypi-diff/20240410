# Comparing `tmp/neural-commons-0.0.5.tar.gz` & `tmp/neural-commons-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.0.5.tar", last modified: Sat Mar 30 21:58:49 2024, max compression
+gzip compressed data, was "neural-commons-0.0.6.tar", last modified: Wed Apr 10 16:50:10 2024, max compression
```

## Comparing `neural-commons-0.0.5.tar` & `neural-commons-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 21:58:49.508992 neural-commons-0.0.5/
--rw-rw-rw-   0        0        0      455 2024-03-30 21:58:49.508001 neural-commons-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-04 23:56:39.000000 neural-commons-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 21:58:49.482042 neural-commons-0.0.5/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-03-17 15:44:00.000000 neural-commons-0.0.5/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 21:58:49.500868 neural-commons-0.0.5/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-03-17 15:41:54.000000 neural-commons-0.0.5/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0     9900 2024-03-23 13:19:18.000000 neural-commons-0.0.5/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-03-30 21:58:49.506996 neural-commons-0.0.5/neural_commons/modules/
--rw-rw-rw-   0        0        0      248 2024-03-10 01:02:13.000000 neural-commons-0.0.5/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-03-10 01:07:51.000000 neural-commons-0.0.5/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0      463 2024-03-30 21:58:34.000000 neural-commons-0.0.5/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0     2853 2024-03-23 01:19:23.000000 neural-commons-0.0.5/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      477 2024-03-23 01:19:12.000000 neural-commons-0.0.5/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0     1350 2024-03-17 01:27:58.000000 neural-commons-0.0.5/neural_commons/modules/PreTrainedLayer.py
--rw-rw-rw-   0        0        0      886 2024-03-06 00:06:41.000000 neural-commons-0.0.5/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-03-16 17:07:31.000000 neural-commons-0.0.5/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-03-17 13:56:24.000000 neural-commons-0.0.5/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-03-10 02:40:36.000000 neural-commons-0.0.5/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      300 2024-03-30 21:50:31.000000 neural-commons-0.0.5/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 21:58:49.497987 neural-commons-0.0.5/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      455 2024-03-30 21:58:49.000000 neural-commons-0.0.5/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-03-30 21:58:49.000000 neural-commons-0.0.5/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 21:58:49.000000 neural-commons-0.0.5/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-03-30 21:58:49.000000 neural-commons-0.0.5/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-30 21:58:49.000000 neural-commons-0.0.5/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 21:58:49.508992 neural-commons-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      968 2024-03-30 21:58:43.000000 neural-commons-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.176476 neural-commons-0.0.6/
+-rw-rw-rw-   0        0        0      455 2024-04-10 16:50:10.175478 neural-commons-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.153478 neural-commons-0.0.6/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.160478 neural-commons-0.0.6/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0    10089 2024-04-08 14:26:47.000000 neural-commons-0.0.6/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.174477 neural-commons-0.0.6/neural_commons/modules/
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0     2818 2024-04-08 14:36:12.000000 neural-commons-0.0.6/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      844 2024-04-10 16:44:22.000000 neural-commons-0.0.6/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0     1350 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/PreTrainedLayer.py
+-rw-rw-rw-   0        0        0      886 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.0.6/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      300 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.158478 neural-commons-0.0.6/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:50:10.176476 neural-commons-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      968 2024-04-10 16:46:59.000000 neural-commons-0.0.6/setup.py
```

### Comparing `neural-commons-0.0.5/neural_commons/helpers/torch_helper.py` & `neural-commons-0.0.6/neural_commons/helpers/torch_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,7 +240,14 @@
                 param_data = matched_param.data
             source_scale = torch.std(param_data).item()
             source_scale = max(source_scale, 1e-10)
             target_scale = torch.std(target_param.data).item()
             param_data = param_data * target_scale / source_scale
             param_data = param_data.detach()
             target_param.data.copy_(param_data)
+
+
+def get_torch_dtype(dtype_str):
+    if hasattr(torch, dtype_str):
+        return getattr(torch, dtype_str)
+    else:
+        raise ValueError(f"Unknown dtype string: {dtype_str}")
```

### Comparing `neural-commons-0.0.5/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.0.6/neural_commons/modules/NeuralLayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-import dataclasses
 import math
 from dataclasses import dataclass
 
 import torch
 from huggingface_hub import PyTorchModelHubMixin
 from torch import nn, Tensor
 from torch.nn import Parameter, init
 import torch.nn.functional as F
 
-
-def get_torch_dtype(dtype_str):
-    if hasattr(torch, dtype_str):
-        return getattr(torch, dtype_str)
-    else:
-        raise ValueError(f"Unknown dtype string: {dtype_str}")
+from neural_commons.helpers.torch_helper import get_torch_dtype
 
 
 @dataclass
 class NeuralLayerConfig:
     in_features: int
     out_features: int
     bias: bool = True
     dtype: str = "float32"
+    slopes_log_std: float = 0.1
 
 
 class NeuralLayer(nn.Module, PyTorchModelHubMixin):
     __constants__ = ['in_features', 'out_features']
     in_features: int
     out_features: int
     weight: Tensor
@@ -36,15 +31,16 @@
             config = NeuralLayerConfig(**config)
         super().__init__()
         dtype = get_torch_dtype(config.dtype)
         self.config = config
         self.convert_input = dtype != torch.float and dtype != torch.float32
         self.in_features = config.in_features
         self.out_features = config.out_features
-        self.slopes = nn.Parameter(torch.ones(self.out_features, dtype=dtype))
+        slopes_t = torch.exp(torch.randn(self.out_features, dtype=dtype) * config.slopes_log_std)
+        self.slopes = nn.Parameter(slopes_t.detach())
         setattr(self.slopes, "__skip_transplant__", True)
         self.weight = Parameter(torch.empty((self.out_features, self.in_features,), dtype=dtype))
         if config.bias:
             self.bias = Parameter(torch.empty(self.out_features, dtype=dtype))
         else:
             self.register_parameter('bias', None)
         self.reset_parameters()
```

### Comparing `neural-commons-0.0.5/neural_commons/modules/PreTrainedLayer.py` & `neural-commons-0.0.6/neural_commons/modules/PreTrainedLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.5/neural_commons/modules/RndNonLinearFunction.py` & `neural-commons-0.0.6/neural_commons/modules/RndNonLinearFunction.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.5/neural_commons/modules/RndProjection.py` & `neural-commons-0.0.6/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.5/neural_commons/modules/SMoE.py` & `neural-commons-0.0.6/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.5/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.0.6/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.5/neural_commons.egg-info/SOURCES.txt` & `neural-commons-0.0.6/neural_commons.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 neural_commons.egg-info/top_level.txt
 neural_commons/helpers/__init__.py
 neural_commons/helpers/torch_helper.py
 neural_commons/modules/GTanh.py
 neural_commons/modules/GaELU.py
 neural_commons/modules/LogShape.py
 neural_commons/modules/NeuralLayer.py
+neural_commons/modules/NeuralLayer2d.py
 neural_commons/modules/ParametricReLU.py
 neural_commons/modules/PreTrainedLayer.py
 neural_commons/modules/RndNonLinearFunction.py
 neural_commons/modules/RndProjection.py
 neural_commons/modules/SMoE.py
 neural_commons/modules/SMoEMixIn.py
 neural_commons/modules/__init__.py
```

### Comparing `neural-commons-0.0.5/setup.py` & `neural-commons-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
     'torch>=2.0.0',
```

