# Comparing `tmp/qbraid-0.6.0.dev20240405150331.tar.gz` & `tmp/qbraid-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.6.0.dev20240405150331.tar", last modified: Fri Apr  5 15:03:34 2024, max compression
+gzip compressed data, was "qbraid-0.6.1.tar", last modified: Wed Apr 10 00:39:54 2024, max compression
```

## Comparing `qbraid-0.6.0.dev20240405150331.tar` & `qbraid-0.6.1.tar`

### file list

```diff
@@ -1,174 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.887107 qbraid-0.6.0.dev20240405150331/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55271 2024-04-05 15:03:34.887107 qbraid-0.6.0.dev20240405150331/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pennylane.png
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/quantinuum.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.867107 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/batch_counts.png
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/conversion_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/hub_spokes.png
--rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/lab_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.867107 qbraid-0.6.0.dev20240405150331/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.compiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.867107 qbraid-0.6.0.dev20240405150331/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 15:03:31.000000 qbraid-0.6.0.dev20240405150331/qbraid/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/ionq.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/get_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/circuit_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/cirq_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qasm3_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qiskit_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.875107 qbraid-0.6.0.dev20240405150331/qbraid/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/abc_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.875107 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pennylane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_qelib1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/custom_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/convert_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55271 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:03:34.887107 qbraid-0.6.0.dev20240405150331/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/tools/set_provider_configs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/tools/verify_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.729268 qbraid-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-10 00:39:49.000000 qbraid-0.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-10 00:39:49.000000 qbraid-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 00:39:49.000000 qbraid-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 00:39:49.000000 qbraid-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55209 2024-04-10 00:39:54.729268 qbraid-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-10 00:39:49.000000 qbraid-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/pennylane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/quantinuum.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.705268 qbraid-0.6.1/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/batch_counts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/conversion_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/hub_spokes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/lab_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.705268 qbraid-0.6.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.compiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-10 00:39:49.000000 qbraid-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/compiler/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/braket/ionq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/get_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/circuit_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.713268 qbraid-0.6.1/qbraid/interface/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/cirq_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/qasm3_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/qiskit_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.713268 qbraid-0.6.1/qbraid/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/abc_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.713268 qbraid-0.6.1/qbraid/programs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/qasm_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/qasm_qelib1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/status_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/transpiler/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/conversions_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/custom_instr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/custom_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/conversions_cirq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/conversions_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/conversions_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.725268 qbraid-0.6.1/qbraid/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/draw_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/draw_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/plot_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/plot_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.725268 qbraid-0.6.1/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55209 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 00:39:49.000000 qbraid-0.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-10 00:39:49.000000 qbraid-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:39:54.729268 qbraid-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.725268 qbraid-0.6.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-10 00:39:49.000000 qbraid-0.6.1/tools/set_provider_configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-10 00:39:49.000000 qbraid-0.6.1/tools/verify_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-10 00:39:49.000000 qbraid-0.6.1/tox.ini
```

### Comparing `qbraid-0.6.0.dev20240405150331/CODE_OF_CONDUCT.md` & `qbraid-0.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/CONTRIBUTING.md` & `qbraid-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/LICENSE` & `qbraid-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/PKG-INFO` & `qbraid-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.6.0.dev20240405150331
+Version: 0.6.1
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,15 +699,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
-Requires-Dist: qbraid-core>=0.1.0.dev4
+Requires-Dist: qbraid-core<0.2.0,>=0.1.1
 Provides-Extra: braket
 Requires-Dist: amazon-braket-sdk<1.77.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
@@ -726,15 +726,14 @@
 Requires-Dist: cirq-ionq<1.4.0,>=1.3.0; extra == "ionq"
 Requires-Dist: pytket-braket<0.36.0,>=0.30.0; extra == "ionq"
 Provides-Extra: visualization
 Requires-Dist: ipython; extra == "visualization"
 Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: pylatexenc; extra == "visualization"
 Provides-Extra: test
