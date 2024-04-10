# Comparing `tmp/pytket-phir-0.6.3.tar.gz` & `tmp/pytket-phir-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-phir-0.6.3.tar", last modified: Tue Apr  2 14:50:35 2024, max compression
+gzip compressed data, was "pytket-phir-0.7.0.tar", last modified: Wed Apr 10 15:52:49 2024, max compression
```

## Comparing `pytket-phir-0.6.3.tar` & `pytket-phir-0.7.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/workflows/pre-commit-au.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/pytket.phir.rebasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/pytket.phir.rst
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/pytket.phir.sharding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.123381 pytket-phir-0.6.3/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.131381 pytket-phir-0.6.3/pytket/phir/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    14653 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/phirgen_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/place_and_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/qtm_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.131381 pytket-phir-0.6.3/pytket/phir/rebasing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/rebasing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/rebasing/rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.131381 pytket-phir-0.6.3/pytket/phir/sharding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/shard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/shards2ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/pytket_phir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.135382 pytket-phir-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.123381 pytket-phir-0.6.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/tests/data/qasm/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/arbitrary_qreg_names.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/baby.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/baby_with_rollup.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/barrier_complex.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/big_gate.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/bv_n10.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/classical_hazards.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/classical_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/cond_1.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/cond_barrier.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/cond_classical.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/exec_order_two_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/eztest.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/group_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/n10_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/oned_brickwork_circuit_n20.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/parallelization_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/qv20_0.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/rxrz.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/rz_exec_order_three_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/simple.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/simple_cond.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/single_qubit_parallel_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/sleep.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/tk2_diff_angles.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/tk2_same_angle.qasm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/tests/data/wasm/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/wasm/add.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/wasm/testfile.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/e2e_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_parallel_tk2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_parallelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_wasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/workflows/pre-commit-au.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/pytket.phir.rebasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/pytket.phir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/pytket.phir.sharding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.898992 pytket-phir-0.7.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.906992 pytket-phir-0.7.0/pytket/phir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/phirgen_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/place_and_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/qtm_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.906992 pytket-phir-0.7.0/pytket/phir/rebasing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/rebasing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/rebasing/rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.906992 pytket-phir-0.7.0/pytket/phir/sharding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/shard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/shards2ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/pytket_phir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.910992 pytket-phir-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/tests/data/qasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/arbitrary_qreg_names.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/baby.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/baby_with_rollup.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/barrier_complex.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/big_gate.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/bv_n10.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/classical_hazards.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/classical_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/cond_1.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/cond_barrier.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/cond_classical.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/exec_order_two_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/eztest.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/group_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/n10_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/oned_brickwork_circuit_n20.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/parallelization_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/qv20_0.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/rxrz.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/rz_exec_order_three_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/simple.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/simple_cond.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/single_qubit_parallel_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/sleep.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/tk2_diff_angles.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/tk2_same_angle.qasm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/tests/data/wasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/wasm/add.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/wasm/testfile.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_parallel_tk2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_parallelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_wasm.py
```

### Comparing `pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md` & `pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/.github/pull_request_template.md` & `pytket-phir-0.7.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/.github/workflows/pre-commit-au.yml` & `pytket-phir-0.7.0/.github/workflows/pre-commit-au.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/.github/workflows/python-app.yml` & `pytket-phir-0.7.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/.github/workflows/python-publish.yml` & `pytket-phir-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/.gitignore` & `pytket-phir-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/CHANGELOG.md` & `pytket-phir-0.7.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.7.0] - 2024-04-10
+
+### Added
+
+* PHIR generation for `ExplicitPredicate`, `ExplicitModifier`, `MultiBitOp` in https://github.com/CQCL/pytket-phir/pull/162
+  * Also fixes a bug with handling conditional ops
+
 ## [0.6.3] - 2024-04-02
 
 ### Fixed
 
 * wasm/phirgen: correct arguments for conditional wasm functions in https://github.com/CQCL/pytket-phir/pull/157
 
 ## [0.6.2] - 2024-03-27
