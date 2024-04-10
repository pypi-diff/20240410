# Comparing `tmp/bibiflags-0.1.0.tar.gz` & `tmp/bibiflags-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibiflags-0.1.0.tar", last modified: Wed Apr 10 06:43:25 2024, max compression
+gzip compressed data, was "bibiflags-0.1.1.tar", last modified: Wed Apr 10 07:14:25 2024, max compression
```

## Comparing `bibiflags-0.1.0.tar` & `bibiflags-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.561262 bibiflags-0.1.0/
--rw-rw-rw-   0        0        0     1067 2021-10-28 05:43:21.000000 bibiflags-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      297 2024-04-10 06:25:01.000000 bibiflags-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2094 2024-04-10 06:43:25.560263 bibiflags-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2024-04-10 06:22:22.000000 bibiflags-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.527063 bibiflags-0.1.0/docs/
--rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiflags-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiflags-0.1.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.530064 bibiflags-0.1.0/docs/source/
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.531064 bibiflags-0.1.0/docs/source/_static/
--rw-rw-rw-   0        0        0    33653 2024-04-10 06:08:59.000000 bibiflags-0.1.0/docs/source/_static/bibiflags.png
--rw-rw-rw-   0        0        0     6901 2024-04-10 05:06:41.000000 bibiflags-0.1.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiflags-0.1.0/docs/source/install.rst
--rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiflags-0.1.0/docs/source/quickstart.rst
--rw-rw-rw-   0        0        0      554 2024-04-10 05:46:02.000000 bibiflags-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 06:43:25.562263 bibiflags-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.518794 bibiflags-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.535064 bibiflags-0.1.0/src/bibiflags/
--rw-rw-rw-   0        0        0       23 2024-04-10 05:07:07.000000 bibiflags-0.1.0/src/bibiflags/__init__.py
--rw-rw-rw-   0        0        0     5138 2024-04-10 06:01:11.000000 bibiflags-0.1.0/src/bibiflags/bibiflags.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.0/src/bibiflags/bibiflags.yaml
--rw-rw-rw-   0        0        0       11 2024-04-10 05:49:39.000000 bibiflags-0.1.0/src/bibiflags/test_bibiflags.yaml
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.559262 bibiflags-0.1.0/src/bibiflags.egg-info/
--rw-rw-rw-   0        0        0     2094 2024-04-10 06:43:25.000000 bibiflags-0.1.0/src/bibiflags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2024-04-10 06:43:25.000000 bibiflags-0.1.0/src/bibiflags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 06:43:25.000000 bibiflags-0.1.0/src/bibiflags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-10 06:43:25.000000 bibiflags-0.1.0/src/bibiflags.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-10 06:43:25.000000 bibiflags-0.1.0/src/bibiflags.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.554261 bibiflags-0.1.0/src/examples/
--rw-rw-rw-   0        0        0      258 2024-04-10 06:03:06.000000 bibiflags-0.1.0/src/examples/main.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.0/src/examples/main.yaml
--rw-rw-rw-   0        0        0      429 2024-04-10 06:02:54.000000 bibiflags-0.1.0/src/examples/prog.py
--rw-rw-rw-   0        0        0        0 2024-04-10 06:01:38.000000 bibiflags-0.1.0/src/examples/prog.yaml
-drwxrwxrwx   0        0        0        0 2024-04-10 06:43:25.558264 bibiflags-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-10 04:59:44.000000 bibiflags-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      295 2024-04-10 05:54:23.000000 bibiflags-0.1.0/tests/test_bibiflags.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.0/tests/test_bibiflags.yaml
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.808660 bibiflags-0.1.1/
+-rw-rw-rw-   0        0        0     1067 2021-10-28 05:43:21.000000 bibiflags-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      297 2024-04-10 06:25:01.000000 bibiflags-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2064 2024-04-10 07:14:25.807661 bibiflags-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1735 2024-04-10 06:22:22.000000 bibiflags-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.770655 bibiflags-0.1.1/docs/
+-rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiflags-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiflags-0.1.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.773654 bibiflags-0.1.1/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.774655 bibiflags-0.1.1/docs/source/_static/
+-rw-rw-rw-   0        0        0    33653 2024-04-10 06:08:59.000000 bibiflags-0.1.1/docs/source/_static/bibiflags.png
+-rw-rw-rw-   0        0        0     6901 2024-04-10 05:06:41.000000 bibiflags-0.1.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiflags-0.1.1/docs/source/install.rst
+-rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiflags-0.1.1/docs/source/quickstart.rst
+-rw-rw-rw-   0        0        0      532 2024-04-10 07:11:05.000000 bibiflags-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 07:14:25.809659 bibiflags-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.762669 bibiflags-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.777659 bibiflags-0.1.1/src/bibiflags/
+-rw-rw-rw-   0        0        0      104 2024-04-10 07:11:18.000000 bibiflags-0.1.1/src/bibiflags/__init__.py
+-rw-rw-rw-   0        0        0     5163 2024-04-10 07:12:05.000000 bibiflags-0.1.1/src/bibiflags/bibiflags.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.1/src/bibiflags/bibiflags.yaml
+-rw-rw-rw-   0        0        0       11 2024-04-10 05:49:39.000000 bibiflags-0.1.1/src/bibiflags/test_bibiflags.yaml
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.806660 bibiflags-0.1.1/src/bibiflags.egg-info/
+-rw-rw-rw-   0        0        0     2064 2024-04-10 07:14:25.000000 bibiflags-0.1.1/src/bibiflags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2024-04-10 07:14:25.000000 bibiflags-0.1.1/src/bibiflags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 07:14:25.000000 bibiflags-0.1.1/src/bibiflags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-10 07:14:25.000000 bibiflags-0.1.1/src/bibiflags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-10 07:14:25.000000 bibiflags-0.1.1/src/bibiflags.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.803655 bibiflags-0.1.1/src/examples/
+-rw-rw-rw-   0        0        0      222 2024-04-10 07:12:56.000000 bibiflags-0.1.1/src/examples/main.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.1/src/examples/main.yaml
+-rw-rw-rw-   0        0        0      402 2024-04-10 07:13:07.000000 bibiflags-0.1.1/src/examples/prog.py
+-rw-rw-rw-   0        0        0        0 2024-04-10 06:01:38.000000 bibiflags-0.1.1/src/examples/prog.yaml
+drwxrwxrwx   0        0        0        0 2024-04-10 07:14:25.805658 bibiflags-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-10 04:59:44.000000 bibiflags-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      265 2024-04-10 07:13:27.000000 bibiflags-0.1.1/tests/test_bibiflags.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.1/tests/test_bibiflags.yaml
```

### Comparing `bibiflags-0.1.0/LICENSE` & `bibiflags-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/PKG-INFO` & `bibiflags-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: bibiflags
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import YAML configs into Arguments for Python
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: OmegaConf>=2.3.0
-Requires-Dist: loguru>=0.7.2
 
 ![bibiflags](./docs/source/_static/bibiflags.png)
 ===
 
 bibiflags is a python tool to import YAML configs into Arguments for Python . 
 
 It provides 2 ways to use it:
