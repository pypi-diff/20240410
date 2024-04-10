# Comparing `tmp/zkstats-0.1.4.tar.gz` & `tmp/zkstats-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkstats-0.1.4.tar", max compression
+gzip compressed data, was "zkstats-0.1.5.tar", max compression
```

## Comparing `zkstats-0.1.4.tar` & `zkstats-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      541 2024-03-13 12:17:36.035932 zkstats-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-13 12:17:36.035932 zkstats-0.1.4/zkstats/__init__.py
--rw-r--r--   0        0        0     3762 2024-03-13 12:17:36.035932 zkstats-0.1.4/zkstats/cli.py
--rw-r--r--   0        0        0     9942 2024-03-13 12:17:36.035932 zkstats-0.1.4/zkstats/computation.py
--rw-r--r--   0        0        0    15371 2024-03-13 12:17:36.035932 zkstats-0.1.4/zkstats/core.py
--rw-r--r--   0        0        0    19283 2024-03-13 12:17:36.035932 zkstats-0.1.4/zkstats/ops.py
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 zkstats-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      541 2024-04-10 14:27:25.251412 zkstats-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:25.255411 zkstats-0.1.5/zkstats/__init__.py
+-rw-r--r--   0        0        0     3857 2024-04-10 14:27:25.255411 zkstats-0.1.5/zkstats/cli.py
+-rw-r--r--   0        0        0     9942 2024-04-10 14:27:25.255411 zkstats-0.1.5/zkstats/computation.py
+-rw-r--r--   0        0        0    15537 2024-04-10 14:27:25.255411 zkstats-0.1.5/zkstats/core.py
+-rw-r--r--   0        0        0    19283 2024-04-10 14:27:25.255411 zkstats-0.1.5/zkstats/ops.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 zkstats-0.1.5/PKG-INFO
```

### Comparing `zkstats-0.1.4/pyproject.toml` & `zkstats-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zkstats"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Jern Kunpittaya", "Kevin Chia"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ezkl = "9.1.0"
 torch = "^2.1.1"
```

### Comparing `zkstats-0.1.4/zkstats/cli.py` & `zkstats-0.1.5/zkstats/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import sys
 from typing import Type
 import importlib.util
 
 import click
 import torch
 
-from .core import prover_gen_proof, prover_gen_settings, setup, verifier_verify, get_data_commitment_maps
+from .core import prover_gen_proof, prover_gen_settings, setup, verifier_verify, generate_data_commitment
 from .computation import computation_to_model
 
 cwd = os.getcwd()
 # TODO: Should make this configurable
 output_dir = f"{cwd}/out"
 os.makedirs(output_dir, exist_ok=True)
 model_onnx_path = f"{output_dir}/model.onnx"
 compiled_model_path = f"{output_dir}/model.compiled"
 pk_path = f"{output_dir}/model.pk"
 vk_path = f"{output_dir}/model.vk"
 proof_path = f"{output_dir}/model.pf"
 settings_path = f"{output_dir}/settings.json"
 witness_path = f"{output_dir}/witness.json"
 comb_data_path = f"{output_dir}/comb_data.json"
-commitment_maps_path = f"{output_dir}/commitment_maps.json"
+data_commitment_path = f"{output_dir}/data_commitment.json"
 
 default_possible_scales = list(range(20))
 
 
 @click.group()
 def cli():
     pass
@@ -34,19 +34,19 @@
 
 @click.command()
 @click.argument('computation_path')
 @click.argument('data_path')
 def prove(computation_path: str, data_path: str):
     computation = load_computation(computation_path)
     _, model = computation_to_model(computation)
-    commitment_maps = get_data_commitment_maps(data_path, default_possible_scales)
-    with open(commitment_maps_path, "w") as f:
-        json.dump(commitment_maps, f)
+    generate_data_commitment(data_path, default_possible_scales, data_commitment_path)
+    with open(data_commitment_path) as f:
+        data_commitment = json.load(f)
     # By default select all columns
-    selected_columns = list(commitment_maps[str(default_possible_scales[0])].keys())
+    selected_columns = list(data_commitment[str(default_possible_scales[0])].keys())
     prover_gen_settings(
         data_path,
         selected_columns,
         comb_data_path,
         model,
         model_onnx_path,
         "default",
@@ -67,41 +67,43 @@
         witness_path,
         compiled_model_path,
         settings_path,
         proof_path,
         pk_path,
     )
     print("Finished generating proof")
-    verifier_verify(proof_path, settings_path, vk_path, selected_columns, commitment_maps)
+    verifier_verify(proof_path, settings_path, vk_path, selected_columns, data_commitment_path)
     print("Proof path:", proof_path)
     print("Settings path:", settings_path)
     print("Verification key path:", vk_path)
-    print("Commitment maps path:", commitment_maps_path)
+    print("Commitment maps path:", data_commitment_path)
 
 
 @click.command()
 def verify():
     # Load commitment maps
-    with open(commitment_maps_path, "r") as f:
-        commitment_maps = json.load(f)
+    with open(data_commitment_path, "r") as f:
+        data_commitment = json.load(f)
     # By default select all columns
-    selected_columns = list(commitment_maps[str(default_possible_scales[0])].keys())
-    verifier_verify(proof_path, settings_path, vk_path, selected_columns, commitment_maps)
+    selected_columns = list(data_commitment[str(default_possible_scales[0])].keys())
+    verifier_verify(proof_path, settings_path, vk_path, selected_columns, data_commitment_path)
 
 
 @click.command()
 @click.argument('data_path')
 @click.argument('scale_str')
 def commit(data_path: str, scale_str: str):
     """
     Now we just assume the data is a list of floats. We should be able to
     """
     scale = int(scale_str)