@@ -167,10 +174,11 @@
 [0.4.4]: https://github.com/CQCL/pytket-phir/compare/v0.4.3...v0.4.4
 [0.5.0]: https://github.com/CQCL/pytket-phir/compare/v0.4.4...v0.5.0
 [0.5.1]: https://github.com/CQCL/pytket-phir/compare/v0.5.0...v0.5.1
 [0.6.0]: https://github.com/CQCL/pytket-phir/compare/v0.5.1...v0.6.0
 [0.6.1]: https://github.com/CQCL/pytket-phir/compare/v0.6.0...v0.6.1
 [0.6.2]: https://github.com/CQCL/pytket-phir/compare/v0.6.1...v0.6.2
 [0.6.3]: https://github.com/CQCL/pytket-phir/compare/v0.6.2...v0.6.3
-[unreleased]: https://github.com/CQCL/pytket-phir/compare/v0.6.3...HEAD
+[0.7.0]: https://github.com/CQCL/pytket-phir/compare/v0.6.3...v0.7.0
+[unreleased]: https://github.com/CQCL/pytket-phir/compare/v0.7.0...HEAD
 
 <!-- markdownlint-configure-file {"MD024": {"siblings_only" : true}, "MD034": false} -->
```

### Comparing `pytket-phir-0.6.3/LICENSE` & `pytket-phir-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/PKG-INFO` & `pytket-phir-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.6.3
+Version: 0.7.0
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket-phir-0.6.3/README.md` & `pytket-phir-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/docs/Makefile` & `pytket-phir-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/docs/source/conf.py` & `pytket-phir-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/docs/source/index.rst` & `pytket-phir-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/docs/source/pytket.phir.rst` & `pytket-phir-0.7.0/docs/source/pytket.phir.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/docs/source/pytket.phir.sharding.rst` & `pytket-phir-0.7.0/docs/source/pytket.phir.sharding.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pyproject.toml` & `pytket-phir-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -61,10 +61,7 @@
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.setuptools_scm]
 version_scheme = "python-simplified-semver"
 
 [tool.refurb]
 python_version = "3.10"
-
-[tool.typos]
-default.extend-words = { lst = "lst" }
```

### Comparing `pytket-phir-0.6.3/pytket/phir/api.py` & `pytket-phir-0.7.0/pytket/phir/api.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/cli.py` & `pytket-phir-0.7.0/pytket/phir/cli.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/machine.py` & `pytket-phir-0.7.0/pytket/phir/machine.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/phirgen.py` & `pytket-phir-0.7.0/pytket/phir/phirgen.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 ##############################################################################
 
 # mypy: disable-error-code="misc"
 
 import json
 import logging
+from copy import deepcopy
 from importlib.metadata import version
 from typing import TYPE_CHECKING, Any, TypeAlias
 
 from typing_extensions import assert_never
 
 import pytket.circuit as tk
 from phir.model import PHIRModel
@@ -214,21 +215,163 @@
                 "qop": gate,
                 "angles": angles,
                 "args": [arg_to_bit(cmd.qubits[0])],
             }
     return qop
 
 
