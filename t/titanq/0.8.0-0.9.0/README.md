# Comparing `tmp/titanq-0.8.0.tar.gz` & `tmp/titanq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanq-0.8.0.tar", last modified: Mon Apr  8 13:59:00 2024, max compression
+gzip compressed data, was "titanq-0.9.0.tar", last modified: Wed Apr 10 17:54:39 2024, max compression
```

## Comparing `titanq-0.8.0.tar` & `titanq-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.821948 titanq-0.8.0/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-01 13:41:38.000000 titanq-0.8.0/LICENSE.txt
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-08 13:59:00.821948 titanq-0.8.0/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-01 18:11:59.000000 titanq-0.8.0/README.md
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-08 13:21:32.000000 titanq-0.8.0/pyproject.toml
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-01 13:41:38.000000 titanq-0.8.0/requirements.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-08 13:59:00.821948 titanq-0.8.0/setup.cfg
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/tests/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-02 15:31:47.000000 titanq-0.8.0/tests/test_client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    25419 2024-04-08 13:39:25.000000 titanq-0.8.0/tests/test_model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-02 15:31:47.000000 titanq-0.8.0/tests/test_numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-05 13:48:53.000000 titanq-0.8.0/tests/test_optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      940 2024-04-05 13:48:53.000000 titanq-0.8.0/tests/test_variable.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/titanq/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-01 13:41:38.000000 titanq-0.8.0/titanq/__init__.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/titanq/_client/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_client/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-02 13:51:42.000000 titanq-0.8.0/titanq/_client/client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_client/model.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.817948 titanq-0.8.0/titanq/_model/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-01 18:11:59.000000 titanq-0.8.0/titanq/_model/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5393 2024-04-08 13:21:32.000000 titanq-0.8.0/titanq/_model/constraints.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/errors.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_model/manifest.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    28359 2024-04-05 18:58:59.000000 titanq-0.8.0/titanq/_model/model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_model/numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-01 13:41:38.000000 titanq-0.8.0/titanq/_model/objective.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4721 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2766 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/variable.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2645 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_model/variable_list.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.821948 titanq-0.8.0/titanq/_storage/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-01 13:41:38.000000 titanq-0.8.0/titanq/_storage/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-05 13:48:53.000000 titanq-0.8.0/titanq/_storage/managed_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_storage/s3_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-02 15:31:47.000000 titanq-0.8.0/titanq/_storage/storage_client.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-08 13:59:00.821948 titanq-0.8.0/titanq.egg-info/
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/SOURCES.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/dependency_links.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/requires.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-08 13:59:00.000000 titanq-0.8.0/titanq.egg-info/top_level.txt
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-01 13:41:38.000000 titanq-0.9.0/LICENSE.txt
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-10 17:54:39.256404 titanq-0.9.0/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-01 18:11:59.000000 titanq-0.9.0/README.md
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-09 20:13:03.000000 titanq-0.9.0/pyproject.toml
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-01 13:41:38.000000 titanq-0.9.0/requirements.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-10 17:54:39.256404 titanq-0.9.0/setup.cfg
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/tests/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-02 15:31:47.000000 titanq-0.9.0/tests/test_client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    22306 2024-04-09 20:13:03.000000 titanq-0.9.0/tests/test_model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-02 15:31:47.000000 titanq-0.9.0/tests/test_numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-05 13:48:53.000000 titanq-0.9.0/tests/test_optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1104 2024-04-09 20:13:03.000000 titanq-0.9.0/tests/test_variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-01 13:41:38.000000 titanq-0.9.0/titanq/__init__.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/_client/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_client/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-02 13:51:42.000000 titanq-0.9.0/titanq/_client/client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_client/model.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/_model/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-01 18:11:59.000000 titanq-0.9.0/titanq/_model/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3449 2024-04-09 20:13:03.000000 titanq-0.9.0/titanq/_model/constraints.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-05 13:48:53.000000 titanq-0.9.0/titanq/_model/errors.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_model/manifest.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    28992 2024-04-09 20:13:03.000000 titanq-0.9.0/titanq/_model/model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_model/numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-01 13:41:38.000000 titanq-0.9.0/titanq/_model/objective.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4721 2024-04-05 13:48:53.000000 titanq-0.9.0/titanq/_model/optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3424 2024-04-09 20:13:03.000000 titanq-0.9.0/titanq/_model/variable.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2685 2024-04-10 17:28:31.000000 titanq-0.9.0/titanq/_model/variable_list.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/_storage/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-01 13:41:38.000000 titanq-0.9.0/titanq/_storage/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-05 13:48:53.000000 titanq-0.9.0/titanq/_storage/managed_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_storage/s3_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_storage/storage_client.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq.egg-info/
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/requires.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/top_level.txt
```

### Comparing `titanq-0.8.0/LICENSE.txt` & `titanq-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/PKG-INFO` & `titanq-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.8.0
+Version: 0.9.0
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.8.0/README.md` & `titanq-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/pyproject.toml` & `titanq-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "titanq"
 description = "The TitanQ SDK for python"
 dynamic = ["dependencies"]
 readme = { file = "README.md", content-type = "text/markdown" }
