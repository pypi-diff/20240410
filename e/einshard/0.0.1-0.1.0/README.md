# Comparing `tmp/einshard-0.0.1.tar.gz` & `tmp/einshard-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einshard-0.0.1.tar", last modified: Tue Apr  9 19:23:54 2024, max compression
+gzip compressed data, was "einshard-0.1.0.tar", last modified: Tue Apr  9 23:44:34 2024, max compression
```

## Comparing `einshard-0.0.1.tar` & `einshard-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ayx      (1289587) primarygroup (89939)        0 2024-04-09 19:23:54.454786 einshard-0.0.1/
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     7048 2024-04-09 18:57:26.000000 einshard-0.0.1/LICENSE
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     1456 2024-04-09 19:23:54.454786 einshard-0.0.1/PKG-INFO
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)      813 2024-04-09 19:16:55.000000 einshard-0.0.1/README.md
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)      780 2024-04-09 19:23:50.000000 einshard-0.0.1/pyproject.toml
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)       38 2024-04-09 19:23:54.454786 einshard-0.0.1/setup.cfg
-drwxr-xr-x   0 ayx      (1289587) primarygroup (89939)        0 2024-04-09 19:23:54.454786 einshard-0.0.1/src/
-drwxr-xr-x   0 ayx      (1289587) primarygroup (89939)        0 2024-04-09 19:23:54.454786 einshard-0.0.1/src/einshard/
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)       31 2024-04-09 18:49:32.000000 einshard-0.0.1/src/einshard/__init__.py
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     4020 2024-04-09 18:49:32.000000 einshard-0.0.1/src/einshard/einshard.py
-drwxr-xr-x   0 ayx      (1289587) primarygroup (89939)        0 2024-04-09 19:23:54.454786 einshard-0.0.1/src/einshard/parsec/
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     1095 2024-04-09 18:49:32.000000 einshard-0.0.1/src/einshard/parsec/Either.py
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)      486 2024-04-09 18:49:32.000000 einshard-0.0.1/src/einshard/parsec/Void.py
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)      338 2024-04-09 18:49:32.000000 einshard-0.0.1/src/einshard/parsec/__init__.py
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     4642 2024-04-09 18:49:32.000000 einshard-0.0.1/src/einshard/parsec/parsec.py
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     2382 2024-04-09 18:51:07.000000 einshard-0.0.1/src/einshard/parser.py
-drwxr-xr-x   0 ayx      (1289587) primarygroup (89939)        0 2024-04-09 19:23:54.454786 einshard-0.0.1/src/einshard.egg-info/
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     1456 2024-04-09 19:23:54.000000 einshard-0.0.1/src/einshard.egg-info/PKG-INFO
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)      427 2024-04-09 19:23:54.000000 einshard-0.0.1/src/einshard.egg-info/SOURCES.txt
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)        1 2024-04-09 19:23:54.000000 einshard-0.0.1/src/einshard.egg-info/dependency_links.txt
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)        9 2024-04-09 19:23:54.000000 einshard-0.0.1/src/einshard.egg-info/requires.txt
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)        9 2024-04-09 19:23:54.000000 einshard-0.0.1/src/einshard.egg-info/top_level.txt
-drwxr-xr-x   0 ayx      (1289587) primarygroup (89939)        0 2024-04-09 19:23:54.454786 einshard-0.0.1/tests/
--rw-r--r--   0 ayx      (1289587) primarygroup (89939)     1936 2024-04-09 18:51:55.000000 einshard-0.0.1/tests/test_einshard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-09 23:44:30.000000 einshard-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 23:44:34.865738 einshard-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-09 23:44:30.000000 einshard-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 23:44:30.000000 einshard-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:44:34.865738 einshard-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.861738 einshard-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/src/einshard/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/einshard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/src/einshard/parsec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/Either.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/Void.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/parsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/src/einshard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-09 23:44:30.000000 einshard-0.1.0/tests/test_einshard.py
```

### Comparing `einshard-0.0.1/LICENSE` & `einshard-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `einshard-0.0.1/pyproject.toml` & `einshard-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "einshard"
-version = "0.0.1"
 authors = [
   { name="Ayaka", email="ayaka@mail.shn.hk" },
   { name="Shin", email="shin@yixiaoer.sg" },
 ]
 description = "High-level array sharding API for JAX"
 readme = "README.md"
 requires-python = ">=3.12"
@@ -21,11 +20,15 @@
     'Topic :: System :: Distributed Computing',
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "jax",
     "mypy",
 ]
+dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/ayaka14732/einshard"
 Issues = "https://github.com/ayaka14732/einshard/issues"
+
+[tool.setuptools.dynamic]
+version = {attr = "einshard.__version__"}
```

### Comparing `einshard-0.0.1/src/einshard/einshard.py` & `einshard-0.1.0/src/einshard/einshard.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,41 @@
 
 def _partition_at_ellipsis(lst: list) -> tuple[list, list]:
     idx = lst.index(...)
     l = lst[:idx]
     r = lst[idx + 1:]
     return l, r
 
