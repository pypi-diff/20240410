# Comparing `tmp/atomicds-0.0.5.tar.gz` & `tmp/atomicds-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomicds-0.0.5.tar", last modified: Thu Apr  4 00:55:25 2024, max compression
+gzip compressed data, was "atomicds-0.0.6.tar", last modified: Wed Apr 10 15:09:45 2024, max compression
```

## Comparing `atomicds-0.0.5.tar` & `atomicds-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.522187 atomicds-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.522187 atomicds-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-04 00:55:20.000000 atomicds-0.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-04 00:55:20.000000 atomicds-0.0.5/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-04 00:55:20.000000 atomicds-0.0.5/.github/workflows/upgrade_dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-04 00:55:20.000000 atomicds-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-04 00:55:20.000000 atomicds-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 00:55:20.000000 atomicds-0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 00:55:20.000000 atomicds-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 00:55:20.000000 atomicds-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-04 00:55:25.534187 atomicds-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:55:20.000000 atomicds-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-04 00:55:20.000000 atomicds-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.530187 atomicds-0.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:55:25.534187 atomicds-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.522187 atomicds-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.530187 atomicds-0.0.5/src/atomicds/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.530187 atomicds-0.0.5/src/atomicds/core/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/src/atomicds/results/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25799 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/rheed_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/rheed_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/xps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/src/atomicds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:20.000000 atomicds-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-04 00:55:20.000000 atomicds-0.0.5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-04 00:55:20.000000 atomicds-0.0.5/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.539180 atomicds-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.543180 atomicds-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-10 15:09:40.000000 atomicds-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 15:09:40.000000 atomicds-0.0.6/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-10 15:09:40.000000 atomicds-0.0.6/.github/workflows/upgrade_dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-10 15:09:40.000000 atomicds-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-10 15:09:40.000000 atomicds-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 15:09:40.000000 atomicds-0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 15:09:40.000000 atomicds-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 15:09:40.000000 atomicds-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 15:09:45.551180 atomicds-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:09:40.000000 atomicds-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-10 15:09:40.000000 atomicds-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.547180 atomicds-0.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:09:45.551180 atomicds-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.539180 atomicds-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.547180 atomicds-0.0.6/src/atomicds/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.547180 atomicds-0.0.6/src/atomicds/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/src/atomicds/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/rheed_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/rheed_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/xps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/src/atomicds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:40.000000 atomicds-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-10 15:09:40.000000 atomicds-0.0.6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-10 15:09:40.000000 atomicds-0.0.6/tests/test_core.py
```

### Comparing `atomicds-0.0.5/.github/workflows/release.yml` & `atomicds-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/.github/workflows/testing.yml` & `atomicds-0.0.6/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/.github/workflows/upgrade_dependencies.yml` & `atomicds-0.0.6/.github/workflows/upgrade_dependencies.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/.gitignore` & `atomicds-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/.pre-commit-config.yaml` & `atomicds-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/LICENSE` & `atomicds-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/PKG-INFO` & `atomicds-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomicds
-Version: 0.0.5
+Version: 0.0.6
 Summary: API client for Atomic Data Sciences.
 Author-email: Atomic Data Sciences <info@atomicdatasciences.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atomicds-0.0.5/pyproject.toml` & `atomicds-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-macos-latest_py3.10.txt` & `atomicds-0.0.6/requirements/requirements-macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-macos-latest_py3.10_extras.txt` & `atomicds-0.0.6/requirements/requirements-macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-macos-latest_py3.11.txt` & `atomicds-0.0.6/requirements/requirements-macos-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-macos-latest_py3.11_extras.txt` & `atomicds-0.0.6/requirements/requirements-macos-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-macos-latest_py3.9.txt` & `atomicds-0.0.6/requirements/requirements-macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-macos-latest_py3.9_extras.txt` & `atomicds-0.0.6/requirements/requirements-macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10.txt` & `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10_extras.txt` & `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11.txt` & `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11_extras.txt` & `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9.txt` & `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9_extras.txt` & `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-windows-latest_py3.10.txt` & `atomicds-0.0.6/requirements/requirements-windows-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-windows-latest_py3.10_extras.txt` & `atomicds-0.0.6/requirements/requirements-windows-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-windows-latest_py3.11.txt` & `atomicds-0.0.6/requirements/requirements-windows-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-windows-latest_py3.11_extras.txt` & `atomicds-0.0.6/requirements/requirements-windows-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-windows-latest_py3.9.txt` & `atomicds-0.0.6/requirements/requirements-windows-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/requirements/requirements-windows-latest_py3.9_extras.txt` & `atomicds-0.0.6/requirements/requirements-windows-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/src/atomicds/client.py` & `atomicds-0.0.6/src/atomicds/client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/src/atomicds/core/client.py` & `atomicds-0.0.6/src/atomicds/core/client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/src/atomicds/core/utils.py` & `atomicds-0.0.6/src/atomicds/core/utils.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/src/atomicds/results/rheed_image.py` & `atomicds-0.0.6/src/atomicds/results/rheed_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,25 +66,25 @@
         Returns:
             (Image): PIL Image object with optional overlays
 
         """
         image = self.processed_image.copy().convert("RGBA")
         draw = ImageDraw.Draw(image)
 
-        if symmetrize:
+        if symmetrize and self.pattern_graph is not None:
             node_df = pd.DataFrame.from_dict(
                 dict(self.pattern_graph.nodes(data=True)), orient="index"
             )
             _, pattern_graph = self._symmetrize(node_df)
         else:
             pattern_graph = self.pattern_graph
 
         if pattern_graph:
             masks = []
-            for _, node_data in pattern_graph.nodes.data():
+            for node_id, node_data in pattern_graph.nodes.data():
                 if show_mask:
                     mask_rle = node_data.get("mask_rle")
                     mask_width = node_data.get("mask_width")
                     mask_height = node_data.get("mask_height")
 
                     if mask_rle and mask_width and mask_height:
                         mask_dict = {
@@ -109,14 +109,20 @@
                                 center[1] - radius,
                                 center[0] + radius,
                                 center[1] + radius,
                             ),
                             fill=color,
                         )
 
+                        draw.text(
+                            xy=(center[0] - (radius / 2), center[1] - radius),
+                            text=str(node_id),
+                            fill=(255, 255, 255, 255),
+                        )
+
             if show_mask:
                 total_mask = np.stack(masks, axis=0).sum(axis=0).squeeze()
                 overlay = np.zeros((*total_mask.shape, 4), dtype=np.uint8)
                 overlay[np.where(total_mask)] = [255, 0, 0, int(0.2 * (255))]
 
                 overlay = PILImage.fromarray(overlay)
                 image.paste(overlay, mask=overlay)
@@ -192,16 +198,16 @@
         return_as_features: bool = False,
     ) -> pd.DataFrame:
         """Featurize the RHEED image collection into a dataframe of node features and edge features.
 
         Args:
             extra_data (dict | None): Dictionary containing field names and values of extra data to be included in the DataFrame object.
                 Defaults to None.
