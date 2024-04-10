# Comparing `tmp/cai_causal_graph-0.4.8.dev0.tar.gz` & `tmp/cai_causal_graph-0.4.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cai_causal_graph-0.4.8.dev0.tar", max compression
+gzip compressed data, was "cai_causal_graph-0.4.8.dev1.tar", max compression
```

## Comparing `cai_causal_graph-0.4.8.dev0.tar` & `cai_causal_graph-0.4.8.dev1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-04-10 12:53:29.339828 cai_causal_graph-0.4.8.dev0/LICENSE
--rw-r--r--   0        0        0     1686 2024-04-10 12:53:29.339828 cai_causal_graph-0.4.8.dev0/README.md
--rw-r--r--   0        0        0     1292 2024-04-10 12:53:44.079739 cai_causal_graph-0.4.8.dev0/cai_causal_graph/__init__.py
--rw-r--r--   0        0        0   101920 2024-04-10 12:53:29.339828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/causal_graph.py
--rw-r--r--   0        0        0     2599 2024-04-10 12:53:29.339828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/exceptions.py
--rw-r--r--   0        0        0    28767 2024-04-10 12:53:29.343828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/graph_components.py
--rw-r--r--   0        0        0    21769 2024-04-10 12:53:29.343828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/identify_utils.py
--rw-r--r--   0        0        0     1865 2024-04-10 12:53:29.343828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/interfaces.py
--rw-r--r--   0        0        0    63360 2024-04-10 12:53:29.343828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/time_series_causal_graph.py
--rw-r--r--   0        0        0     4427 2024-04-10 12:53:29.343828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/type_definitions.py
--rw-r--r--   0        0        0     4914 2024-04-10 12:53:29.343828 cai_causal_graph-0.4.8.dev0/cai_causal_graph/utils.py
--rw-r--r--   0        0        0     2575 2024-04-10 12:53:44.079739 cai_causal_graph-0.4.8.dev0/pyproject.toml
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 cai_causal_graph-0.4.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/LICENSE
+-rw-r--r--   0        0        0     1686 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/README.md
+-rw-r--r--   0        0        0     1292 2024-04-10 13:07:46.178974 cai_causal_graph-0.4.8.dev1/cai_causal_graph/__init__.py
+-rw-r--r--   0        0        0   101920 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/causal_graph.py
+-rw-r--r--   0        0        0     2599 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/exceptions.py
+-rw-r--r--   0        0        0    28767 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/graph_components.py
+-rw-r--r--   0        0        0    21769 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/identify_utils.py
+-rw-r--r--   0        0        0     1865 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/interfaces.py
+-rw-r--r--   0        0        0    63360 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/time_series_causal_graph.py
+-rw-r--r--   0        0        0     4427 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/type_definitions.py
+-rw-r--r--   0        0        0     4914 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/utils.py
+-rw-r--r--   0        0        0     2575 2024-04-10 13:07:46.178974 cai_causal_graph-0.4.8.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 cai_causal_graph-0.4.8.dev1/PKG-INFO
```

### Comparing `cai_causal_graph-0.4.8.dev0/LICENSE` & `cai_causal_graph-0.4.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/README.md` & `cai_causal_graph-0.4.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/__init__.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'EDGE_T',  # Keep for backwards compatibility.
     'NODE_T',  # Keep for backwards compatibility.
     # Time series specific tags
     'TIME_LAG',
     'VARIABLE_NAME',
 ]
 
-__version__ = '0.4.8.dev0'
+__version__ = '0.4.8.dev1'
 
 from cai_causal_graph.causal_graph import CausalGraph, Skeleton
 from cai_causal_graph.time_series_causal_graph import TimeSeriesCausalGraph
 from cai_causal_graph.type_definitions import (
     EDGE_T,
     NODE_T,
     TIME_LAG,
```

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/causal_graph.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/causal_graph.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/exceptions.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/graph_components.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/graph_components.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/identify_utils.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/identify_utils.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/interfaces.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/interfaces.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/time_series_causal_graph.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/time_series_causal_graph.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/type_definitions.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/type_definitions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/cai_causal_graph/utils.py` & `cai_causal_graph-0.4.8.dev1/cai_causal_graph/utils.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev0/pyproject.toml` & `cai_causal_graph-0.4.8.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 check_untyped_defs = true
 ignore_missing_imports = true
 pretty = true
 cache_dir = '/dev/null'
 
 [tool.poetry]
 name = "cai-causal-graph"
-version = "0.4.8.dev0"
+version = "0.4.8.dev1"
 description = "A Causal AI package for causal graphs."
 license = "Apache-2.0"
 authors = ["causaLens <opensource@causalens.com>"]
 readme = "README.md"
 homepage = "https://causalgraph.causalens.com/"
 repository = "https://github.com/causalens/cai-causal-graph"
 documentation = "https://causalgraph.causalens.com/"
```

### Comparing `cai_causal_graph-0.4.8.dev0/PKG-INFO` & `cai_causal_graph-0.4.8.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cai-causal-graph
-Version: 0.4.8.dev0
+Version: 0.4.8.dev1
 Summary: A Causal AI package for causal graphs.
 Home-page: https://causalgraph.causalens.com/
 License: Apache-2.0
 Author: causaLens
 Author-email: opensource@causalens.com
 Requires-Python: >=3.8.0,<3.13.0
 Classifier: License :: OSI Approved :: Apache Software License
```

