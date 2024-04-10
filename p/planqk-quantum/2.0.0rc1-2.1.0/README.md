# Comparing `tmp/planqk-quantum-2.0.0rc1.tar.gz` & `tmp/planqk-quantum-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-2.0.0rc1.tar", last modified: Tue Apr  2 16:32:20 2024, max compression
+gzip compressed data, was "planqk-quantum-2.1.0.tar", last modified: Wed Apr 10 10:24:16 2024, max compression
```

## Comparing `planqk-quantum-2.0.0rc1.tar` & `planqk-quantum-2.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/dwave/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/dwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/dwave/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/dto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/job_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/planqk_runtime_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/ionq_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/job_input_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcp_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcz_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/runtime_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.031513 planqk-quantum-2.1.0/planqk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.031513 planqk-quantum-2.1.0/planqk/dwave/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/dwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/dwave/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.031513 planqk-quantum-2.1.0/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.031513 planqk-quantum-2.1.0/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/client/dto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/client/job_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/planqk_runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/planqk/qiskit/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/aws/aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/aws_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/aws_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/azure/ionq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/azure_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/planqk/qiskit/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/ibm/ibm_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/ibm/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/pcp_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/pcz_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/qryd_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/qryd_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/qryd_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/planqk/qiskit/runtime_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-10 10:24:15.000000 planqk-quantum-2.1.0/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 10:24:15.000000 planqk-quantum-2.1.0/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:24:15.000000 planqk-quantum-2.1.0/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-10 10:24:15.000000 planqk-quantum-2.1.0/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 10:24:15.000000 planqk-quantum-2.1.0/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:24:16.035513 planqk-quantum-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 10:24:03.000000 planqk-quantum-2.1.0/setup.py
```

### Comparing `planqk-quantum-2.0.0rc1/LICENSE` & `planqk-quantum-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/PKG-INFO` & `planqk-quantum-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.0.0rc1
+Version: 2.1.0
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.0.0rc1/README.md` & `planqk-quantum-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/context.py` & `planqk-quantum-2.1.0/planqk/context.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/credentials.py` & `planqk-quantum-2.1.0/planqk/credentials.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/dwave/provider.py` & `planqk-quantum-2.1.0/planqk/dwave/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/exceptions.py` & `planqk-quantum-2.1.0/planqk/exceptions.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/backend.py` & `planqk-quantum-2.1.0/planqk/qiskit/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import copy
 
 from qiskit.circuit import Measure
 from qiskit.providers import BackendV2, Provider
 from qiskit.providers.models import QasmBackendConfiguration, GateConfig
 from qiskit.transpiler import Target
 
-from .client.backend_dtos import ConfigurationDto, TYPE, BackendDto, ConnectivityDto, PROVIDER, HARDWARE_PROVIDER
+from .client.backend_dtos import ConfigurationDto, TYPE, BackendDto, ConnectivityDto, PROVIDER
 from .client.job_dtos import JobDto
 from .job import PlanqkJob
 from .options import OptionsV2
 from .providers.adapter import ProviderAdapterFactory
 
 
 class PlanqkBackend(BackendV2, ABC):
@@ -41,22 +41,22 @@
             name: name of actual
             description: description of actual
             online_date: online date
             backend_version: actual version
             **fields: other arguments
         """
 
-        super().__init__(
-            provider=provider,
-            name=name,
-            description=description,
-            online_date=online_date,
-            backend_version=backend_version,
-            **fields,
-        )
+        BackendV2.__init__(self,
+                           provider=provider,
+                           name=name,
+                           description=description,
+                           online_date=online_date,
+                           backend_version=backend_version,
+                           **fields,
+                           )
         self._backend_info = backend_info
         self._target = self._planqk_backend_to_target()
         self._configuration = self._planqk_backend_dto_to_configuration()
         self._instance = None
 
     def _planqk_backend_to_target(self) -> Target:
         """Converts properties of a PlanQK actual into Qiskit Target object.
