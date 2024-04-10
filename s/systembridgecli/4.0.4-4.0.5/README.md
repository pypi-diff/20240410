# Comparing `tmp/systembridgecli-4.0.4.tar.gz` & `tmp/systembridgecli-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgecli-4.0.4.tar", last modified: Sun Apr  7 12:17:41 2024, max compression
+gzip compressed data, was "systembridgecli-4.0.5.tar", last modified: Wed Apr 10 00:54:45 2024, max compression
```

## Comparing `systembridgecli-4.0.4.tar` & `systembridgecli-4.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/systembridgecli/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/systembridgecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/systembridgecli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-07 12:17:39.000000 systembridgecli-4.0.4/systembridgecli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/systembridgecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:54:45.657866 systembridgecli-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 00:54:20.000000 systembridgecli-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 00:54:45.657866 systembridgecli-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-10 00:54:20.000000 systembridgecli-4.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-04-10 00:54:20.000000 systembridgecli-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:54:45.657866 systembridgecli-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-10 00:54:20.000000 systembridgecli-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:54:45.657866 systembridgecli-4.0.5/systembridgecli/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 00:54:20.000000 systembridgecli-4.0.5/systembridgecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-10 00:54:20.000000 systembridgecli-4.0.5/systembridgecli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 00:54:44.000000 systembridgecli-4.0.5/systembridgecli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:54:45.657866 systembridgecli-4.0.5/systembridgecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 00:54:45.000000 systembridgecli-4.0.5/systembridgecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-10 00:54:45.000000 systembridgecli-4.0.5/systembridgecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:54:45.000000 systembridgecli-4.0.5/systembridgecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 00:54:45.000000 systembridgecli-4.0.5/systembridgecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 00:54:45.000000 systembridgecli-4.0.5/systembridgecli.egg-info/top_level.txt
```

### Comparing `systembridgecli-4.0.4/LICENSE` & `systembridgecli-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgecli-4.0.4/PKG-INFO` & `systembridgecli-4.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: systembridgecli
-Version: 4.0.4
+Version: 4.0.5
 Summary: System Bridge CLI
 Home-page: https://github.com/timmo001/system-bridge-cli
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: incremental==22.10.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: systembridgeconnector>=4.0.5
 Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.1
+Requires-Dist: typer==0.12.3
 
 # System Bridge - CLI
 
 This is a CLI interface package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgecli-4.0.4/pyproject.toml` & `systembridgecli-4.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgecli-4.0.4/setup.py` & `systembridgecli-4.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgecli-4.0.4/systembridgecli/__main__.py` & `systembridgecli-4.0.5/systembridgecli/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgecli-4.0.4/systembridgecli.egg-info/PKG-INFO` & `systembridgecli-4.0.5/systembridgecli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: systembridgecli
-Version: 4.0.4
+Version: 4.0.5
 Summary: System Bridge CLI
 Home-page: https://github.com/timmo001/system-bridge-cli
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: incremental==22.10.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: systembridgeconnector>=4.0.5
 Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.1
+Requires-Dist: typer==0.12.3
 
 # System Bridge - CLI
 
 This is a CLI interface package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

