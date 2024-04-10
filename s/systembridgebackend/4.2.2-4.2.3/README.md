# Comparing `tmp/systembridgebackend-4.2.2.tar.gz` & `tmp/systembridgebackend-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-4.2.2.tar", last modified: Sun Apr  7 14:05:07 2024, max compression
+gzip compressed data, was "systembridgebackend-4.2.3.tar", last modified: Wed Apr 10 01:03:46 2024, max compression
```

## Comparing `systembridgebackend-4.2.2.tar` & `systembridgebackend-4.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.253085 systembridgebackend-4.2.2/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 14:05:04.000000 systembridgebackend-4.2.2/systembridgebackend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.257085 systembridgebackend-4.2.2/systembridgebackend/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.257085 systembridgebackend-4.2.2/systembridgebackend/handlers/media/
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/media/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.257085 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13483 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/tests/test__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.746523 systembridgebackend-4.2.3/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-10 01:03:44.000000 systembridgebackend-4.2.3/systembridgebackend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.746523 systembridgebackend-4.2.3/systembridgebackend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.746523 systembridgebackend-4.2.3/systembridgebackend/handlers/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/media/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/tests/test__version.py
```

### Comparing `systembridgebackend-4.2.2/LICENSE` & `systembridgebackend-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/PKG-INFO` & `systembridgebackend-4.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.2
+Version: 4.2.3
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
@@ -16,17 +16,17 @@
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: screeninfo==0.8.1
-Requires-Dist: systembridgeconnector>=4.0.5
-Requires-Dist: systembridgemodels>=4.0.4
-Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.1
+Requires-Dist: systembridgeconnector==4.1.2
+Requires-Dist: systembridgemodels==4.1.0
+Requires-Dist: systembridgeshared==4.0.4
+Requires-Dist: typer==0.12.3
 Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: zeroconf==0.132.0
 
 # System Bridge - Backend
 
 This is the backend package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgebackend-4.2.2/pyproject.toml` & `systembridgebackend-4.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/setup.py` & `systembridgebackend-4.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/__init__.py` & `systembridgebackend-4.2.3/systembridgebackend/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/__main__.py` & `systembridgebackend-4.2.3/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/action.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/data.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/keyboard.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/media/__init__.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/media/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/media/windows.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/media/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/power.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/__init__.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/data.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/media.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/update.py` & `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/__init__.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/battery.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/battery.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/cpu.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/disks.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/displays.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/displays.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/gpus.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/listeners.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/media.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/memory.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/networks.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/processes.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/processes.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/sensors.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/modules/system.py` & `systembridgebackend-4.2.3/systembridgebackend/modules/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """System."""
 
 import asyncio
+from enum import StrEnum
 import getpass
 import os
 import platform
 import re
 import socket
 import sys
 from typing import Any, override
@@ -12,21 +13,29 @@
 
 import aiohttp
 from packaging.version import parse
 from plyer import uniqueid
 from psutil import boot_time, users
 from psutil._common import suser
 
-from systembridgemodels.modules.system import RunMode, System, SystemUser
+from systembridgemodels.modules.system import System, SystemUser
 from systembridgeshared.common import get_user_data_directory
 
 from .._version import __version__
 from .base import ModuleUpdateBase
 
 
+# Replace this with systembridgebackend.modules.system.RunMode when possible
+class RunMode(StrEnum):
+    """Run Mode."""
+
+    STANDALONE = "standalone"
+    PYTHON = "python"
+
+
 class SystemUpdate(ModuleUpdateBase):
     """System Update."""
 
     def __init__(self) -> None:
         """Initialise."""
         super().__init__()
         self._mac_address: str = self._get_mac_address()
@@ -340,15 +349,15 @@
             fqdn=fqdn,
             hostname=hostname,
             ip_address_4=ip_address_4,
             mac_address=self._mac_address,
             platform_version=platform_version,
             platform=platform_result,
             uptime=uptime,
-            run_mode=self._run_mode,
+            # run_mode=self._run_mode,
             users=[
                 SystemUser(
                     name=user.name,
                     active=user.name == active_user_name,
                     terminal=user.terminal,
                     host=user.host,
                     started=user.started,
@@ -357,11 +366,11 @@
                 for user in users_result
             ],
             uuid=self._uuid,
             version=self._version or "",
             camera_usage=camera_usage,
             ip_address_6=ip_address_6,
             pending_reboot=pending_reboot,
-            version_latest_url=self._version_latest_url,
+            # version_latest_url=self._version_latest_url,
             version_latest=version_latest,
             version_newer_available=await self._get_version_newer_available(),
         )
```

### Comparing `systembridgebackend-4.2.2/systembridgebackend/server/__init__.py` & `systembridgebackend-4.2.3/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/server/api.py` & `systembridgebackend-4.2.3/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/server/mdns.py` & `systembridgebackend-4.2.3/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend/server/websocket.py` & `systembridgebackend-4.2.3/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.2/systembridgebackend.egg-info/PKG-INFO` & `systembridgebackend-4.2.3/systembridgebackend.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.2
+Version: 4.2.3
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
@@ -16,17 +16,17 @@
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: screeninfo==0.8.1
-Requires-Dist: systembridgeconnector>=4.0.5
-Requires-Dist: systembridgemodels>=4.0.4
-Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.1
+Requires-Dist: systembridgeconnector==4.1.2
+Requires-Dist: systembridgemodels==4.1.0
+Requires-Dist: systembridgeshared==4.0.4
+Requires-Dist: typer==0.12.3
 Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: zeroconf==0.132.0
 
 # System Bridge - Backend
 
 This is the backend package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgebackend-4.2.2/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-4.2.3/systembridgebackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