-            fields_to_retain (list[str] | None): Fields to ensure are kept in the DataFrame object. Defaults to None which
             symmetrize (bool): Whether to symmetrize the data across the vertical axis. Defaults to False.
+            return_as_features (bool): Whether to return a feature-foward version of the DataFrame. Defaults to False.
 
         Returns:
             (DataFrame): Pandas DataFrame object of RHEED node and edge features.
         """
 
         extra_data = extra_data or {}
 
@@ -256,33 +262,29 @@
             columns={col: (col, "") for col in extra_data_df.columns}
         )
         feature_df.columns = pd.MultiIndex.from_tuples(feature_df.columns)
 
         keep_cols = node_feature_cols + list(extra_data.keys())
 
         if return_as_features:
-            return feature_df[keep_cols]
+            return feature_df[keep_cols]  # type: ignore  # noqa: PGH003
 
-        return node_df  # , feature_df[keep_cols]  # type: ignore  # noqa: PGH003
+        return node_df  # type: ignore  # noqa: PGH003
 
     @staticmethod
     def _symmetrize(node_df: pd.DataFrame):
         """Symmetrize a DataFrame object containing RHEED image node data"""
 
-        # def reflect_mask(mask_obj: str, height, width) -> str:
-        #     """Reflect a list of RLE masks across the vertical axis"""
-        #     mask_obj = mask.decode({"counts": mask_obj, "size": (height, width)})
-        #     reflected_mask = np.asfortranarray(np.fliplr(mask_obj))
-        #     return mask.encode(reflected_mask)['counts']
-
-        def reflect_mask(mask_obj: str, height: int, width: int, origin: float) -> str:
+        def reflect_mask(
+            mask_obj: str, height: int, width: int, origin: float
+        ) -> str | bytes:
             """Reflect a list of RLE masks across the vertical axis"""
 
             mask_array: np.ndarray = mask.decode(
-                {"counts": mask_obj, "size": (height, width)}
+                {"counts": mask_obj, "size": (height, width)}  # type: ignore  # noqa: PGH003
             )
             origin = int(np.round(origin, 0))
             num_cols_to_mirror = mask_array.shape[1] - origin
 
             reflected_array = mask_array.copy()
 
             # For columns before the origin position, swap them with their mirrored counterparts
@@ -295,18 +297,19 @@
                     )
 
             return mask.encode(np.asfortranarray(reflected_array))["counts"]
 
         def merge_masks(masks: list[str], height, width) -> str:
             """Merge a list of RLE masks using logical OR"""
             mask_objs = [
-                mask.decode({"counts": mm, "size": (height, width)}) for mm in masks
+                mask.decode({"counts": mm, "size": (height, width)})  # type: ignore  # noqa: PGH003
+                for mm in masks
             ]
             merged_mask = np.asfortranarray(np.logical_or.reduce(mask_objs))
-            return mask.encode(merged_mask)
+            return mask.encode(merged_mask)  # type: ignore  # noqa: PGH003
 
         def merge_overlaps(node_df):
             """Merge overlapping nodes in a DataFrame object. Use recursively until no overlaps remain."""
 
             first_row = node_df.iloc[[0]]
             original_dtypes = first_row.dtypes
 
@@ -355,27 +358,33 @@
                         ),
                         axis=1,
                     )
                 ]
 
                 merged_row = overlapping_nodes.agg(agg_dict)
 
-                new_mask = merge_masks(
+                new_mask = merge_masks(  # type: ignore  # noqa: PGH003
                     merged_row["mask_rle"],
                     merged_row["mask_height"],
                     merged_row["mask_width"],
                 )["counts"]
                 merged_row["mask_rle"] = new_mask
 
                 new_df = pd.concat([new_df, merged_row], axis=1)
 
             new_df = new_df.T.astype(original_dtypes).reset_index(drop=True)
-            agg_dict["mask_rle"] = lambda x: merge_masks(
-                x, new_df["mask_height"].iloc[0], new_df["mask_width"].iloc[0]
-            )["counts"]
+
+            agg_dict["mask_rle"] = lambda x: merge_masks(  # type: ignore  # noqa: PGH003
+                x,
+                new_df["mask_height"].iloc[0],  # type: ignore  # noqa: PGH003
+                new_df["mask_width"].iloc[0],  # type: ignore  # noqa: PGH003
+            )[
+                "counts"
+            ]
+
             new_df = new_df.groupby("node_id").agg(agg_dict).reset_index(drop=True)
 
             # relabel node_id > 1000 to monotonically increase from the largest ID < 1000
             while new_df["node_id"].max() > 1000:
                 max_id = new_df.loc[new_df["node_id"] < 1000]["node_id"].max()
                 new_df.loc[new_df["node_id"] == new_df["node_id"].max(), "node_id"] = (
                     max_id + 1
@@ -384,14 +393,15 @@
             return new_df
 
         reflection_plane = node_df["specular_origin_1"].mean()
 
         left_nodes = node_df.loc[node_df["centroid_1"] < reflection_plane]
         right_nodes = node_df.loc[node_df["centroid_1"] > reflection_plane]
 
+        # TODO: The repeat code here can be condensed.
         left_to_right = left_nodes.copy()
         left_to_right["centroid_1"] = reflection_plane + (
             reflection_plane - left_to_right["centroid_1"]
         )
         left_to_right["intensity_centroid_1"] = -left_to_right["intensity_centroid_1"]
         left_to_right["relative_centroid_1"] = -left_to_right["relative_centroid_1"]
         left_to_right["mask_rle"] = left_to_right["mask_rle"].apply(
@@ -405,14 +415,15 @@
 
         new_max = (
             reflection_plane + (reflection_plane - left_to_right["bbox_minc"])
         ).astype(int)
         new_min = (
             reflection_plane + (reflection_plane - left_to_right["bbox_maxc"])
         ).astype(int)
+
         left_to_right["bbox_maxc"] = new_max
         left_to_right["bbox_minc"] = new_min
 
         left_to_right["node_id"] = left_to_right["node_id"] + 1000
 
         right_to_left = right_nodes.copy()
         right_to_left["centroid_1"] = reflection_plane - (
@@ -447,18 +458,18 @@
         if node_df.empty:
             return node_df
 
         node_df = node_df.drop(columns=["last_updated", "version"])
 
         new_df = merge_overlaps(node_df)
         while len(new_df) != len(node_df):
-            node_df = new_df.copy(deep=True)
+            node_df = new_df.copy(deep=True)  # type: ignore  # noqa: PGH003
             new_df = merge_overlaps(node_df)
 
-        new_pattern_graph = generate_graph_from_nodes(new_df)
+        new_pattern_graph = generate_graph_from_nodes(new_df)  # type: ignore  # noqa: PGH003
 
         return new_df, new_pattern_graph
 
 
 # TODO: Add tests for RHEEDImageCollection
 class RHEEDImageCollection(MSONable):
     def __init__(
@@ -469,14 +480,15 @@
     ):
         """Collection of RHEED images
 
         Args:
             rheed_images (list[RHEEDImageResult]): List of RHEEDImageResult objects.
             extra_data (list[dict] | None): List of dictionaries containing field names and values of extra data to be included in the DataFrame object.
                 Defaults to None.
