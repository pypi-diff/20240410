# Comparing `tmp/sniffles-2.3.tar.gz` & `tmp/sniffles-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffles-2.3.tar", last modified: Wed Apr 10 13:38:48 2024, max compression
+gzip compressed data, was "sniffles-2.3.1.tar", last modified: Wed Apr 10 19:32:59 2024, max compression
```

## Comparing `sniffles-2.3.tar` & `sniffles-2.3.1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.434989 sniffles-2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 13:38:44.000000 sniffles-2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-10 13:38:48.434989 sniffles-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-10 13:38:44.000000 sniffles-2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 13:38:44.000000 sniffles-2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-10 13:38:48.434989 sniffles-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-10 13:38:44.000000 sniffles-2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.426989 sniffles-2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.430989 sniffles-2.3/src/sniffles/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/consensus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25903 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/leadprov.py
--rw-r--r--   0 runner    (1001) docker     (127)    24149 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/snf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21199 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/sniffles
--rwxr-xr-x   0 runner    (1001) docker     (127)    24081 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/sv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18412 2024-04-10 13:38:44.000000 sniffles-2.3/src/sniffles/vcf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:38:48.430989 sniffles-2.3/src/sniffles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 13:38:48.000000 sniffles-2.3/src/sniffles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.614698 sniffles-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 19:32:49.000000 sniffles-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 19:32:59.614698 sniffles-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-10 19:32:49.000000 sniffles-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 19:32:49.000000 sniffles-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 19:32:59.614698 sniffles-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-10 19:32:49.000000 sniffles-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.606698 sniffles-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.610698 sniffles-2.3.1/src/sniffles/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25903 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/leadprov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24149 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/snf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21208 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/sniffles
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24081 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/sv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.614698 sniffles-2.3.1/src/sniffles/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/utils/resmon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18412 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.614698 sniffles-2.3.1/src/sniffles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/top_level.txt
```

### Comparing `sniffles-2.3/LICENSE` & `sniffles-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/PKG-INFO` & `sniffles-2.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.3
+Version: 2.3.1
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
 Author: Moritz Smolka, Hermann Romanek
 Author-email: moritz.g.smolka@gmail.com, sniffles@romanek.at
 License: MIT
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pysam>=0.21.0
-Provides-Extra: align
-Requires-Dist: edlib>=1.3.9; extra == "align"
-Provides-Extra: mem
-Requires-Dist: psutil>=5.9.4; extra == "mem"
-Provides-Extra: all
-Requires-Dist: edlib>=1.3.9; extra == "all"
-Requires-Dist: psutil>=5.9.4; extra == "all"
+Requires-Dist: edlib>=1.3.9
+Requires-Dist: psutil>=5.9.4
 
 # Sniffles2
 A fast structural variant caller for long-read sequencing, Sniffles2 accurately detect SVs on germline, somatic and population-level for PacBio and Oxford Nanopore read data.
 
 ## Quick Start: Germline SV calling using Sniffles2
 To call SVs from long read alignments (PacBio / ONT), you can use:
```

### Comparing `sniffles-2.3/README.md` & `sniffles-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/setup.cfg` & `sniffles-2.3.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sniffles
-version = 2.3
+version = 2.3.1
 author = Moritz Smolka, Hermann Romanek
 author_email = moritz.g.smolka@gmail.com, sniffles@romanek.at
 description = A fast structural variation caller for long-read sequencing data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritzsedlazeck/Sniffles
 project_urls = 
@@ -17,25 +17,18 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	pysam>=0.21.0
-scripts = 
-	src/sniffles/sniffles
-
-[options.extras_require]
-align = 
-	edlib>=1.3.9
-mem = 
-	psutil>=5.9.4
-all = 
 	edlib>=1.3.9
 	psutil>=5.9.4
+scripts = 
+	src/sniffles/sniffles
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sniffles-2.3/src/sniffles/cluster.py` & `sniffles-2.3.1/src/sniffles/cluster.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/config.py` & `sniffles-2.3.1/src/sniffles/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import argparse
 
 from typing import Union, Optional
 
 from sniffles import util
 
 VERSION = "Sniffles2"
-BUILD = "2.3.0"
+BUILD = "2.3.1"
 SNF_VERSION = "S2_rc4"
 
 
 class ArgFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
     pass
```

### Comparing `sniffles-2.3/src/sniffles/consensus.py` & `sniffles-2.3.1/src/sniffles/consensus.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/leadprov.py` & `sniffles-2.3.1/src/sniffles/leadprov.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/parallel.py` & `sniffles-2.3.1/src/sniffles/parallel.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/postprocessing.py` & `sniffles-2.3.1/src/sniffles/postprocessing.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/result.py` & `sniffles-2.3.1/src/sniffles/result.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/snf.py` & `sniffles-2.3.1/src/sniffles/snf.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/sniffles` & `sniffles-2.3.1/src/sniffles/sniffles`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Maintainer:  Hermann Romanek
 # Contact:     sniffles@romanek.at
 #
 import logging
 import logging.config
 from typing import Optional
 
-from utils.resmon import ResourceMonitor
+from sniffles.utils.resmon import ResourceMonitor
 
 DEV_MONITOR_MEM = False
 
 import sys
 
 if not sys.version_info >= (3, 10):
     print(f"Error: Sniffles2 must be run with Python version 3.10 or above (detected Python version: {sys.version_info.major}.{sys.version_info.minor}). Exiting")
```

### Comparing `sniffles-2.3/src/sniffles/sv.py` & `sniffles-2.3.1/src/sniffles/sv.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/util.py` & `sniffles-2.3.1/src/sniffles/util.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles/vcf.py` & `sniffles-2.3.1/src/sniffles/vcf.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3/src/sniffles.egg-info/PKG-INFO` & `sniffles-2.3.1/src/sniffles.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.3
+Version: 2.3.1
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
 Author: Moritz Smolka, Hermann Romanek
 Author-email: moritz.g.smolka@gmail.com, sniffles@romanek.at
 License: MIT
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pysam>=0.21.0
-Provides-Extra: align
-Requires-Dist: edlib>=1.3.9; extra == "align"
-Provides-Extra: mem
-Requires-Dist: psutil>=5.9.4; extra == "mem"
-Provides-Extra: all
-Requires-Dist: edlib>=1.3.9; extra == "all"
-Requires-Dist: psutil>=5.9.4; extra == "all"
+Requires-Dist: edlib>=1.3.9
+Requires-Dist: psutil>=5.9.4
 
 # Sniffles2
 A fast structural variant caller for long-read sequencing, Sniffles2 accurately detect SVs on germline, somatic and population-level for PacBio and Oxford Nanopore read data.
 
 ## Quick Start: Germline SV calling using Sniffles2
 To call SVs from long read alignments (PacBio / ONT), you can use:
```

### Comparing `sniffles-2.3/src/sniffles.egg-info/SOURCES.txt` & `sniffles-2.3.1/src/sniffles.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 src/sniffles/sv.py
 src/sniffles/util.py
 src/sniffles/vcf.py
 src/sniffles.egg-info/PKG-INFO
 src/sniffles.egg-info/SOURCES.txt
 src/sniffles.egg-info/dependency_links.txt
 src/sniffles.egg-info/requires.txt
-src/sniffles.egg-info/top_level.txt
+src/sniffles.egg-info/top_level.txt
+src/sniffles/utils/__init__.py
+src/sniffles/utils/resmon.py
```

