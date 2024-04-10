# Comparing `tmp/haskellian-asyn-0.2.1.tar.gz` & `tmp/haskellian-asyn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-asyn-0.2.1.tar", last modified: Mon Apr  8 18:54:33 2024, max compression
+gzip compressed data, was "haskellian-asyn-0.2.2.tar", last modified: Tue Apr  9 17:08:20 2024, max compression
```

## Comparing `haskellian-asyn-0.2.1.tar` & `haskellian-asyn-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.2.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-04-08 18:54:31.000000 haskellian-asyn-0.2.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/asyn/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      195 2024-04-08 18:53:43.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      103 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      390 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/ops.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/promise.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-04-08 18:53:36.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2062 2024-04-08 18:53:32.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/iterables.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      756 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      567 2024-04-08 18:48:30.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/prefetching.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      564 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.2.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      512 2024-04-09 17:08:17.000000 haskellian-asyn-0.2.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 17:08:20.290687 haskellian-asyn-0.2.2/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/src/haskellian/asyn/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      195 2024-04-08 18:53:43.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/src/haskellian/asyn/awaitables/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      103 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/awaitables/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/awaitables/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      390 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/awaitables/ops.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/awaitables/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-04-08 18:53:36.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2062 2024-04-08 18:53:32.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/iterables.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      756 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      567 2024-04-08 18:48:30.000000 haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 17:08:20.300687 haskellian-asyn-0.2.2/src/haskellian_asyn.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-09 17:08:20.000000 haskellian-asyn-0.2.2/src/haskellian_asyn.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-09 17:08:20.000000 haskellian-asyn-0.2.2/src/haskellian_asyn.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 17:08:20.000000 haskellian-asyn-0.2.2/src/haskellian_asyn.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-09 17:08:20.000000 haskellian-asyn-0.2.2/src/haskellian_asyn.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-09 17:08:20.000000 haskellian-asyn-0.2.2/src/haskellian_asyn.egg-info/top_level.txt
```

### Comparing `haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/iterables.py` & `haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/iterables.py`

 * *Files identical despite different names*

### Comparing `haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/managed.py` & `haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/prefetching.py` & `haskellian-asyn-0.2.2/src/haskellian/asyn/iterables/prefetching.py`

 * *Files identical despite different names*

### Comparing `haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/SOURCES.txt` & `haskellian-asyn-0.2.2/src/haskellian_asyn.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 src/haskellian/asyn/iterables/__init__.py
 src/haskellian/asyn/iterables/iterables.py
 src/haskellian/asyn/iterables/managed.py
 src/haskellian/asyn/iterables/prefetching.py
 src/haskellian_asyn.egg-info/PKG-INFO
 src/haskellian_asyn.egg-info/SOURCES.txt
 src/haskellian_asyn.egg-info/dependency_links.txt
+src/haskellian_asyn.egg-info/requires.txt
 src/haskellian_asyn.egg-info/top_level.txt
```