-    commitment_maps = get_data_commitment_maps(data_path, [scale])
-    print("Commitment maps:", commitment_maps)
+    generate_data_commitment(data_path, [scale], data_commitment_path)
+    with open(data_commitment_path) as f:
+        data_commitment = json.load(f)
+    print("Commitment maps:", data_commitment)
 
 
 def main():
     cli()
 
 
 def load_computation(module_path: str) -> Type[torch.nn.Module]:
```

### Comparing `zkstats-0.1.4/zkstats/computation.py` & `zkstats-0.1.5/zkstats/computation.py`

 * *Files identical despite different names*

### Comparing `zkstats-0.1.4/zkstats/core.py` & `zkstats-0.1.5/zkstats/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,25 +187,25 @@
 
 # commitment_map is a mapping[column_name, commitment_hex]
 # E.g. {
 #     "columns_0": "0x...",
 #     ...
 # }
 TCommitmentMap = Mapping[str, str]
-# commitment_maps is a mapping[scale, mapping[column_name, commitment_hex]]
+# data_commitment is a mapping[scale, mapping[column_name, commitment_hex]]
 # E.g. {
 #     scale_0: {
 #         "columns_0": "0x...",
 #         ...
 #     },
 #     ...
 # }
 TCommitmentMaps = Mapping[str, TCommitmentMap]
 
-def verifier_verify(proof_path: str, settings_path: str, vk_path: str, selected_columns: Sequence[str], commitment_maps: TCommitmentMaps) -> torch.Tensor:
+def verifier_verify(proof_path: str, settings_path: str, vk_path: str, selected_columns: Sequence[str], data_commitment_path: str) -> torch.Tensor:
   """
   Verify the proof and return the result.
 
   :param proof_path: path to the proof file
   :param settings_path: path to the settings file
   :param vk_path: path to the verification key file
   :param expected_data_commitments: expected data commitments for columns. The i-th commitment should
@@ -233,23 +233,25 @@
   outputs = proof_instance[len(input_scales):]
   len_inputs = len(inputs)
   len_outputs = len(outputs)
   # `instances` = input commitments + params (which is 0 in our case) + output
   assert len(proof_instance) == len_inputs + len_outputs, f"lengths mismatch: {len(proof_instance)=}, {len_inputs=}, {len_outputs=}"
 
   # 2.1 Check input commitments
+  with open(data_commitment_path) as f:
+    data_commitment = json.load(f)
   # All inputs are hashed so are commitments
   assert len_inputs == len(selected_columns), f"lengths mismatch: {len_inputs=}, {len(selected_columns)=}"
   # Sanity check
   # Check each commitment is correct
   for i, (actual_commitment, column_name) in enumerate(zip(inputs, selected_columns)):
     #  actual_commitment_str = ezkl.vecu64_to_felt(actual_commitment)
      actual_commitment_str = (actual_commitment)
      input_scale = input_scales[i]
-     expected_commitment = commitment_maps[str(input_scale)][column_name]
+     expected_commitment = data_commitment[str(input_scale)][column_name]
      assert actual_commitment_str == expected_commitment, f"commitment mismatch: {i=}, {actual_commitment_str=}, {expected_commitment=}"
 
   # 2.2 Check output is correct
   # - is a tuple (is_in_error, result)
   # - is_valid is True
   # Sanity check
   is_in_error = ezkl.felt_to_float(outputs[0], output_scales[0])
@@ -259,34 +261,37 @@
     result_arr.append(ezkl.felt_to_float(outputs[index+1], output_scales[1]))
   return result_arr
 
 
 # ===================================================================================================
 # ===================================================================================================
 
-def get_data_commitment_maps(data_path: str, scales: Sequence[int]) -> TCommitmentMaps:
+def generate_data_commitment(data_path: str, scales: Sequence[int], data_commitment_path: str) -> None:
   """
-  Generate a data commitment map for each scale. Commitments for different scales are required
-  so that verifiers can verify proofs with different scales.
+  Generate and store data commitment maps for different scales so that verifiers can verify
+  proofs with different scales.
 
   :param data_path: path to the data file. The data file should be a JSON file with the following format:
     {
       "column_0": [number_0, number_1, ...],
       "column_1": [number_0, number_1, ...],
     }
-  :param scales: a list of scales to use for the commitments.
-  :return: a map from scale to column name to commitment.
+  :param scales: a list of scales to use for the commitments
+  :param data_commitment_path: path to store the generated data commitment maps
   """
+
   with open(data_path) as f:
     data_json = json.load(f)
-  return {
+  data_commitments = {
     str(scale): {
       k: _get_commitment_for_column(v, scale) for k, v in data_json.items()
     } for scale in scales
   }
+  with open(data_commitment_path, "w") as f:
+    json.dump(data_commitments, f)
 
 
 # ===================================================================================================
 # Private functions
 # ===================================================================================================
 
 def _export_onnx(model: Type[IModel], data_tensor_array: list[torch.Tensor], model_loc: str) -> None:
```

### Comparing `zkstats-0.1.4/zkstats/ops.py` & `zkstats-0.1.5/zkstats/ops.py`

 * *Files identical despite different names*

### Comparing `zkstats-0.1.4/PKG-INFO` & `zkstats-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkstats
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Jern Kunpittaya
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