-Requires-Dist: qbraid~=0.5.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
```

### Comparing `qbraid-0.6.0.dev20240405150331/README.md` & `qbraid-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/cards/jupyter.png` & `qbraid-0.6.1/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/cards/python.png` & `qbraid-0.6.1/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/cards/terminal.png` & `qbraid-0.6.1/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/favicon.ico` & `qbraid-0.6.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/logo.png` & `qbraid-0.6.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/braket.png` & `qbraid-0.6.1/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/cirq.png` & `qbraid-0.6.1/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pennylane.png` & `qbraid-0.6.1/docs/_static/pkg-logos/pennylane.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.6.1/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qasm.png` & `qbraid-0.6.1/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qir.png` & `qbraid-0.6.1/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.6.1/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/quantinuum.png` & `qbraid-0.6.1/docs/_static/pkg-logos/quantinuum.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/batch_counts.png` & `qbraid-0.6.1/docs/_static/sdk-files/batch_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/conversion_graph.png` & `qbraid-0.6.1/docs/_static/sdk-files/conversion_graph.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/get_devices.png` & `qbraid-0.6.1/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/hub_spokes.png` & `qbraid-0.6.1/docs/_static/sdk-files/hub_spokes.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/lab_jobs.png` & `qbraid-0.6.1/docs/_static/sdk-files/lab_jobs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.6.1/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/conf.py` & `qbraid-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/index.rst` & `qbraid-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/sdk/devices.rst` & `qbraid-0.6.1/docs/sdk/devices.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/sdk/jobs.rst` & `qbraid-0.6.1/docs/sdk/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/sdk/overview.rst` & `qbraid-0.6.1/docs/sdk/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/sdk/programs.rst` & `qbraid-0.6.1/docs/sdk/programs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/sdk/results.rst` & `qbraid-0.6.1/docs/sdk/results.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/docs/sdk/transpiler.rst` & `qbraid-0.6.1/docs/sdk/transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/pyproject.toml` & `qbraid-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Topic :: Scientific/Engineering :: Physics"
 ]
 dependencies = [
     "networkx>=2.5,<4.0",
     "numpy>=1.17,<1.27",
     "openqasm3[parser]>=0.4.0,<0.6.0",
     "ply>=3.6",
-    "qbraid-core>=0.1.0.dev4"
+    "qbraid-core>=0.1.1,<0.2.0"
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/en/stable/"
 "Source Code" = "https://github.com/qBraid/qBraid"
@@ -46,15 +46,15 @@
 pennylane = ["pennylane>=0.33.1,<0.36.0"]
 pytket = ["pytket>=1.16.0,<1.27.0"]
 pyquil = ["pyquil>=3.5.4,<4.4.0"]
 qir = ["qbraid-qir>=0.1.1,<0.2.0"]
 qiskit = ["qiskit>=0.44.0,<1.1.0", "qiskit-ibm-provider>=0.5.3,<0.11.0", "qiskit-ibm-runtime>=0.18.0,<0.21.0", "qiskit[visualization]"]
 ionq = ["cirq-core>=1.3.0,<1.4.0", "cirq-ionq>=1.3.0,<1.4.0", "pytket-braket>=0.30.0,<0.36.0"]
 visualization = ["ipython", "matplotlib", "pylatexenc"]
-test = ["qbraid~=0.5.3", "pytest", "pytest-cov"]
+test = ["pytest", "pytest-cov"]
 lint = ["black", "isort", "pylint"]
 docs = ["sphinx~=7.2.6", "sphinx-autodoc-typehints>=1.24,<2.1", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.21"]
 
 [project.entry-points."qbraid.programs"]
 braket = "qbraid.programs.libs.braket:BraketCircuit"
 cirq = "qbraid.programs.libs.cirq:CirqCircuit"
 pennylane = "qbraid.programs.libs.pennylane:PennylaneTape"
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/__init__.py` & `qbraid-0.6.1/qbraid/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/_about.py` & `qbraid-0.6.1/qbraid/_about.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/_compat.py` & `qbraid-0.6.1/qbraid/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/_display.py` & `qbraid-0.6.1/qbraid/_display.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/_import.py` & `qbraid-0.6.1/qbraid/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/compiler/__init__.py` & `qbraid-0.6.1/qbraid/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/__init__.py` & `qbraid-0.6.1/qbraid/compiler/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/ionq.py` & `qbraid-0.6.1/qbraid/compiler/braket/ionq.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 Module for converting generic quantum circuits to basis gate set compatible with IonQ devices.
 
 """
 from typing import Union
 
 import pytket
-import pytket.extensions.braket
 from braket.circuits import Circuit
 
 try:
     # pytket >= 1.22
     from pytket.circuit_library import TK1_to_RzRx  # type: ignore
 except (ModuleNotFoundError, ImportError):  # prama: no cover
     try:
@@ -114,20 +113,16 @@
                 PSwap
                 Unitary
 
         - Otherwise, the circuit is transpiled using ``pytket-braket``'s ``braket_to_tk``.
 
     """
     if isinstance(circuit, Circuit):
-        try:
-            tk_circuit = pytket.extensions.braket.braket_convert.braket_to_tk(circuit)
-        except NotImplementedError:
-            tk_circuit = transpile(circuit, "pytket")
+        tk_circuit = transpile(circuit, "pytket")
     else:
         tk_circuit = circuit
 
     cu = CompilationUnit(tk_circuit, preds)
     ionq_rebase_pass.apply(cu)
     if not cu.check_all_predicates():
         raise CompilerError("Circuit cannot be compiled to IonQ Harmony.")
-    compiled, _, _ = pytket.extensions.braket.braket_convert.tk_to_braket(cu.circuit)
-    return compiled
+    return transpile(cu.circuit, "braket")
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/compiler/exceptions.py` & `qbraid-0.6.1/qbraid/compiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/exceptions.py` & `qbraid-0.6.1/qbraid/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/get_devices.py` & `qbraid-0.6.1/qbraid/get_devices.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/get_jobs.py` & `qbraid-0.6.1/qbraid/get_jobs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/interface/__init__.py` & `qbraid-0.6.1/qbraid/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/interface/circuit_equality.py` & `qbraid-0.6.1/qbraid/interface/circuit_equality.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/__init__.py` & `qbraid-0.6.1/qbraid/interface/random/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/cirq_random.py` & `qbraid-0.6.1/qbraid/interface/random/cirq_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qasm3_random.py` & `qbraid-0.6.1/qbraid/interface/random/qasm3_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qiskit_random.py` & `qbraid-0.6.1/qbraid/interface/random/qiskit_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/random.py` & `qbraid-0.6.1/qbraid/interface/random/random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/__init__.py` & `qbraid-0.6.1/qbraid/programs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
    get_qasm_version
    get_program_type
    load_program
    remove_qasm_barriers
    unfold_qasm_gate_defs
    flatten_qasm_program
    decompose_qasm_qelib1
+   convert_qasm_pi_to_decimal
 
 Classes
 --------
 
 .. autosummary::
    :toctree: ../stubs/
 
@@ -56,9 +57,14 @@
 
 """
 from ._import import QPROGRAM, QPROGRAM_LIBS, QPROGRAM_TYPES, SUPPORTED_QPROGRAMS
 from .abc_program import QuantumProgram
 from .exceptions import PackageValueError, ProgramTypeError, QasmError
 from .inspector import get_program_type, get_qasm_version
 from .loader import load_program
-from .qasm_passes import flatten_qasm_program, remove_qasm_barriers, unfold_qasm_gate_defs
+from .qasm_passes import (
+    convert_qasm_pi_to_decimal,
+    flatten_qasm_program,
+    remove_qasm_barriers,
+    unfold_qasm_gate_defs,
+)
 from .qasm_qelib1 import decompose_qasm_qelib1
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/_import.py` & `qbraid-0.6.1/qbraid/programs/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/abc_program.py` & `qbraid-0.6.1/qbraid/programs/abc_program.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/exceptions.py` & `qbraid-0.6.1/qbraid/programs/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/inspector.py` & `qbraid-0.6.1/qbraid/programs/inspector.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/__init__.py` & `qbraid-0.6.1/qbraid/programs/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/braket.py` & `qbraid-0.6.1/qbraid/programs/libs/braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/cirq.py` & `qbraid-0.6.1/qbraid/programs/libs/cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pennylane.py` & `qbraid-0.6.1/qbraid/programs/libs/pennylane.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pyquil.py` & `qbraid-0.6.1/qbraid/programs/libs/pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pytket.py` & `qbraid-0.6.1/qbraid/programs/libs/pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm2.py` & `qbraid-0.6.1/qbraid/programs/libs/qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm3.py` & `qbraid-0.6.1/qbraid/programs/libs/qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qiskit.py` & `qbraid-0.6.1/qbraid/programs/libs/qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/loader.py` & `qbraid-0.6.1/qbraid/programs/loader.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_passes.py` & `qbraid-0.6.1/qbraid/programs/qasm_passes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,36 @@
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for preprocessing qasm string to before it is passed to parser.
 
 """
+import math
 import re
 
 from .qasm_qelib1 import decompose_qasm_qelib1
 
 
+def convert_qasm_pi_to_decimal(qasm_str: str) -> str:
+    """Convert all instances of 'pi' in the QASM string to their decimal value."""
+
+    pattern = r"(\d*\.?\d*\s*[*/+-]\s*)?pi(\s*[*/+-]\s*\d*\.?\d*)?"
+
+    def replace_with_decimal(match):
+        expr = match.group()
+        try:
+            value = eval(expr.replace("pi", str(math.pi)))  # pylint: disable=eval-used
+        except SyntaxError:
+            return expr
+        return str(value)
+
+    return re.sub(pattern, replace_with_decimal, qasm_str)
+
+
 def remove_qasm_barriers(qasm_str: str) -> str:
     """Returns a copy of the input QASM with all barriers removed.
 
     Args:
         qasm_str: QASM to remove barriers from.
     """
     quoted_re = r"(?:\"[^\"]*?\")"
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_qelib1.py` & `qbraid-0.6.1/qbraid/programs/qasm_qelib1.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/__init__.py` & `qbraid-0.6.1/qbraid/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/_import.py` & `qbraid-0.6.1/qbraid/providers/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/__init__.py` & `qbraid-0.6.1/qbraid/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/device.py` & `qbraid-0.6.1/qbraid/providers/aws/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/job.py` & `qbraid-0.6.1/qbraid/providers/aws/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/provider.py` & `qbraid-0.6.1/qbraid/providers/aws/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/result.py` & `qbraid-0.6.1/qbraid/providers/aws/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/tracker.py` & `qbraid-0.6.1/qbraid/providers/aws/tracker.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/device.py` & `qbraid-0.6.1/qbraid/providers/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/enums.py` & `qbraid-0.6.1/qbraid/providers/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/exceptions.py` & `qbraid-0.6.1/qbraid/providers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/__init__.py` & `qbraid-0.6.1/qbraid/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/device.py` & `qbraid-0.6.1/qbraid/providers/ibm/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/job.py` & `qbraid-0.6.1/qbraid/providers/ibm/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/provider.py` & `qbraid-0.6.1/qbraid/providers/ibm/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/result.py` & `qbraid-0.6.1/qbraid/providers/ibm/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/job.py` & `qbraid-0.6.1/qbraid/providers/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/provider.py` & `qbraid-0.6.1/qbraid/providers/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,14 @@
 class QuantumProvider(ABC):
     """
     This class is responsible for managing the interactions and
     authentications with various Quantum services.
     """
 
     @abstractmethod
-    def save_config(self):
-        """Save the current configuration."""
-
-    @abstractmethod
     def get_devices(self):
         """Return a list of backends matching the specified filtering."""
 
     @abstractmethod
     def get_device(self, device_id: str):
         """Return quantum device corresponding to the specified device ID."""
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/result.py` & `qbraid-0.6.1/qbraid/providers/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/providers/status_maps.py` & `qbraid-0.6.1/qbraid/providers/status_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/__init__.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,44 +5,31 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module providing unified conversions interface between supported
-quantum program types.
+Cirq conversions
 
-.. currentmodule:: qbraid.transpiler
+.. currentmodule:: qbraid.transpiler.conversions.cirq
 
 Classes
---------
+----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   ConversionGraph
-   Conversion
+   QasmParser
 
 Functions
------------
+----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   transpile
-
-Exceptions
------------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   CircuitConversionError
-   NodeNotFoundError
-   ConversionPathNotFoundError
+   qasm2_to_cirq
+   cirq_to_qasm2
 
 """
-from .converter import transpile
-from .edge import Conversion
-from .exceptions import CircuitConversionError, ConversionPathNotFoundError, NodeNotFoundError
-from .graph import ConversionGraph
+from .cirq_qasm_parser import QasmParser
+from .conversions_qasm import cirq_to_qasm2, qasm2_to_cirq
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/__init__.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_from_braket.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_from_braket.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,47 +29,21 @@
 from cirq import protocols
 
 try:
     import cirq_ionq.ionq_native_gates as cirq_ionq_ops
 except ImportError:
     cirq_ionq_ops = None
 
-from qbraid.transpiler.conversions.cirq.cirq_gates import matrix_gate
+from qbraid.transpiler.conversions.cirq.custom_ops import matrix_gate as matrix_to_cirq_gate
 from qbraid.transpiler.exceptions import CircuitConversionError
 
+from .custom_instr import gate_to_matrix as braket_gate_to_matrix
 
-def _gate_to_matrix_braket(gate: braket_gates.Unitary) -> np.ndarray:
-    matrix = gate.to_matrix()
-    unitary_gate = braket_gates.Unitary(matrix)
-    nqubits = int(np.log2(len(matrix)))
-    qubits = list(range(nqubits)) if nqubits > 1 else 0
-    circuit = BKCircuit([BKInstruction(unitary_gate, qubits)])
-    return circuit.to_unitary()
 
-
-def unitary_braket_instruction(instr: BKInstruction) -> BKInstruction:
-    """Converts a Braket instruction to a unitary gate instruction.
-
-    Args:
-        instr: Braket instruction to convert.
-
-    Raises:
-        CircuitConversionError: If the instruction cannot be converted
-    """
-    gate = instr.operator
-
-    try:
-        matrix = _gate_to_matrix_braket(gate)
-        gate_name = "U" if gate.name is None else gate.name
-        return BKInstruction(braket_gates.Unitary(matrix, display_name=gate_name), instr.target)
-    except (ValueError, TypeError) as err:
-        raise CircuitConversionError(f"Unable to convert the instruction {instr}.") from err
-
-
-def braket_to_cirq(circuit: BKCircuit) -> Circuit:
+def _braket_to_cirq(circuit: BKCircuit) -> Circuit:
     """Returns a Cirq circuit equivalent to the input Braket circuit.
 
     Note: The returned Cirq circuit acts on cirq.LineQubit's with indices equal
     to the qubit indices of the Braket circuit.
 
     Args:
         circuit: Braket circuit to convert to a Cirq circuit.
@@ -107,15 +81,15 @@
 
         if nqubits == 3:
             if isinstance(instr.operator, braket_gates.CCNot):
                 return [cirq_ops.TOFFOLI.on(*qubits)]
             if isinstance(instr.operator, braket_gates.CSwap):
                 return [cirq_ops.FREDKIN.on(*qubits)]
             try:
-                matrix = _gate_to_matrix_braket(instr.operator)
+                matrix = braket_gate_to_matrix(instr.operator)
                 return [cirq_ops.MatrixGate(matrix).on(*qubits)]
             except (ValueError, TypeError) as err:
                 raise CircuitConversionError(
                     f"Unable to convert the instruction {instr} to Cirq."
                 ) from err
 
         # Unknown instructions.
@@ -198,15 +172,15 @@
         return [
             cirq_ops.GeneralizedAmplitudeDampingChannel(gate.probability, gate.gamma).on(*qubits)
         ]
     if isinstance(gate, braket_noise_gate.PhaseDamping):
         return [cirq_ops.PhaseDampingChannel(gate.gamma).on(*qubits)]
 
     try:
-        matrix = _gate_to_matrix_braket(gate)
+        matrix = braket_gate_to_matrix(gate)
         return [cirq_ops.MatrixGate(matrix).on(*qubits)]
     except (ValueError, TypeError) as err:
         raise ValueError(f"Unable to convert the instruction {instr} to Cirq.") from err
 
 
 def _from_two_qubit_braket_instruction(
     instr: BKInstruction, qubits: List[LineQubit]
@@ -289,12 +263,12 @@
                 phi0=gate.angle_1 / (2 * np.pi),
                 phi1=gate.angle_2 / (2 * np.pi),
                 theta=gate.angle_3 / (2 * np.pi),
             ).on(*qubits)
         ]
 
     try:
-        matrix = _gate_to_matrix_braket(gate)
-        unitary_gate = matrix_gate(matrix)
+        matrix = braket_gate_to_matrix(gate)
+        unitary_gate = matrix_to_cirq_gate(matrix)
         return [unitary_gate.on(*qubits)]
     except (ValueError, TypeError) as err:
         raise ValueError(f"Unable to convert the instruction {instr} to Cirq.") from err
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_to_braket.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_to_braket.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,18 +34,18 @@
     import cirq_ionq.ionq_native_gates as cirq_ionq_ops
 except ImportError:
     cirq_ionq_ops = None
 
 import qbraid.programs.libs.cirq
 from qbraid.transpiler.exceptions import CircuitConversionError
 
-from .custom_gates import C as BKControl
+from .custom_instr import C as BKControl
 
 
-def cirq_to_braket(circuit: Circuit) -> BKCircuit:
+def _cirq_to_braket(circuit: Circuit) -> BKCircuit:
     """Returns a Braket circuit equivalent to the input Cirq circuit.
 
     Args:
         circuit: Cirq circuit to convert to a Braket circuit.
 
     Returns:
         Braket circuit equivalent to the input Cirq circuit.
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/custom_gates.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/braket/custom_instr.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,21 +13,51 @@
 
 """
 import itertools
 from typing import Any, List
 
 import braket.ir.jaqcd as ir
 import numpy as np
-from braket.circuits import Gate, Instruction, QubitSet, circuit
+from braket.circuits import Circuit, Gate, Instruction, QubitSet, circuit
 from braket.circuits.gates import Unitary, format_complex
 from braket.circuits.serialization import OpenQASMSerializationProperties
 
+from qbraid.transpiler.exceptions import CircuitConversionError
+
 # pylint: disable=missing-function-docstring
 
 
+def gate_to_matrix(gate: Unitary) -> np.ndarray:
+    matrix = gate.to_matrix()
+    unitary_gate = Unitary(matrix)
+    nqubits = int(np.log2(len(matrix)))
+    qubits = list(range(nqubits)) if nqubits > 1 else 0
+    bk_circuit = Circuit([Instruction(unitary_gate, qubits)])
+    return bk_circuit.to_unitary()
+
+
+def unitary_instruction(instr: Instruction) -> Instruction:
+    """Converts a Braket instruction to a unitary gate instruction.
+
+    Args:
+        instr: Braket instruction to convert.
+
+    Raises:
+        CircuitConversionError: If the instruction cannot be converted
+    """
+    gate = instr.operator
+
+    try:
+        matrix = gate_to_matrix(gate)
+        gate_name = "U" if gate.name is None else gate.name
+        return Instruction(Unitary(matrix, display_name=gate_name), instr.target)
+    except (ValueError, TypeError) as err:
+        raise CircuitConversionError(f"Unable to convert the instruction {instr}.") from err
+
+
 class C(Gate):
     """Controlled gate
     Args:
         sub_gate (Gate): Quantum Gate.
         targets (QubitSet): Target qubits.
     """
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/__init__.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,31 +5,21 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Cirq conversions
+Pennylane conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.cirq
-
-Classes
-----------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   QasmParser
+.. currentmodule:: qbraid.transpiler.conversions.pennylane
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   qasm2_to_cirq
-   cirq_to_qasm2
+   pennylane_to_qasm2
 
 """
-from qbraid.transpiler.conversions.cirq.cirq_qasm_parser import QasmParser
-from qbraid.transpiler.conversions.cirq.conversions_qasm import cirq_to_qasm2, qasm2_to_cirq
+from .conversions_qasm import pennylane_to_qasm2
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_gates.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/custom_ops.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from ply import yacc
 
 from cirq import ops, Circuit, NamedQubit, CX
 from cirq.circuits.qasm_output import QasmUGate
 from cirq.contrib.qasm_import._lexer import QasmLexer
 from cirq.contrib.qasm_import.exception import QasmException
 
-import qbraid.transpiler.conversions.cirq.cirq_gates as qbraid_cirq_gates
+import qbraid.transpiler.conversions.cirq.custom_ops as qbraid_cirq_gates
 
 # Redefined lexer tokens (4/7/21) to surpress warning:
 # Token ['IF', 'NE'] defined, but not used
 QasmLexer.tokens = [
     "FORMAT_SPEC",
     "NUMBER",
     "NATURAL_NUMBER",
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/conversions_qasm.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/conversions_qasm.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from cirq import ops
 from cirq.contrib.qasm_import.exception import QasmException as CirqQasmException
 
 from qbraid._version import __version__ as qbraid_version
 from qbraid.programs.exceptions import QasmError as QbraidQasmError
 from qbraid.programs.qasm_passes import flatten_qasm_program
 
-from .cirq_gates import _map_zpow_and_unroll
 from .cirq_qasm_parser import QasmParser
+from .custom_ops import _map_zpow_and_unroll
 
 QASMType = str
 
 
 def _to_qasm_output(
     circuit: cirq.Circuit,
     header: Optional[str] = None,
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/__init__.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,12 +20,8 @@
    :toctree: ../stubs/
 
    qasm2_to_qasm3
    openqasm3_to_qasm3
    qasm3_to_openqasm3
 
 """
-from qbraid.transpiler.conversions.openqasm3.convert_qasm import (
-    openqasm3_to_qasm3,
-    qasm2_to_qasm3,
-    qasm3_to_openqasm3,
-)
+from .conversions_qasm import openqasm3_to_qasm3, qasm2_to_qasm3, qasm3_to_openqasm3
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/convert_qasm.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/__init__.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Pennylane conversions
+PyQuil conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.pennylane
+.. currentmodule:: qbraid.transpiler.conversions.pyquil
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   pennylane_to_qasm2
+   pyquil_to_cirq
+   cirq_to_pyquil
 
 """
-from qbraid.transpiler.conversions.pennylane.conversions_qasm import pennylane_to_qasm2
+
+from .conversions_cirq import cirq_to_pyquil, pyquil_to_cirq
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/conversions_qasm.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/__init__.py` & `qbraid-0.6.1/qbraid/visualization/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,16 @@
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
-
 """
-PyQuil conversions
-
-.. currentmodule:: qbraid.transpiler.conversions.pyquil
-
-Functions
-----------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   pyquil_to_cirq
-   cirq_to_pyquil
+Module for exceptions raised by visualization tools.
 
 """
+from qbraid.exceptions import QbraidError
+
 
-from qbraid.transpiler.conversions.pyquil.conversions import cirq_to_pyquil, pyquil_to_cirq
+class VisualizationError(QbraidError):
+    """Class for errors raised when using visualization features."""
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/conversions.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/conversions_cirq.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,33 +9,41 @@
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module containing functions to convert between Cirq's circuit
 representation and pyQuil's circuit representation (Quil programs).
 
 """
-from cirq import Circuit, LineQubit
-from cirq.ops import QubitOrder
+from typing import TYPE_CHECKING
+
 from pyquil import Program
 
 from qbraid.transpiler.exceptions import CircuitConversionError
 
-from .quil_input import circuit_from_quil
-from .quil_output import QuilOutput
+if TYPE_CHECKING:
+    import cirq.circuits
+    import pyquil.quil
 
 
-def cirq_to_pyquil(circuit: Circuit) -> Program:
+def cirq_to_pyquil(circuit: "cirq.circuits.Circuit") -> "pyquil.quil.Program":
     """Returns a pyQuil Program equivalent to the input Cirq circuit.
 
     Args:
         circuit: Cirq circuit to convert to a pyQuil Program.
 
     Returns:
         pyquil.Program object equivalent to the input Cirq circuit.
     """
+    # pylint: disable=import-outside-toplevel
+    from cirq import LineQubit, QubitOrder
+
+    from .cirq_quil_output import QuilOutput
+
+    # pylint: enable=import-outside-toplevel
+
     input_qubits = circuit.all_qubits()
     max_qubit = max(input_qubits)
     # if we are using LineQubits, keep the qubit labeling the same
     if isinstance(max_qubit, LineQubit):
         qubit_range = max_qubit.x + 1
         qubit_order = LineQubit.range(qubit_range)
     # otherwise, use the default ordering (starting from zero)
@@ -48,22 +56,25 @@
         return Program(quil_str)
     except ValueError as err:
         raise CircuitConversionError(
             f"Cirq qasm converter doesn't yet support {err.args[0][32:]}."
         ) from err
 
 
-def pyquil_to_cirq(program: Program) -> Circuit:
+def pyquil_to_cirq(program: "pyquil.quil.Program") -> "cirq.circuits.Circuit":
     """Returns a Cirq circuit equivalent to the input pyQuil Program.
 
     Args:
         program: PyQuil Program to convert to a Cirq circuit.
 
     Returns:
         Cirq circuit representation equivalent to the input pyQuil Program.
     """
+    # pylint: disable-next=import-outside-toplevel
+    from .cirq_quil_input import circuit_from_quil
+
     try:
         return circuit_from_quil(program.out())
     except Exception as err:
         raise CircuitConversionError(
             "qBraid transpiler doesn't yet support pyQuil noise gates."
         ) from err
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_input.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_output.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/__init__.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/braket/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-PyTKET conversions
+Amazon Braket conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.pytket
+.. currentmodule:: qbraid.transpiler.conversions.braket
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   pytket_to_qasm2
-   qasm2_to_pytket
+   braket_to_cirq
+   cirq_to_braket
+   braket_to_qasm3
+   qasm3_to_braket
 
 """
-from qbraid.transpiler.conversions.pytket.conversions_qasm import pytket_to_qasm2, qasm2_to_pytket
+from .conversions_cirq import braket_to_cirq, cirq_to_braket
+from .conversions_qasm import braket_to_qasm3, qasm3_to_braket
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/conversions_qasm.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/pytket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/__init__.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,13 +21,8 @@
 
    qasm3_to_qiskit
    qiskit_to_qasm3
    qasm2_to_qiskit
    qiskit_to_qasm2
 
 """
-from qbraid.transpiler.conversions.qiskit.conversions_qasm import (
-    qasm2_to_qiskit,
-    qasm3_to_qiskit,
-    qiskit_to_qasm2,
-    qiskit_to_qasm3,
-)
+from .conversions_qasm import qasm2_to_qiskit, qasm3_to_qiskit, qiskit_to_qasm2, qiskit_to_qasm3
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/conversions_qasm.py` & `qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/converter.py` & `qbraid-0.6.1/qbraid/transpiler/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
+
 """
 Module for transpiling quantum programs between different quantum programming languages
 
 """
 import logging
 import warnings
 from copy import deepcopy
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/edge.py` & `qbraid-0.6.1/qbraid/transpiler/edge.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,42 +8,48 @@
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for defining custom conversions
 
 """
+import importlib
 import inspect
 from typing import TYPE_CHECKING, Any, Callable, Union
 
 from qbraid.programs import SUPPORTED_QPROGRAMS, get_program_type
 
 if TYPE_CHECKING:
     import qbraid
 
 
 class Conversion:
     """
     Class for defining and handling custom conversions between different quantum program packages.
-
     """
 
     def __init__(self, source: str, target: str, conversion_func: Callable):
         """
         Initialize a Conversion instance with source and target packages and a conversion function.
 
         Args:
             source (str): The source package from which conversion starts.
             target (str): The target package to which conversion is done.
             conversion_func (Callable): The function that performs the actual conversion.
         """
         self._source = source
         self._target = target
         self._conversion_func = conversion_func
-        self._native = self._is_native()
+        self._extras = getattr(conversion_func, "requires_extras", [])
+
+        module = inspect.getmodule(conversion_func)
+        self._native = (
+            module is not None and module.__name__.startswith("qbraid") and len(self._extras) == 0
+        )
+        self._supported = self._check_supported()
 
     @property
     def source(self) -> str:
         """
         The source package of the conversion.
 
         Returns:
@@ -67,31 +73,39 @@
         True if the conversion function is native to qbraid package, False otherwise.
 
         Returns:
             bool: Whether the conversion function is native to qbraid package.
         """
         return self._native
 
-    def _is_native(self) -> bool:
+    @property
+    def supported(self) -> bool:
         """
-        Check if a conversion function is native to qbraid package.
-
-        Args:
-            func (Callable): The conversion function to check.
+        True if all packages required to perform the conversion are installed. False otherwise.
 
         Returns:
-            bool: True if the function is native, False otherwise.
+            bool: Whether the conversion function supported in the current runtime environment.
         """
-        module = inspect.getmodule(self._conversion_func)
+        return self._supported
 
-        if module is None:
-            return False
+    def _check_supported(self) -> bool:
+        """
+        Determine if the required packages for the conversion are installed.
 
-        package = module.__name__.split(".")[0]
-        return package == "qbraid"
+        Returns:
+            bool: True if supported, otherwise False.
+        """
+        if self._native:
+            return True
+        for extra in self._extras:
+            try:
+                importlib.import_module(extra)
+            except ImportError:
+                return False
+        return True
 
     def convert(
         self, program: "qbraid.programs.QPROGRAM"
     ) -> Union["qbraid.programs.QPROGRAM", Any]:
         """
         Convert a quantum program from the source package to the target package.
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/exceptions.py` & `qbraid-0.6.1/qbraid/transpiler/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
+
 """
 Module defining exceptions for errors raised during conversions
 
 """
 from typing import List, Optional
 
 from qbraid.exceptions import QbraidError
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/graph.py` & `qbraid-0.6.1/qbraid/transpiler/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,28 @@
 
 class ConversionGraph(nx.DiGraph):
     """
     Class for coordinating conversions between different quantum software programs
 
     """
 
-    def __init__(self, conversions: Optional[List[Conversion]] = None):
+    def __init__(
+        self, conversions: Optional[List[Conversion]] = None, requires_extras: bool = False
+    ):
         """
         Initialize a ConversionGraph instance.
 
         Args:
             conversions (optional, List[Conversion]): List of conversion edges. If None, default
                                                           conversion edges are created.
+            requires_extras (bool): If True, include unsupported "requires_extras" conversion
+                                    functions. Defaults to False.
         """
         super().__init__()
+        self.requires_extras = requires_extras
         self._conversions = conversions or self.load_default_conversions()
         self.create_conversion_graph()
 
     @staticmethod
     def load_default_conversions() -> List[Conversion]:
         """
         Create a list of default conversion nodes using predefined conversion functions.
@@ -59,14 +64,16 @@
         """
         Create a directed graph from a list of conversion functions.
 
         Returns:
             None
         """
         for edge in self._conversions:
+            if not self.requires_extras and not edge.supported:
+                continue
             self.add_edge(edge.source, edge.target, native=edge.native, func=edge.convert)
 
     def conversions(self) -> List[Conversion]:
         """
         Get the list of conversion edges.
 
         Returns:
@@ -98,14 +105,27 @@
             if old_edge.source == source and old_edge.target == target:
                 self._conversions.remove(old_edge)
                 break
 
         self._conversions.append(edge)
         self.add_edge(source, target, native=edge.native, func=edge.convert)
 
+    def remove_conversion(self, source: str, target: str) -> None:
+        """Safely remove a conversion from the graph."""
+        try:
+            self.remove_edge(source, target)
+        except nx.NetworkXError as err:
+            raise ValueError(f"Conversion from {source} to {target} does not exist.") from err
+
+        self._conversions = [
+            conv
+            for conv in self._conversions.copy()
+            if not (conv.source == source and conv.target == target)
+        ]
+
     def find_shortest_conversion_path(self, source: str, target: str) -> List[str]:
         """
         Find the shortest conversion path between two nodes in a graph.
 
         Args:
             source (str): The starting node for the path.
             target (str): The target node for the path.
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/visualization/__init__.py` & `qbraid-0.6.1/qbraid/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_circuit.py` & `qbraid-0.6.1/qbraid/visualization/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_qasm3.py` & `qbraid-0.6.1/qbraid/visualization/draw_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/visualization/exceptions.py` & `qbraid-0.6.1/qbraid/_version.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
-"""
-Module for exceptions raised by visualization tools.
 
 """
-from qbraid.exceptions import QbraidError
+Module containing version information
 
+Version number (major.minor.patch[-label])
 
-class VisualizationError(QbraidError):
-    """Class for errors raised when using visualization features."""
+"""
+__version__ = "0.6.1"
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_conversions.py` & `qbraid-0.6.1/qbraid/visualization/plot_conversions.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     # Set default colors if not provided
     if colors is None:
         colors = {
             "qbraid_node": "lightblue",
             "external_node": "lightgray",
             "qbraid_edge": "gray",
             "external_edge": "blue",
+            "extras_edge": "red",
         }
 
     # Extract colors and apply them in the drawing
     ncolors = [
         colors["qbraid_node"] if node in QPROGRAM_LIBS else colors["external_node"]
         for node in graph.nodes()
     ]
@@ -79,15 +80,15 @@
         for edge in graph.edges()
         if (edge[0], edge[1]) in conversion_dict
     ]
     ecolors = [
         (
             colors["qbraid_edge"]
             if graph[edge.source][edge.target]["native"]
-            else colors["external_edge"]
+            else colors["external_edge"] if edge.supported else colors["extras_edge"]
         )
         for edge in conversions_ordered
     ]
 
     pos = nx.spring_layout(graph, seed=seed)  # good seeds: 123, 134
     nx.draw_networkx_nodes(graph, pos, node_color=ncolors, node_size=node_size)
     nx.draw_networkx_edges(graph, pos, edge_color=ecolors, min_target_margin=min_target_margin)