+            sort_key (str | None): Key used to sort the data with.
         """
 
         extra_data = extra_data or []  # type: ignore  # noqa: PGH003
 
         if len(extra_data) > 0 and len(extra_data) != len(rheed_images):
             raise ValueError(
                 "List of extra data must be the same length as the RHEED image collection."
@@ -485,18 +497,19 @@
         for idx, rheed_image in enumerate(rheed_images):
             if rheed_image.pattern_graph:
                 for node in rheed_image.pattern_graph.nodes:
                     rheed_image.pattern_graph.nodes[node]["pattern_id"] = idx
 
         self._rheed_images = rheed_images
         self._extra_data = extra_data
+
         self._sort_key = sort_key
-        if self._sort_key is None:
-            self._sort_key = next(iter(self._extra_data[0].keys()))
-        self._sort_by_extra_data_key(self._sort_key)
+
+        if self._sort_key is not None:
+            self._sort_by_extra_data_key(self._sort_key)
 
     @property
     def rheed_images(self):
         return self._rheed_images
 
     @property
     def extra_data(self):
@@ -517,15 +530,14 @@
             (tuple[DataFrame, list[RHEEDImageResult]): Pandas DataFrame object with aligned RHEED fingerprint data
         """
 
         image_scales = [
             rheed_image.processed_image.size for rheed_image in self.rheed_images
         ]
         image_scale = np.amax(image_scales, axis=0)
