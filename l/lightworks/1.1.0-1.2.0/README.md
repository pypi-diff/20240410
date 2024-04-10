# Comparing `tmp/lightworks-1.1.0.tar.gz` & `tmp/lightworks-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightworks-1.1.0.tar", last modified: Thu Mar 21 10:31:48 2024, max compression
+gzip compressed data, was "lightworks-1.2.0.tar", last modified: Wed Apr 10 10:00:07 2024, max compression
```

## Comparing `lightworks-1.1.0.tar` & `lightworks-1.2.0.tar`

### file list

```diff
@@ -1,96 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.836816 lightworks-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-21 10:31:41.000000 lightworks-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-03-21 10:31:48.836816 lightworks-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-21 10:31:41.000000 lightworks-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.824816 lightworks-1.1.0/lightworks/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/__version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.824816 lightworks-1.1.0/lightworks/emulator/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.824816 lightworks-1.1.0/lightworks/emulator/annotated_state/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/annotated_state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/annotated_state/annotated_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.828816 lightworks-1.1.0/lightworks/emulator/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/backend/permanent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/backend/slos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.828816 lightworks-1.1.0/lightworks/emulator/components/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/components/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/components/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.828816 lightworks-1.1.0/lightworks/emulator/results/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/results/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    19540 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/results/simulation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.828816 lightworks-1.1.0/lightworks/emulator/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/simulation/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/simulation/probability_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/simulation/quick_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16587 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/simulation/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/simulation/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.828816 lightworks-1.1.0/lightworks/emulator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/utils/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/emulator/utils/state_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.828816 lightworks-1.1.0/lightworks/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.828816 lightworks-1.1.0/lightworks/sdk/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21864 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/circuit/circuit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/circuit/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/circuit/unitary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.832816 lightworks-1.1.0/lightworks/sdk/optimisation/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/optimisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/optimisation/optimisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.832816 lightworks-1.1.0/lightworks/sdk/state/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.832816 lightworks-1.1.0/lightworks/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/utils/circuit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/utils/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/utils/permutation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/utils/state_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.832816 lightworks-1.1.0/lightworks/sdk/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/visualisation/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/visualisation/display_components_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14026 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/visualisation/display_components_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/visualisation/draw_circuit_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-03-21 10:31:41.000000 lightworks-1.1.0/lightworks/sdk/visualisation/draw_circuit_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.836816 lightworks-1.1.0/lightworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-03-21 10:31:48.000000 lightworks-1.1.0/lightworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-03-21 10:31:48.000000 lightworks-1.1.0/lightworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:31:48.000000 lightworks-1.1.0/lightworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-21 10:31:48.000000 lightworks-1.1.0/lightworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-21 10:31:48.000000 lightworks-1.1.0/lightworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-21 10:31:41.000000 lightworks-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:31:48.836816 lightworks-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-21 10:31:41.000000 lightworks-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.824816 lightworks-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.836816 lightworks-1.1.0/tests/emulator/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/analyzer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/annotatedstate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/cnot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/detector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/quicksampler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/result_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/simulator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/emulator/source_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:31:48.836816 lightworks-1.1.0/tests/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19554 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/sdk/circuit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/sdk/compiledcircuit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/sdk/display_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/sdk/parameter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/sdk/state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-21 10:31:41.000000 lightworks-1.1.0/tests/sdk/util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 10:00:02.000000 lightworks-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-10 10:00:07.165912 lightworks-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-10 10:00:02.000000 lightworks-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/emulator/annotated_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/annotated_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/annotated_state/annotated_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/emulator/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/permanent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/slos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/components/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/components/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/results/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/results/simulation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/probability_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/quick_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/utils/state_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21867 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/circuit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/unitary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/optimisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/optimisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/optimisation/optimisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/qubit/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/qubit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/qubit/single_qubit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/qubit/two_qubit_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.161912 lightworks-1.2.0/lightworks/sdk/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.161912 lightworks-1.2.0/lightworks/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/circuit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/matrix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/permutation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/state_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.161912 lightworks-1.2.0/lightworks/sdk/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/display_components_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/display_components_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/lightworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 10:00:03.000000 lightworks-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:00:07.165912 lightworks-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-10 10:00:03.000000 lightworks-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/tests/emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/analyzer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/annotatedstate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/cnot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/detector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/quicksampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/simulator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/source_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/tests/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19554 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/circuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/compiledcircuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/display_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/parameter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/qubit_gate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/util_test.py
```

### Comparing `lightworks-1.1.0/LICENSE` & `lightworks-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/PKG-INFO` & `lightworks-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightworks
-Version: 1.1.0
+Version: 1.2.0
 Summary: Open-source Python SDK for photonic quantum computation.
 Home-page: https://github.com/Aegiq/lightworks
 Author: Aegiq Ltd.
 License: Apache 2.0
 Project-URL: Source, https://github.com/Aegiq/lightworks
 Project-URL: Documentation, https://aegiq.github.io/lightworks/
 Classifier: License :: OSI Approved :: Apache Software License