@@ -126,14 +126,15 @@
             memory=self._backend_info.configuration.memory_result_supported,
             max_shots=self._backend_info.configuration.shots_range.max,
             coupling_map=self.coupling_map,
             supported_instructions=self._target.instructions,
             max_experiments=self._backend_info.configuration.shots_range.max,  # Only one circuit is supported per job
             description=self._backend_info.documentation.description,
             min_shots=self._backend_info.configuration.shots_range.min,
+            online_date=self._backend_info.updated_at  # TODO replace with online date
         )
 
     def _get_gate_config_from_target(self, name) -> GateConfig:
         operations = [operation for operation in self._target.operations
                       if isinstance(operation.name, str)  # Filters out the IBM conditional instructions having no name
                       and operation.name.casefold() == name.casefold()]
         if len(operations) == 1:
@@ -171,16 +172,14 @@
             circuit (QuantumCircuit): circuit to run. Currently only a single circuit can be executed per job.
             **kwargs: additional arguments for the execution (see below)
         Returns:
             PlanqkJob: The job instance for the circuit that was run.
         """
         from planqk.qiskit.providers.job_input_converter import convert_to_backend_input, convert_to_backend_params
 
-        self._validate_provider_for_backend()
-
         if isinstance(circuit, (list, tuple)):
             if len(circuit) > 1:
                 raise ValueError("Multi-experiment jobs are not supported")
             circuit = circuit[0]
 
         # PennyLane-Qiskit Plugin identifies the result based on the circuit name which must be "circ0"
         circuit.name = "circ0"
@@ -190,33 +189,27 @@
         options = copy(self.options)
         if kwargs:
             for field in kwargs:
                 if field in options.data:
                     options[field] = kwargs[field]
 
         supported_input_formats = self._backend_info.configuration.supported_input_formats
+
         backend_input = convert_to_backend_input(supported_input_formats, circuit, self, options)
         input_params = convert_to_backend_params(self._backend_info.provider, circuit, options)
 
         job_request = JobDto(backend_id=self._backend_info.id,
                              provider=self._backend_info.provider.name,
                              input_format=backend_input[0],
                              input=backend_input[1],
                              shots=shots,
                              input_params=input_params)
 
         return PlanqkJob(backend=self, job_details=job_request)
 
-    def _validate_provider_for_backend(self):
-        from planqk.qiskit.runtime_provider import PlanqkQiskitRuntimeService
-        if (self._backend_info.hardware_provider == HARDWARE_PROVIDER.IBM
-                and not isinstance(self.provider, PlanqkQiskitRuntimeService)):
-            raise ValueError(f"Jobs for IBM backends must not be created with {self.provider.__class__.__name__}. "
-                             f"Use {PlanqkQiskitRuntimeService.__name__} instead.")
-
     def retrieve_job(self, job_id: str) -> PlanqkJob:
         """Return a single job.
 
         Args:
             job_id: id of the job to retrieve.
 
         Returns:
```

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-2.1.0/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/client/client.py` & `planqk-quantum-2.1.0/planqk/qiskit/client/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/client/job_dtos.py` & `planqk-quantum-2.1.0/planqk/qiskit/client/job_dtos.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from enum import Enum
 from typing import Optional, Dict, Set, Union
 
 from pydantic import BaseModel
 
 
 class INPUT_FORMAT(str, Enum):
+    BRAKET_OPEN_QASM_V3 = "BRAKET_OPEN_QASM_V3"
     OPEN_QASM_V3 = "OPEN_QASM_V3"
     IONQ_CIRCUIT_V1 = "IONQ_CIRCUIT_V1"
-    QISKIT_PRIMITIVE = "QISKIT_PRIMITIVE"
+    QISKIT = "QISKIT"
     QOQO = "QOQO"
 
 
 class JOB_STATUS(str, Enum):
     COMPLETED = "COMPLETED"
     PENDING = "PENDING"
     RUNNING = "RUNNING"
@@ -45,14 +46,14 @@
             self.error_data = json.loads(self.error_data)
         if self.input_params is not None and isinstance(self.input_params, str):
             self.input_params = json.loads(self.input_params)
 
 
 class RuntimeJobParamsDto(BaseModel):
     program_id: str
-    image: Optional[str]
+    image: Optional[str] = None
     hgp: Optional[str]
-    log_level: Optional[str]
-    session_id: Optional[str]
+    log_level: Optional[str] = None
+    session_id: Optional[str] = None
     max_execution_time: Optional[int] = None
     start_session: Optional[bool] = False
     session_time: Optional[int] = None
```

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/job.py` & `planqk-quantum-2.1.0/planqk/qiskit/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional
 
