# Comparing `tmp/haskellian-asyn-iter-0.1.0.tar.gz` & `tmp/haskellian-asyn-iter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-asyn-iter-0.1.0.tar", last modified: Wed Apr 10 05:11:58 2024, max compression
+gzip compressed data, was "haskellian-asyn-iter-0.1.1.tar", last modified: Wed Apr 10 05:18:09 2024, max compression
```

## Comparing `haskellian-asyn-iter-0.1.0.tar` & `haskellian-asyn-iter-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      343 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-10 04:56:14.000000 haskellian-asyn-iter-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      533 2024-04-10 04:56:14.000000 haskellian-asyn-iter-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      108 2024-04-10 05:05:14.000000 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       27 2024-04-10 05:05:09.000000 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1321 2024-04-10 05:07:33.000000 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/iter/iter.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-04-10 05:07:12.000000 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2124 2024-04-10 05:01:34.000000 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/ops/ops.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      540 2024-04-10 05:09:46.000000 haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/ops/prefetching.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:11:58.795880 haskellian-asyn-iter-0.1.0/src/haskellian_asyn_iter.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      343 2024-04-10 05:11:58.000000 haskellian-asyn-iter-0.1.0/src/haskellian_asyn_iter.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      454 2024-04-10 05:11:58.000000 haskellian-asyn-iter-0.1.0/src/haskellian_asyn_iter.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-10 05:11:58.000000 haskellian-asyn-iter-0.1.0/src/haskellian_asyn_iter.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-10 05:11:58.000000 haskellian-asyn-iter-0.1.0/src/haskellian_asyn_iter.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.125877 haskellian-asyn-iter-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      343 2024-04-10 05:18:09.125877 haskellian-asyn-iter-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-10 04:56:14.000000 haskellian-asyn-iter-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      533 2024-04-10 05:18:07.000000 haskellian-asyn-iter-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-10 05:18:09.125877 haskellian-asyn-iter-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.115877 haskellian-asyn-iter-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.115877 haskellian-asyn-iter-0.1.1/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.115877 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.115877 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      114 2024-04-10 05:18:01.000000 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.115877 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-10 05:17:31.000000 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      409 2024-04-10 05:17:42.000000 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/iter/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1321 2024-04-10 05:07:33.000000 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/iter/iter.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.115877 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-04-10 05:07:12.000000 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2124 2024-04-10 05:01:34.000000 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/ops/ops.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      540 2024-04-10 05:09:46.000000 haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/ops/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:18:09.125877 haskellian-asyn-iter-0.1.1/src/haskellian_asyn_iter.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      343 2024-04-10 05:18:09.000000 haskellian-asyn-iter-0.1.1/src/haskellian_asyn_iter.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      493 2024-04-10 05:18:09.000000 haskellian-asyn-iter-0.1.1/src/haskellian_asyn_iter.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-10 05:18:09.000000 haskellian-asyn-iter-0.1.1/src/haskellian_asyn_iter.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-10 05:18:09.000000 haskellian-asyn-iter-0.1.1/src/haskellian_asyn_iter.egg-info/top_level.txt
```

### Comparing `haskellian-asyn-iter-0.1.0/pyproject.toml` & `haskellian-asyn-iter-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-asyn-iter"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "FP-style tools for async iterables"
 dependencies = [
   
 ]
```

### Comparing `haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/iter/iter.py` & `haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/iter/iter.py`

 * *Files identical despite different names*

### Comparing `haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/ops/ops.py` & `haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/ops/ops.py`

 * *Files identical despite different names*

### Comparing `haskellian-asyn-iter-0.1.0/src/haskellian/asyn/iter/ops/prefetching.py` & `haskellian-asyn-iter-0.1.1/src/haskellian/asyn/iter/ops/prefetching.py`

 * *Files identical despite different names*