```

### Comparing `bibiflags-0.1.0/README.md` & `bibiflags-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/docs/Makefile` & `bibiflags-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/docs/source/_static/bibiflags.png` & `bibiflags-0.1.1/docs/source/_static/bibiflags.png`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/docs/source/conf.py` & `bibiflags-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/docs/source/quickstart.rst` & `bibiflags-0.1.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/pyproject.toml` & `bibiflags-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [project]
 name = "bibiflags"
-version = "0.1.0"
+version = "0.1.1"
 description = "Import YAML configs into Arguments for Python"
 authors = [
     {name = "Chunqi SHI", email = "chunqishi@gmail.com"},
 ]
 dependencies = [
     "PyYAML>=6.0.1",
     "OmegaConf>=2.3.0",
-    "loguru>=0.7.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 
 [build-system]
 requires = ["setuptools>=61", "wheel"]
```

### Comparing `bibiflags-0.1.0/src/bibiflags/bibiflags.py` & `bibiflags-0.1.1/src/bibiflags/bibiflags.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import argparse
 import builtins
 import inspect
 import os
 import pathlib
 from collections import OrderedDict
 from pprint import pformat
-
-from loguru import logger
+import logging
+logger = logging.getLogger(__name__)
 from omegaconf import OmegaConf
 
 
 class BibiFlags:
     names = [
         'dest',
         'type',
```

### Comparing `bibiflags-0.1.0/src/bibiflags/bibiflags.yaml` & `bibiflags-0.1.1/src/bibiflags/bibiflags.yaml`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/src/bibiflags.egg-info/PKG-INFO` & `bibiflags-0.1.1/src/bibiflags.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: bibiflags
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import YAML configs into Arguments for Python
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: OmegaConf>=2.3.0
-Requires-Dist: loguru>=0.7.2
 
 ![bibiflags](./docs/source/_static/bibiflags.png)
 ===
 
 bibiflags is a python tool to import YAML configs into Arguments for Python . 
 
 It provides 2 ways to use it:
```

### Comparing `bibiflags-0.1.0/src/bibiflags.egg-info/SOURCES.txt` & `bibiflags-0.1.1/src/bibiflags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/src/examples/main.yaml` & `bibiflags-0.1.1/src/examples/main.yaml`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.0/tests/test_bibiflags.yaml` & `bibiflags-0.1.1/tests/test_bibiflags.yaml`

 * *Files identical despite different names*