+def cop_from_op_name(op_name: str) -> str:
+    """Get PHIR classical op name from pytket op name."""
+    match op_name:
+        case "AND":
+            cop = "&"
+        case "OR":
+            cop = "|"
+        case "XOR":
+            cop = "^"
+        case "NOT":
+            cop = "~"
+        case name:
+            raise NotImplementedError(name)
+    return cop
+
+
+def convert_classicalevalop(op: tk.ClassicalEvalOp, cmd: tk.Command) -> JsonDict | None:
+    """Return PHIR dict for a pytket ClassicalEvalOp."""
+    # Exclude conditional bits from args
+    args = cmd.args[cmd.op.width :] if isinstance(cmd.op, tk.Conditional) else cmd.args
+    out: JsonDict | None = None
+    match op:
+        case tk.CopyBitsOp():
+            if len(cmd.bits) != len(args) // 2:
+                msg = "LHS and RHS lengths mismatch for CopyBits"
+                raise TypeError(msg)
+            out = assign_cop(
+                [arg_to_bit(bit) for bit in cmd.bits],
+                [arg_to_bit(args[i]) for i in range(len(args) // 2)],
+            )
+        case tk.SetBitsOp():
+            if len(cmd.bits) != len(op.values):
+                logger.error("LHS and RHS lengths mismatch for classical assignment")
+                raise ValueError
+            out = assign_cop(
+                [arg_to_bit(bit) for bit in cmd.bits], list(map(int, op.values))
+            )
+        case tk.RangePredicateOp():  # where the condition is a range
+            cond: JsonDict
+            match op.lower, op.upper:
+                case l, u if l == u:
+                    cond = {
+                        "cop": "==",
+                        "args": [args[0].reg_name, u],
+                    }
+                case l, u if u == UINTMAX:
+                    cond = {
+                        "cop": ">=",
+                        "args": [args[0].reg_name, l],
+                    }
+                case 0, u:
+                    cond = {
+                        "cop": "<=",
+                        "args": [args[0].reg_name, u],
+                    }
+            out = {
+                "block": "if",
+                "condition": cond,
+                "true_branch": [assign_cop([arg_to_bit(cmd.bits[0])], [1])],
+            }
+        case tk.MultiBitOp():
+            if len(args) % len(cmd.bits) != 0:
+                msg = "Input bit- and output bit lengths mismatch."
+                raise TypeError(msg)
+
+            cop = cop_from_op_name(op.basic_op.get_name())
+            is_explicit = op.basic_op.type == tk.OpType.ExplicitPredicate
+
+            # determine number of register operands involved in the operation
+            operand_count = len(args) // len(cmd.bits) - is_explicit
+
+            iters = [iter(args)] * (operand_count + is_explicit)
+            iter2 = deepcopy(iters)
+
+            # Columns of expressions, e.g.,
+            #   AND (*2) a[0], b[0], c[0]
+            #          , a[1], b[1], c[1]
+            #   would be [(a[0], a[1]), (b[0], b[1]), (c[0], c[1])]
+            # and AND (*2) a[0], a[1], b[0]
+            #            , b[1], c[0], c[1]
+            #   would be [(a[0], b[1]), (a[1], c[0]), (b[0], c[1])]
+            cols = zip(*zip(*iters, strict=True), strict=True)
+
+            if all(
+                all(col[0].reg_name == bit.reg_name for bit in col) for col in cols
+            ):  # expression can be applied register-wise
+                out = assign_cop(
+                    [cmd.bits[0].reg_name],
+                    [
+                        {
+                            "cop": cop,
+                            "args": [arg.reg_name for arg in args[:operand_count]],
+                        }
+                    ],
+                )
+            else:  # apply a sequence of bit-wise ops
+                exps = zip(*iter2, strict=True)
+                out = {
+                    "block": "sequence",
+                    "ops": [
+                        assign_cop(
+                            [arg_to_bit(bit)],
+                            [
+                                {
+                                    "cop": cop,
+                                    "args": [
+                                        arg_to_bit(arg) for arg in exp[:operand_count]
+                                    ],
+                                }
+                            ],
+                        )
+                        for bit, exp in zip(cmd.bits, exps, strict=True)
+                    ],
+                }
+        case _:
+            raise NotImplementedError(op)
+
+    return out
+
+
+def multi_bit_condition(args: "list[UnitID]", value: int) -> JsonDict:
+    """Construct bitwise condition."""
+    return {
+        "cop": "&",
+        "args": [
+            {"cop": "==", "args": [arg_to_bit(arg), bval]}
+            for (arg, bval) in zip(
+                args[::-1], map(int, f"{value:0{len(args)}b}"), strict=True
+            )
+        ],
+    }
+
+
 def convert_subcmd(op: tk.Op, cmd: tk.Command) -> JsonDict | None:
     """Return PHIR dict given a tket op and its arguments."""
     if op.is_gate():
         return convert_gate(op, cmd)
 
     out: JsonDict | None = None
     match op:  # non-quantum op
+        case tk.Conditional():
+            out = {
+                "block": "if",
+                "condition": {"cop": "==", "args": [arg_to_bit(cmd.args[0]), op.value]}
+                if op.width == 1
+                else multi_bit_condition(cmd.args[: op.width], op.value),
+                "true_branch": [convert_subcmd(op.op, cmd)],
+            }
+
         case tk.BarrierOp():
             if op.data:
                 # See https://github.com/CQCL/tket/blob/0ec603986821d994caa3a0fb9c4640e5bc6c0a24/pytket/pytket/qasm/qasm.py#L419-L459
                 match op.data[0:5]:
                     case "sleep":
                         duration = op.data.removeprefix("sleep(").removesuffix(")")
                         out = {
@@ -242,86 +385,52 @@
                         raise TypeError(op.data)
             else:
                 out = {
                     "meta": "barrier",
                     "args": [arg_to_bit(qbit) for qbit in cmd.qubits],
                 }
 
-        case tk.Conditional():  # where the condition is equality check
-            out = {
-                "block": "if",
-                "condition": {
-                    "cop": "==",
-                    "args": [
-                        arg_to_bit(cmd.args[0])
-                        if op.width == 1
-                        else cmd.args[0].reg_name,
-                        op.value,
-                    ],
-                },
-                "true_branch": [convert_subcmd(op.op, cmd)],
-            }
-
-        case tk.RangePredicateOp():  # where the condition is a range
-            cond: JsonDict
-            match op.lower, op.upper:
-                case l, u if l == u:
-                    cond = {
-                        "cop": "==",
-                        "args": [cmd.args[0].reg_name, u],
-                    }
-                case l, u if u == UINTMAX:
-                    cond = {
-                        "cop": ">=",
-                        "args": [cmd.args[0].reg_name, l],
-                    }
-                case 0, u:
-                    cond = {
-                        "cop": "<=",
-                        "args": [cmd.args[0].reg_name, u],
-                    }
-            out = {
-                "block": "if",
-                "condition": cond,
-                "true_branch": [assign_cop([arg_to_bit(cmd.bits[0])], [1])],
-            }
-
         case tk.ClassicalExpBox():
             exp = op.get_exp()
             match exp:
                 case BitLogicExp():
                     rhs = [classical_op(exp, bitwise=True)]
                     out = assign_cop([arg_to_bit(cmd.bits[0])], rhs)
                 case RegLogicExp():
                     rhs = [classical_op(exp)]
                     out = assign_cop([cmd.bits[0].reg_name], rhs)
 
-        case tk.SetBitsOp():
-            if len(cmd.bits) != len(op.values):
-                logger.error("LHS and RHS lengths mismatch for classical assignment")
-                raise ValueError
-            out = assign_cop(
-                [arg_to_bit(bit) for bit in cmd.bits], list(map(int, op.values))
-            )
-
-        case tk.CopyBitsOp():
-            if len(cmd.bits) != len(cmd.args) // 2:
-                logger.warning("LHS and RHS lengths mismatch for CopyBits")
-            out = assign_cop(
-                [arg_to_bit(bit) for bit in cmd.bits],
-                [arg_to_bit(cmd.args[i]) for i in range(len(cmd.args) // 2)],
-            )
+        case tk.ClassicalEvalOp():
+            return convert_classicalevalop(op, cmd)
 
         case tk.WASMOp():
             return create_wasm_op(cmd, op)
 
         case _:
-            # TODO(kartik): NYI
-            # https://github.com/CQCL/pytket-phir/issues/25
-            raise NotImplementedError
+            # Exclude conditional bits from args
+            args = (
+                cmd.args[cmd.op.width :]
+                if isinstance(cmd.op, tk.Conditional)
+                else cmd.args
+            )
+            match op.type:
+                case tk.OpType.ExplicitPredicate | tk.OpType.ExplicitModifier:
+                    # exclude output bit when not modifying in place
+                    args = args[:-1] if op.type == tk.OpType.ExplicitPredicate else args
+                    out = assign_cop(
+                        [arg_to_bit(cmd.bits[0])],
+                        [
+                            {
+                                "cop": cop_from_op_name(op.get_name()),
+                                "args": [arg_to_bit(arg) for arg in args],
+                            }
+                        ],
+                    )
+                case _:
+                    raise NotImplementedError(op.type)
 
     return out
 
 
 def append_cmd(cmd: tk.Command, ops: list[JsonDict]) -> None:
     """Convert a pytket command to a PHIR command and append to `ops`.
```

### Comparing `pytket-phir-0.6.3/pytket/phir/phirgen_parallel.py` & `pytket-phir-0.7.0/pytket/phir/phirgen_parallel.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/place_and_route.py` & `pytket-phir-0.7.0/pytket/phir/place_and_route.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/placement.py` & `pytket-phir-0.7.0/pytket/phir/placement.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/qtm_machine.py` & `pytket-phir-0.7.0/pytket/phir/qtm_machine.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/rebasing/rebaser.py` & `pytket-phir-0.7.0/pytket/phir/rebasing/rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/routing.py` & `pytket-phir-0.7.0/pytket/phir/routing.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/sharding/shard.py` & `pytket-phir-0.7.0/pytket/phir/sharding/shard.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket/phir/sharding/sharder.py` & `pytket-phir-0.7.0/pytket/phir/sharding/sharder.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     OpType.Measure,
     OpType.Reset,
     OpType.Barrier,
     OpType.SetBits,
     OpType.ClassicalExpBox,  # some classical operations are rolled up into a box
     OpType.RangePredicate,
     OpType.ExplicitPredicate,
+    OpType.ExplicitModifier,
+    OpType.MultiBit,
     OpType.CopyBits,
     OpType.WASM,
 ]
 
 logger = logging.getLogger(__name__)
```

### Comparing `pytket-phir-0.6.3/pytket/phir/sharding/shards2ops.py` & `pytket-phir-0.7.0/pytket/phir/sharding/shards2ops.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/pytket_phir.egg-info/PKG-INFO` & `pytket-phir-0.7.0/pytket_phir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.6.3
+Version: 0.7.0
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket-phir-0.6.3/pytket_phir.egg-info/SOURCES.txt` & `pytket-phir-0.7.0/pytket_phir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/data/qasm/arbitrary_qreg_names.qasm` & `pytket-phir-0.7.0/tests/data/qasm/arbitrary_qreg_names.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/data/qasm/bv_n10.qasm` & `pytket-phir-0.7.0/tests/data/qasm/bv_n10.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/data/qasm/oned_brickwork_circuit_n20.qasm` & `pytket-phir-0.7.0/tests/data/qasm/oned_brickwork_circuit_n20.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/data/qasm/qv20_0.qasm` & `pytket-phir-0.7.0/tests/data/qasm/qv20_0.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/data/wasm/add.wat` & `pytket-phir-0.7.0/tests/data/wasm/add.wat`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/data/wasm/testfile.wat` & `pytket-phir-0.7.0/tests/data/wasm/testfile.wat`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/e2e_test.py` & `pytket-phir-0.7.0/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/test_api.py` & `pytket-phir-0.7.0/tests/test_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 # Use of this source code is governed by a BSD-style
 # license that can be found in the LICENSE file.
 #
 ##############################################################################
 
 # mypy: disable-error-code="misc"
 
-import json
 import logging
 
 import pytest
 
-from pytket.circuit import Bit, Circuit
 from pytket.phir.api import pytket_to_phir, qasm_to_phir
 from pytket.phir.qtm_machine import QtmMachine
 
 from .test_utils import QasmFile, get_qasm_as_circuit
 
 logger = logging.getLogger(__name__)
 
@@ -46,35 +44,14 @@
     @pytest.mark.parametrize("test_file", list(QasmFile))
     def test_pytket_to_phir_h1_1_all(self, test_file: QasmFile) -> None:
         """Standard case."""
         circuit = get_qasm_as_circuit(test_file)
 
         assert pytket_to_phir(circuit, QtmMachine.H1)
 
-    def test_pytket_classical_only(self) -> None:
-        c = Circuit(1)
-        a = c.add_c_register("a", 2)
-        b = c.add_c_register("b", 3)
-
-        c.add_c_copyreg(a, b)
-        c.add_c_copybits([Bit("b", 2), Bit("a", 1)], [Bit("a", 0), Bit("b", 0)])
-
-        phir = json.loads(pytket_to_phir(c))
-
-        assert phir["ops"][3] == {
-            "cop": "=",
-            "returns": [["b", 0], ["b", 1]],
-            "args": [["a", 0], ["a", 1]],
-        }
-        assert phir["ops"][5] == {
-            "cop": "=",
-            "returns": [["a", 0], ["b", 0]],
-            "args": [["b", 2], ["a", 1]],
-        }
-
     def test_qasm_to_phir(self) -> None:
         """Test the qasm string entrypoint works."""
         qasm = """
         OPENQASM 2.0;
         include "qelib1.inc";
 
         qreg q[3];
```

### Comparing `pytket-phir-0.6.3/tests/test_parallel_tk2.py` & `pytket-phir-0.7.0/tests/test_parallel_tk2.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/test_parallelization.py` & `pytket-phir-0.7.0/tests/test_parallelization.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/test_placement.py` & `pytket-phir-0.7.0/tests/test_placement.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/test_rebaser.py` & `pytket-phir-0.7.0/tests/test_rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/test_sharder.py` & `pytket-phir-0.7.0/tests/test_sharder.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/test_utils.py` & `pytket-phir-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.3/tests/test_wasm.py` & `pytket-phir-0.7.0/tests/test_wasm.py`

 * *Files identical despite different names*