@@ -30,22 +30,17 @@
 [![Tests](https://github.com/Aegiq/lightworks/actions/workflows/tests.yml/badge.svg?event=push)](https://github.com/Aegiq/lightworks/actions/workflows/tests.yml)
 [![Docs](https://github.com/Aegiq/lightworks/actions/workflows/sphinx_deploy.yml/badge.svg?event=push)](https://github.com/Aegiq/lightworks/actions/workflows/sphinx_deploy.yml)
 [![Pyversions](https://img.shields.io/pypi/pyversions/lightworks.svg?style=plastic)](https://pypi.org/project/lightworks/)
 
 
 # Lightworks
 
-Lightworks is an open source Python SDK, designed for the encoding of linear optic circuits for application in photonic quantum computing. These circuits can be packaged with the other SDK components to create quantum jobs for execution on photonic hardware. Lightworks focuses on discrete-variable quantum computing, and can be utilized for both qubit and boson sampling paradigms.
+Lightworks is an open-source Python SDK, designed for the encoding of linear optic circuits for application in photonic quantum computing. These circuits can be packaged with the other SDK components to create quantum jobs for execution on photonic hardware. Lightworks focuses on discrete-variable quantum computing, and can be utilized for both qubit and boson sampling paradigms.
 
-Included within Lightworks in also an emulator, allowing users to evaluate the operation and performance of a particular configuration before hardware execution. There is a number of simulation objects, each offering a differing functionality, ranging from direct quantum state evolution to replicating the typical sampling process from a photonic system. The emulator also supports complex photonic specific noise modelling, providing a valuable insight into the effect of imperfections in photon generation, QPU programming, and detectors, on a target algorithm.
-
-Key features:
-- Circuit
-- State
-- Emulator
+Included within Lightworks is also an emulator, allowing users to evaluate the operation and performance of a particular configuration before hardware execution. There is a number of simulation objects, each offering a differing functionality, ranging from direct quantum state evolution to replicating the typical sampling process from a photonic system. The emulator also supports complex photonic specific noise modelling, providing a valuable insight into the effect of imperfections in photon generation, QPU programming, and detectors, on a target algorithm.
 
 ## Usage
 
 Python 3.10+ is required.
 
 Lightworks can be installed through pip using the command:
```

### Comparing `lightworks-1.1.0/README.md` & `lightworks-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 [![Tests](https://github.com/Aegiq/lightworks/actions/workflows/tests.yml/badge.svg?event=push)](https://github.com/Aegiq/lightworks/actions/workflows/tests.yml)
 [![Docs](https://github.com/Aegiq/lightworks/actions/workflows/sphinx_deploy.yml/badge.svg?event=push)](https://github.com/Aegiq/lightworks/actions/workflows/sphinx_deploy.yml)
 [![Pyversions](https://img.shields.io/pypi/pyversions/lightworks.svg?style=plastic)](https://pypi.org/project/lightworks/)
 
 
 # Lightworks
 
-Lightworks is an open source Python SDK, designed for the encoding of linear optic circuits for application in photonic quantum computing. These circuits can be packaged with the other SDK components to create quantum jobs for execution on photonic hardware. Lightworks focuses on discrete-variable quantum computing, and can be utilized for both qubit and boson sampling paradigms.
+Lightworks is an open-source Python SDK, designed for the encoding of linear optic circuits for application in photonic quantum computing. These circuits can be packaged with the other SDK components to create quantum jobs for execution on photonic hardware. Lightworks focuses on discrete-variable quantum computing, and can be utilized for both qubit and boson sampling paradigms.
 
-Included within Lightworks in also an emulator, allowing users to evaluate the operation and performance of a particular configuration before hardware execution. There is a number of simulation objects, each offering a differing functionality, ranging from direct quantum state evolution to replicating the typical sampling process from a photonic system. The emulator also supports complex photonic specific noise modelling, providing a valuable insight into the effect of imperfections in photon generation, QPU programming, and detectors, on a target algorithm.
-
-Key features:
-- Circuit
-- State
-- Emulator
+Included within Lightworks is also an emulator, allowing users to evaluate the operation and performance of a particular configuration before hardware execution. There is a number of simulation objects, each offering a differing functionality, ranging from direct quantum state evolution to replicating the typical sampling process from a photonic system. The emulator also supports complex photonic specific noise modelling, providing a valuable insight into the effect of imperfections in photon generation, QPU programming, and detectors, on a target algorithm.
 
 ## Usage
 
 Python 3.10+ is required.
 
 Lightworks can be installed through pip using the command:
```

### Comparing `lightworks-1.1.0/lightworks/__init__.py` & `lightworks-1.2.0/lightworks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,14 @@
 from .sdk import Circuit, Unitary
 from .sdk import Parameter, ParameterDict
 from .sdk import Display
 from .sdk import State
 from .sdk import random_unitary, random_permutation
 from .sdk import db_loss_to_transmission, transmission_to_db_loss
 from .sdk import Optimisation
+from .sdk import qubit
 from .sdk.utils.exceptions import *
 
 __all__ = ["Circuit", "Unitary", "Display", "State", "random_unitary", 
            "random_permutation", "db_loss_to_transmission", 
            "transmission_to_db_loss", "Parameter", "ParameterDict", 
            "Optimisation"]
```

### Comparing `lightworks-1.1.0/lightworks/__version.py` & `lightworks-1.2.0/lightworks/__version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
```

### Comparing `lightworks-1.1.0/lightworks/emulator/__init__.py` & `lightworks-1.2.0/lightworks/emulator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,9 +45,9 @@
 """
 
 from .components import *
 from .simulation import *
 from .backend import *
 from .utils import *
 
-__all__ = ["Simulator", "Sampler", "fidelity", "Source", "Detector", 
+__all__ = ["Simulator", "Sampler", "Source", "Detector", 
            "Analyzer", "QuickSampler", "Backend"]
```

### Comparing `lightworks-1.1.0/lightworks/emulator/annotated_state/__init__.py` & `lightworks-1.2.0/lightworks/emulator/annotated_state/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/annotated_state/annotated_state.py` & `lightworks-1.2.0/lightworks/emulator/annotated_state/annotated_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,20 @@
         state (list) : The fock basis state to use with the class, this should
             be a list of lists, each containing labels for the photons. The 
             number of labels in the list will dictate the total photon number 
             in the mode.
     
     """
     
+    __slots__ = ["__s"]
     def __init__(self, state: list) -> None:
         for s in state:
             if type(s) != list:
                 raise TypeError("Provided state labels should be lists.")
         self.__s = [sorted(s) for s in state]
-        self.__n_modes = len(state)
         return
     
     @property
     def n_photons(self) -> int:
         """Returns the number of photons in a State."""
         return sum([len(s) for s in self.__s])
     
@@ -57,23 +57,23 @@
     @s.setter
     def s(self, value: Any) -> None:
         raise AnnotatedStateError(
             "State value should not be modified directly.")
     
     @property
     def n_modes(self) -> None:
-        return self.__n_modes
+        return len(self.__s)
     
     @n_modes.setter
     def n_modes(self, value: Any) -> None:
         raise AnnotatedStateError("Number of modes cannot be modified.")
     
     def merge(self, merge_state: "AnnotatedState") -> "AnnotatedState":
         """Combine two states, summing the number of photons per mode."""
-        if self.__n_modes == merge_state.__n_modes:
+        if self.n_modes == merge_state.n_modes:
             return AnnotatedState([n1 + n2 for n1, n2 in zip(self.__s, 
                                                              merge_state.s)])
         else:
             raise ValueError("Merged states must be the same length.")
     
     def __str__(self) -> str:
         return annotated_state_to_string(self.__s)
@@ -94,15 +94,15 @@
         else:
             return False
     
     def __hash__(self) -> str:
         return hash(self.__str__())
         
     def __len__(self) -> int:
-        return self.__n_modes
+        return self.n_modes
     
     def __setitem__(self, key: Any, value: Any) -> None:
         raise AnnotatedStateError(
             "AnnotatedState object does not support item assignment.")
     
     def __getitem__(self, indices: int | slice) -> "AnnotatedState":
         if isinstance(indices, slice):
```

### Comparing `lightworks-1.1.0/lightworks/emulator/backend/__init__.py` & `lightworks-1.2.0/lightworks/emulator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/backend/backend.py` & `lightworks-1.2.0/lightworks/emulator/backend/backend.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/backend/permanent.py` & `lightworks-1.2.0/lightworks/emulator/backend/permanent.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         factor_m = prod([factorial(i) for i in in_state])
         factor_n = prod([factorial(i) for i in out_state])
         # Calculate permanent for given input/output
         p = (perm(partition(U, in_state, out_state)) / 
              (np.sqrt(factor_m*factor_n)))    
         return p
 
-def partition(U: np.ndarray, in_state: State, 
-                out_state: State) -> np.ndarray:
+def partition(U: np.ndarray, in_state: State, out_state: State) -> np.ndarray:
     """
     Converts the unitary matrix into a larger matrix used for in the 
     permanent calculation.
     """
     N = len(in_state) # Number of modes
     # Construct the matrix of indices for the partition
     X, Y = [], []
```

### Comparing `lightworks-1.1.0/lightworks/emulator/backend/slos.py` & `lightworks-1.2.0/lightworks/emulator/backend/slos.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/components/__init__.py` & `lightworks-1.2.0/lightworks/emulator/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/components/detector.py` & `lightworks-1.2.0/lightworks/emulator/components/detector.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/components/source.py` & `lightworks-1.2.0/lightworks/emulator/components/source.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/results/__init__.py` & `lightworks-1.2.0/lightworks/emulator/results/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/results/sampling_result.py` & `lightworks-1.2.0/lightworks/emulator/results/sampling_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,25 +30,24 @@
     
         results (dict | np.ndarray) : The results which are to be stored.
         
         input (State) : The input state used in the sampling experiment.
                
     """
     
-    def __init__(self, results: dict, input: State, 
-                 **kwargs) -> None:
+    def __init__(self, results: dict, input: State, **kwargs) -> None:
         
         if not isinstance(input, State):
             raise ResultCreationError("Input state should have type State.")
         self.__input = input
         self.__dict = results
         self.__outputs = list(results.keys())
         # Store any additional provided data from kwargs as attributes    
         for k in kwargs:
-            self.__dict__[k] = kwargs[k]
+            setattr(self, k, kwargs[k])
         
         return
     
     @property
     def dictionary(self) -> dict:
         """Stores the raw results dictionary generated in the experiment."""
         return self.__dict
@@ -76,15 +75,15 @@
     def __str__(self) -> str:
         return str(self.dictionary)
     
     def __len__(self) -> int:
         return len(self.dictionary)
     
     def __iter__(self) -> iter:
-        """Iterable to allow to do 'for param in ParameterDict'."""
+        """Iterable to allow to do 'for output in SamplingResult'."""
         for p in self.dictionary:
             yield p
     
     def items(self) -> iter:
         return self.dictionary.items()
     
     def keys(self) -> iter:
@@ -197,26 +196,20 @@
         ax.set_ylabel("Counts")
            
         # Optionally use show on plot if specified
         if show:
             plt.show()
             return 
         else:
-            return fig, ax
+            return (fig, ax)
     
-    def print_outputs(self, rounding: int = 4) -> None:
+    def print_outputs(self) -> None:
         """
         Print the output results for each input into the system. This is 
         compatible with all possible result types.
-        
-        Args:
-        
-            rounding (int, optional) : Set the number of decimal places which 
-                each number will be rounded to, defaults to 4.
-                
         """
 
         to_print = str(self.input) + " -> "
         for ostate, p in self.dictionary.items():
             to_print += str(ostate) + " : " + str(p) + ", "
         to_print = to_print[:-2]    
         print(to_print)
@@ -257,21 +250,8 @@
             re = np.real(val) if abs(np.real(val)) > threshold else 0
             im = np.imag(val) if abs(np.imag(val)) > threshold else 0
             data[i] = re if abs(im) == 0 else re + 1j*im
         # Convert array to floats when not non complex results used
         data = data.astype(int)
         # Create dataframe
         df = pd.DataFrame(data, index = out_strings, columns = in_strings)
-        return df.transpose()
-        
-    def _complex_round(self, value: float | complex, 
-                       round_points: int) -> float | complex:
-        """
-        Function to perform rounding of complex numbers to the given number of
-        decimal places. It is also compatible with real numbers and will 
-        return the rounded real value in this case.
-        """
-        if not isinstance(value, complex):
-            return round(value, round_points)
-        else:
-            return (round(value.real, round_points) + 
-                    round(value.imag, round_points) * 1j)
+        return df.transpose()
```

### Comparing `lightworks-1.1.0/lightworks/emulator/results/simulation_result.py` & `lightworks-1.2.0/lightworks/emulator/results/simulation_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             for j, ostate in enumerate(self.__outputs):
                 input_results[ostate] = self.__array[i,j]
             dict_results[istate] = input_results
         self.__dict = dict_results
             
         # Store any additional provided data from kwargs as attributes    
         for k in kwargs:
-            self.__dict__[k] = kwargs[k]
+            setattr(self, k, kwargs[k])
         
         return
     
     @property
     def array(self) -> np.ndarray:
         """
         The calculated array of data, where the first dimension corresponds to
@@ -100,63 +100,69 @@
     @property
     def result_type(self) -> dict:
         """
         Details where the result is a probability or probability amplitude.
         """
         return self.__result_type
     
-    def __getitem__(self, item: State | slice) -> float | dict:
+    def __getitem__(self, item: State | tuple) -> float | dict:
         """Custom get item behaviour - used when object accessed with []."""
         if isinstance(item, State):
             # When only one input is used, automatically return output value
             # from dictionary instead of dictionary
             if len(self.inputs) == 1:
                 if item in self.dictionary[self.inputs[0]]:
                     return self.dictionary[self.inputs[0]][item]
                 else:
                     raise KeyError("Provided output state not in data.")
             else:
                 if item in self.dictionary:
                     return self.dictionary[item]
                 else:
                     raise KeyError("Provided input state not in data.")
-        elif isinstance(item, slice):
-            # Separate slice into two states
-            istate = item.start
-            ostate = item.stop
-            # For : slice return all data, unless a single input is present in 
-            # which case just return that
-            if istate is None and ostate is None:
-                if len(self.inputs) == 1:
-                    return self.dictionary[self.inputs[0]]
-                else:
-                    return self.dictionary
+        elif isinstance(item, tuple):
+            # Check only two values have been provided
+            if len(item) > 2:
+                raise ValueError(
+                    "Get item can only contain a maximum of two values.")
+            # Separate data into two states
+            istate = item[0]
+            ostate = item[1]
             # Check all aspects are valid
             if (not isinstance(istate, State) or 
                 not isinstance(ostate, (State, type(None)))):
                 raise ValueError(
-                    "Items used in slices should have type State.")
+                    "Get item values should have type State.")
             if istate in self.dictionary:
                 sub_r = self.dictionary[istate]
             else:
-                raise KeyError("Provided input state not in data.")
-            # If open ended slice used then return all results for input
+                raise KeyError("Requested input state not in data.")
+            # If None provided as second value then return all results for input
             if ostate is None:
                 return sub_r
             # Else return requested value
             elif ostate in sub_r:
                 return sub_r[ostate]
             else:
-                raise KeyError("Provided output State not in data.")
+                raise KeyError("Requested output state not in data.")
+        elif isinstance(item, slice):
+            raise DeprecationWarning(
+                "Retrieval of data through slicing is no longer supported.")
         else:
-            raise ValueError("Get item value must be a State or slice.")
+            raise ValueError(
+                "Get item value must be either one or two States.")
         
     def __str__(self) -> str:
         return str(self.dictionary)
     
+    def __iter__(self) -> iter:
+        """Iterable to allow to do 'for input in SimulationResult'."""
+        for p in self.dictionary:
+            yield p
+    
     def apply_threshold_mapping(self, invert: bool = False
                                 ) -> "SimulationResult":
         """
         Apply a threshold mapping to the results from the object and return 
         this as a dictionary.
         
         Args:
@@ -352,15 +358,15 @@
                 ax[0].set_ylabel("real(amplitude)")
                 ax[1].set_ylabel("imag(amplitude)")
         # Optionally use show on plot if specified
         if show:
             plt.show()
             return 
         
-        return fig, ax
+        return (fig, ax)
     
     def print_outputs(self, rounding: int = 4) -> None:
         """
         Print the output results for each input into the system. This is 
         compatible with all possible result types.
         
         Args:
@@ -374,15 +380,15 @@
         for istate in self.inputs:
             to_print = str(istate) + " -> "
             for ostate, p in self.dictionary[istate].items():
                 # Adjust print order based on quantity
                 if self.result_type == "counts":
                     to_print += str(ostate) + " : " + str(p) + ", "
                 else:
-                    p = self._complex_round(p, rounding)
+                    p = np.round(p, rounding)
                     if abs(p.real) > 0 or abs(p.imag) > 0:
                         to_print += str(p) + "*" + str(ostate) + " + "
             to_print = to_print[:-2]    
             print(to_print)
                 
         return
     
@@ -433,21 +439,8 @@
             data = abs(data)
             if self.result_type == "counts" and not conv_to_probability:
                 data = data.astype(int)
             else:
                 data = data.astype(float)
         # Create dataframe
         df = pd.DataFrame(data, index = in_strings, columns = out_strings)
-        return df
-        
-    def _complex_round(self, value: float | complex, 
-                       round_points: int) -> float | complex:
-        """
-        Function to perform rounding of complex numbers to the given number of
-        decimal places. It is also compatible with real numbers and will 
-        return the rounded real value in this case.
-        """
-        if not isinstance(value, complex):
-            return round(value, round_points)
-        else:
-            return (round(value.real, round_points) + 
-                    round(value.imag, round_points) * 1j)
+        return df
```

### Comparing `lightworks-1.1.0/lightworks/emulator/simulation/__init__.py` & `lightworks-1.2.0/lightworks/emulator/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/simulation/analyzer.py` & `lightworks-1.2.0/lightworks/emulator/simulation/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,16 @@
         full_inputs = []
         # Check dimensions of input and add heralded photons
         for state in inputs:
             if len(state) != n_modes:
                 raise ModeMismatchError(
                     "Input states are of the wrong dimension. Remember to "
                     "subtract heralded modes.")
+            # Also validate state values
+            state._validate()
             full_inputs += [self._build_state(state, self.in_heralds)]
         # Add extra states for loss modes here when included
         if self.__circuit_built.loss_modes > 0:
             full_inputs = [s + State([0]*self.__circuit_built.loss_modes) 
                            for s in full_inputs]
         return full_inputs
```

### Comparing `lightworks-1.1.0/lightworks/emulator/simulation/probability_distribution.py` & `lightworks-1.2.0/lightworks/emulator/simulation/probability_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..backend import Backend
-from ..utils import fock_basis
 from ...sdk import State
 from ...sdk.circuit.circuit_compiler import CompiledCircuit
 
 class ProbabilityDistributionCalc:
     
     @staticmethod
     def state_prob_calc(circuit: CompiledCircuit, inputs: dict,
```

### Comparing `lightworks-1.1.0/lightworks/emulator/simulation/quick_sampler.py` & `lightworks-1.2.0/lightworks/emulator/simulation/quick_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     
     @input_state.setter
     def input_state(self, value: State) -> None:
         if type(value) != State:
             raise TypeError("A single input of type State should be provided.")
         if len(value) != self.circuit.n_modes:
             raise ModeMismatchError("Incorrect input length.")
+        # Also validate state values
+        value._validate()
         self.__input_state = value
         
     @property
     def herald(self) -> FunctionType:
         """A function to be used to post-selection of outputs."""
         return self.__herald
```

### Comparing `lightworks-1.1.0/lightworks/emulator/simulation/sampler.py` & `lightworks-1.2.0/lightworks/emulator/simulation/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,16 @@
     @input_state.setter
     def input_state(self, value: State) -> None:
         if type(value) != State:
             raise TypeError("A single input of type State should be provided.")
         if len(value) != self.circuit.n_modes:
             raise ModeMismatchError(
                 "Incorrect input length for provided circuit.")
+        # Also validate state values
+        value._validate()
         self.__input_state = value
         
     @property
     def source(self) -> Source:
         """
         Details the properties of the Source used for creation of inputs to 
         the Sampler."""
```

### Comparing `lightworks-1.1.0/lightworks/emulator/simulation/simulator.py` & `lightworks-1.2.0/lightworks/emulator/simulation/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,17 @@
                 raise TypeError(
                     "inputs should be a State or list of State objects.")  
             # Dimension check
             if len(state) != self.circuit.n_modes:
                 raise ModeMismatchError(
                     "One or more input states have an incorrect number of "
                     "modes, correct number of modes is "
-                    f"{self.circuit.n_modes}.") 
+                    f"{self.circuit.n_modes}.")
+            # Also validate state values
+            state._validate()
         return inputs
     
     def _process_outputs(self, inputs: list, 
                          outputs: list | None) -> tuple[list, list]:
         """
         Processes the provided outputs or generates them if no inputs were 
         provided. Returns both the inputs and outputs.
@@ -151,14 +153,16 @@
                         "outputs should be a State or list of State objects.")  
                 # Dimension check
                 if len(state) != self.circuit.n_modes:
                     raise ModeMismatchError(
                         "One or more input states have an incorrect number of "
                         "modes, correct number of modes is "
                         f"{self.circuit.n_modes}.")
+                # Also validate state values
+                state._validate()
             # Ensure photon numbers are the same in all states - variation not 
             # currently supported
             ns = [s.n_photons for s in inputs + outputs]
             if min(ns) != max(ns):
                 raise PhotonNumberError(
                     "Mismatch in photon numbers between some inputs/outputs, "
                     "this is not currently supported in the Simulator.")
```

### Comparing `lightworks-1.1.0/lightworks/emulator/utils/__init__.py` & `lightworks-1.2.0/lightworks/sdk/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,10 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .matrix_utils import fidelity, check_unitary
-from .state_utils import fock_basis, annotated_state_to_string
-from .exceptions import *
+from .matrix_utils import check_unitary, random_unitary, random_permutation
+from .state_utils import fock_basis, state_to_string
+from .exceptions import *
+from .conversion import db_loss_to_transmission, transmission_to_db_loss
+from .permutation_conversion import permutation_mat_from_swaps_dict
+from .circuit_utils import unpack_circuit_spec
+from .circuit_utils import convert_non_adj_beamsplitters
+from .circuit_utils import compress_mode_swaps
```

### Comparing `lightworks-1.1.0/lightworks/emulator/utils/exceptions.py` & `lightworks-1.2.0/lightworks/emulator/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/emulator/utils/state_utils.py` & `lightworks-1.2.0/lightworks/emulator/utils/state_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/__init__.py` & `lightworks-1.2.0/lightworks/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/circuit/__init__.py` & `lightworks-1.2.0/lightworks/sdk/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/circuit/circuit.py` & `lightworks-1.2.0/lightworks/sdk/circuit/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,16 +104,16 @@
         raise AttributeError("Number of circuit modes cannot be modified.")
     
     @property
     def _display_spec(self) -> list:
         """Returns display spec for the circuit."""
         return self._get_display_spec()
         
-    def add(self, circuit: Union["Circuit", "Unitary"],                        # type: ignore - ignores Pylance warning raised by undefined unitary component
-            mode: int = 0, group: bool = False, name: str = "Circuit") -> None:
+    def add(self, circuit: Union["Circuit", "Unitary"], mode: int = 0,         # type: ignore - ignores Pylance warning raised by undefined unitary component
+            group: bool = False, name: str = "Circuit") -> None:
         """
         Can be used to add either another Circuit or a Unitary component to the
         existing circuit. This can either have the same size or be smaller than
         the circuit which is being added to.
         
         Args:
         
@@ -401,15 +401,15 @@
             elif cs == "loss":
                 circuit.add_loss(*got_params)
             elif cs == "barrier":
                 circuit.add_barrier(got_params[0])
             elif cs == "mode_swaps":
                 circuit.add_mode_swaps(got_params[0])
             elif cs == "unitary":
-                unitary = CompiledUnitary(params[1])
+                unitary = CompiledUnitary(params[1], params[2])
                 circuit.add(unitary, params[0])
             else:
                 raise CircuitCompilationError(
                     "Component in circuit spec not recognised.")
         
         return circuit
     
@@ -502,15 +502,15 @@
             elif cs == "barrier":
                 display_spec.append(("barrier", cparams[0], None))
             elif cs == "mode_swaps":
                 display_spec.append(("mode_swaps", cparams[0], None))
             elif cs == "unitary":
                 nm = params[1].shape[0]
                 display_spec.append(("unitary", [cparams[0], cparams[0]+nm-1], 
-                                   None))
+                                     params[2]))
             elif cs == "group":
                 display_spec.append(("group", [params[2], params[3]], 
                                    (params[1])))
             else:
                 raise DisplayError("Component in circuit spec not recognised.")
             
         return display_spec
```

### Comparing `lightworks-1.1.0/lightworks/sdk/circuit/circuit_compiler.py` & `lightworks-1.2.0/lightworks/sdk/circuit/circuit_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
         self.U_full = U_full @ self.U_full
         self._display_spec = self._display_spec + [("mode_swaps", swaps, 
                                                     None)]
 
         return
     
     def display(self, display_loss: bool = False, 
-                mode_labels: list | None = None,
+                mode_labels: list | None = None, 
                 display_type: str = "svg") -> None:
         """
         Displays the current circuit.
         
         Args:
         
             display_loss (bool, optional) : Choose whether to display loss
@@ -464,27 +464,31 @@
     
     Args:
     
         unitary (np.ndarray) : The target NxN unitary matrix which is to be 
             implemented.
     
     """
-    def __init__(self, unitary: np.ndarray) -> None:
+    def __init__(self, unitary: np.ndarray, label: str = "U") -> None:
         
         # Check type of supplied unitary
         if not isinstance(unitary, (np.ndarray, list)):
             raise TypeError("Unitary should be a numpy array or list.")
         unitary = np.array(unitary)
         
         # Ensure unitary is valid
         if not check_unitary(unitary):
             raise ValueError("Matrix is not unitary.")
+        if not isinstance(label, str):
+            raise TypeError("Label for unitary should be a string.")
+        
+        # Also check label
         # Assign attributes of unitary
         self.U = unitary
         self.U_full = unitary
         self.n_modes = unitary.shape[0]
         self._loss_included = False
         self._loss_modes = 0
         # Will need to add unitary to build spec
-        self._display_spec = [("unitary", [0, self.n_modes-1], None)]
+        self._display_spec = [("unitary", [0, self.n_modes-1], label)]
         
         return
```

### Comparing `lightworks-1.1.0/lightworks/sdk/circuit/parameters.py` & `lightworks-1.2.0/lightworks/sdk/circuit/parameters.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/circuit/unitary.py` & `lightworks-1.2.0/lightworks/sdk/circuit/unitary.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,22 +28,26 @@
     
     Args:
     
         unitary (np.ndarray) : The target NxN unitary matrix which is to be 
             implemented.
     
     """
-    def __init__(self, unitary: np.ndarray) -> None:
+    def __init__(self, unitary: np.ndarray, label: str = "U") -> None:
         
         # Check type of supplied unitary
         if not isinstance(unitary, (np.ndarray, list)):
             raise TypeError("Unitary should be a numpy array or list.")
         unitary = np.array(unitary)
         
         # Ensure unitary is valid
         if not check_unitary(unitary):
             raise ValueError("Provided matrix is not unitary.")
         
+        # Also check label is a string
+        if not isinstance(label, str):
+            raise TypeError("Label for unitary should be a string.")
+        
         super().__init__(int(unitary.shape[0]))
-        self._Circuit__circuit_spec = [["unitary", (0, unitary)]]
+        self._Circuit__circuit_spec = [["unitary", (0, unitary, label)]]
         
         return
```

### Comparing `lightworks-1.1.0/lightworks/sdk/optimisation/__init__.py` & `lightworks-1.2.0/lightworks/sdk/optimisation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/optimisation/optimisation.py` & `lightworks-1.2.0/lightworks/sdk/optimisation/optimisation.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/state/__init__.py` & `lightworks-1.2.0/lightworks/sdk/state/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/state/state.py` & `lightworks-1.2.0/lightworks/sdk/state/state.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,23 +31,22 @@
     Args:
     
         state (list) : The fock basis state to use with the class, this should
             be a list of photon numbers per mode.
     
     """
 
+    __slots__ = ["__s"]
     def __init__(self, state: list) -> None:
         # If already list then assign to attribute
         if isinstance(state, list):
             self.__s = state
         # Otherwise try to convert
         else:
             self.__s = list(state)
-        # Pre-calculate number of modes
-        self.__n_modes = len(self.__s)
         return
     
     @property
     def n_photons(self) -> int:
         """Returns the number of photons in a State."""
         return sum(self.__s)
         
@@ -59,26 +58,38 @@
     @s.setter
     def s(self, value: Any) -> None:
         raise StateError("State value should not be modified directly.")
     
     @property
     def n_modes(self) -> int:
         """The total number of modes in the state."""
-        return self.__n_modes
+        return len(self.__s)
     
     @n_modes.setter
     def n_modes(self, value: Any) -> None:
         raise StateError("Number of modes cannot be modified.")
     
     def merge(self, merge_state: "State") -> "State":
         """Combine two states, summing the number of photons per mode."""
-        if self.__n_modes == merge_state.n_modes:
+        if self.n_modes == merge_state.n_modes:
             return State([n1 + n2 for n1, n2 in zip(self.__s, merge_state.s)])
         else:
             raise ValueError("Merged states must be the same length.")
+        
+    def _validate(self) -> None:
+        """
+        Function to perform some validation of a state, including checking that
+        the values are all integers and that no negative values are included.
+        """
+        for s in self.__s:
+            if not isinstance(s, int) or isinstance(s, bool):
+                raise TypeError(
+                    "State mode occupation numbers should be integers.")
+            if s < 0:
+                raise ValueError("Mode occupation numbers cannot be negative.")
 
     def __str__(self) -> str:
         return state_to_string(self.__s)
     
     def __repr__(self) -> str: # Confirm this is the correct way to do this
             return f"State({state_to_string(self.__s)})"
     
@@ -94,15 +105,15 @@
         else:
             return False
     
     def __hash__(self) -> str:
         return hash(self.__str__())
         
     def __len__(self) -> int:
-        return self.__n_modes
+        return self.n_modes
     
     def __setitem__(self, key: Any, value: Any) -> None:
         raise StateError("State object does not support item assignment.")
     
     def __getitem__(self, indices: slice | int) -> "State":
         if isinstance(indices, slice):
             return State(self.__s[indices])
```

### Comparing `lightworks-1.1.0/lightworks/sdk/utils/circuit_utils.py` & `lightworks-1.2.0/lightworks/sdk/utils/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/utils/conversion.py` & `lightworks-1.2.0/lightworks/sdk/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/utils/exceptions.py` & `lightworks-1.2.0/lightworks/sdk/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/utils/matrix_utils.py` & `lightworks-1.2.0/lightworks/sdk/utils/matrix_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,41 +17,14 @@
 matrices.
 """
 
 import numpy as np
 from scipy.stats import unitary_group
 from typing import Any
 
-def fidelity(U_target: np.ndarray, U_calculated: np.ndarray) -> float:
-    """
-    Function to calculate the fidelity between target and calculated unitary
-    matrices. Note: It is important that these two matrices both either contain
-    probability amplitudes or normalised probabilities.
-    
-    Args:
-    
-        U_target (np.ndarray) : The target unitary matrix.
-        
-        U_calculated (np.ndarray) : The calculated unitary matrix from the 
-            simulation.
-    
-    Returns:
-    
-        float : The calculated fidelity between the two matrices.
-        
-    """
-    U_target, U_calculated = np.array(U_target), np.array(U_calculated)
-    N = U_target.shape[0]
-    # Find h.c. of calculated unitary to condense code
-    Udag = np.conj(np.transpose(U_calculated))
-    # Calculate fidelity using the unitary matrices
-    fidelity = (abs(np.trace(Udag @ U_target)) ** 2 / 
-                (N * np.trace(Udag @ U_calculated)))
-    return float(np.real(fidelity))
-
 def random_unitary(N: int, seed: int = None) -> np.ndarray:
     """
     Generate a random NxN unitary matrix. Seed can be used to produce the same
     unitary each time the function is called.
     
     Args:
```

### Comparing `lightworks-1.1.0/lightworks/sdk/utils/permutation_conversion.py` & `lightworks-1.2.0/lightworks/sdk/utils/permutation_conversion.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/utils/state_utils.py` & `lightworks-1.2.0/lightworks/sdk/utils/state_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,25 @@
     if statistic_type == "bosonic":
         return list(_sums(N,n))
     elif statistic_type == "fermionic":
         return _fermionic_basis(N, n)
     else:
         raise ValueError("statistic_type should be 'bosonic' or 'fermionic'.")
     
-def _fermionic_basis(N,n):
+def _fermionic_basis(N: int, n: int) -> list:
     """This returns the possible states of n fermions in N modes as vectors."""
     if n == 0:
         return [[0]*N]
     if N == n:
         return [[1]*N]
     arrays_with_zero = [[0]+arr for arr in _fermionic_basis(N - 1, n)]
     arrays_with_one = [[1]+arr for arr in _fermionic_basis(N - 1, n - 1)]
     return arrays_with_zero + arrays_with_one
 
-def _sums(length, total_sum):
+def _sums(length: int, total_sum: int):
     if length == 1:
         yield [total_sum,]
     else:
         for value in range(total_sum + 1):
             for permutation in _sums(length-1, total_sum-value):
                 yield permutation + [value,]
```

### Comparing `lightworks-1.1.0/lightworks/sdk/visualisation/__init__.py` & `lightworks-1.2.0/lightworks/sdk/visualisation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/visualisation/display.py` & `lightworks-1.2.0/lightworks/sdk/visualisation/display.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/lightworks/sdk/visualisation/display_components_mpl.py` & `lightworks-1.2.0/lightworks/sdk/visualisation/display_components_mpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             self._add_wg(xloc, i, con_length)
         # Update mode locations
         for i in modes:
             self.locations[i] = xloc + con_length
             
         return
     
-    def _add_unitary(self, mode1: int, mode2: int) -> None:
+    def _add_unitary(self, mode1: int, mode2: int, label: str) -> None:
         """Add a unitary representation to the axis."""
         size_x = 1 # Unitary x size
         con_length = 0.5 # Input/output waveguide lengths
         offset = 0.5 # Offset of unitary square from modes
         size_y = offset + abs(mode2 - mode1) # Find total unitary size
         # Get x and y positions
         yloc = min(mode1, mode2)
@@ -241,17 +241,20 @@
             self._add_wg(xloc, i, con_length)
         xloc += con_length
         # Add unitary shape and label
         rect = patches.Rectangle((xloc, yloc-offset/2), size_x, size_y, 
                                  facecolor = "#1a0f36", 
                                  edgecolor = "black")
         self.ax.add_patch(rect)
+        s = 10 if len(label) == 1 else 8
+        r = 90 if len(label) > 2 else 0
         self.ax.text(xloc + size_x/2, yloc + abs(mode2 - mode1)/2, 
-                     "U", horizontalalignment = "center", size= 8,
-                     verticalalignment = "center", color= "white")
+                     label, horizontalalignment = "center", size = s,
+                     verticalalignment = "center", color = "white",
+                     rotation = r)
         xloc += size_x
         # Add output waveguides
         for i in modes:
             self._add_wg(xloc, i, con_length)
         # Update mode positions
         for i in modes:
             self.locations[i] = xloc + con_length
```

### Comparing `lightworks-1.1.0/lightworks/sdk/visualisation/display_components_svg.py` & `lightworks-1.2.0/lightworks/sdk/visualisation/display_components_svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             self._add_wg(xloc, (i+1)*self.dy, con_length)
         # Update mode locations
         for i in modes:
             self.locations[i] = xloc + con_length
         
         return
     
-    def _add_unitary(self, mode1: int, mode2: int) -> None:
+    def _add_unitary(self, mode1: int, mode2: int, label: str) -> None:
         """Add a unitary matrix representation to the drawing."""
         size_x = 100 # Unitary x size
         con_length = 50 # Input/output waveguide lengths
         offset = 50 # Offset of unitary square from modes
         size_y = offset + abs(mode2 - mode1)*self.dy # Find total size
         # Get x and y positions
         yloc = (min(mode1, mode2)+1)*self.dy
@@ -131,16 +131,19 @@
         # Add input waveguides
         modes = range(min(mode1, mode2), max(mode1, mode2)+1, 1)
         for i in modes:
             self._add_wg(xloc, (i+1)*self.dy, con_length)
         xloc += con_length
         # Add unitary shape and U label
         self.draw_spec += [("unitary", (xloc, yloc, size_x, size_y, offset/2))]
-        self.draw_spec += [("text", (f"U", xloc+size_x/2, 
-                                     yloc + (size_y-offset)/2, 0, 35, 
+        s = 25 if self.N > 2 else 20
+        s = 35 if len(label) == 1 else s
+        r = 270 if len(label) > 2 else 0
+        self.draw_spec += [("text", (label, xloc+size_x/2, 
+                                     yloc + (size_y-offset)/2, r, s, 
                                      "white", "centred"))]
         xloc += size_x
         # Add output waveguides and update mode positions
         for i in modes:
             self._add_wg(xloc, (i+1)*self.dy, con_length)
             self.locations[i] = xloc + con_length
```

### Comparing `lightworks-1.1.0/lightworks/sdk/visualisation/draw_circuit_mpl.py` & `lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_mpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 self._add_barrier(modes)
             elif c == "mode_swaps":
                 self._add_mode_swaps(modes)
             elif c == "unitary":
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
-                self._add_unitary(m1, m2)
+                self._add_unitary(m1, m2, params)
             elif c == "group":
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
                 self._add_grouped_circuit(m1, m2, params)
         # Add any final lengths as required
         final_loc = max(self.locations)
```

### Comparing `lightworks-1.1.0/lightworks/sdk/visualisation/draw_circuit_svg.py` & `lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 self._add_barrier(modes)
             elif c == "mode_swaps":
                 self._add_mode_swaps(modes)
             elif c == "unitary":
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
-                self._add_unitary(m1, m2)
+                self._add_unitary(m1, m2, params)
             elif c == "group":
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
                 self._add_grouped_circuit(m1, m2, params)
         
         maxloc = max(self.locations)
```

### Comparing `lightworks-1.1.0/lightworks.egg-info/PKG-INFO` & `lightworks-1.2.0/lightworks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightworks
-Version: 1.1.0
+Version: 1.2.0
 Summary: Open-source Python SDK for photonic quantum computation.
 Home-page: https://github.com/Aegiq/lightworks
 Author: Aegiq Ltd.
 License: Apache 2.0
 Project-URL: Source, https://github.com/Aegiq/lightworks
 Project-URL: Documentation, https://aegiq.github.io/lightworks/
 Classifier: License :: OSI Approved :: Apache Software License
@@ -30,22 +30,17 @@
 [![Tests](https://github.com/Aegiq/lightworks/actions/workflows/tests.yml/badge.svg?event=push)](https://github.com/Aegiq/lightworks/actions/workflows/tests.yml)
 [![Docs](https://github.com/Aegiq/lightworks/actions/workflows/sphinx_deploy.yml/badge.svg?event=push)](https://github.com/Aegiq/lightworks/actions/workflows/sphinx_deploy.yml)
 [![Pyversions](https://img.shields.io/pypi/pyversions/lightworks.svg?style=plastic)](https://pypi.org/project/lightworks/)
 
 
 # Lightworks
 
-Lightworks is an open source Python SDK, designed for the encoding of linear optic circuits for application in photonic quantum computing. These circuits can be packaged with the other SDK components to create quantum jobs for execution on photonic hardware. Lightworks focuses on discrete-variable quantum computing, and can be utilized for both qubit and boson sampling paradigms.
+Lightworks is an open-source Python SDK, designed for the encoding of linear optic circuits for application in photonic quantum computing. These circuits can be packaged with the other SDK components to create quantum jobs for execution on photonic hardware. Lightworks focuses on discrete-variable quantum computing, and can be utilized for both qubit and boson sampling paradigms.
 
-Included within Lightworks in also an emulator, allowing users to evaluate the operation and performance of a particular configuration before hardware execution. There is a number of simulation objects, each offering a differing functionality, ranging from direct quantum state evolution to replicating the typical sampling process from a photonic system. The emulator also supports complex photonic specific noise modelling, providing a valuable insight into the effect of imperfections in photon generation, QPU programming, and detectors, on a target algorithm.
-
-Key features:
-- Circuit
-- State
-- Emulator
+Included within Lightworks is also an emulator, allowing users to evaluate the operation and performance of a particular configuration before hardware execution. There is a number of simulation objects, each offering a differing functionality, ranging from direct quantum state evolution to replicating the typical sampling process from a photonic system. The emulator also supports complex photonic specific noise modelling, providing a valuable insight into the effect of imperfections in photon generation, QPU programming, and detectors, on a target algorithm.
 
 ## Usage
 
 Python 3.10+ is required.
 
 Lightworks can be installed through pip using the command:
```

### Comparing `lightworks-1.1.0/lightworks.egg-info/SOURCES.txt` & `lightworks-1.2.0/lightworks.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,24 +26,26 @@
 lightworks/emulator/simulation/analyzer.py
 lightworks/emulator/simulation/probability_distribution.py
 lightworks/emulator/simulation/quick_sampler.py
 lightworks/emulator/simulation/sampler.py
 lightworks/emulator/simulation/simulator.py
 lightworks/emulator/utils/__init__.py
 lightworks/emulator/utils/exceptions.py
-lightworks/emulator/utils/matrix_utils.py
 lightworks/emulator/utils/state_utils.py
 lightworks/sdk/__init__.py
 lightworks/sdk/circuit/__init__.py
 lightworks/sdk/circuit/circuit.py
 lightworks/sdk/circuit/circuit_compiler.py
 lightworks/sdk/circuit/parameters.py
 lightworks/sdk/circuit/unitary.py
 lightworks/sdk/optimisation/__init__.py
 lightworks/sdk/optimisation/optimisation.py
+lightworks/sdk/qubit/__init__.py
+lightworks/sdk/qubit/single_qubit_gates.py
+lightworks/sdk/qubit/two_qubit_gates.py
 lightworks/sdk/state/__init__.py
 lightworks/sdk/state/state.py
 lightworks/sdk/utils/__init__.py
 lightworks/sdk/utils/circuit_utils.py
 lightworks/sdk/utils/conversion.py
 lightworks/sdk/utils/exceptions.py
 lightworks/sdk/utils/matrix_utils.py
@@ -67,9 +69,10 @@
 tests/emulator/simulator_test.py
 tests/emulator/source_test.py
 tests/sdk/__init__.py
 tests/sdk/circuit_test.py
 tests/sdk/compiledcircuit_test.py
 tests/sdk/display_test.py
 tests/sdk/parameter_test.py
+tests/sdk/qubit_gate_test.py
 tests/sdk/state_test.py
 tests/sdk/util_test.py
```

### Comparing `lightworks-1.1.0/setup.py` & `lightworks-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/__init__.py` & `lightworks-1.2.0/tests/emulator/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/analyzer_test.py` & `lightworks-1.2.0/tests/emulator/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/annotatedstate_test.py` & `lightworks-1.2.0/tests/emulator/annotatedstate_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/backend_test.py` & `lightworks-1.2.0/tests/emulator/backend_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/cnot_test.py` & `lightworks-1.2.0/tests/emulator/cnot_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/detector_test.py` & `lightworks-1.2.0/tests/emulator/detector_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/quicksampler_test.py` & `lightworks-1.2.0/tests/emulator/quicksampler_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/result_test.py` & `lightworks-1.2.0/tests/emulator/result_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,14 +71,22 @@
     def test_single_input_plot(self):
         """
         Confirm plotting is able to work without errors for single input case.
         """
         r = SamplingResult(self.test_dict, self.test_input)
         r.plot()
         plt.close()
+        
+    def test_extra_attribute_assignment(self):
+        """
+        Check that miscellaneous additional kwargs can be provided in the 
+        initial function call and that these are assigned to attributes.
+        """
+        r = SamplingResult(self.test_dict, self.test_input, test_attr = 2.5)
+        assert r.test_attr == 2.5
             
 class TestSimulationResult:
     """Unit tests for SimulationResult object."""
     
     @pytest.fixture(autouse=True)
     def setup_data(self) -> None:
         """Create a variety of useful pieces of data for testing."""
@@ -102,27 +110,23 @@
         r = SimulationResult(self.test_array, "probability_amplitude", 
                              inputs = self.test_inputs, 
                              outputs = self.test_outputs)
         assert r[State([1,1,0,0])] == {State([1,0,1,0]): 0.3, 
                                        State([0,1,0,1]): 0.2, 
                                        State([0,0,2,0]): 0.1}
         
-    def test_result_slicing(self):
+    def test_result_indexing(self):
         """
         Confirms that result retrieval works correctly for multi input case,
-        with slicing used to specify the input and output.
+        with both the input and output used to get a single value.
         """
         r = SimulationResult(self.test_array, "probability_amplitude", 
                              inputs = self.test_inputs, 
                              outputs = self.test_outputs)
-        assert r[State([1,1,0,0]):State([0,0,2,0])] == 0.1
-        # Also check open ended slicing
-        assert r[State([1,1,0,0]):] == {State([1,0,1,0]): 0.3, 
-                                        State([0,1,0,1]): 0.2, 
-                                        State([0,0,2,0]): 0.1}
+        assert r[State([1,1,0,0]), State([0,0,2,0])] == 0.1
             
     def test_multi_input_plot(self):
         """
         Confirm plotting is able to work without errors for multi input case.
         """
         # NOTE: There is a non intermittent issue that occurs during testing
         # with the subplots method in mpl. This can be fixed by altering the
@@ -136,8 +140,18 @@
         # Test initial plot
         r.plot()
         plt.close()
         # Test plot with conv_to_probability_option
         r.plot(conv_to_probability=True)
         plt.close()
         # Reset backend after test
-        matplotlib.use(original_backend)
+        matplotlib.use(original_backend)
+        
+    def test_extra_attribute_assignment(self):
+        """
+        Check that miscellaneous additional kwargs can be provided in the 
+        initial function call and that these are assigned to attributes.
+        """
+        r = SimulationResult(self.test_array, "probability_amplitude", 
+                             inputs = self.test_inputs, 
+                             outputs = self.test_outputs, test_attr = 2.5)
+        assert r.test_attr == 2.5
```

### Comparing `lightworks-1.1.0/tests/emulator/sampler_test.py` & `lightworks-1.2.0/tests/emulator/sampler_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/simulator_test.py` & `lightworks-1.2.0/tests/emulator/simulator_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/emulator/source_test.py` & `lightworks-1.2.0/tests/emulator/source_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/sdk/__init__.py` & `lightworks-1.2.0/tests/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/sdk/circuit_test.py` & `lightworks-1.2.0/tests/sdk/circuit_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/sdk/compiledcircuit_test.py` & `lightworks-1.2.0/tests/sdk/compiledcircuit_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/sdk/display_test.py` & `lightworks-1.2.0/tests/sdk/display_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/sdk/parameter_test.py` & `lightworks-1.2.0/tests/sdk/parameter_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.1.0/tests/sdk/state_test.py` & `lightworks-1.2.0/tests/sdk/state_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,8 +59,29 @@
         assert len(State([0,0,0,0])) == 4
         assert len(State([])) == 0
         
     def test_photon_number(self):
         """Checks calculated photon number value is correct."""
         assert State([1,0,2,1,1]).n_photons == 5
         assert State([0,0,0,0,0]).n_photons == 0
-        assert State([]).n_photons == 0
+        assert State([]).n_photons == 0
+
+    @pytest.mark.parametrize("state", [[1,0,0,0],[1,1,1,1],[1,0,2,0],
+                                       [0,0,0,0]])
+    def test_pass_validation(self, state):
+        """
+        Checks that the _validate method of state does not raise an exception
+        when an valid configuration is provided.
+        """
+        s = State(state)
+        s._validate()
+    
+    @pytest.mark.parametrize("state", [[1,0,-1,0],[1,1,-1,0],[1,0,0.5,0],
+                                       [1.0,0,0,0]])
+    def test_fail_validation(self, state):
+        """
+        Checks that the _validate method of state raises an exception when an
+        invalid configuration is provided.
+        """
+        s = State(state)
+        with pytest.raises((ValueError, TypeError)):
+            s._validate()
```

### Comparing `lightworks-1.1.0/tests/sdk/util_test.py` & `lightworks-1.2.0/tests/sdk/util_test.py`

 * *Files identical despite different names*