-def einshard(arr: Array, expression: str) -> Array:
-    """
-    Shards a :class:`jax.Array` according to a specified pattern, using a human-readable expression similar to that used in einsum notation.
+def sharding(expression: str, *, n_dims: int | None = None) -> NamedSharding:
+    '''
+    Get sharding from einshard expression.
 
     Args:
-        arr (jax.Array): The Array to be processed with tensor parallelism.
-        expression (str): A human-readable expression similar to einsum notation that specifies the sharding pattern.
+        expression (str): The einshard expression.
+        n_dims (int | None): The number of dimensions of the array to be sharded. This argument must be provided if ellipsis is used in the einshard expression.
 
     Returns:
-        Array: The sharded array.
-    """
+        jax.sharding.NamedSharding: The :class:`jax.sharding.Sharding` object corresponding to the given expression.
+    '''
     n_devices = jax.device_count()
 
     res = parse_expression(expression, 0)
     if not res.is_success():
         idx, desc = res.error
         raise ValueError(f'Cannot parse einshard expression "{expression}", expected {desc} at position {idx}.')
     _, (elements_left, elements_right) = res.value
 
     n_left_ellipses = sum(element_left is ... for element_left in elements_left)
     n_right_ellipses = sum(element_right is ... for element_right in elements_right)
     assert n_left_ellipses == n_right_ellipses and n_left_ellipses <= 1
 
-    if n_left_ellipses > 0:  # == 1
-        n_dims = len(arr.shape)
+    if n_left_ellipses == 0:
+        assert n_dims == len(elements_left)
+    else:  # == 1
+        assert n_dims is not None
         n_dims_elided = n_dims - len(elements_left) + 1
         axis_names_for_left_augmented = [f'?{i}' for i in range(n_dims_elided)]
         axis_names_for_right_augmented = [(identifier, 1, False) for identifier in axis_names_for_left_augmented]  # 1: `sharding_number`, False: `is_proportional`
 
         elements_left_left, elements_left_right = _partition_at_ellipsis(elements_left)
         elements_left = [*elements_left_left, *axis_names_for_left_augmented, *elements_left_right]
 
@@ -77,9 +79,24 @@
 
     # print(mesh_shape)
     # print(axis_names)
     # print(partition_spec)
 
     devices = mesh_utils.create_device_mesh(mesh_shape)
     mesh = Mesh(devices, axis_names=axis_names)
-    arr = jax.make_array_from_callback(arr.shape, NamedSharding(mesh, P(*partition_spec)), lambda idx: arr[idx])
+    sharding_ = NamedSharding(mesh, P(*partition_spec))
+    return sharding_
+
+def shard(arr: Array, expression: str) -> Array:
+    '''
+    Shards a :class:`jax.Array` according to the given einshard expression.
+
+    Args:
+        arr (jax.Array): The array to be sharded.
+        expression (str): The einshard expression.
+
+    Returns:
+        jax.Array: The sharded array.
+    '''
+    sharding_ = sharding(expression, n_dims=len(arr.shape))
+    arr = jax.make_array_from_callback(arr.shape, sharding_, lambda idx: arr[idx])
     return arr
```

### Comparing `einshard-0.0.1/src/einshard/parsec/Either.py` & `einshard-0.1.0/src/einshard/parsec/Either.py`

 * *Files identical despite different names*

### Comparing `einshard-0.0.1/src/einshard/parsec/parsec.py` & `einshard-0.1.0/src/einshard/parsec/parsec.py`

 * *Files identical despite different names*

### Comparing `einshard-0.0.1/src/einshard/parser.py` & `einshard-0.1.0/src/einshard/parser.py`

 * *Files identical despite different names*

### Comparing `einshard-0.0.1/tests/test_einshard.py` & `einshard-0.1.0/tests/test_einshard.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import subprocess
 
 from jax import Array
 import jax.numpy as jnp
 
-from einshard import einshard
+import einshard
 
 def set_device_count(n: int) -> None:
     os.environ['JAX_PLATFORMS'] = 'cpu'
     os.environ['XLA_FLAGS'] = os.environ.get('XLA_FLAGS', '') + f' --xla_force_host_platform_device_count={n}'
 
 def get_shard_shape(a: Array) -> tuple[int, ...]:
     return a.addressable_data(0).shape
@@ -57,15 +57,15 @@
         'ans': (1, 8, 4),
     },
 ]
 
 def invoke_test(spec) -> None:
     set_device_count(spec['n_devices'])
     a = jnp.zeros(spec['shape'])
-    a = einshard(a, spec['expr'])
+    a = einshard.shard(a, spec['expr'])
     assert_equal(get_shard_shape(a), spec['ans'])
 
 def main() -> None:
     if len(sys.argv) < 2:  # no command-line arguments provided
         for i in range(len(tests)):
             result = subprocess.call([sys.executable, __file__, f'{i}'])
             if result != 0:
```

