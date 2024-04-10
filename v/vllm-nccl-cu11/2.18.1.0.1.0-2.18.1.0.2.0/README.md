# Comparing `tmp/vllm_nccl_cu11-2.18.1.0.1.0.tar.gz` & `tmp/vllm_nccl_cu11-2.18.1.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm_nccl_cu11-2.18.1.0.1.0.tar", last modified: Wed Apr  3 20:55:17 2024, max compression
+gzip compressed data, was "vllm_nccl_cu11-2.18.1.0.2.0.tar", last modified: Wed Apr 10 19:56:14 2024, max compression
```

## Comparing `vllm_nccl_cu11-2.18.1.0.1.0.tar` & `vllm_nccl_cu11-2.18.1.0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:55:17.926626 vllm_nccl_cu11-2.18.1.0.1.0/
--rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu11-2.18.1.0.1.0/LICENSE
--rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-03 20:55:17.926495 vllm_nccl_cu11-2.18.1.0.1.0/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)       41 2024-04-02 16:28:30.000000 vllm_nccl_cu11-2.18.1.0.1.0/README.md
--rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-03 20:55:17.926735 vllm_nccl_cu11-2.18.1.0.1.0/setup.cfg
--rw-r--r--   0 youkaichao   (501) staff       (20)     2909 2024-04-03 20:54:50.000000 vllm_nccl_cu11-2.18.1.0.1.0/setup.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:55:17.925881 vllm_nccl_cu11-2.18.1.0.1.0/vllm_nccl/
--rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu11-2.18.1.0.1.0/vllm_nccl/__init__.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:55:17.926337 vllm_nccl_cu11-2.18.1.0.1.0/vllm_nccl_cu11.egg-info/
--rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-03 20:55:17.000000 vllm_nccl_cu11-2.18.1.0.1.0/vllm_nccl_cu11.egg-info/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-03 20:55:17.000000 vllm_nccl_cu11-2.18.1.0.1.0/vllm_nccl_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-03 20:55:17.000000 vllm_nccl_cu11-2.18.1.0.1.0/vllm_nccl_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-03 20:55:17.000000 vllm_nccl_cu11-2.18.1.0.1.0/vllm_nccl_cu11.egg-info/top_level.txt
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-10 19:56:14.861949 vllm_nccl_cu11-2.18.1.0.2.0/
+-rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu11-2.18.1.0.2.0/LICENSE
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-10 19:56:14.861723 vllm_nccl_cu11-2.18.1.0.2.0/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      164 2024-04-03 20:59:04.000000 vllm_nccl_cu11-2.18.1.0.2.0/README.md
+-rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-10 19:56:14.862001 vllm_nccl_cu11-2.18.1.0.2.0/setup.cfg
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2454 2024-04-10 19:55:09.000000 vllm_nccl_cu11-2.18.1.0.2.0/setup.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-10 19:56:14.861066 vllm_nccl_cu11-2.18.1.0.2.0/vllm_nccl/
+-rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu11-2.18.1.0.2.0/vllm_nccl/__init__.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-10 19:56:14.861551 vllm_nccl_cu11-2.18.1.0.2.0/vllm_nccl_cu11.egg-info/
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-10 19:56:14.000000 vllm_nccl_cu11-2.18.1.0.2.0/vllm_nccl_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-10 19:56:14.000000 vllm_nccl_cu11-2.18.1.0.2.0/vllm_nccl_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-10 19:56:14.000000 vllm_nccl_cu11-2.18.1.0.2.0/vllm_nccl_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-10 19:56:14.000000 vllm_nccl_cu11-2.18.1.0.2.0/vllm_nccl_cu11.egg-info/top_level.txt
```

### Comparing `vllm_nccl_cu11-2.18.1.0.1.0/LICENSE` & `vllm_nccl_cu11-2.18.1.0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm_nccl_cu11-2.18.1.0.1.0/setup.py` & `vllm_nccl_cu11-2.18.1.0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 # this is actually a download and install script
 # it appears in `pip` style `setup.py` file, to be easily installable with `pip install`
-# and files can be removed with `pip uninstall`
-# unfortunately, this brings nccl into the wheel, which will exceed the 100MB limit of PyPI.
-# so we don't upload this to PyPI, but instead, we can install it from github
-# its argument is derived from environment variable `VLLM_INSTALL_NCCL`,
-# e.g. `VLLM_INSTALL_NCCL=2.18+cu12 pip install https://github.com/vllm-project/vllm-nccl.git`
-# after installation, files are available in `{sys.prefix}/vllm_nccl` directory
 
 from setuptools import setup, find_packages
 import platform
 import os
 from dataclasses import dataclass
 
 # for reference, we can download nccl from the following links
@@ -41,20 +35,20 @@
     DistInfo('11.0', '2.20.3', '2.20.3', 'nccl_2.20.3-1+cuda11.0_x86_64.txz'),
     DistInfo('12.2', '2.20.3', '2.20.3', 'nccl_2.20.3-1+cuda12.2_x86_64.txz'),
 ]
 
 package_name = "vllm_nccl_cu11"
 cuda_name = package_name[-4:]
 nccl_version = "2.18.1"
-vllm_nccl_verion = "0.1.0"
+vllm_nccl_verion = "0.2.0"
 version = ".".join([nccl_version, vllm_nccl_verion])
 
 assert nccl_version == "2.18.1", f"only support nccl 2.18.1, got {version}"
 
-url = f"https://storage.googleapis.com/vllm-public-assets/nccl/{cuda_name}/libnccl.so.{nccl_version}"
+url = f"https://github.com/vllm-project/vllm-nccl/releases/download/v0.1.0/{cuda_name}-libnccl.so.{nccl_version}"
 
 import urllib.request
 import os
 
 # desination path is ~/.config/vllm/nccl/cu12/libnccl.so.2.18.1
 destination = os.path.expanduser(f"~/.config/vllm/nccl/{cuda_name}/libnccl.so.{nccl_version}")
```

