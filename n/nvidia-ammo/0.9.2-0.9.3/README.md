# Comparing `tmp/nvidia_ammo-0.9.2.tar.gz` & `tmp/nvidia_ammo-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_ammo-0.9.2.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_ammo-0.9.3.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_ammo-0.9.2.tar` & `nvidia_ammo-0.9.3.tar`

### file list

```diff
@@ -1,2 +1,2 @@
 -rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
--rw-r--r--   0        0        0     3525 1993-04-05 07:00:00.000000 PKG-INFO
+-rw-r--r--   0        0        0     3510 1993-04-05 07:00:00.000000 PKG-INFO
```

### PKG-INFO

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nvidia-ammo
-Version: 0.9.2
+Version: 0.9.3
 Summary: Ammo: a unified algorithmic model optimization and deployment toolkit.
 Author-email: "Nvidia, Inc." <ammo-support@exchange.nvidia.com>
 License: NVIDIA Proprietary Software
 Project-URL: Homepage, https://nvidia.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ninja
 Requires-Dist: networkx
 Requires-Dist: numpy
-Requires-Dist: onnx <1.16,>=1.14.0
-Requires-Dist: onnxruntime ~=1.16.1
+Requires-Dist: onnx
+Requires-Dist: onnxruntime ~=1.16.3
 Requires-Dist: onnx-graphsurgeon
 Requires-Dist: packaging
 Requires-Dist: pydantic >=2.0
 Requires-Dist: rich
 Requires-Dist: scipy
 Requires-Dist: torch >=1.11
 Requires-Dist: tqdm
```

