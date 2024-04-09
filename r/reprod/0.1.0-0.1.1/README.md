# Comparing `tmp/reprod-0.1.0.tar.gz` & `tmp/reprod-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprod-0.1.0.tar", last modified: Tue Apr  9 18:35:59 2024, max compression
+gzip compressed data, was "reprod-0.1.1.tar", last modified: Tue Apr  9 19:27:20 2024, max compression
```

## Comparing `reprod-0.1.0.tar` & `reprod-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:35:59.816308 reprod-0.1.0/
--rw-r--r--   0 wyd      (826206) primarygroup (89939)    11357 2024-04-09 18:03:36.000000 reprod-0.1.0/LICENSE
--rw-r--r--   0 wyd      (826206) primarygroup (89939)    13299 2024-04-09 18:35:59.816022 reprod-0.1.0/PKG-INFO
--rw-r--r--   0 wyd      (826206) primarygroup (89939)       39 2024-04-09 18:03:36.000000 reprod-0.1.0/README.md
--rw-r--r--   0 wyd      (826206) primarygroup (89939)      401 2024-04-09 18:35:52.000000 reprod-0.1.0/pyproject.toml
-drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:35:59.812993 reprod-0.1.0/reprod/
--rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:13:03.000000 reprod-0.1.0/reprod/__init__.py
-drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:35:59.814710 reprod-0.1.0/reprod/gpt2_jax/
--rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:04:11.000000 reprod-0.1.0/reprod/gpt2_jax/__init__.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)      188 2024-04-09 18:04:11.000000 reprod-0.1.0/reprod/gpt2_jax/config.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)     8044 2024-04-09 18:08:49.000000 reprod-0.1.0/reprod/gpt2_jax/model.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)      167 2024-04-09 18:04:11.000000 reprod-0.1.0/reprod/gpt2_jax/sample.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:04:11.000000 reprod-0.1.0/reprod/gpt2_jax/train.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)      588 2024-04-09 18:09:59.000000 reprod-0.1.0/reprod/gpt2_jax/utils.py
-drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:35:59.815474 reprod-0.1.0/reprod/gpt2_numpy/
--rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:03:36.000000 reprod-0.1.0/reprod/gpt2_numpy/__init__.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)      209 2024-04-09 18:06:22.000000 reprod-0.1.0/reprod/gpt2_numpy/config.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)     6191 2024-04-09 18:06:32.000000 reprod-0.1.0/reprod/gpt2_numpy/modeling_np.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)       81 2024-04-09 18:06:38.000000 reprod-0.1.0/reprod/gpt2_numpy/sample.py
--rw-r--r--   0 wyd      (826206) primarygroup (89939)      581 2024-04-09 18:09:44.000000 reprod-0.1.0/reprod/gpt2_numpy/utils.py
-drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:35:59.815734 reprod-0.1.0/reprod.egg-info/
--rw-r--r--   0 wyd      (826206) primarygroup (89939)    13299 2024-04-09 18:35:59.000000 reprod-0.1.0/reprod.egg-info/PKG-INFO
--rw-r--r--   0 wyd      (826206) primarygroup (89939)      472 2024-04-09 18:35:59.000000 reprod-0.1.0/reprod.egg-info/SOURCES.txt
--rw-r--r--   0 wyd      (826206) primarygroup (89939)        1 2024-04-09 18:35:59.000000 reprod-0.1.0/reprod.egg-info/dependency_links.txt
--rw-r--r--   0 wyd      (826206) primarygroup (89939)        7 2024-04-09 18:35:59.000000 reprod-0.1.0/reprod.egg-info/top_level.txt
--rw-r--r--   0 wyd      (826206) primarygroup (89939)       38 2024-04-09 18:35:59.816369 reprod-0.1.0/setup.cfg
+drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 19:27:20.813263 reprod-0.1.1/
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)     1064 2024-04-09 19:01:53.000000 reprod-0.1.1/LICENSE
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)     1596 2024-04-09 19:27:20.813064 reprod-0.1.1/PKG-INFO
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)       77 2024-04-09 19:03:04.000000 reprod-0.1.1/README.md
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)      401 2024-04-09 19:10:11.000000 reprod-0.1.1/pyproject.toml
+drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 19:27:20.808794 reprod-0.1.1/reprod/
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/__init__.py
+drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 19:27:20.810494 reprod-0.1.1/reprod/gpt2_jax/
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_jax/__init__.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)      188 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_jax/config.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)     8044 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_jax/model.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)      167 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_jax/sample.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_jax/train.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)      588 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_jax/utils.py
+drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 19:27:20.812286 reprod-0.1.1/reprod/gpt2_numpy/
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_numpy/__init__.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)      209 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_numpy/config.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)     6191 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_numpy/modeling_np.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)       81 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_numpy/sample.py
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)      581 2024-04-09 18:55:16.000000 reprod-0.1.1/reprod/gpt2_numpy/utils.py
+drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 19:27:20.812840 reprod-0.1.1/reprod.egg-info/
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)     1596 2024-04-09 19:27:20.000000 reprod-0.1.1/reprod.egg-info/PKG-INFO
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)      492 2024-04-09 19:27:20.000000 reprod-0.1.1/reprod.egg-info/SOURCES.txt
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)        1 2024-04-09 19:27:20.000000 reprod-0.1.1/reprod.egg-info/dependency_links.txt
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)        7 2024-04-09 19:27:20.000000 reprod-0.1.1/reprod.egg-info/top_level.txt
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)       38 2024-04-09 19:27:20.813310 reprod-0.1.1/setup.cfg
+drwxr-xr-x   0 wyd      (826206) primarygroup (89939)        0 2024-04-09 19:27:20.812505 reprod-0.1.1/tests/
+-rw-r--r--   0 wyd      (826206) primarygroup (89939)       38 2024-04-09 18:55:16.000000 reprod-0.1.1/tests/test_dummy.py
```

### Comparing `reprod-0.1.0/reprod/gpt2_jax/model.py` & `reprod-0.1.1/reprod/gpt2_jax/model.py`

 * *Files identical despite different names*

### Comparing `reprod-0.1.0/reprod/gpt2_jax/utils.py` & `reprod-0.1.1/reprod/gpt2_jax/utils.py`

 * *Files identical despite different names*

### Comparing `reprod-0.1.0/reprod/gpt2_numpy/modeling_np.py` & `reprod-0.1.1/reprod/gpt2_numpy/modeling_np.py`

 * *Files identical despite different names*

### Comparing `reprod-0.1.0/reprod/gpt2_numpy/utils.py` & `reprod-0.1.1/reprod/gpt2_numpy/utils.py`

 * *Files identical despite different names*

