# Comparing `tmp/nvfuser_cu121-0.2.0.dev20240408.tar.gz` & `tmp/nvfuser_cu121-0.2.0.dev20240409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvfuser_cu121-0.2.0.dev20240408.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvfuser_cu121-0.2.0.dev20240409.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvfuser_cu121-0.2.0.dev20240408.tar` & `nvfuser_cu121-0.2.0.dev20240409.tar`

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvfuser_cu121
-Version: 0.2.0.dev20240408
+Version: 0.2.0.dev20240409
 Summary: A Fusion Code Generator for NVIDIA GPUs (commonly known as 'nvFuser')
 Home-page: https://github.com/NVIDIA/Fuser
 License: BSD-3-Clause
 License-File: LICENSE
 Provides-Extra: test
 Provides-Extra: torch
 Stub-Only: True
```