-        # data_ids = [rheed_image.data_id for rheed_image in self.rheed_images]
 
         if node_df is None:
             node_dfs = [
                 rheed_image.get_pattern_dataframe(
                     extra_data=extra_data, symmetrize=False, return_as_features=False
                 )
                 for rheed_image, extra_data in zip(self.rheed_images, self.extra_data)
@@ -574,14 +586,17 @@
         return_as_features: bool = True,
     ) -> tuple[pd.DataFrame, pd.DataFrame]:
         """Featurize the RHEED image collection into a dataframe of node features and edge features.
 
         Args:
             streamline (bool): Whether to remove streamline the DataFrame object and remove null values. Defaults to True.
             normalize (bool): Whether to min/max normalize the feature data across all images. Defaults to True.
+            symmetrize (bool): Whether to symmetrize the RHEEED images and segmented patterns about the vertical axis before
+                obtaining the DataFrame representation. Defaults to False.
+            return_as_features (bool): Whether to return the final feature-forward DataFrame. Defaults to True.
 
         Returns:
             (DataFrame): Pandas DataFrame object of RHEED node and edge features.
         """
 
         node_feature_cols = [
             "spot_area",
@@ -600,72 +615,48 @@
             "axis_major_length",
             "axis_minor_length",
         ]
 
         # TODO: add edge features
         # edge_feature_cols = ["weight", "horizontal_weight", "vertical_weight", "horizontal_overlap"]
 