-from planqk.qiskit.client.client import _PlanqkClient
-from planqk.qiskit.client.job_dtos import JobDto
 from qiskit.providers import JobV1, JobStatus, Backend
 from qiskit.qobj import QobjExperimentHeader
 from qiskit.result import Result
 from qiskit.result.models import ExperimentResult, ExperimentResultData
 
+from planqk.qiskit.client.client import _PlanqkClient
+from planqk.qiskit.client.job_dtos import JobDto
+
 JobStatusMap = {
     "CREATED": JobStatus.INITIALIZING,
     "PENDING": JobStatus.QUEUED,
     "RUNNING": JobStatus.RUNNING,
     "COMPLETED": JobStatus.DONE,
     "FAILED": JobStatus.ERROR,
     "CANCELLING": JobStatus.RUNNING,
```

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/options.py` & `planqk-quantum-2.1.0/planqk/qiskit/options.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/planqk_runtime_job.py` & `planqk-quantum-2.1.0/planqk/qiskit/planqk_runtime_job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/provider.py` & `planqk-quantum-2.1.0/planqk/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/adapter.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_adapter.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/aws_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure_adapter.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/azure_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_adapter.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/ibm/ibm_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/job_input_converter.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/job_input_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import json
 from typing import List, Tuple
 
 from braket.circuits import Circuit
 from braket.circuits.circuit_helpers import validate_circuit_and_shots
-from planqk.qiskit.backend import PlanqkBackend
-from planqk.qiskit.client.backend_dtos import PROVIDER
-from planqk.qiskit.client.job_dtos import INPUT_FORMAT
-from planqk.qiskit.providers.aws_converters import transform_to_qasm_3_program
-from planqk.qiskit.providers.qryd.qryd_converters import convert_to_wire_format, create_qoqu_input_params
 from qiskit import QuantumCircuit
 from qiskit.providers import Options
 from qiskit_braket_provider.providers.adapter import to_braket
 from qiskit_ibm_runtime import RuntimeEncoder
 from qiskit_ionq.helpers import qiskit_circ_to_ionq_circ
 
+from planqk.qiskit.backend import PlanqkBackend
+from planqk.qiskit.client.backend_dtos import PROVIDER
+from planqk.qiskit.client.job_dtos import INPUT_FORMAT
+from planqk.qiskit.providers.aws_converters import transform_braket_to_qasm_3_program
+from planqk.qiskit.providers.qryd.qryd_converters import convert_to_wire_format, create_qoqu_input_params
+
 
-def _convert_to_open_qasm_3(circuit: QuantumCircuit, backend: PlanqkBackend, options: Options):
+def _convert_to_braket_qasm_3(circuit: QuantumCircuit, backend: PlanqkBackend, options: Options):
     shots = options.get("shots", 1)
     inputs = options.get("inputs", {})
     verbatim = options.get("verbatim", False)
 
     basis_gates = backend.operation_names if not verbatim else None
     braket_circuit = to_braket(circuit, basis_gates, verbatim=verbatim)
 
     validate_circuit_and_shots(braket_circuit, shots)
 
-    return transform_to_qasm_3_program(braket_circuit, False, inputs)
+    return transform_braket_to_qasm_3_program(braket_circuit, False, inputs)
 
 
 def _convert_to_ionq(circuit: QuantumCircuit, backend: PlanqkBackend, options: Options):
     gateset = options.get("gateset", "qis")
     ionq_circ, _, _ = qiskit_circ_to_ionq_circ(circuit, gateset=gateset)
     return {
         "gateset": gateset,
@@ -58,17 +59,17 @@
 
 
 def _create_empty_input_params(circuit: Circuit, options: Options):
     return {}
 
 
 input_format_converter_factory = {
-    INPUT_FORMAT.OPEN_QASM_V3: _convert_to_open_qasm_3,
+    INPUT_FORMAT.BRAKET_OPEN_QASM_V3: _convert_to_braket_qasm_3,
     INPUT_FORMAT.IONQ_CIRCUIT_V1: _convert_to_ionq,
-    INPUT_FORMAT.QISKIT_PRIMITIVE: _convert_to_qiskit_primitive,
+    INPUT_FORMAT.QISKIT: _convert_to_qiskit_primitive,
     INPUT_FORMAT.QOQO: _convert_to_qoqo_circuit
 }
 
 input_params_factory = {
     PROVIDER.AWS: _create_aws_input_params,
     PROVIDER.QRYD: _create_qoqo_input_params
 }
```

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcp_gate.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/pcp_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcz_gate.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/pcz_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_adapter.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/qryd_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_backend.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/qryd_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_converters.py` & `planqk-quantum-2.1.0/planqk/qiskit/providers/qryd/qryd_converters.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/planqk/qiskit/runtime_provider.py` & `planqk-quantum-2.1.0/planqk/qiskit/runtime_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,37 +68,28 @@
         if options is None:
             qrt_options = RuntimeOptions()
         elif isinstance(options, Dict):
             qrt_options = RuntimeOptions(**options)
 
         qrt_options.validate(channel=self.channel)
 
-        hgp_name = 'ibm-q/open/main'  # TODO determine dynamically
-        # if self._channel == "ibm_quantum":
-        #     # Find the right hgp
-        #     hgp = self._get_hgp(instance=qrt_options.instance, backend_name=qrt_options.backend)
-        #     hgp_name = hgp.name
-        # backend = self.backend(name=qrt_options.backend, instance=hgp_name)
-        # status = backend.status()
-        # if status.operational is True and status.status_msg != "active":
-        #     logger.warning(
-        #         f"The backend {backend.name} currently has a status of {status.status_msg}."
-        #     )
+        hgp_name = 'ibm-q/open/main'
+        
         runtime_job_params = RuntimeJobParamsDto(
             program_id=program_id,
             image=qrt_options.image,
             hgp=hgp_name,
             log_level=qrt_options.log_level,
             session_id=session_id,
             max_execution_time=qrt_options.max_execution_time,
             start_session=start_session,
             session_time=qrt_options.session_time,
         )
 
-        input_data = convert_to_backend_input([INPUT_FORMAT.QISKIT_PRIMITIVE], inputs)
+        input_data = convert_to_backend_input([INPUT_FORMAT.QISKIT], inputs)
 
         backend_id = options.get('backend')
         backend = self.backend(backend_id)
 
         run_options = inputs.get('run_options')
         if run_options is None:
             shots = backend.min_shots
```

### Comparing `planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-2.1.0/planqk_quantum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.0.0rc1
+Version: 2.1.0
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-2.1.0/planqk_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0rc1/setup.py` & `planqk-quantum-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="2.0.0rc1",
+    version="2.1.0",
     author='Anaqor AG',
     author_email='info@anaqor.io',
     url='https://github.com/planqk/planqk-quantum',
     description='Python SDK for the PlanQK Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

