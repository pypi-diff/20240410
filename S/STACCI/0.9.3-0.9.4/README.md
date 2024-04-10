# Comparing `tmp/stacci-0.9.3.tar.gz` & `tmp/stacci-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stacci-0.9.3.tar", max compression
+gzip compressed data, was "stacci-0.9.4.tar", max compression
```

## Comparing `stacci-0.9.3.tar` & `stacci-0.9.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6004 2024-03-29 08:44:39.782535 stacci-0.9.3/README.md
--rw-r--r--   0        0        0      166 2024-03-15 15:29:04.555776 stacci-0.9.3/STACCI/__init__.py
--rw-r--r--   0        0        0    39940 2024-03-15 15:22:41.667792 stacci-0.9.3/STACCI/ccci.py
--rw-r--r--   0        0        0    10212 2024-03-15 16:51:31.767571 stacci-0.9.3/STACCI/data_handler.py
--rw-r--r--   0        0        0     6378 2024-03-15 16:45:15.675586 stacci-0.9.3/STACCI/model.py
--rw-r--r--   0        0        0     6734 2024-03-29 08:19:04.442599 stacci-0.9.3/STACCI/pipeline.py
--rw-r--r--   0        0        0    65268 2024-03-15 15:22:41.667792 stacci-0.9.3/STACCI/pl.py
--rw-r--r--   0        0        0     5219 2024-03-15 15:22:41.667792 stacci-0.9.3/STACCI/tl.py
--rw-r--r--   0        0        0     3765 2024-03-15 16:46:00.507584 stacci-0.9.3/STACCI/trainer.py
--rw-r--r--   0        0        0    32812 2024-03-29 08:35:18.818558 stacci-0.9.3/STACCI/utils.py
--rw-r--r--   0        0        0      796 2024-03-29 08:45:44.986532 stacci-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     7437 1970-01-01 00:00:00.000000 stacci-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     6004 2024-03-29 08:44:39.782535 stacci-0.9.4/README.md
+-rw-r--r--   0        0        0      166 2024-03-15 15:29:04.555776 stacci-0.9.4/STACCI/__init__.py
+-rw-r--r--   0        0        0    39940 2024-03-15 15:22:41.667792 stacci-0.9.4/STACCI/ccci.py
+-rw-r--r--   0        0        0    10212 2024-03-15 16:51:31.767571 stacci-0.9.4/STACCI/data_handler.py
+-rw-r--r--   0        0        0     6378 2024-03-15 16:45:15.675586 stacci-0.9.4/STACCI/model.py
+-rw-r--r--   0        0        0     6734 2024-03-29 08:19:04.442599 stacci-0.9.4/STACCI/pipeline.py
+-rw-r--r--   0        0        0    65268 2024-03-15 15:22:41.667792 stacci-0.9.4/STACCI/pl.py
+-rw-r--r--   0        0        0     5219 2024-03-15 15:22:41.667792 stacci-0.9.4/STACCI/tl.py
+-rw-r--r--   0        0        0     3765 2024-03-15 16:46:00.507584 stacci-0.9.4/STACCI/trainer.py
+-rw-r--r--   0        0        0    32812 2024-03-29 08:35:18.818558 stacci-0.9.4/STACCI/utils.py
+-rw-r--r--   0        0        0      773 2024-04-10 12:58:04.110833 stacci-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     7396 1970-01-01 00:00:00.000000 stacci-0.9.4/PKG-INFO
```

### Comparing `stacci-0.9.3/README.md` & `stacci-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/ccci.py` & `stacci-0.9.4/STACCI/ccci.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/data_handler.py` & `stacci-0.9.4/STACCI/data_handler.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/model.py` & `stacci-0.9.4/STACCI/model.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/pipeline.py` & `stacci-0.9.4/STACCI/pipeline.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/pl.py` & `stacci-0.9.4/STACCI/pl.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/tl.py` & `stacci-0.9.4/STACCI/tl.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/trainer.py` & `stacci-0.9.4/STACCI/trainer.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/STACCI/utils.py` & `stacci-0.9.4/STACCI/utils.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.3/pyproject.toml` & `stacci-0.9.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "STACCI"
-version = "0.9.3"
+version = "0.9.4"
 description = "STACCI for STCase"
 authors = ["Lzcstan <lzcstan@outlook.com>"]
 readme = "README.md"
 packages = [
   { include = "STACCI", from = "." },
 ]
 
 [tool.poetry.dependencies]
 scipy = "*"
-numpy = "*"
 scikit-learn = "*"
 scikit-misc = "*"
 anndata = "*"
 matplotlib = "*"
 pandas = "*"
 scanpy = "*"
 louvain = "*"
@@ -24,15 +23,14 @@
 pyscenic = "*"
 netgraph = "*"
 pycirclize = "*"
 plotnine = "*"
 kneed = "*"
 pot = "*"
 rich = "*"
-rpy2 = "*"
 torch-geometric = "*"
 torch = "*"
 torch-cluster = "*"
 torch-scatter = "*"
 torch-sparse = "*"
 torch-spline-conv = "*"
 pyg_lib = "*"
```

### Comparing `stacci-0.9.3/PKG-INFO` & `stacci-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STACCI
-Version: 0.9.3
+Version: 0.9.4
 Summary: STACCI for STCase
 Author: Lzcstan
 Author-email: lzcstan@outlook.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -19,23 +19,21 @@
 Requires-Dist: arboreto
 Requires-Dist: ctxcore
 Requires-Dist: kneed
 Requires-Dist: leidenalg
 Requires-Dist: louvain
 Requires-Dist: matplotlib
 Requires-Dist: netgraph
-Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotnine
 Requires-Dist: pot
 Requires-Dist: pycirclize
 Requires-Dist: pyg_lib
 Requires-Dist: pyscenic
 Requires-Dist: rich
-Requires-Dist: rpy2
 Requires-Dist: scanpy
 Requires-Dist: scikit-learn
 Requires-Dist: scikit-misc
 Requires-Dist: scipy
 Requires-Dist: torch
 Requires-Dist: torch-cluster
 Requires-Dist: torch-geometric
```