@@ -99,14 +100,15 @@
 
     if legend:
         # Create legend elements using a loop
         legend_info = [
             ("qBraid - Node", "o", colors["qbraid_node"], None),
             ("External - Node", "o", colors["external_node"], None),
             ("qBraid - Edge", None, colors["qbraid_edge"], "-"),
+            ("Extras - Edge", None, colors["extras_edge"], "-"),
             ("External - Edge", None, colors["external_edge"], "-"),
         ]
         legend_elements = [
             plt.Line2D(
                 [0],
                 [0],
                 marker=marker,
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_counts.py` & `qbraid-0.6.1/qbraid/visualization/plot_counts.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/PKG-INFO` & `qbraid-0.6.1/qbraid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.6.0.dev20240405150331
+Version: 0.6.1
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,15 +699,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
-Requires-Dist: qbraid-core>=0.1.0.dev4
+Requires-Dist: qbraid-core<0.2.0,>=0.1.1
 Provides-Extra: braket
 Requires-Dist: amazon-braket-sdk<1.77.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
@@ -726,15 +726,14 @@
 Requires-Dist: cirq-ionq<1.4.0,>=1.3.0; extra == "ionq"
 Requires-Dist: pytket-braket<0.36.0,>=0.30.0; extra == "ionq"
 Provides-Extra: visualization
 Requires-Dist: ipython; extra == "visualization"
 Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: pylatexenc; extra == "visualization"
 Provides-Extra: test
-Requires-Dist: qbraid~=0.5.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/SOURCES.txt` & `qbraid-0.6.1/qbraid.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -102,39 +102,43 @@
 qbraid/providers/aws/tracker.py
 qbraid/providers/ibm/__init__.py
 qbraid/providers/ibm/device.py
 qbraid/providers/ibm/job.py
 qbraid/providers/ibm/provider.py
 qbraid/providers/ibm/result.py
 qbraid/transpiler/__init__.py
+qbraid/transpiler/annotations.py
 qbraid/transpiler/converter.py
 qbraid/transpiler/edge.py
 qbraid/transpiler/exceptions.py
 qbraid/transpiler/graph.py
 qbraid/transpiler/conversions/__init__.py
 qbraid/transpiler/conversions/braket/__init__.py
 qbraid/transpiler/conversions/braket/cirq_from_braket.py
 qbraid/transpiler/conversions/braket/cirq_to_braket.py
+qbraid/transpiler/conversions/braket/conversions_cirq.py
 qbraid/transpiler/conversions/braket/conversions_qasm.py
-qbraid/transpiler/conversions/braket/custom_gates.py
+qbraid/transpiler/conversions/braket/custom_instr.py
 qbraid/transpiler/conversions/cirq/__init__.py
-qbraid/transpiler/conversions/cirq/cirq_gates.py
 qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
 qbraid/transpiler/conversions/cirq/conversions_qasm.py
+qbraid/transpiler/conversions/cirq/custom_ops.py
 qbraid/transpiler/conversions/openqasm3/__init__.py
-qbraid/transpiler/conversions/openqasm3/convert_qasm.py
+qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
 qbraid/transpiler/conversions/pennylane/__init__.py
 qbraid/transpiler/conversions/pennylane/conversions_qasm.py
 qbraid/transpiler/conversions/pyquil/__init__.py
-qbraid/transpiler/conversions/pyquil/conversions.py
-qbraid/transpiler/conversions/pyquil/quil_input.py
-qbraid/transpiler/conversions/pyquil/quil_output.py
+qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
+qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
+qbraid/transpiler/conversions/pyquil/conversions_cirq.py
 qbraid/transpiler/conversions/pytket/__init__.py
+qbraid/transpiler/conversions/pytket/conversions_braket.py
 qbraid/transpiler/conversions/pytket/conversions_qasm.py
 qbraid/transpiler/conversions/qiskit/__init__.py
+qbraid/transpiler/conversions/qiskit/conversions_braket.py
 qbraid/transpiler/conversions/qiskit/conversions_qasm.py
 qbraid/visualization/__init__.py
 qbraid/visualization/draw_circuit.py
 qbraid/visualization/draw_qasm3.py
 qbraid/visualization/exceptions.py
 qbraid/visualization/plot_conversions.py
 qbraid/visualization/plot_counts.py
```

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/entry_points.txt` & `qbraid-0.6.1/qbraid.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/requires.txt` & `qbraid-0.6.1/qbraid.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 networkx<4.0,>=2.5
 numpy<1.27,>=1.17
 openqasm3[parser]<0.6.0,>=0.4.0
 ply>=3.6
-qbraid-core>=0.1.0.dev4
+qbraid-core<0.2.0,>=0.1.1
 
 [braket]
 amazon-braket-sdk<1.77.0,>=1.42.1
 
 [cirq]
 cirq-core<1.4.0,>=1.3.0
 
@@ -41,15 +41,14 @@
 [qiskit]
 qiskit<1.1.0,>=0.44.0
 qiskit-ibm-provider<0.11.0,>=0.5.3
 qiskit-ibm-runtime<0.21.0,>=0.18.0
 qiskit[visualization]
 
 [test]
-qbraid~=0.5.3
 pytest
 pytest-cov
 
 [visualization]
 ipython
 matplotlib
 pylatexenc
```

### Comparing `qbraid-0.6.0.dev20240405150331/tools/set_provider_configs.py` & `qbraid-0.6.1/tools/set_provider_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 def qbraid_configure(api_key: Optional[str] = None) -> None:
     """Initializes qBraid configuration and credentials files."""
     api_key = api_key or os.getenv("QBRAID_API_KEY", "MYAPIKEY")
     session = QbraidSession(api_key=api_key)
     session.save_config()
 
 
-def ibm_configure(token: Optional[str] = None) -> None:
+def ibm_configure(token: Optional[str] = None, overwrite: bool = True, **kwargs) -> None:
     """Initializes IBM Quantum configuration and credentials files."""
     token = token or os.getenv("QISKIT_IBM_TOKEN", "MYTOKEN")
-    IBMProvider.save_account(token=token)
+    IBMProvider.save_account(token=token, overwrite=overwrite, **kwargs)
 
 
 def aws_configure(
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     region: Optional[str] = None,
 ) -> None:
```

### Comparing `qbraid-0.6.0.dev20240405150331/tools/verify_headers.py` & `qbraid-0.6.1/tools/verify_headers.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240405150331/tox.ini` & `qbraid-0.6.1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     unit-tests
     docs
     linters
     format-check
 skip_missing_interpreter = true
 
 [testenv]
-package = editable-legacy
+commands_pre = python -m pip install --editable .
 basepython = python3
 deps =
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/requirements-dev.txt
 pass_env =
     QBRAID_API_KEY
     AWS_ACCESS_KEY_ID
@@ -32,17 +32,17 @@
                               tests/visualization \
                               tests/top_level \
                            -W ignore::DeprecationWarning \
                            -W ignore::PendingDeprecationWarning \
                            -W ignore::urllib3.exceptions.InsecureRequestWarning \
                            -W ignore::RuntimeWarning
     coverage combine
-    coverage report --omit=qbraid/transpiler/conversions/cirq/cirq_gates.py, \
-                           qbraid/visualization/draw_circuit.py, \
-                           qbraid/visualization/plot_conversions.py, \
+    coverage report --omit=qbraid/transpiler/conversions/cirq/custom_ops.py \
+                           qbraid/visualization/draw_circuit.py \
+                           qbraid/visualization/plot_conversions.py \
                            qbraid/_compat.py
     coverage html
     coverage xml
 
 [testenv:docs]
 description = Use sphinx to build the HTML docs.
 extras =
```

