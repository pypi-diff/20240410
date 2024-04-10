# Comparing `tmp/leakysim-0.2.1.tar.gz` & `tmp/leakysim-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leakysim-0.2.1.tar", last modified: Tue Apr  9 04:22:43 2024, max compression
+gzip compressed data, was "leakysim-0.2.2.tar", last modified: Wed Apr 10 08:44:06 2024, max compression
```

## Comparing `leakysim-0.2.1.tar` & `leakysim-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:22:43.938683 leakysim-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 04:22:35.000000 leakysim-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-09 04:22:43.938683 leakysim-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 04:22:35.000000 leakysim-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 04:22:35.000000 leakysim-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:22:43.938683 leakysim-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-09 04:22:35.000000 leakysim-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:22:43.934683 leakysim-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:22:43.934683 leakysim-0.2.1/src/leaky/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 04:22:35.000000 leakysim-0.2.1/src/leaky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-04-09 04:22:35.000000 leakysim-0.2.1/src/leaky/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 04:22:35.000000 leakysim-0.2.1/src/leaky/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-09 04:22:35.000000 leakysim-0.2.1/src/leaky/leaky_pybind_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-09 04:22:35.000000 leakysim-0.2.1/src/leaky/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-09 04:22:35.000000 leakysim-0.2.1/src/leaky/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:22:43.938683 leakysim-0.2.1/src/leakysim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-09 04:22:43.000000 leakysim-0.2.1/src/leakysim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 04:22:43.000000 leakysim-0.2.1/src/leakysim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:22:43.000000 leakysim-0.2.1/src/leakysim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:22:43.000000 leakysim-0.2.1/src/leakysim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 04:22:43.000000 leakysim-0.2.1/src/leakysim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 04:22:43.000000 leakysim-0.2.1/src/leakysim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:44:06.353879 leakysim-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 08:43:57.000000 leakysim-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-10 08:44:06.353879 leakysim-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 08:43:57.000000 leakysim-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 08:43:57.000000 leakysim-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:44:06.353879 leakysim-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-10 08:43:57.000000 leakysim-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:44:06.349879 leakysim-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:44:06.349879 leakysim-0.2.2/src/leaky/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 08:43:57.000000 leakysim-0.2.2/src/leaky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15962 2024-04-10 08:43:57.000000 leakysim-0.2.2/src/leaky/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 08:43:57.000000 leakysim-0.2.2/src/leaky/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-10 08:43:57.000000 leakysim-0.2.2/src/leaky/leaky_pybind_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-10 08:43:57.000000 leakysim-0.2.2/src/leaky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-10 08:43:57.000000 leakysim-0.2.2/src/leaky/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:44:06.349879 leakysim-0.2.2/src/leakysim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-10 08:44:06.000000 leakysim-0.2.2/src/leakysim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 08:44:06.000000 leakysim-0.2.2/src/leakysim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:44:06.000000 leakysim-0.2.2/src/leakysim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:44:06.000000 leakysim-0.2.2/src/leakysim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 08:44:06.000000 leakysim-0.2.2/src/leakysim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 08:44:06.000000 leakysim-0.2.2/src/leakysim.egg-info/top_level.txt
```

### Comparing `leakysim-0.2.1/LICENSE` & `leakysim-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leakysim-0.2.1/PKG-INFO` & `leakysim-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: leakysim
-Version: 0.2.1
+Version: 0.2.2
 Summary: An implementation of Google's Pauli+ simulator.
 Home-page: https://github.com/inmzhang/leaky
 Author: Yiming Zhang
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stim==1.13
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 
 # leaky
```

### Comparing `leakysim-0.2.1/README.md` & `leakysim-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `leakysim-0.2.1/setup.py` & `leakysim-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,10 +158,10 @@
     package_dir={"": "src"},
     package_data={
         "": [*HEADER_FILES, "src/leaky/__init__.pyi", "pyproject.toml"]
     },
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     extras_require={"test": ["pytest>=6.0"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=["stim==1.13"],
 )
```

### Comparing `leakysim-0.2.1/src/leaky/__init__.py` & `leakysim-0.2.2/src/leaky/__init__.py`

 * *Files identical despite different names*

### Comparing `leakysim-0.2.1/src/leaky/__init__.pyi` & `leakysim-0.2.2/src/leaky/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             >>> channel.add_transition(0, 0, 1, 0.5)
             >>> channel
             LeakyPauliChannel(is_single_qubit_channel=true, with 2 transitions attached)
         """
         ...
 
 class Instruction:
-    """An instruction almost the same as `stim.CircuitInstruction`.
+    """An instruction almost the same as `leaky.Instruction`.
 
     This is a simplified re-implemented since `stim.PyCircuitInstruction` is not exposed
     by `libstim` C++ API.
     """
     def __init__(
         self,
         gate_name: str,
@@ -273,16 +273,16 @@
                 efficient for large repeated simulations. For large repeated
                 simulations, it is recommended to use the `sample_batch` method.
 
         Examples:
             >>> import stim
             >>> import leaky
             >>> circuit = stim.Circuit()
-            >>> circuit.append_operation(stim.CircuitInstruction("X", [0]))
-            >>> circuit.append_operation(stim.CircuitInstruction("M", [0]))
+            >>> circuit.append_operation(leaky.Instruction("X", [0]))
+            >>> circuit.append_operation(leaky.Instruction("M", [0]))
             >>> simulator = leaky.Simulator(1)
             >>> simulator.do_circuit(circuit)
         """
         ...
 
     def do(
         self,
@@ -381,15 +381,15 @@
 
         Args:
             clear_bound_channels: Whether to also clear the bound leaky channels.
 
         Examples:
             >>> import leaky
             >>> simulator = leaky.Simulator(1)
-            >>> simulator.do(stim.CircuitInstruction("X", [0]))
+            >>> simulator.do(leaky.Instruction("X", [0]))
             >>> simulator.clear()
         """
         ...
 
     def current_measurement_record(
         self,
         readout_strategy: "leaky.ReadoutStrategy" = ReadoutStrategy.RawLabel,
@@ -401,15 +401,15 @@
 
         Returns:
             The measurement record.
 
         Examples:
             >>> import leaky
             >>> simulator = leaky.Simulator(1)
-            >>> simulator.do(stim.CircuitInstruction("M", [0]))
+            >>> simulator.do(leaky.Instruction("M", [0]))
             >>> simulator.current_measurement_record()
             array([0], dtype=uint8)
         """
         ...
 
     def sample_batch(
         self,
```

### Comparing `leakysim-0.2.1/src/leaky/leaky_pybind_test.py` & `leakysim-0.2.2/src/leaky/leaky_pybind_test.py`

 * *Files identical despite different names*

### Comparing `leakysim-0.2.1/src/leaky/utils.py` & `leakysim-0.2.2/src/leaky/utils.py`

 * *Files identical despite different names*

### Comparing `leakysim-0.2.1/src/leaky/utils_test.py` & `leakysim-0.2.2/src/leaky/utils_test.py`

 * *Files identical despite different names*

### Comparing `leakysim-0.2.1/src/leakysim.egg-info/PKG-INFO` & `leakysim-0.2.2/src/leakysim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: leakysim
-Version: 0.2.1
+Version: 0.2.2
 Summary: An implementation of Google's Pauli+ simulator.
 Home-page: https://github.com/inmzhang/leaky
 Author: Yiming Zhang
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stim==1.13
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 
 # leaky
```

