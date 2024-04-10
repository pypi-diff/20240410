# Comparing `tmp/approx_umap-0.1.0.tar.gz` & `tmp/approx_umap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approx_umap-0.1.0.tar", max compression
+gzip compressed data, was "approx_umap-0.1.1.tar", max compression
```

## Comparing `approx_umap-0.1.0.tar` & `approx_umap-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1735 2024-04-03 16:55:42.482140 approx_umap-0.1.0/README.md
--rw-r--r--   0        0        0       46 2024-04-03 16:17:03.972887 approx_umap-0.1.0/approx_umap/__init__.py
--rw-r--r--   0        0        0     5399 2024-04-03 16:58:35.915758 approx_umap-0.1.0/approx_umap/approx_umap.py
--rw-r--r--   0        0        0      484 2024-04-03 16:57:37.414691 approx_umap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 approx_umap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-03 17:09:04.702968 approx_umap-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2116 2024-04-10 06:57:58.332889 approx_umap-0.1.1/README.md
+-rw-r--r--   0        0        0       46 2024-04-03 16:17:03.972887 approx_umap-0.1.1/approx_umap/__init__.py
+-rw-r--r--   0        0        0     5399 2024-04-03 16:58:35.915758 approx_umap-0.1.1/approx_umap/approx_umap.py
+-rw-r--r--   0        0        0      639 2024-04-10 07:21:45.707931 approx_umap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 approx_umap-0.1.1/PKG-INFO
```

### Comparing `approx_umap-0.1.0/README.md` & `approx_umap-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 # Approximate UMAP
 
 Modification of the UMAP algorithm to allow for fast approximate projections of
 new data points.
 
 ## Description
 
-This package provides a class `ApproxUMAP` that allows for fast approximate projections of new data points in the target space.
+This package provides a class `ApproxUMAP` that allows for fast approximate projections of new data points in the target
+space.
 
 The `fit` and `fit_transform` methods of `ApproxUMAP` are nearly identical to those of `umap.UMAP`;
 they simply fit an additional `sklearn.neighbors.NearestNeighbors` estimator.
 
-Only the `transform` method significantly differs; it approximates the projection of new data points 
+Only the `transform` method significantly differs; it approximates the projection of new data points
 in the embedding space to improve the projection speed.
 The projections are approximated by finding the nearest neighbors in the
 source space and computing their weighted average in the embedding space.
 The weights are the inverse of the distances in the source space.
 
 Formally, the projection of a new point $x$ is approximated as follows:
-$$
-u=\sum_i^n\frac{\frac{1}{d_i}}{\sum^n_j\frac{1}{d_j}}u_i
-$$
-with $x_1\dots x_k$ the $k$ nearest neighbours of x in the source space 
+$$u=\sum_i^k\frac{\frac{1}{d_i}}{\sum_j^k\frac{1}{d_j}}u_i$$
+with $x_1\dots x_k$ the $k$ nearest neighbours of $x$ in the source space
 among the points used for training (i.e., passed to `fit` or `fit_transform`),
-$d_i=distance(x, x_i)$, and $u_1\dots u_i$ the exact UMAP projections of $x_1\dots x_k$. 
+$d_i=distance(x, x_i)$, and $u_1\dots u_i$ the exact UMAP projections of $x_1\dots x_k$.
 
 ## Installation
 
 The package can be installed via pip:
+
 ```bash
 pip install approx-umap
 ```
 
 ## Usage
 