-        if self.extra_data:
-            node_dfs = [
-                rheed_image.get_pattern_dataframe(
-                    extra_data=extra_data,
-                    symmetrize=symmetrize,
-                    return_as_features=False,
-                )
-                for rheed_image, extra_data in zip(self.rheed_images, self.extra_data)
-            ]
-            feature_dfs = [
-                rheed_image.get_pattern_dataframe(
-                    extra_data=extra_data,
-                    symmetrize=symmetrize,
-                    return_as_features=True,
-                )
-                for rheed_image, extra_data in zip(self.rheed_images, self.extra_data)
-            ]
-        else:
-            node_dfs = [
-                rheed_image.get_pattern_dataframe(
-                    symmetrize=symmetrize, return_as_features=False
-                )
-                for rheed_image in self.rheed_images
-            ]
-            feature_dfs = [
-                rheed_image.get_pattern_dataframe(
-                    symmetrize=symmetrize, return_as_features=True
-                )
-                for rheed_image in self.rheed_images
-            ]
+        image_iter = (
+            zip(self.rheed_images, self.extra_data)
+            if self.extra_data
+            else zip(self.rheed_images, [None] * len(self.rheed_images))
+        )
 
-        node_df = pd.concat(node_dfs, axis=0).reset_index(drop=True)
-        feature_df = pd.concat(feature_dfs, axis=0).reset_index(drop=True)
+        dfs = [
+            rheed_image.get_pattern_dataframe(
+                extra_data=extra_data,
+                symmetrize=symmetrize,
+                return_as_features=return_as_features,
+            )
+            for rheed_image, extra_data in image_iter
+        ]
+
+        data_df = pd.concat(dfs, axis=0).reset_index(drop=True)
 
         keep_cols = node_feature_cols + list(
             {key for extra_data in self.extra_data for key in extra_data}
         )
 
-        feature_df = feature_df[keep_cols]
-
-        if streamline:
-            feature_df = feature_df.dropna(axis=1)
-
-        if normalize:
-            for col in node_feature_cols:
-                feature_df[col] = (feature_df[col] - feature_df[col].mean()) / (
-                    feature_df[col].std()
-                )
+        if return_as_features:
+            data_df = data_df[keep_cols]
 
-            # min max normalization
-            # feature_df[node_feature_cols].apply(
-            #     lambda x: (x - x.min()) / (x.max() - x.min()), inp
-            # )
+            if streamline:
+                data_df = data_df.dropna(axis=1)
 
-        if return_as_features:
-            return feature_df
+            if normalize:
+                for col in node_feature_cols:
+                    data_df[col] = (data_df[col] - data_df[col].mean()) / data_df[
+                        col
+                    ].std()
 
-        return node_df  # , feature_df  # type: ignore  # noqa: PGH003
+        return data_df  # type: ignore  # noqa: PGH003
 
     def _sort_by_extra_data_key(self, key: str):
         """Sort the RHEEDImageCollection by an extra data key"""
         if key not in self.extra_data[0]:
             raise ValueError(
                 f"Extra data key {key} not found in the extra data dictionary."
             )
@@ -682,12 +673,14 @@
 
         if isinstance(key, slice):
             return self.__class__(
                 self.rheed_images[key], self.extra_data[key], self.sort_key
             )
 
         return self.__class__(
-            self.rheed_images[key], self.extra_data[key], self.sort_key
+            self.rheed_images[key],  # type: ignore  # noqa: PGH003
+            self.extra_data[key],  # type: ignore  # noqa: PGH003
+            self.sort_key,
         )
 
     def __len__(self) -> int:
         return len(self.rheed_images)
```

### Comparing `atomicds-0.0.5/src/atomicds/results/rheed_video.py` & `atomicds-0.0.6/src/atomicds/results/rheed_video.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/src/atomicds/results/xps.py` & `atomicds-0.0.6/src/atomicds/results/xps.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/src/atomicds.egg-info/PKG-INFO` & `atomicds-0.0.6/src/atomicds.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomicds
-Version: 0.0.5
+Version: 0.0.6
 Summary: API client for Atomic Data Sciences.
 Author-email: Atomic Data Sciences <info@atomicdatasciences.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atomicds-0.0.5/src/atomicds.egg-info/SOURCES.txt` & `atomicds-0.0.6/src/atomicds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/tests/test_client.py` & `atomicds-0.0.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.5/tests/test_core.py` & `atomicds-0.0.6/tests/test_core.py`

 * *Files identical despite different names*

