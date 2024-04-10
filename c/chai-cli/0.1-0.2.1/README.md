# Comparing `tmp/chai-cli-0.1.tar.gz` & `tmp/chai-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chai-cli-0.1.tar", last modified: Wed Apr 10 18:54:55 2024, max compression
+gzip compressed data, was "chai-cli-0.2.1.tar", last modified: Wed Apr 10 20:06:27 2024, max compression
```

## Comparing `chai-cli-0.1.tar` & `chai-cli-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2024-04-10 18:54:55.037515 chai-cli-0.1/
--rw-rw-r--   0 deep      (1000) deep      (1000)      158 2024-04-10 18:54:55.037515 chai-cli-0.1/PKG-INFO
--rw-rw-r--   0 deep      (1000) deep      (1000)       38 2024-04-10 18:54:55.037515 chai-cli-0.1/setup.cfg
--rw-rw-r--   0 deep      (1000) deep      (1000)      472 2024-04-10 18:54:07.000000 chai-cli-0.1/setup.py
-drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2024-04-10 18:54:55.033515 chai-cli-0.1/src/
-drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2024-04-10 18:54:55.037515 chai-cli-0.1/src/chai/
--rw-rw-r--   0 deep      (1000) deep      (1000)     1224 2024-04-10 18:41:48.000000 chai-cli-0.1/src/chai/__init__.py
--rw-rw-r--   0 deep      (1000) deep      (1000)       57 2024-04-10 13:28:04.000000 chai-cli-0.1/src/chai/__main__.py
-drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2024-04-10 18:54:55.037515 chai-cli-0.1/src/chai_cli.egg-info/
--rw-rw-r--   0 deep      (1000) deep      (1000)      158 2024-04-10 18:54:54.000000 chai-cli-0.1/src/chai_cli.egg-info/PKG-INFO
--rw-rw-r--   0 deep      (1000) deep      (1000)      268 2024-04-10 18:54:54.000000 chai-cli-0.1/src/chai_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)        1 2024-04-10 18:54:54.000000 chai-cli-0.1/src/chai_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)       35 2024-04-10 18:54:54.000000 chai-cli-0.1/src/chai_cli.egg-info/entry_points.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)       16 2024-04-10 18:54:54.000000 chai-cli-0.1/src/chai_cli.egg-info/requires.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)        5 2024-04-10 18:54:54.000000 chai-cli-0.1/src/chai_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.792179 chai-cli-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 20:06:24.000000 chai-cli-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-10 20:06:27.788179 chai-cli-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-10 20:06:24.000000 chai-cli-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:06:27.792179 chai-cli-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 20:06:24.000000 chai-cli-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.788179 chai-cli-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.788179 chai-cli-0.2.1/src/chai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-10 20:06:24.000000 chai-cli-0.2.1/src/chai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 20:06:24.000000 chai-cli-0.2.1/src/chai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:06:27.788179 chai-cli-0.2.1/src/chai_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 20:06:27.000000 chai-cli-0.2.1/src/chai_cli.egg-info/top_level.txt
```

### Comparing `chai-cli-0.1/src/chai/__init__.py` & `chai-cli-0.2.1/src/chai/__init__.py`

 * *Files identical despite different names*

