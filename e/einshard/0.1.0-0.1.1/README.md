# Comparing `tmp/einshard-0.1.0.tar.gz` & `tmp/einshard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einshard-0.1.0.tar", last modified: Tue Apr  9 23:44:34 2024, max compression
+gzip compressed data, was "einshard-0.1.1.tar", last modified: Wed Apr 10 00:37:58 2024, max compression
```

## Comparing `einshard-0.1.0.tar` & `einshard-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-09 23:44:30.000000 einshard-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 23:44:34.865738 einshard-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-09 23:44:30.000000 einshard-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 23:44:30.000000 einshard-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:44:34.865738 einshard-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.861738 einshard-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/src/einshard/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/einshard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/src/einshard/parsec/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/Either.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/Void.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parsec/parsec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-09 23:44:30.000000 einshard-0.1.0/src/einshard/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/src/einshard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 23:44:34.000000 einshard-0.1.0/src/einshard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:34.865738 einshard-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-09 23:44:30.000000 einshard-0.1.0/tests/test_einshard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:37:58.748621 einshard-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-10 00:37:52.000000 einshard-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-10 00:37:58.748621 einshard-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-10 00:37:52.000000 einshard-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-10 00:37:52.000000 einshard-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:37:58.748621 einshard-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:37:58.744621 einshard-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:37:58.744621 einshard-0.1.1/src/einshard/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 00:37:52.000000 einshard-0.1.1/src/einshard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:37:58.748621 einshard-0.1.1/src/einshard/parsec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 00:37:52.000000 einshard-0.1.1/src/einshard/parsec/Either.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 00:37:52.000000 einshard-0.1.1/src/einshard/parsec/Void.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 00:37:52.000000 einshard-0.1.1/src/einshard/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-10 00:37:52.000000 einshard-0.1.1/src/einshard/parsec/parsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-10 00:37:52.000000 einshard-0.1.1/src/einshard/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-10 00:37:52.000000 einshard-0.1.1/src/einshard/shard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:37:58.748621 einshard-0.1.1/src/einshard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-10 00:37:58.000000 einshard-0.1.1/src/einshard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 00:37:58.000000 einshard-0.1.1/src/einshard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:37:58.000000 einshard-0.1.1/src/einshard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 00:37:58.000000 einshard-0.1.1/src/einshard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 00:37:58.000000 einshard-0.1.1/src/einshard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:37:58.748621 einshard-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-10 00:37:52.000000 einshard-0.1.1/tests/test_einshard.py
```

### Comparing `einshard-0.1.0/LICENSE` & `einshard-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `einshard-0.1.0/PKG-INFO` & `einshard-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einshard
-Version: 0.1.0
+Version: 0.1.1
 Summary: High-level array sharding API for JAX
 Author-email: Ayaka <ayaka@mail.shn.hk>, Shin <shin@yixiaoer.sg>
 Project-URL: Homepage, https://github.com/ayaka14732/einshard
 Project-URL: Issues, https://github.com/ayaka14732/einshard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Topic :: System :: Distributed Computing
@@ -31,14 +31,16 @@
 
 This library requires at least Python 3.12.
 
 ```sh
 pip install einshard
 ```
 
+You need to have JAX installed by [choosing the correct installation method](https://jax.readthedocs.io/en/latest/installation.html) before installing Einshard.
+
 ## Usage
 
 For testing purpose, we initialise the JAX CPU backend with 16 devices. This should be run before the actual code (e.g. placed at the top of the script):
 
 ```python
 n_devices = 16
 import os
@@ -72,19 +74,23 @@
 │          │          │          │          │
 │          │          │          │          │
 └──────────┴──────────┴──────────┴──────────┘
 ```
 
 ## Development
 
+Crente venv:
+
 ```sh
 python3.12 -m venv venv
 . venv/bin/activate
 ```
 
+Install dependencies:
+
 ```sh
 pip install -U pip
 pip install -U wheel
 pip install "jax[cpu]"
 pip install -r requirements.txt
 ```
```

### Comparing `einshard-0.1.0/README.md` & `einshard-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 This library requires at least Python 3.12.
 
 ```sh
 pip install einshard
 ```
 