-version = "0.8.0"
+version = "0.9.0"
 license = { text = "Apache 2.0" }
 keywords = ["titan", "titanq", "optimization", "platform", "infinity", "infinityq"]
 requires-python = ">= 3.9"
 maintainers = [
     { name = "InfinityQ", email = "support@infinityq.tech" }
 ]
 classifiers = [
```

### Comparing `titanq-0.8.0/tests/test_client.py` & `titanq-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/tests/test_model.py` & `titanq-0.9.0/tests/test_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -202,64 +202,14 @@
     assert mock_s3_storage.array_uploaded['weights'] == np_array_to_bytes(weights)
     assert mock_s3_storage.array_uploaded['constraint_weights'] == None
     assert mock_s3_storage.array_uploaded['constraint_bounds'] == None
 
     assert mock_s3_storage.file_removed
 
 
-def test_optimize_with_set_constraints_matrices(model_s3_client, mock_s3_storage, mock_metrics, mock_result):
-    model = model_s3_client
-
-    # optimize using sdk
-    weights = np.random.rand(10, 10).astype(np.float32)
-    constraint_weights = np.random.rand(4, 10).astype(np.float32)
-    bias = np.random.rand(10).astype(np.float32)
-    constraint_bounds = np.random.rand(4, 2).astype(np.float32)
-
-    model.add_variable_vector('x', 10, Vtype.BINARY)
-    model.set_objective_matrices(weights, bias)
-    model.set_constraints_matrices(constraint_weights, constraint_bounds)
-    response = model.optimize()
-
-    assert response.computation_metrics() == mock_metrics["computation_metrics"]
-    assert (response.result_vector() == mock_result).all()
-
-    assert mock_s3_storage.array_uploaded['bias'] == np_array_to_bytes(bias)
-    assert mock_s3_storage.array_uploaded['weights'] == np_array_to_bytes(weights)
-    assert mock_s3_storage.array_uploaded['constraint_weights'] == np_array_to_bytes(constraint_weights)
-    assert mock_s3_storage.array_uploaded['constraint_bounds'] == np_array_to_bytes(constraint_bounds)
-
-    assert mock_s3_storage.file_removed
-
-
-@pytest.mark.parametrize("constraint_weights_shape, constraint_bounds_shape, error", [
-    ((2, 10), (2,2), None),
-    ((10, 10), (10,2), None),
-    ((2, 10), (3,2), ValueError),
-    ((2, 10), (2,), ValueError),
-    ((2, 10), (10,2), ValueError),
-    ((10, 2), (2,2), ValueError),
-    ((10, ), (1,2), ValueError),
-    ((2, 10), (3,2), ValueError),
-    ((2, 11), (2,2), ValueError),
-    ((0, 10), (0,2), ValueError),
-])
-def test_set_constraints(model_s3_client, constraint_weights_shape, constraint_bounds_shape, error):
-    model_s3_client.add_variable_vector('x', 10, Vtype.BINARY)
-
-    constraint_weights = np.random.rand(*constraint_weights_shape).astype(np.float32)
-    constraint_bounds = np.random.rand(*constraint_bounds_shape).astype(np.float32)
-
-    if error:
-        with pytest.raises(error):
-            model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
-    else:
-        model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
-
-
 @pytest.mark.parametrize("vtype", [
     (Vtype.BINARY),
     (Vtype.BIPOLAR),
 ])
 def test_vtype_sent(model_s3_client, mock_titanq_client, vtype):
     model = model_s3_client
     mock_client = mock_titanq_client
@@ -272,42 +222,19 @@
     model.set_objective_matrices(weights, bias)
 
     model.optimize()
 
     assert mock_client.request_sent.parameters.variable_types == str(vtype)
 
 
-@pytest.mark.parametrize("constraint_weights_dtype, constraint_bounds_dtype, error", [
-    (np.float32, np.float32, None),
-    (np.float64, np.float32, ValueError),
-    (np.float32, np.float64, ValueError),
-    (np.int32, np.int32, ValueError),
-])
-def test_constraints_dtype(model_s3_client, constraint_weights_dtype, constraint_bounds_dtype, error):
-    model_s3_client.add_variable_vector('x', 10, Vtype.BINARY)
-
-    constraint_weights = np.random.rand(2, 10).astype(constraint_weights_dtype)
-    constraint_bounds = np.random.rand(2, 2).astype(constraint_bounds_dtype)
-
-    if error:
-        with pytest.raises(error):
-            model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
-    else:
-        model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
-
-
-
 def test_constraints_without_variable(model_s3_client):
     constraint_weights = np.random.rand(2, 10).astype(np.float32)
     constraint_bounds = np.random.rand(2).astype(np.float32)
 
     with pytest.raises(errors.MissingVariableError):
-        model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
-
-    with pytest.raises(errors.MissingVariableError):
         model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
 
     with pytest.raises(errors.MissingVariableError):
         model_s3_client.add_set_partitioning_constraint(np.array([0, 1]))
 
     with pytest.raises(errors.MissingVariableError):
         model_s3_client.add_cardinality_constraints_matrix(np.array([[1, 0, 1, 0], [0, 1, 1, 1]]), np.array([2, 3]))
```

### Comparing `titanq-0.8.0/tests/test_numpy_util.py` & `titanq-0.9.0/tests/test_numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/tests/test_optimize_response.py` & `titanq-0.9.0/tests/test_optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/tests/test_variable.py` & `titanq-0.9.0/tests/test_variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import numpy as np
 import pytest
 
-from titanq._model.variable import BinaryVariableVector, BipolarVariableVector, IntegerVariableVector, Vtype
+from titanq._model.variable import BinaryVariableVector, BipolarVariableVector, ContinuousVariableVector, IntegerVariableVector, Vtype
 
 
 @pytest.mark.parametrize("variable_vector, expected",  [
     (BinaryVariableVector('x', 3), Vtype.BINARY),
     (BipolarVariableVector('x', 3), Vtype.BIPOLAR),
     (IntegerVariableVector('x', 3, [(1, 2)] * 3), Vtype.INTEGER),
+    (ContinuousVariableVector('x', 3, [(1, 2)] * 3), Vtype.CONTINUOUS),
 ])
 def test_variable_types(variable_vector, expected):
     assert variable_vector.vtype() == expected
 
 
 @pytest.mark.parametrize("variable_vector, expected",  [
     (BinaryVariableVector('x', 3), "bbb"),
     (IntegerVariableVector('x', 4, [(1, 2)] * 4), "iiii"),
+    (ContinuousVariableVector('x', 8, [(2, 6)] * 8), "cccccccc"),
 ])
 def test_variable_types_as_list(variable_vector, expected):
     assert variable_vector.variable_types_as_list() == expected
 
 
 def test_binary_variable_bounds():
     variable_vector = BinaryVariableVector("x", 3)
```

### Comparing `titanq-0.8.0/titanq/__init__.py` & `titanq-0.9.0/titanq/__init__.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_client/client.py` & `titanq-0.9.0/titanq/_client/client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_client/model.py` & `titanq-0.9.0/titanq/_client/model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_model/constraints.py` & `titanq-0.9.0/titanq/_model/constraints.py`

 * *Files 23% similar despite different names*

```diff
@@ -87,52 +87,7 @@
     def _constraints_rows(self) -> int:
         """
         :return: The number of constraints (row) already set, 0 if never set
         """
         if self._constraint_weights is None:
             return 0
         return self._constraint_weights.shape[0]
-
-    def set_constraint_matrices(
-        self,
-        constraint_weights: np.ndarray,
-        constraint_bounds: np.ndarray
-    ) -> None:
-        """
-        Overides add_constraint and manually set the constraint weights and the constraint bounds
-
-        NOTE: Should be removed when equality and inequality constraints are added
-
-        :param constraint_weights: already formed constraint weights
-        :param constraint_bounds: already formed constraint bounds
-        """
-        weights_shape = constraint_weights.shape
-        bounds_shape = constraint_bounds.shape
-
-        # validate shapes
-        if len(weights_shape) != 2:
-            raise ValueError(f"constraint_weights should be a 2d matrix. Got something with shape: {weights_shape}")
-
-        if len(bounds_shape) != 2:
-            raise ValueError(f"constraint_bounds should be a 2d matrix. Got something with shape: {bounds_shape}")
-
-        if weights_shape[1] != self._variable_size:
-            raise ValueError(f"constraint_weights shape does not match variable size. Expected (M, {self._variable_size}) where M is the number of constraints")
-        n_constraints = weights_shape[0]
-
-        if n_constraints == 0:
-            raise ValueError("Need at least 1 constraints")
-
-        if bounds_shape[0] != n_constraints:
-            raise ValueError(f"constraint_bounds shape does not match constraint_weights size. Expected ({n_constraints}, 2)")
-
-        if bounds_shape[1] != 2:
-            raise ValueError(f"constraint_bounds shape is expected to be ({n_constraints}, 2)")
-
-        if constraint_weights.dtype != np.float32:
-            raise ValueError(f"Weights constraints vector dtype should be np.float32")
-
-        if constraint_bounds.dtype != np.float32:
-            raise ValueError(f"Bounds constraints vector dtype should be np.float32")
-
-        self._constraint_weights = constraint_weights
-        self._constraint_bounds = constraint_bounds
```

### Comparing `titanq-0.8.0/titanq/_model/errors.py` & `titanq-0.9.0/titanq/_model/errors.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_model/manifest.py` & `titanq-0.9.0/titanq/_model/manifest.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_model/model.py` & `titanq-0.9.0/titanq/_model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     MissingObjectiveError,
     ObjectiveAlreadySetError,
     OptimizeError
 )
 from .objective import Objective, Target
 from .optimize_response import OptimizeResponse
 from .manifest import Manifest
