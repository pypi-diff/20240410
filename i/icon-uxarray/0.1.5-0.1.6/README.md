# Comparing `tmp/icon_uxarray-0.1.5.tar.gz` & `tmp/icon_uxarray-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icon_uxarray-0.1.5.tar", last modified: Tue Apr  9 13:45:27 2024, max compression
+gzip compressed data, was "icon_uxarray-0.1.6.tar", last modified: Tue Apr  9 15:36:01 2024, max compression
```

## Comparing `icon_uxarray-0.1.5.tar` & `icon_uxarray-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.683740 icon_uxarray-0.1.5/icon_uxarray/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/icon_uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/Torus_Triangles_100m_x_100m_res5m.nc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.915298 icon_uxarray-0.1.6/icon_uxarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/icon_uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/Torus_Triangles_100m_x_100m_res5m.nc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/test_base.py
```

### Comparing `icon_uxarray-0.1.5/HISTORY.md` & `icon_uxarray-0.1.6/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Add base module to top level. [Jacopo]
+- Fix package name in installation command. [Jacopo]
+
+
+0.1.5 (2024-04-09)
+------------------
+- Release: version 0.1.5 🚀 [Jacopo]
 - Refactor remove_torus_boundaries function to handle invalid input
   gracefully. [Jacopo]
 - Actually get make release to work properly with tags. [Jacopo]
 
 
 0.1.4 (2024-04-09)
 ------------------
```

### Comparing `icon_uxarray-0.1.5/LICENSE` & `icon_uxarray-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.5/PKG-INFO` & `icon_uxarray-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.5
+Version: 0.1.6
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
@@ -37,15 +37,15 @@
 [![CI](https://github.com/jcanton/icon_uxarray/actions/workflows/main.yml/badge.svg)](https://github.com/jcanton/icon_uxarray/actions/workflows/main.yml)
 
 Awesome icon_uxarray created by jcanton
 
 ## Install it from PyPI
 
 ```bash
-pip install icon_uxarray
+pip install icon-uxarray
 ```
 
 ## Usage
 
 Convert an icon grid to be UGRID-compatible
 
 ```py
```

### Comparing `icon_uxarray-0.1.5/README.md` & `icon_uxarray-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![CI](https://github.com/jcanton/icon_uxarray/actions/workflows/main.yml/badge.svg)](https://github.com/jcanton/icon_uxarray/actions/workflows/main.yml)
 
 Awesome icon_uxarray created by jcanton
 
 ## Install it from PyPI
 
 ```bash
-pip install icon_uxarray
+pip install icon-uxarray
 ```
 
 ## Usage
 
 Convert an icon grid to be UGRID-compatible
 
 ```py
```

### Comparing `icon_uxarray-0.1.5/icon_uxarray/base.py` & `icon_uxarray-0.1.6/icon_uxarray/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 """
 
 import os
 import numpy as np
 import xarray as xr
 import uxarray as ux
 
+__all__ = [
+    "icon_grid_2_ugrid",
+    "remove_torus_boundaries",
+]
+
 
 # ==============================================================================
 def icon_grid_2_ugrid(icon_grid_fname: str) -> str:
     """
     Convert an ICON grid to being UGRID-compatible.
 
     Parameters:
```

### Comparing `icon_uxarray-0.1.5/icon_uxarray/cli.py` & `icon_uxarray-0.1.6/icon_uxarray/cli.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.5/icon_uxarray.egg-info/PKG-INFO` & `icon_uxarray-0.1.6/icon_uxarray.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.5
+Version: 0.1.6
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
@@ -37,15 +37,15 @@
 [![CI](https://github.com/jcanton/icon_uxarray/actions/workflows/main.yml/badge.svg)](https://github.com/jcanton/icon_uxarray/actions/workflows/main.yml)
 
 Awesome icon_uxarray created by jcanton
 
 ## Install it from PyPI
 
 ```bash
-pip install icon_uxarray
+pip install icon-uxarray
 ```
 
 ## Usage
 
 Convert an icon grid to be UGRID-compatible
 
 ```py
```

### Comparing `icon_uxarray-0.1.5/setup.py` & `icon_uxarray-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.5/tests/Torus_Triangles_100m_x_100m_res5m.nc` & `icon_uxarray-0.1.6/tests/Torus_Triangles_100m_x_100m_res5m.nc`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.5/tests/conftest.py` & `icon_uxarray-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.5/tests/test_base.py` & `icon_uxarray-0.1.6/tests/test_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Test module.
 """
 
-import pytest
 import os
+import pytest
 import xarray as xr
 import uxarray as ux
 from icon_uxarray.base import (
     icon_grid_2_ugrid,
     is_boundary_triangle,
     remove_torus_boundaries,
 )
```

