# Comparing `tmp/haskellian-asyn-0.2.3.tar.gz` & `tmp/haskellian-asyn-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-asyn-0.2.3.tar", last modified: Wed Apr 10 05:12:08 2024, max compression
+gzip compressed data, was "haskellian-asyn-0.3.1.tar", last modified: Wed Apr 10 07:03:21 2024, max compression
```

## Comparing `haskellian-asyn-0.2.3.tar` & `haskellian-asyn-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:12:08.695881 haskellian-asyn-0.2.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-10 05:12:08.685881 haskellian-asyn-0.2.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.2.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      512 2024-04-10 05:12:06.000000 haskellian-asyn-0.2.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-10 05:12:08.695881 haskellian-asyn-0.2.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:12:08.685881 haskellian-asyn-0.2.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:12:08.685881 haskellian-asyn-0.2.3/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:12:08.685881 haskellian-asyn-0.2.3/src/haskellian/asyn/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      109 2024-04-10 05:09:39.000000 haskellian-asyn-0.2.3/src/haskellian/asyn/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:12:08.685881 haskellian-asyn-0.2.3/src/haskellian/asyn/awaitables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      103 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.3/src/haskellian/asyn/awaitables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.3/src/haskellian/asyn/awaitables/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      390 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.3/src/haskellian/asyn/awaitables/ops.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.3/src/haskellian/asyn/awaitables/promise.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:12:08.685881 haskellian-asyn-0.2.3/src/haskellian/asyn/iterables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-04-10 05:09:35.000000 haskellian-asyn-0.2.3/src/haskellian/asyn/iterables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      756 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.3/src/haskellian/asyn/iterables/managed.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 05:12:08.685881 haskellian-asyn-0.2.3/src/haskellian_asyn.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-10 05:12:08.000000 haskellian-asyn-0.2.3/src/haskellian_asyn.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      518 2024-04-10 05:12:08.000000 haskellian-asyn-0.2.3/src/haskellian_asyn.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-10 05:12:08.000000 haskellian-asyn-0.2.3/src/haskellian_asyn.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-10 05:12:08.000000 haskellian-asyn-0.2.3/src/haskellian_asyn.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-10 05:12:08.000000 haskellian-asyn-0.2.3/src/haskellian_asyn.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.3.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      512 2024-04-10 07:03:19.000000 haskellian-asyn-0.3.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/src/haskellian/asyn/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-04-10 06:58:33.000000 haskellian-asyn-0.3.1/src/haskellian/asyn/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/src/haskellian/asyn/promises/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      127 2024-04-10 06:58:19.000000 haskellian-asyn-0.3.1/src/haskellian/asyn/promises/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      395 2024-04-10 06:58:10.000000 haskellian-asyn-0.3.1/src/haskellian/asyn/promises/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.3.1/src/haskellian/asyn/promises/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      396 2024-04-10 07:01:42.000000 haskellian-asyn-0.3.1/src/haskellian/asyn/promises/ops.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.3.1/src/haskellian/asyn/promises/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:03:21.315885 haskellian-asyn-0.3.1/src/haskellian_asyn.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-10 07:03:21.000000 haskellian-asyn-0.3.1/src/haskellian_asyn.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      465 2024-04-10 07:03:21.000000 haskellian-asyn-0.3.1/src/haskellian_asyn.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-10 07:03:21.000000 haskellian-asyn-0.3.1/src/haskellian_asyn.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-10 07:03:21.000000 haskellian-asyn-0.3.1/src/haskellian_asyn.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-10 07:03:21.000000 haskellian-asyn-0.3.1/src/haskellian_asyn.egg-info/top_level.txt
```

### Comparing `haskellian-asyn-0.2.3/pyproject.toml` & `haskellian-asyn-0.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-asyn"
-version = "0.2.3"
+version = "0.3.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "FP-style tools for async code"
 dependencies = [
   "ramda"
 ]
```