-from .variable import BinaryVariableVector, BipolarVariableVector, IntegerVariableVector, Vtype
+from .variable import BinaryVariableVector, BipolarVariableVector, ContinuousVariableVector, IntegerVariableVector, Vtype
 from .._client import api_model, Client
 from .._storage import ManagedStorage, StorageClient
 from .numpy_util import (
     is_ndarray_binary,
     is_upperbound_bigger_equal_lowerbound,
     ndarray_contains_nan_inf,
     reshape_to_2d,
@@ -93,29 +93,34 @@
         """
         Add a vector of variable to the model. Only a single vector of variables can be set.
         Calling this method again will override the current vector of variables
 
         :param name: The name given to this variable vector.
         :param size: The size of the vector.
         :param vtype: Type of the variables inside the vector.
+        :param variable_bounds: Lower and upper bounds for the variable vector.
 
         :raise MaximumVariableLimitError: If a variable is already defined.
         :raise ValueError: If the size of the vector is < 1.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
         import numpy as np
         from titanq import Model, Vtype
 
         # set up model
         ...
 
-        model.add_variable_vector('x', size, Vtype.BINARY)
+        # set up variable vectors
+        bounds = [[2.3, 4.6], [3.1, 5.3], [1.1, 4]]
+
+        model.add_variable_vector('x', 10, Vtype.BINARY)
+        model.add_variable_vector('y', 3, Vtype.CONTINUOUS, bounds)
         """
         # validation
         if not self._constraints.is_empty():
             raise ConstraintAlreadySetError("Cannot add additional variable once constraints have been defined")
 
         if self._objective is not None:
             raise ObjectiveAlreadySetError("Cannot add additional variable once objective have been defined")
@@ -130,14 +135,17 @@
             if variable_bounds:
                 raise ValueError("variable_bounds is not supported with Vtype.BIPOLAR")
             variables = BipolarVariableVector(name, size)
 
         elif vtype is Vtype.INTEGER:
             variables = IntegerVariableVector(name, size, variable_bounds)
 
+        elif vtype is Vtype.CONTINUOUS:
+            variables = ContinuousVariableVector(name, size, variable_bounds)
+
         else:
             raise NotImplementedError(f"Unsupported variable type: {vtype}")
 
         self._variables.add(variables)
         self._constraints.augment_size(size)
 
         log.debug(f"add variable name='{name}', type={str(vtype)}, size={size}.")
@@ -193,35 +201,14 @@
             raise ObjectiveAlreadySetError("An objective has already have been set for this model.")
 
         log.debug(f"set objective matrix and bias vector.")
 
         self._objective = Objective(self._variables.total_variable_size(), weights, bias, target)
 
 
-    def set_constraints_matrices(self, constraint_weights: np.ndarray, constraint_bounds: np.ndarray):
-        """
-        Set the constraints matrices for the model.
-
-        :param constraint_weights: The constraint_weights matrix of shape (M, N) where M the number of constraints and N is the number of variables
-        :type constraint_weights: a NumPy 2-D dense ndarray (must be float32)
-
-        :param constraint_bounds: The constraint_bounds vector of shape (M,2) where M is the number of constraints
-        :type constraint_bounds:  a NumPy 1-D ndarray (must be float32)
-
-        :raise MissingVariableError: If no variable have been added to the model.
-        :raise ValueError: If the constraint_weights shape or the constraint_bounds shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_weights or constraint_bounds data type is not f32.
-        """
-        if self._variables.n_variables() == 0:
-            raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
-
-        log.debug(f"set weights constraints matrix and bias constraints vector.")
-        self._constraints.set_constraint_matrices(constraint_weights, constraint_bounds)
-
-
     def add_set_partitioning_constraints_matrix(self, constraint_mask: np.ndarray):
         """
         Adds set partitioning constraints in matrix format to the model.
 
         :param constraint_mask: The constraint_mask matrix of shape (M, N) where M the number of constraints and N is the number of variables.
         :type constraint_mask: A NumPy 2-D dense ndarray (must be binary)
 
@@ -402,14 +389,29 @@
         :param limit: The limit vector of shape (M,) where M is the number of constraints
         :type limit: A NumPy 1-D array (float32)
 
         :raise MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exceed the limit.
         :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
         :raise ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
+
+        Example
+        ~~~~~~~
+        ..  highlight:: python
+        ..  code-block:: python
+
+        from titanq import Model
+
+        # set up model
+        ...
+
+        constraint_mask = np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32)
+        limit = np.array([2, 10], dtype=np.float32)
+
+        model.add_equality_constraints_matrix(constraint_mask, limit)
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.dtype != np.float32 or limit.dtype != np.float32:
             raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {limit.dtype}")
 
@@ -445,14 +447,29 @@
         :param limit: Limit value to the constraint mask
         :type limit: np.float32
 
         :raise MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
         :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
         :raise ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
+
+        Example
+        ~~~~~~~
+        ..  highlight:: python
+        ..  code-block:: python
+
+        from titanq import Model
+
+        # set up model
+        ...
+
+        constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
+        limit = -3.45
+
+        model.add_equality_constraint(constraint_mask, limit)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_equality_constraint() function with a matrix, " \
                 "please use add_equality_constraint_matrix() insead")
 
         self.add_equality_constraints_matrix(reshape_to_2d(constraint_mask), np.full((1,), limit, dtype=np.float32))
@@ -468,14 +485,29 @@
         :type constraint_bounds: A NumPy 2-D ndarray (float32)
 
         :raise MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
         :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
         :raise ValueError: A lowerbound is equal or higher than its given upperbound
         :raise ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
+
+        Example
+        ~~~~~~~
+        ..  highlight:: python
+        ..  code-block:: python
+
+        from titanq import Model
+
+        # set up model
+        ...
+
+        constraint_mask = np.array([[-3.51, 0], [10, 0]], dtype=np.float32)
+        constraint_bounds = np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32)
+
+        model.add_inequality_constraints_matrix(constraint_mask, constraint_bounds)
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.dtype != np.float32 or constraint_bounds.dtype != np.float32:
             raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {constraint_bounds.dtype}")
 
@@ -507,14 +539,29 @@
         :type constraint_bounds: A NumPy 1-D ndarray (float32)
 
         :raise MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
         :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
         :raise ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
         :raise ValueError: Lowerbound is equal or higher than the upperbound
+
+        Example
+        ~~~~~~~
+        ..  highlight:: python
+        ..  code-block:: python
+
+        from titanq import Model
+
+        # set up model
+        ...
+
+        constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
+        constraint_bounds = np.array([1.0, np.nan], dtype=np.float32)
+
+        model.add_inequality_constraint(constraint_mask, constraint_bounds)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_inequality_constraint() function with a matrix, " \
                 "please use add_inequality_constraint_matrix() insead")
 
         self.add_inequality_constraints_matrix(reshape_to_2d(constraint_mask), reshape_to_2d(constraint_bounds))
```

### Comparing `titanq-0.8.0/titanq/_model/numpy_util.py` & `titanq-0.9.0/titanq/_model/numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_model/objective.py` & `titanq-0.9.0/titanq/_model/objective.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_model/optimize_response.py` & `titanq-0.9.0/titanq/_model/optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_model/variable.py` & `titanq-0.9.0/titanq/_model/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 from numpy._typing import NDArray
 
 class Vtype(str, enum.Enum):
     BINARY = 'binary'
     BIPOLAR = 'bipolar'
     INTEGER = 'integer'
+    CONTINUOUS = 'continuous'
 
     def __str__(self) -> str:
         return str(self.value)
 
 class VariableVector(abc.ABC):
     """
     Object That represent a vector of variable to be optimized.
@@ -44,15 +45,15 @@
         :return: Type of variable in the vector.
         """
 
 
     @abc.abstractmethod
     def variable_types_as_list(self) -> str:
         """
-        :return: Generate a string of 'b' or 'i' depending on the variable type
+        :return: Generate a string of 'b', 'i' or 'c' depending on the variable type
         """
 
 
     @abc.abstractmethod
     def variable_bounds(self) -> NDArray:
         """
         :return: The variable bounds associated to this variable vector
@@ -100,8 +101,29 @@
 
 
     def variable_types_as_list(self) -> str:
         return "i" * self.size()
 
 
     def variable_bounds(self) -> NDArray:
+        return self._variable_bounds
+
+class ContinuousVariableVector(VariableVector):
+    def __init__(self, name: str, size: int, variable_bounds: List[Tuple[int, int]]) -> None:
+        super().__init__(name, size)
+
+        if len(variable_bounds) != self.size():
+            raise ValueError("variable_bounds need to be the same length as variable size")
+
+        self._variable_bounds = np.array(variable_bounds, dtype=np.float32)
+
+
+    def vtype(self) -> Vtype:
+        return Vtype.CONTINUOUS
+
+
+    def variable_types_as_list(self) -> str:
+        return "c" * self.size()
+
+
+    def variable_bounds(self) -> NDArray:
         return self._variable_bounds
```

### Comparing `titanq-0.8.0/titanq/_model/variable_list.py` & `titanq-0.9.0/titanq/_model/variable_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if n_variable == 0:
             return ""
 
         elif n_variable == 1:
             variable = self._variables[0]
             if equality_constraint or inequality_constraint:
                 return variable.variable_types_as_list()
-            elif variable.vtype() is Vtype.INTEGER:
+            elif variable.vtype() is Vtype.INTEGER or variable.vtype() is Vtype.CONTINUOUS:
                 return variable.variable_types_as_list()
             else:
                 return str(variable.vtype())
 
         else: # n_variable > 1
             return "".join(v.variable_types_as_list() for v in self._variables)
```

### Comparing `titanq-0.8.0/titanq/_storage/managed_storage.py` & `titanq-0.9.0/titanq/_storage/managed_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_storage/s3_storage.py` & `titanq-0.9.0/titanq/_storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq/_storage/storage_client.py` & `titanq-0.9.0/titanq/_storage/storage_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.8.0/titanq.egg-info/PKG-INFO` & `titanq-0.9.0/titanq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.8.0
+Version: 0.9.0
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.8.0/titanq.egg-info/SOURCES.txt` & `titanq-0.9.0/titanq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