+You need to have JAX installed by [choosing the correct installation method](https://jax.readthedocs.io/en/latest/installation.html) before installing Einshard.
+
 ## Usage
 
 For testing purpose, we initialise the JAX CPU backend with 16 devices. This should be run before the actual code (e.g. placed at the top of the script):
 
 ```python
 n_devices = 16
 import os
@@ -55,19 +57,23 @@
 │          │          │          │          │
 │          │          │          │          │
 └──────────┴──────────┴──────────┴──────────┘
 ```
 
 ## Development
 
+Crente venv:
+
 ```sh
 python3.12 -m venv venv
 . venv/bin/activate
 ```
 
+Install dependencies:
+
 ```sh
 pip install -U pip
 pip install -U wheel
 pip install "jax[cpu]"
 pip install -r requirements.txt
 ```
```

### Comparing `einshard-0.1.0/pyproject.toml` & `einshard-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `einshard-0.1.0/src/einshard/einshard.py` & `einshard-0.1.1/src/einshard/shard.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     _, (elements_left, elements_right) = res.value
 
     n_left_ellipses = sum(element_left is ... for element_left in elements_left)
     n_right_ellipses = sum(element_right is ... for element_right in elements_right)
     assert n_left_ellipses == n_right_ellipses and n_left_ellipses <= 1
 
     if n_left_ellipses == 0:
-        assert n_dims == len(elements_left)
+        if n_dims is not None:
+            assert n_dims == len(elements_left)
     else:  # == 1
         assert n_dims is not None
         n_dims_elided = n_dims - len(elements_left) + 1
         axis_names_for_left_augmented = [f'?{i}' for i in range(n_dims_elided)]
         axis_names_for_right_augmented = [(identifier, 1, False) for identifier in axis_names_for_left_augmented]  # 1: `sharding_number`, False: `is_proportional`
 
         elements_left_left, elements_left_right = _partition_at_ellipsis(elements_left)
```

### Comparing `einshard-0.1.0/src/einshard/parsec/Either.py` & `einshard-0.1.1/src/einshard/parsec/Either.py`

 * *Files identical despite different names*

### Comparing `einshard-0.1.0/src/einshard/parsec/parsec.py` & `einshard-0.1.1/src/einshard/parsec/parsec.py`

 * *Files identical despite different names*

### Comparing `einshard-0.1.0/src/einshard/parser.py` & `einshard-0.1.1/src/einshard/parser.py`

 * *Files identical despite different names*

### Comparing `einshard-0.1.0/src/einshard.egg-info/PKG-INFO` & `einshard-0.1.1/src/einshard.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einshard
-Version: 0.1.0
+Version: 0.1.1
 Summary: High-level array sharding API for JAX
 Author-email: Ayaka <ayaka@mail.shn.hk>, Shin <shin@yixiaoer.sg>
 Project-URL: Homepage, https://github.com/ayaka14732/einshard
 Project-URL: Issues, https://github.com/ayaka14732/einshard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Topic :: System :: Distributed Computing
@@ -31,14 +31,16 @@
 
 This library requires at least Python 3.12.
 
 ```sh
 pip install einshard
 ```
 
+You need to have JAX installed by [choosing the correct installation method](https://jax.readthedocs.io/en/latest/installation.html) before installing Einshard.
+
 ## Usage
 
 For testing purpose, we initialise the JAX CPU backend with 16 devices. This should be run before the actual code (e.g. placed at the top of the script):
 
 ```python
 n_devices = 16
 import os
@@ -72,19 +74,23 @@
 │          │          │          │          │
 │          │          │          │          │
 └──────────┴──────────┴──────────┴──────────┘
 ```
 
 ## Development
 
+Crente venv:
+
 ```sh
 python3.12 -m venv venv
 . venv/bin/activate
 ```
 
+Install dependencies:
+
 ```sh
 pip install -U pip
 pip install -U wheel
 pip install "jax[cpu]"
 pip install -r requirements.txt
 ```
```

### Comparing `einshard-0.1.0/tests/test_einshard.py` & `einshard-0.1.1/tests/test_einshard.py`

 * *Files identical despite different names*