-The usage of `ApproxUMAP` is similar to that of any [scikit-learn](https://scikit-learn.org/stable/index.html) transformer:
+The usage of `ApproxUMAP` is similar to that of any [scikit-learn](https://scikit-learn.org/stable/index.html)
+transformer:
+
 ```python
 import numpy as np
 from approx_umap import ApproxUMAP
 
 X = np.random.rand(100, 10)
-emb_exact = ApproxUMAP().fit_transform(X) # exact UMAP projections
-emb_approx = ApproxUMAP().fit(X).transform(X) # approximate UMAP projection
+emb_exact = ApproxUMAP().fit_transform(X)  # exact UMAP projections
+emb_approx = ApproxUMAP().fit(X).transform(X)  # approximate UMAP projection
 ```
 
 ## Citation
 
 Please, cite this work as:
+
 ```bibtex
-@inproceedings{
-TODO
+@inproceedings{approx-umap2024,
+    title = {Approximate UMAP allows for high-rate online visualization of high-dimensional data streams},
+    author = {Peter Wassenaar and Pierre Guetschel and Michael Tangermann},
+    year = {2024},
+    month = {September},
+    booktitle = {8th Graz Brain-Computer Interface Conference},
+    address = {Graz, Austria},
+    url = {https://arxiv.org/abs/2404.04001},
 }
 ```
```

### Comparing `approx_umap-0.1.0/approx_umap/approx_umap.py` & `approx_umap-0.1.1/approx_umap/approx_umap.py`

 * *Files identical despite different names*

### Comparing `approx_umap-0.1.0/PKG-INFO` & `approx_umap-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 Metadata-Version: 2.1
 Name: approx-umap
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Modification of the UMAP algorithm to allow for fast approximate projections of new data points.
+Home-page: https://github.com/PierreGtch/approx-umap
 License: BSD-3-Clause
 Author: Pierre Guetschel
 Author-email: pierre.guetschel@donders.ru.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: umap-learn (>=0.5.5,<0.6.0)
+Project-URL: Repository, https://github.com/PierreGtch/approx-umap
 Description-Content-Type: text/markdown
 
 # Approximate UMAP
 
 Modification of the UMAP algorithm to allow for fast approximate projections of
 new data points.
 
 ## Description
 
-This package provides a class `ApproxUMAP` that allows for fast approximate projections of new data points in the target space.
+This package provides a class `ApproxUMAP` that allows for fast approximate projections of new data points in the target
+space.
 
 The `fit` and `fit_transform` methods of `ApproxUMAP` are nearly identical to those of `umap.UMAP`;
 they simply fit an additional `sklearn.neighbors.NearestNeighbors` estimator.
 
-Only the `transform` method significantly differs; it approximates the projection of new data points 
+Only the `transform` method significantly differs; it approximates the projection of new data points
 in the embedding space to improve the projection speed.
 The projections are approximated by finding the nearest neighbors in the
 source space and computing their weighted average in the embedding space.
 The weights are the inverse of the distances in the source space.
 
 Formally, the projection of a new point $x$ is approximated as follows:
-$$
-u=\sum_i^n\frac{\frac{1}{d_i}}{\sum^n_j\frac{1}{d_j}}u_i
-$$
-with $x_1\dots x_k$ the $k$ nearest neighbours of x in the source space 
+$$u=\sum_i^k\frac{\frac{1}{d_i}}{\sum_j^k\frac{1}{d_j}}u_i$$
+with $x_1\dots x_k$ the $k$ nearest neighbours of $x$ in the source space
 among the points used for training (i.e., passed to `fit` or `fit_transform`),
-$d_i=distance(x, x_i)$, and $u_1\dots u_i$ the exact UMAP projections of $x_1\dots x_k$. 
+$d_i=distance(x, x_i)$, and $u_1\dots u_i$ the exact UMAP projections of $x_1\dots x_k$.
 
 ## Installation
 
 The package can be installed via pip:
+
 ```bash
 pip install approx-umap
 ```
 
 ## Usage
 
-The usage of `ApproxUMAP` is similar to that of any [scikit-learn](https://scikit-learn.org/stable/index.html) transformer:
+The usage of `ApproxUMAP` is similar to that of any [scikit-learn](https://scikit-learn.org/stable/index.html)
+transformer:
+
 ```python
 import numpy as np
 from approx_umap import ApproxUMAP
 
 X = np.random.rand(100, 10)
-emb_exact = ApproxUMAP().fit_transform(X) # exact UMAP projections
-emb_approx = ApproxUMAP().fit(X).transform(X) # approximate UMAP projection
+emb_exact = ApproxUMAP().fit_transform(X)  # exact UMAP projections
+emb_approx = ApproxUMAP().fit(X).transform(X)  # approximate UMAP projection
 ```
 
 ## Citation
 
 Please, cite this work as:
+
 ```bibtex
-@inproceedings{
-TODO
+@inproceedings{approx-umap2024,
+    title = {Approximate UMAP allows for high-rate online visualization of high-dimensional data streams},
+    author = {Peter Wassenaar and Pierre Guetschel and Michael Tangermann},
+    year = {2024},
+    month = {September},
+    booktitle = {8th Graz Brain-Computer Interface Conference},
+    address = {Graz, Austria},
+    url = {https://arxiv.org/abs/2404.04001},
 }
 ```
```

