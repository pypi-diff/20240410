# Comparing `tmp/feature_clock-0.0.2.tar.gz` & `tmp/feature_clock-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/dist/.tmp-vubsnggq/feature_clock-0.0.2.ta", last modified: Fri Apr  5 16:02:01 2024, max compression
+gzip compressed data, was "feature_clock-0.0.3.tar", last modified: Wed Apr 10 00:57:57 2024, max compression
```

## Comparing `feature_clock-0.0.2.tar` & `feature_clock-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-05 16:02:01.505091 feature_clock-0.0.2/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    11356 2024-03-27 01:55:39.000000 feature_clock-0.0.2/LICENSE
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3205 2024-04-05 16:02:01.504865 feature_clock-0.0.2/PKG-INFO
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      897 2024-04-05 15:44:34.000000 feature_clock-0.0.2/README.md
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1924 2024-04-05 16:01:21.000000 feature_clock-0.0.2/pyproject.toml
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       38 2024-04-05 16:02:01.505143 feature_clock-0.0.2/setup.cfg
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-05 16:02:01.496780 feature_clock-0.0.2/src/
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-05 16:02:01.504462 feature_clock-0.0.2/src/feature_clock.egg-info/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3205 2024-04-05 16:02:01.000000 feature_clock-0.0.2/src/feature_clock.egg-info/PKG-INFO
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      635 2024-04-05 16:02:01.000000 feature_clock-0.0.2/src/feature_clock.egg-info/SOURCES.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        1 2024-04-05 16:02:01.000000 feature_clock-0.0.2/src/feature_clock.egg-info/dependency_links.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      799 2024-04-05 16:02:01.000000 feature_clock-0.0.2/src/feature_clock.egg-info/requires.txt
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       16 2024-04-05 16:02:01.000000 feature_clock-0.0.2/src/feature_clock.egg-info/top_level.txt
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-05 16:02:01.498781 feature_clock-0.0.2/src/nonlinear_clock/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        0 2024-02-16 15:04:27.000000 feature_clock-0.0.2/src/nonlinear_clock/__init__.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1265 2024-03-27 01:35:12.000000 feature_clock-0.0.2/src/nonlinear_clock/graph.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    42585 2024-04-05 15:43:14.000000 feature_clock-0.0.2/src/nonlinear_clock/plot.py
-drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-05 16:02:01.504304 feature_clock-0.0.2/test/
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     9870 2024-03-27 01:04:51.000000 feature_clock-0.0.2/test/test_bankrupcy.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12356 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_cancer.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5901 2024-03-27 01:03:18.000000 feature_clock-0.0.2/test/test_gaussians.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5570 2024-03-27 01:03:18.000000 feature_clock-0.0.2/test/test_gene_expr.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    22283 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_iris.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    10836 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_melody.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    19796 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_neftel.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    14491 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_pima.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12538 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_pima_autoencoder.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8075 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_pima_nn.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8198 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_pima_nn_2out.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5570 2024-03-27 01:03:18.000000 feature_clock-0.0.2/test/test_real_data.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12705 2024-04-05 15:43:14.000000 feature_clock-0.0.2/test/test_support.py
--rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        0 2024-03-18 00:23:21.000000 feature_clock-0.0.2/test/test_ventilator.py
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.822473 feature_clock-0.0.3/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    11356 2024-03-27 01:55:39.000000 feature_clock-0.0.3/LICENSE
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3205 2024-04-10 00:57:57.822250 feature_clock-0.0.3/PKG-INFO
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      897 2024-04-07 19:03:08.000000 feature_clock-0.0.3/README.md
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1924 2024-04-10 00:56:54.000000 feature_clock-0.0.3/pyproject.toml
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       38 2024-04-10 00:57:57.822519 feature_clock-0.0.3/setup.cfg
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.815426 feature_clock-0.0.3/src/
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.816784 feature_clock-0.0.3/src/feature_clock/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        0 2024-02-16 15:04:27.000000 feature_clock-0.0.3/src/feature_clock/__init__.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     1265 2024-03-27 01:35:12.000000 feature_clock-0.0.3/src/feature_clock/graph.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    47421 2024-04-10 00:41:31.000000 feature_clock-0.0.3/src/feature_clock/plot.py
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.821914 feature_clock-0.0.3/src/feature_clock.egg-info/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     3205 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/PKG-INFO
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      605 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)        1 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)      799 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/requires.txt
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)       14 2024-04-10 00:57:57.000000 feature_clock-0.0.3/src/feature_clock.egg-info/top_level.txt
+drwxr-xr-x   0 olga_ovcharenko   (501) staff       (20)        0 2024-04-10 00:57:57.821173 feature_clock-0.0.3/test/
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     9874 2024-04-07 23:09:41.000000 feature_clock-0.0.3/test/test_bankrupcy.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12360 2024-04-07 23:09:42.000000 feature_clock-0.0.3/test/test_cancer.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5899 2024-04-07 23:09:45.000000 feature_clock-0.0.3/test/test_gaussians.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5574 2024-04-07 23:10:02.000000 feature_clock-0.0.3/test/test_gene_expr.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    22299 2024-04-07 23:10:04.000000 feature_clock-0.0.3/test/test_iris.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12881 2024-04-10 00:52:12.000000 feature_clock-0.0.3/test/test_melody.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    27733 2024-04-09 23:58:30.000000 feature_clock-0.0.3/test/test_neftel.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    13901 2024-04-10 00:10:01.000000 feature_clock-0.0.3/test/test_pima.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    12620 2024-04-07 23:10:00.000000 feature_clock-0.0.3/test/test_pima_autoencoder.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8103 2024-04-10 00:02:31.000000 feature_clock-0.0.3/test/test_pima_nn.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     8329 2024-04-10 00:05:40.000000 feature_clock-0.0.3/test/test_pima_nn_2out.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)     5574 2024-04-07 23:09:49.000000 feature_clock-0.0.3/test/test_real_data.py
+-rw-r--r--   0 olga_ovcharenko   (501) staff       (20)    41830 2024-04-09 20:49:21.000000 feature_clock-0.0.3/test/test_support.py
```

### Comparing `feature_clock-0.0.2/LICENSE` & `feature_clock-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_clock-0.0.2/PKG-INFO` & `feature_clock-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_clock
-Version: 0.0.2
+Version: 0.0.3
 Summary: Feature Clock, provides visualizations that eliminate the need for multiple plots to inspect the influence of original variables in the latent space. Feature Clock enhances the explainability and compactness of visualizations of embedded data.
 Author-email: Olga Ovcharenko <ovcharenko.folga@gmail.com>
 Project-URL: Homepage, https://github.com/OlgaOvcharenko/feature_clock_visualization
 Project-URL: Issues, https://github.com/OlgaOvcharenko/feature_clock_visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `feature_clock-0.0.2/README.md` & `feature_clock-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `feature_clock-0.0.2/pyproject.toml` & `feature_clock-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "feature_clock"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Olga Ovcharenko", email="ovcharenko.folga@gmail.com" },
 ]
 description = "Feature Clock, provides visualizations that eliminate the need for multiple plots to inspect the influence of original variables in the latent space. Feature Clock enhances the explainability and compactness of visualizations of embedded data."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `feature_clock-0.0.2/src/feature_clock.egg-info/PKG-INFO` & `feature_clock-0.0.3/src/feature_clock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_clock
-Version: 0.0.2
+Version: 0.0.3
 Summary: Feature Clock, provides visualizations that eliminate the need for multiple plots to inspect the influence of original variables in the latent space. Feature Clock enhances the explainability and compactness of visualizations of embedded data.
 Author-email: Olga Ovcharenko <ovcharenko.folga@gmail.com>
 Project-URL: Homepage, https://github.com/OlgaOvcharenko/feature_clock_visualization
 Project-URL: Issues, https://github.com/OlgaOvcharenko/feature_clock_visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `feature_clock-0.0.2/src/feature_clock.egg-info/SOURCES.txt` & `feature_clock-0.0.3/src/feature_clock.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
+src/feature_clock/__init__.py
+src/feature_clock/graph.py
+src/feature_clock/plot.py
 src/feature_clock.egg-info/PKG-INFO
 src/feature_clock.egg-info/SOURCES.txt
 src/feature_clock.egg-info/dependency_links.txt
 src/feature_clock.egg-info/requires.txt
 src/feature_clock.egg-info/top_level.txt
-src/nonlinear_clock/__init__.py
-src/nonlinear_clock/graph.py
-src/nonlinear_clock/plot.py
 test/test_bankrupcy.py
 test/test_cancer.py
 test/test_gaussians.py
 test/test_gene_expr.py
 test/test_iris.py
 test/test_melody.py
 test/test_neftel.py
 test/test_pima.py
 test/test_pima_autoencoder.py
 test/test_pima_nn.py
 test/test_pima_nn_2out.py
 test/test_real_data.py
-test/test_support.py
-test/test_ventilator.py
+test/test_support.py
```

### Comparing `feature_clock-0.0.2/src/feature_clock.egg-info/requires.txt` & `feature_clock-0.0.3/src/feature_clock.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `feature_clock-0.0.2/src/nonlinear_clock/graph.py` & `feature_clock-0.0.3/src/feature_clock/graph.py`

 * *Files identical despite different names*

### Comparing `feature_clock-0.0.2/src/nonlinear_clock/plot.py` & `feature_clock-0.0.3/src/feature_clock/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 import numpy as np
 import pandas as pd
 import matplotlib.colors as mcolors
 from skspatial.objects import Line
 import math
 import matplotlib.patheffects as pe
 from sklearn.manifold import TSNE
-from src.nonlinear_clock.graph import Graph
+from src.feature_clock.graph import Graph
 import warnings
 from sklearn.preprocessing import StandardScaler
+from scipy.stats import norm
+from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
 
 
 class NonLinearClock:
     def __init__(
         self,
         high_dim_data: np.array,
         observations: list,
@@ -92,15 +94,15 @@
         self.method = "tSNE"
         tsne = TSNE(args)
         self.low_dim_data = tsne.fit_transform(self.high_dim_data)
         return self.low_dim_data
 
     def _compute_HDBSCAN_hulls(self):
         hdb = HDBSCAN(min_samples=10, min_cluster_size=30)
-        labels = hdb.fit_predict(self.low_dim_data)
+        labels = hdb.fit_predict(self.high_dim_data)
         return labels
 
     def _standartize_data(self):
         for col in self.low_dim_data.columns:
             self.low_dim_data[col] = (
                 self.low_dim_data[col] - self.low_dim_data[col].mean()
             ) / self.low_dim_data[col].std()
@@ -180,14 +182,26 @@
             )
             for angle in self.angles
         ]
         self.projections = np.array(projections).T
 
     def _get_importance(self, X, y, significance: float = 0.05, univar: bool = False):
         coefs, pvals, is_significant, std_x, std_y = [], [], [], [], []
+        
+        remove_cols = []
+        for j in range(X.shape[1]):
+            val1 = X[0, j] 
+            for i in range(X.shape[0]):
+                if X[i, j] != val1:
+                    break
+                if i == X.shape[0]-1 and X[i, j] == val1:
+                    remove_cols.append(j)
+        for k in remove_cols:
+            X = np.delete(X, k, 1)
+
         for i in range(y.shape[1]):
             if univar:
                 coefs_a, pvals_a, is_significant_a = [], [], []
                 for j in range(X.shape[1]):
                     lm = sm.OLS(y[:, i], X[:, j]).fit()
                     coefs_a.append(lm.params[0])
                     pvals_a.append(lm.pvalues[0])
@@ -195,25 +209,89 @@
 
                 coefs.append(np.array(coefs_a))
                 std_x.append(np.ones((len(coefs_a),)))
                 std_y.append(np.ones((len(coefs_a),)))
                 pvals.append(pvals_a)
                 is_significant.append(is_significant_a)
 
-                # FIXME add std X, y
-
             else:
-                lm = sm.OLS(y[:, i], X).fit()
-                pval = np.array(lm.pvalues)
-                coefs.append(np.array(lm.params))
+                # lm = sm.OLS(y[:, i], X).fit()
+                lm = sm.OLS(y[:, i], np.c_[np.ones(X.shape[0]), X]).fit()
+                
+                coefs_tmp = lm.params[1:]
+                pvals_tmp = lm.pvalues[1:]
+                x_std_tmp = X.std(axis=0)
+                
+                for k in remove_cols:
+                    coefs_tmp = np.insert(coefs_tmp, k, 0)
+                    pvals_tmp = np.insert(pvals_tmp, k, 0)
+                    x_std_tmp = np.insert(x_std_tmp, k, 1)
+                    
+                coefs.append(np.array(coefs_tmp))
+
+                pval = np.array(pvals_tmp)
                 pvals.append(pval)
                 is_significant.append(pval <= significance)
 
-                std_x.append(X.std(axis=0))
+                std_x.append(np.array(x_std_tmp))
                 std_y.append(y[:, i].std())
+
+        return (
+            np.array(coefs),
+            np.array(pvals),
+            np.array(is_significant),
+            np.array(std_x),
+            np.array(std_y),
+        )
+    
+    def _logit_pvalue(self, model, x):
+        """ Calculate z-scores for scikit-learn LogisticRegression.
+        parameters:
+            model: fitted sklearn.linear_model.LogisticRegression with intercept and large C
+            x:     matrix on which the model was fit
+        This function uses asymtptics for maximum likelihood estimates.
+        """
+        p = model.predict_proba(x)
+        n = len(p)
+        m = len(model.coef_[0]) + 1
+        coefs = np.concatenate([model.intercept_, model.coef_[0]])
+        x_full = np.matrix(np.insert(np.array(x), 0, 1, axis = 1))
+        ans = np.zeros((m, m))
+        for i in range(n):
+            ans = ans + np.dot(np.transpose(x_full[i, :]), x_full[i, :]) * p[i,1] * p[i, 0]
+        vcov = np.linalg.inv(np.matrix(ans))
+        se = np.sqrt(np.diag(vcov))
+        t =  coefs/se  
+        p = (1 - norm.cdf(abs(t))) * 2
+        return p
+
+
+    def _get_importance_between(self, X, mst, significance: float = 0.05, univar: bool = False):
+        coefs, pvals, is_significant, std_x, std_y = [], [], [], [], []
+
+        for val in mst:
+            ix = np.logical_or((self.cluster_labels == val[0]), (self.cluster_labels == val[1]))
+            X_i = X[ix]
+            y = self.cluster_labels[np.logical_or((self.cluster_labels == val[0]), (self.cluster_labels == val[1]))]
+            lm = LogisticRegressionCV(cv=5, fit_intercept=True, penalty="l2").fit(X_i, y)
+
+            pval = np.array(self._logit_pvalue(lm, X_i)[1:])
+            coefs.append(np.array(lm.coef_[0]))
+            pvals.append(pval)
+            is_significant.append(pval <= significance)
+
+            std_x.append(X_i.std(axis=0))
+            std_y.append(y.std())
+
+            # for i, val in enumerate(self.observations):
+            #     print(val)
+            #     print(lm.coef_[0][i])
+            #     print(pval[i])
+            #     print(pval[i] <= significance)
+
         return (
             np.array(coefs),
             np.array(pvals),
             np.array(is_significant),
             np.array(std_x),
             np.array(std_y),
         )
@@ -252,16 +330,17 @@
             coefs_points = [[x, y] for x, y in zip(coefs[0], coefs[1])]
             coefs_new = np.array(
                 [math.sqrt((x * x) + (y * y)) for x, y in zip(coefs[0], coefs[1])]
             )
 
             if plot_top_k != 0:
                 min_ix = list(
-                    np.argsort(coefs_new)[0 : len(coefs_new) - plot_top_k]
+                    np.argsort(np.abs(coefs_new) * is_significant)[0 : len(coefs_new) - plot_top_k]
                 )  # FISME * is_significant
+
                 is_significant[min_ix] = False
 
             coefs = coefs_new
 
             arrows, arrow_labels = self._plot_central(
                 ax,
                 self.low_dim_data,
@@ -454,28 +533,46 @@
         annotate,
         x_center,
         y_center,
         radius,
         c_min,
         c_max,
         ann_sign=[1, 1],
+        clock_label="",
+        clock_label_angle=270
     ):
         for i in list(range(1, num_circles))[::-1]:
             radius_circle = round(i * annotate, 1)
             if i == num_circles - 1:
                 circle = patches.Circle(
                     (x_center, y_center),
                     radius=radius_circle,
                     edgecolor="gray",
                     linewidth=1,
                     linestyle="--",
                     facecolor=(0.941, 0.973, 1.0, 0.5),
                     fill=True,
                     zorder=10,
                 )
+
+                circle_an = math.radians(clock_label_angle)
+                x_ann, y_ann = (
+                    x_center + math.cos(circle_an) * radius_circle * 1.2,
+                    y_center + math.sin(circle_an) * radius_circle * 1.2,
+                )
+
+                ax.annotate(
+                    clock_label,
+                    xy=(x_ann, y_ann),
+                    ha="center",
+                    color="gray",
+                    path_effects=[pe.withStroke(linewidth=2, foreground="white")],
+                    fontsize=7,
+                    zorder=20
+                )
             else:
                 circle = patches.Circle(
                     (x_center, y_center),
                     radius=radius_circle,
                     edgecolor="gray",
                     linewidth=1,
                     linestyle="--",
@@ -600,28 +697,29 @@
             c_min,
             c_max,
             ann_sign=ann_sign,
         )
         return arrows, arrow_labels
 
     def _draw_clusters(self, ax, data, alpha):
+        print(data["cluster"].unique())
         for i in data["cluster"].unique():
             if i >= 0:
                 points = data[data["cluster"] == i]
                 if points.shape[0] > 2:
                     hull = ConvexHull(points[["emb1", "emb2"]].to_numpy())
                     vert = np.append(hull.vertices, hull.vertices[0])
 
                     a, b = points["emb1"].iloc[vert], points["emb2"].iloc[vert]
                     ax.plot(a, b, "--", c="gray", alpha=alpha)
                     ax.fill(a, b, alpha=alpha, c="gray")
 
     def _get_plot(self, ax, data, draw_hulls: bool = True, plot_scatter: bool = True):
         alpha = 0.1
-
+        print(draw_hulls)
         if draw_hulls:
             self._draw_clusters(ax, data, alpha)
         if plot_scatter:
             ax.scatter(data["emb1"], data["emb2"], color="gray", s=2, alpha=alpha)
 
     def _plot_small(
         self,
@@ -634,14 +732,16 @@
         labels,
         biggest_arrow: bool = True,
         scale_circle: float = 1.0,
         annotate: float = 0.2,
         move_circle: list = [0, 0],
         arrow_width: float = 0.01,
         points: list = [],
+        clock_label: str = "",
+        clocks_label_angle: float = 270
     ):
         x_center, y_center = self._get_center(data)
 
         x_center += move_circle[0]
         y_center += move_circle[1]
 
         radius = np.abs(coefs).max() * scale_circle
@@ -739,14 +839,16 @@
             annotate,
             x_center,
             y_center,
             radius,
             c_min,
             c_max,
             ann_sign=ann_sign,
+            clock_label=clock_label,
+            clock_label_angle=clocks_label_angle
         )
 
         return arrows, labels_all
 
     def _plot_small_clock(
         self,
         ax,
@@ -757,14 +859,16 @@
         scale_circle,
         move_circle,
         annotate,
         arrow_width,
         plot_scatter,
         plot_hulls,
         plot_top_k,
+        clocks_labels,
+        clocks_labels_angles
     ):
         dist_clusters = self.low_dim_data["cluster"].unique()
         dist_clusters.sort()
         dist_clusters = dist_clusters[1:] if dist_clusters[0] == -1 else dist_clusters
 
         self._get_plot(ax, self.low_dim_data, plot_hulls, plot_scatter)
 
@@ -777,14 +881,15 @@
         )
         arrows_dict = {}
         for cl in dist_clusters:
             ind = (self.low_dim_data["cluster"] == cl).values.reshape(
                 (self.low_dim_data.shape[0], 1)
             )
 
+
             data_cl = self.low_dim_data[ind]
             new_data_cl = self.high_dim_data[ind]
             projections_cl = self.projections[ind[:, 0], :]
 
             coefs, _, is_significant, std_x, std_y = self._get_importance(
                 new_data_cl.to_numpy(),
                 projections_cl,
@@ -797,15 +902,15 @@
                 coefs_points = [[x, y] for x, y in zip(coefs[0], coefs[1])]
                 coefs_new = np.array(
                     [math.sqrt((x * x) + (y * y)) for x, y in zip(coefs[0], coefs[1])]
                 )
 
                 if plot_top_k != 0:
                     min_ix = list(
-                        np.argsort(coefs_new)[0 : len(coefs_new) - plot_top_k]
+                        np.argsort(np.abs(coefs_new))[0 : len(coefs_new) - plot_top_k]
                     )
                     is_significant[min_ix] = False
 
                 coefs = coefs_new * is_significant
                 all_points.append(coefs_points)
 
             else:
@@ -857,14 +962,16 @@
                     self.observations,
                     scale_circle=scale,
                     annotate=a,
                     biggest_arrow=biggest_arrow,
                     move_circle=move_circle[i],
                     arrow_width=arrow_width,
                     points=all_points[i] if len(all_points) > 0 else [],
+                    clock_label=clocks_labels[i] if len(clocks_labels) == len(dist_clusters) else "",
+                    clocks_label_angle=clocks_labels_angles[i] if len(clocks_labels_angles) == len(dist_clusters) else 270
                 )
 
                 for arrow, lbl in zip(arrows, arrow_labels):
                     if arrows_dict.get(lbl) is None:
                         arrows_dict[lbl] = arrow
 
             else:
@@ -915,14 +1022,16 @@
         angles,
         scale_circle,
         move_circle,
         annotate,
         arrow_width,
         plot_scatter,
         plot_hulls,
+        clocks_labels,
+        clocks_labels_angles
     ):
         alpha = 0.1
 
         # Scatter plot
         if plot_scatter:
             ax.scatter(
                 data["emb1"], data["emb2"], color="gray", s=2, alpha=alpha, zorder=0
@@ -933,46 +1042,43 @@
 
         # Add lines and clock
         clock_centers = []
         coefs_scaled = copy.deepcopy(coefs)
         for i, val in enumerate(mst):
             p_a, p_b = cl_means[val[0]], cl_means[val[1]]
 
-            # FIXME
-            # ax.plot(
-            #     (p_a[0], p_b[0]),
-            #     (p_a[1], p_b[1]),
-            #     c="gray",
-            #     linestyle="--",
-            #     alpha=0.7,
-            #     linewidth=1,
-            #     zorder=10,
-            # )
-
             # Add clock
             x_center, y_center = (
                 np.mean((p_a[0], p_b[0])) + move_circle[i][0],
                 np.mean((p_a[1], p_b[1])) + move_circle[i][1],
             )
+            
             clock_centers.append([x_center, y_center])
 
             radius = (math.dist(p_a, p_b) / 2) * scale_circle[i]
             c_min, c_max = self._get_cmin_cmax(coefs=coefs[i])
             num_circles = math.floor(radius / annotate[i]) + 1
             self._add_circles_lines(
                 ax, num_circles, annotate[i], 90, x_center, y_center
             )
 
             # num_circles - one circle per annotation
             self._add_circles(
-                ax, num_circles, annotate[i], x_center, y_center, radius, c_min, c_max
+                ax, num_circles, annotate[i], x_center, y_center, radius, c_min, c_max, 
+                clock_label=f"{clocks_labels[val[0]]} "+ u"\u21FE" f" {clocks_labels[val[1]]}" if len(clocks_labels) > 1 else f"{val[0]}"+ u"\u21FE" f"{val[1]}",
+                clock_label_angle=clocks_labels_angles[i] if len(clocks_labels_angles) == len(mst) else 270
             )
 
             coefs_scaled[i] = coefs_scaled[i] * (radius / max(abs(c_max), abs(c_min)))
 
+            if val[0] > val[1] and p_a[0] < p_b[0]:
+                coefs_scaled[i] = coefs_scaled[i] * (-1)
+            elif val[0] < val[1] and p_a[0] > p_b[0]:
+                coefs_scaled[i] = coefs_scaled[i] * (-1)
+
         # Add arrows
         arrows = {}
         for j in range(len(mst)):
             for i in abs(coefs_scaled[j]).argsort(axis=None)[::-1]:
                 # Add actual arrow
                 a = math.radians(angles[j])
                 x_center, y_center = clock_centers[min(mst[j][0], mst[j][1])]
@@ -1010,52 +1116,52 @@
         scale_circle,
         move_circle,
         annotate,
         arrow_width,
         plot_scatter,
         plot_hulls,
         plot_top_k,
+        clocks_labels,
+        clocks_labels_angles
     ):
         dist_clusters = self.low_dim_data["cluster"].unique()
         dist_clusters.sort()
         dist_clusters = dist_clusters[1:] if dist_clusters[0] == -1 else dist_clusters
 
         cl_means = self._get_cluster_centers(dist_clusters)
         adj_matrix = self._build_adj_matrix(cl_means)
         mst = self._build_MST(len(dist_clusters), adj_matrix)
 
         mst_proj, angles = [], []
         for val in mst:
             angle = math.degrees(
                 self._get_angle_to_x(cl_means[val[0]], cl_means[val[1]])
             )
-            proj = self._project_line(
-                self.low_dim_data,
-                angle,
-                point_a=cl_means[val[0]],
-                point_b=cl_means[val[1]],
-            )
-            mst_proj.append(proj)
             angles.append(angle)
 
         self.mst_proj = np.array(mst_proj).T
-        coefs, _, is_significant, std_x, std_y = self._get_importance(
+        coefs, _, is_significant, std_x, std_y = self._get_importance_between(
             self.high_dim_data.to_numpy(),
-            self.mst_proj,
+            mst,
             univar=univar_importance,
             significance=feature_significance,
         )
 
         if plot_top_k != 0:
-            min_ix = np.argsort(coefs * is_significant, axis=1)[::-1][:, 0:plot_top_k]
+            # print(coefs)
+            min_ix = np.argsort(np.abs(coefs) * is_significant, axis=1)[:, 0 : len(coefs) - plot_top_k-1]
+            # print(min_ix)
             for i in range(is_significant.shape[0]):
                 for j in range(is_significant.shape[1]):
-                    if j not in min_ix[i]:
+                    if j in min_ix[i]:
                         is_significant[i, j] = False
         if is_significant.sum() == 0:
+            warnings.warn(
+                    "no significant features."
+                )
             return [], []
 
         if standartize_coef:
             coefs = coefs / std_x
             if np.isnan(coefs).any():
                 coefs = np.nan_to_num(coefs)
                 warnings.warn(
@@ -1075,14 +1181,16 @@
             angles,
             scale_circle,
             move_circle,
             annotate,
             arrow_width,
             plot_scatter,
             plot_hulls,
+            clocks_labels,
+            clocks_labels_angles
         )
 
         return arrows, labels
 
     def get_num_clusters(self):
         return self.low_dim_data["cluster"].nunique()
 
@@ -1148,14 +1256,16 @@
         scale_circles: list = [],
         move_circles: list = [],
         annotates: list = [],
         arrow_width: float = 0.1,
         plot_scatter: bool = True,
         plot_hulls: bool = True,
         plot_top_k: int = 0,
+        clocks_labels: list = [],
+        clocks_labels_angles: list = [],
     ):
         if not self.is_projected or self.shift != angle_shift:
             self.is_projected = True
             self.shift = angle_shift
             self._prepare_data(standartize_data=standartize_data)
 
             if biggest_arrow_method:
@@ -1194,14 +1304,16 @@
             scale_circle=scale_circles,
             move_circle=move_circles,
             annotate=annotates,
             arrow_width=arrow_width,
             plot_scatter=plot_scatter,
             plot_hulls=plot_hulls,
             plot_top_k=plot_top_k,
+            clocks_labels=clocks_labels,
+            clocks_labels_angles=clocks_labels_angles
         )
         return arrows_all, arrow_labels_all
 
     def plot_between_clock(
         self,
         ax: matplotlib.axis.Axis,
         standartize_data: bool = True,
@@ -1212,36 +1324,38 @@
         scale_circles: list = [],
         move_circles: list = [],
         annotates: list = [],
         arrow_width: float = 0.03,
         plot_scatter: bool = True,
         plot_hulls: bool = True,
         plot_top_k: int = 0,
+        clocks_labels: list = [],
+        clocks_labels_angles: list = [],
     ):
 
         if not self.is_projected or self.shift != angle_shift:
             self.is_projected = True
             self.shift = angle_shift
             self._prepare_data(standartize_data=standartize_data)
-            self._create_angles_projections(angle_shift=angle_shift)
+            # self._create_angles_projections(angle_shift=angle_shift)
 
         if plot_top_k < 0:
             raise Exception(
                 f"Invalid value for plot_top_k: {plot_top_k} (0 - plot all, ncol > k > 0)."
             )
 
         if plot_top_k > self.high_dim_data.shape[1]:
             raise Exception(
                 f"Invalid value for plot_top_k: {plot_top_k} (0 - plot all, ncol > k > 0). plot_top_k greater than umber of columns."
             )
 
         n_clusters = self.low_dim_data["cluster"].nunique() - 1
         if n_clusters != len(scale_circles) != len(move_circles) != len(annotates):
             raise Exception(
-                f"Length of annotates, move_circles, scale_circles should be equal number of clusters {n_clusters}."
+                f"Length of annotates, move_circles, scale_circles should be equal number of edges {n_clusters}."
             )
 
         if len(scale_circles) == len(move_circles) == len(annotates) == 0:
             for _ in range(n_clusters):
                 scale_circles.append(1)
                 move_circles.append([0, 0])
                 annotates.append(0.3)
@@ -1254,10 +1368,12 @@
             scale_circle=scale_circles,
             move_circle=move_circles,
             annotate=annotates,
             arrow_width=arrow_width,
             plot_scatter=plot_scatter,
             plot_hulls=plot_hulls,
             plot_top_k=plot_top_k,
+            clocks_labels=clocks_labels,
+            clocks_labels_angles = clocks_labels_angles
         )
 
         return arrows, labels
```

### Comparing `feature_clock-0.0.2/test/test_bankrupcy.py` & `feature_clock-0.0.3/test/test_bankrupcy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from matplotlib import pyplot as plt
 import numpy as np
 import pandas as pd
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_bankrupcy_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/bankrupcy.csv"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/bankrupcy.csv"
     X = read_data(file_name)
 
     names = dict()
     for name in list(X.columns):
         names[name] = str.strip(name)
     X.rename(columns=names, inplace=True)
     X = X.dropna()
```

### Comparing `feature_clock-0.0.2/test/test_cancer.py` & `feature_clock-0.0.3/test/test_cancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from matplotlib import pyplot as plt
 import numpy as np
 import pandas as pd
 from sklearn.discriminant_analysis import StandardScaler
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 from sklearn import preprocessing
 
@@ -19,15 +19,15 @@
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_cancer_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/Cancer_Data.csv"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/Cancer_Data.csv"
     X = read_data(file_name)
 
     X.drop(columns=["id"], inplace=True)
     X = X.dropna()
     X.diagnosis = X.diagnosis.map({'M': 0, 'B': 1})
     
     labels = X["diagnosis"]
```

### Comparing `feature_clock-0.0.2/test/test_gaussians.py` & `feature_clock-0.0.3/test/test_gaussians.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import matplotlib
 sys.path.append('src/')
 
 import numpy as np
 import scanpy as sp
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import scanpy.external as sce
 import phate
 import pandas as pd
 import scipy.stats as ss
 import matplotlib.pyplot as plt 
 
 np.random.seed(42)
```

### Comparing `feature_clock-0.0.2/test/test_gene_expr.py` & `feature_clock-0.0.3/test/test_gene_expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import scanpy as sp
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import scanpy.external as sce
 import phate
 import pandas as pd
 
 def read_data(path):
     return pd.read_csv(path, sep=";", header=0)
 
 def setup_data(method = "umap"):
-    file_name = '/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/E-GEOD-46817-query-results.csv'
+    file_name = '/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/E-GEOD-46817-query-results.csv'
     X = read_data(file_name)
 
     obs = [ 
            "A2058",   "A375",   "C32",  "Malme3M",  "SKMEL28",  "SKMEL5",  "WM2664"
            ]
     
     new_data = X[obs].dropna()
```

### Comparing `feature_clock-0.0.2/test/test_iris.py` & `feature_clock-0.0.3/test/test_iris.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from matplotlib import gridspec, pyplot as plt
 import matplotlib
 import numpy as np
 import pandas as pd
 from sklearn.discriminant_analysis import StandardScaler
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from sklearn import decomposition  # decomposition.PCA
 from sklearn import manifold 
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
@@ -21,15 +21,15 @@
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_iris_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/Iris.csv"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/Iris.csv"
     X = read_data(file_name)
     X.rename(columns={"SepalLengthCm": "SepalLength", 
                       "SepalWidthCm": "SepalWidth", 
                       "PetalLengthCm": "PetalLength", 
                       "PetalWidthCm": "PetalWidth"}, inplace=True)
     
     X.drop(columns={"Id"}, inplace=True)
@@ -132,15 +132,15 @@
         num=None,
         figsize=fig_size,
         dpi=dpi,
         facecolor="w",
         edgecolor="k",
     )
 
-    df = pd.read_csv("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/Iris.csv")
+    df = pd.read_csv("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/Iris.csv")
     labels = df.Species.map({"Iris-setosa":0, "Iris-versicolor":1, "Iris-virginica":2}).to_numpy()
     
     df.rename(columns={"SepalLengthCm": "SepalLength", 
                       "SepalWidthCm": "SepalWidth", 
                       "PetalLengthCm": "PetalLength", 
                       "PetalWidthCm": "PetalWidth"}, inplace=True)
     
@@ -547,15 +547,15 @@
 
     spec23 = gridspec.GridSpecFromSubplotSpec(2, 2, subplot_spec=spec2[1], wspace=0.05)
     ax21 = fig.add_subplot(spec23[0, 0])
     ax22 = fig.add_subplot(spec23[0, 1])
     ax23 = fig.add_subplot(spec23[1, 0])
     ax24 = fig.add_subplot(spec23[1, 1])
 
-    df = pd.read_csv("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/Iris.csv")
+    df = pd.read_csv("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/Iris.csv")
     labels = df.Species.map({"Iris-setosa":0, "Iris-versicolor":1, "Iris-virginica":2}).to_numpy()
     
     df.rename(columns={"SepalLengthCm": "SepalLength", 
                       "SepalWidthCm": "SepalWidth", 
                       "PetalLengthCm": "PetalLength", 
                       "PetalWidthCm": "PetalWidth"}, inplace=True)
```

### Comparing `feature_clock-0.0.2/test/test_neftel.py` & `feature_clock-0.0.3/test/test_neftel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from matplotlib import gridspec, pyplot as plt
+from matplotlib import cm, gridspec, pyplot as plt
+import matplotlib
 import numpy as np
 import scanpy as sp
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import scanpy.external as sce
 import phate
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
+from hdbscan import HDBSCAN
 
 def make_legend_arrow(legend, orig_handle,
                       xdescent, ydescent,
                       width, height, fontsize):
     p = mpatches.FancyArrow(0, 0.5*height, width, 0, length_includes_head=True, head_width=0.75*height )
     return p
 
 
 def read_data(path):
     return sp.read_h5ad(path)
 
 
 def setup_neftel_data(method="tsne"):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/neftel_malignant.h5ad"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/neftel_malignant.h5ad"
     X = read_data(file_name)
 
     obs = [
         "MESlike2",
         "MESlike1",
         "AClike",
         "OPClike",
@@ -65,15 +67,18 @@
     npc = np.stack((X_new.X[:, 4], X_new.X[:, 5]))
     ac, opc = X_new.X[:, 2], X_new.X[:, 3]
     mes_max = np.max(mes, axis=0)
     npc_max = np.max(npc, axis=0)
     res_vect = np.stack((ac, opc, mes_max, npc_max))
     res_labels = np.max(res_vect, axis=0)
 
-    return new_data, obs, standard_embedding, res_labels
+    clusters = HDBSCAN(min_samples=10, min_cluster_size=30).fit_predict(new_data)
+
+
+    return new_data, obs, standard_embedding, res_labels, clusters
 
 
 def test_umap():
     X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
 
     plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, "UMAP")
 
@@ -413,15 +418,15 @@
         top=0.95,
         bottom=0.08,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_biggest_only_clock.pdf")
 
 
 def test_experiment2():
-    X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
+    X_new, obs, standard_embedding, labels, _ = setup_neftel_data(method="umap")
 
     fig, ax = plt.subplots(1, figsize=(3.4775/2, 3.4775/2))
     plt.tight_layout()
     plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, "UMAP")
     arrows, arrow_labels = plot_inst.plot_global_clock(
         standartize_data=True,
         standartize_coef=True,
@@ -507,15 +512,15 @@
         top=0.95,
         bottom=0.08,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/neftel/neftel_all_15_degree.pdf")
 
 
 def test_all_4_in_row():
-    X_new, obs, standard_embedding, labels = setup_neftel_data(method="umap")
+    X_new, obs, standard_embedding, labels, _ = setup_neftel_data(method="umap")
 
     # fig, axi = plt.subplots(1, 3, figsize=(7.125-0.66, 2.375))
     # plt.tight_layout()
 
     dpi = 1000
     fig_size = ((7.125-0.17), ((7.125-0.17)/1.8)/1.618)
 
@@ -659,11 +664,214 @@
                         pad=0.02, aspect=40)
     cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/neftel/neftel_3.pdf")
 
 
+def test_all_4_in_row_hdbscan():
+    X_new, obs, standard_embedding, labels, clusters = setup_neftel_data(method="umap")
+
+    # fig, axi = plt.subplots(1, 3, figsize=(7.125-0.66, 2.375))
+    # plt.tight_layout()
+
+    dpi = 1000
+    fig_size = ((7.125-0.17), ((7.125-0.17)/1.8)/1.618)
+
+    fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=dpi, facecolor="w",edgecolor="k",)
+    spec2 = gridspec.GridSpec(ncols=4, nrows=1, figure=fig, 
+                     left=0.02, right=1, top=0.77, bottom=0.06, wspace=0.15)
+    ax1 = fig.add_subplot(spec2[0])
+    ax2 = fig.add_subplot(spec2[1])
+    ax3 = fig.add_subplot(spec2[2])
+
+    spec23 = gridspec.GridSpecFromSubplotSpec(3, 3, subplot_spec=spec2[3], wspace=0.05)
+    ax4_11 = fig.add_subplot(spec23[0, 0])
+    ax4_12 = fig.add_subplot(spec23[0, 1])
+    ax4_13 = fig.add_subplot(spec23[0, 2])
+    ax4_21 = fig.add_subplot(spec23[1, 0])
+    ax4_22 = fig.add_subplot(spec23[1, 1])
+    ax4_23 = fig.add_subplot(spec23[1, 2])
+    ax4_31 = fig.add_subplot(spec23[2, 0])
+    ax4_32 = fig.add_subplot(spec23[2, 1])
+    ax4_33 = fig.add_subplot(spec23[2, 2])
+
+    scs = []
+    for val, i in zip([-1, 0, 1], [0, 2, 4]):
+        if val == -1:
+            sc = ax1.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
+                            color="gray", alpha=0.1, s=30)
+            ax2.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
+                            color="gray", alpha=0.1, s=30)
+            ax3.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
+                       color="gray", alpha=0.1, s=30)
+            
+        else:
+            sc = ax1.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
+                                color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=30)
+            
+            ax2.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
+                        color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=30)
+            ax3.scatter(standard_embedding[clusters == val,0], standard_embedding[clusters == val,1], marker= '.', 
+                       color=matplotlib.colormaps["Paired"].colors[i], alpha=0.2, s=30)
+        
+        scs.append(sc)
+
+    print(clusters)
+
+    plot_inst = NonLinearClock(X_new, obs, standard_embedding, labels, method="UMAP", cluster_labels=clusters)
+    arrows1, arrow_labels1 = plot_inst.plot_global_clock(
+        standartize_data=False,
+        standartize_coef=True,
+        biggest_arrow_method=True,
+        univar_importance=True,
+        ax=ax1,
+        scale_circle=1.5,
+        move_circle=[0, 0],
+        annotate=5.5,
+        arrow_width=0.5,
+        plot_scatter=False
+    )
+
+    ax1.set_yticks([])
+    ax1.set_xticks([])
+    ax1.set_ylabel("UMAP2", size=8)
+    ax1.set_xlabel("UMAP1", size=8)
+    ax1.set_title("Global clock", size=8)
+    ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
+
+    # Local
+    arrows2, arrow_labels2 = plot_inst.plot_local_clocks(
+        standartize_data=False,
+        standartize_coef=True,
+        biggest_arrow_method=True,
+        univar_importance=True,
+        ax=ax2,
+        scale_circles=[0.3, 0.4],
+        clocks_labels=["0", "1"],
+        clocks_labels_angles = [45, 270],
+        move_circles=[[0, 0], [0, 0]],
+        annotates=[5, 3],
+        arrow_width=0.45,
+        plot_hulls=False,
+        plot_scatter=False
+    )
+
+    ax2.set_yticks([])
+    ax2.set_xticks([])
+    ax2.set_ylabel("UMAP2", size=8)
+    ax2.set_xlabel("UMAP1", size=8)
+    ax2.set_title("Local clock", size=8)
+    ax2.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax2.xaxis.set_label_coords(x=0.5, y=-0.02)
+
+    # Between
+    arrows3, arrow_labels3 = plot_inst.plot_between_clock(
+        standartize_data=False,
+        standartize_coef=True,
+        univar_importance=True,
+        ax=ax3,
+        scale_circles=[1, 1],
+        move_circles=[[0, 0], [0.0, 0]],
+        annotates=[5],
+        arrow_width=0.5,
+        plot_hulls=False,
+        plot_scatter=False
+    )
+
+    arrows_dict = {}
+    for i, val in enumerate(arrow_labels3):
+        arrows_dict[val] = arrows3[i]
+    for i, val in enumerate(arrow_labels1):
+        arrows_dict[val] = arrows1[i]
+    for i, val in enumerate(arrow_labels2):
+        arrows_dict[val] = arrows2[i]
+    
+    hatches = [plt.plot([],marker="", ls="")[0]]*2 + \
+        [list(arrows_dict.values())[0]] + [scs[1]] + \
+        [list(arrows_dict.values())[1]] + [scs[2]] + \
+        [list(arrows_dict.values())[2]] + [scs[0]] + \
+        [list(arrows_dict.values())[3]] + [plt.plot([],marker="", ls="")[0]] + \
+        [list(arrows_dict.values())[4]] + [plt.plot([],marker="", ls="")[0]] + \
+        [list(arrows_dict.values())[5]] + [plt.plot([],marker="", ls="")[0]] + \
+        [list(arrows_dict.values())[6]] + [plt.plot([],marker="", ls="")[0]] + \
+        [list(arrows_dict.values())[7]] + [plt.plot([],marker="", ls="")[0]] + \
+        [list(arrows_dict.values())[8]] + [plt.plot([],marker="", ls="")[0]]
+
+    labels = ["Factors:", "Labels:"] + \
+        [list(arrows_dict.keys())[0]] + ["0"] + \
+        [list(arrows_dict.keys())[1]] + ["1"] + \
+        [list(arrows_dict.keys())[2]] + ["No class"] + \
+        [list(arrows_dict.keys())[3]] + [""] + \
+        [list(arrows_dict.keys())[4]] + [""] + \
+        [list(arrows_dict.keys())[5]] + [""] + \
+        [list(arrows_dict.keys())[6]] + [""] + \
+        [list(arrows_dict.keys())[7]] + [""] + \
+        [list(arrows_dict.keys())[8]] + [""]
+
+    leg = ax3.legend(
+        hatches,
+        labels,
+        loc="lower center",
+        bbox_to_anchor=(-0.13, 1.1),
+        fontsize=7,
+        ncol=10,
+        markerscale=0.6,
+        handlelength=1.5,
+        columnspacing=0.8,
+        handletextpad=0.5,
+        handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
+    )
+    for vpack in leg._legend_handle_box.get_children()[:1]:
+        for hpack in vpack.get_children():
+            hpack.get_children()[0].set_width(0)
+    for lh in leg.legendHandles: 
+        lh.set_alpha(1)
+
+    ax3.set_yticks([])
+    ax3.set_xticks([])
+    ax3.set_ylabel("UMAP2", size=8)
+    ax3.set_xlabel("UMAP1", size=8)
+    ax3.set_title("Inter-cluster clock", size=8)
+    ax3.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax3.xaxis.set_label_coords(x=0.5, y=-0.02)
+
+    X_new, obs, standard_embedding, labels, clusters = setup_neftel_data(method="umap")
+    
+    for (i, o), axi in zip(enumerate(obs), [ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33]):
+        im = axi.scatter(
+            standard_embedding[:, 0],
+            standard_embedding[:, 1],
+            marker=".",
+            s=1.3,
+            c=X_new[o],
+            cmap=cm.coolwarm,
+            # vmin=0, vmax=1
+        )
+        axi.set_yticks([])
+        axi.set_xticks([])
+        # axi.yaxis.set_label_coords(x=-0.01, y=0.5)
+        # axi.xaxis.set_label_coords(x=0.5, y=-0.02)
+        
+        if o == "genes_expressed":
+            o = "genes_exp."
+        axi.set_title(o, size=5, pad=-14)
+
+    ax4_21.set_ylabel("UMAP2", size=8)
+    ax4_32.set_xlabel("UMAP1", size=8)
+
+    ax4_21.yaxis.set_label_coords(x=-0.01, y=0.5)
+    ax4_32.xaxis.set_label_coords(x=0.55, y=-0.07)
+
+    cbar = fig.colorbar(im, ax=[ax4_11, ax4_12, ax4_13, ax4_21, ax4_22, ax4_23, ax4_31, ax4_32, ax4_33], 
+                        pad=0.02, aspect=40)
+    cbar.ax.tick_params(labelsize=5, pad=0.2, length=0.8, grid_linewidth=0.1) #labelrotation=90,
+    cbar.outline.set_visible(False)
+
+    plt.savefig("plots/paper/neftel/neftel_3.pdf")
+
+
 # test_between_all()
-test_all_4_in_row()
+test_all_4_in_row_hdbscan()
 # print_neftel_all()
 # test_experiment2()
```

### Comparing `feature_clock-0.0.2/test/test_pima.py` & `feature_clock-0.0.3/test/test_pima.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from matplotlib import pyplot as plt
 from matplotlib.legend_handler import HandlerPatch
 import numpy as np
 import pandas as pd
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
 def make_legend_arrow(legend, orig_handle,
@@ -18,15 +18,15 @@
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_pima_data(method="tsne", drop_labels=True):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/diabetes.csv"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
@@ -133,15 +133,15 @@
         handletextpad=0.5,
     )
 
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
-    ax.set_title("Diabetis", size=8)
+    ax.set_title("Diabetes", size=8)
     ax.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax.xaxis.set_label_coords(x=0.5, y=-0.02)
     plt.subplots_adjust(
         left=0.05,
         right=0.95,
         top=0.79,
         bottom=0.05,  # wspace=0.21, hspace=0.33
@@ -174,15 +174,15 @@
     #     handletextpad=0.5,
     # )
 
     ax.set_yticks([])
     ax.set_xticks([])
     ax.set_ylabel("UMAP2", size=8)
     ax.set_xlabel("UMAP1", size=8)
-    ax.set_title("Diabetis", size=8)
+    ax.set_title("Diabetes", size=8)
     ax.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax.xaxis.set_label_coords(x=0.5, y=-0.02)
     plt.subplots_adjust(
         left=0.05,
         right=0.95,
         top=0.79,
         bottom=0.05,  # wspace=0.21, hspace=0.33
@@ -272,36 +272,25 @@
     axi[0].set_xlabel("UMAP1", size=8)
     axi[0].set_title("Global clock", size=8)
     axi[0].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[0].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # Local
     sc = axi[1].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
-    # legend2 = axi[1].legend(
-    #     handles = sc.legend_elements()[0],
-    #     loc="upper center",
-    #     # bbox_to_anchor=(0.0, 0.0),
-    #     fontsize=7,
-    #     ncol=3,
-    #     markerscale=0.6,
-    #     handlelength=1.5,
-    #     columnspacing=0.8,
-    #     handletextpad=0.1,
-    #     labels=["Healthy", "Diabetis"])
-    # axi[1].add_artist(legend2)
 
     arrows2, arrow_labels2 = plot_inst.plot_local_clocks(
         standartize_data=True,
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=axi[1],
         scale_circles=[1.5, 1.5],
         move_circles=[[-2.2, 0], [2.5, 0]],
         annotates=[0.9, 0.9],
+        clocks_labels=["Healthy", "Diabetes"],
         arrow_width=0.08,
         plot_scatter=False,
         plot_hulls=False
     )
 
     axi[1].set_yticks([])
     axi[1].set_xticks([])
@@ -309,38 +298,27 @@
     axi[1].set_xlabel("UMAP1", size=8)
     axi[1].set_title("Local clock", size=8)
     axi[1].yaxis.set_label_coords(x=-0.01, y=0.5)
     axi[1].xaxis.set_label_coords(x=0.5, y=-0.02)
 
     # Between
     sc = axi[2].scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.2)
-    # legend3 = axi[2].legend(
-    #     handles = sc.legend_elements()[0],
-    #     labels=["Healthy", "Diabetis"],
-    #     loc="upper center",
-    #     # bbox_to_anchor=(0.0, 0.0),
-    #     fontsize=7,
-    #     ncol=3,
-    #     markerscale=0.6,
-    #     handlelength=1.5,
-    #     columnspacing=0.8,
-    #     handletextpad=0.1,)
-    # axi[2].add_artist(legend3)
 
     arrows3, arrow_labels3 = plot_inst.plot_between_clock(
         standartize_data=True,
         standartize_coef=True,
         univar_importance=False,
         ax=axi[2],
         scale_circles=[4],
         move_circles=[[0, 0]],
         annotates=[0.7],
         arrow_width=0.08,
         plot_scatter=False,
-        plot_hulls=False
+        plot_hulls=False,
+        clocks_labels=["Healthy", "Diabetes"],
     )
 
     arrows_dict = {}
     for i, val in enumerate(arrow_labels3):
         arrows_dict[val] = arrows3[i]
     for i, val in enumerate(arrow_labels1):
         arrows_dict[val] = arrows1[i]
@@ -352,15 +330,15 @@
 
     hatches = [plt.plot([],marker="", ls="")[0]]*2 + \
         [list(arrows_dict.values())[0]] + [sc.legend_elements()[0][0]] + \
         [list(arrows_dict.values())[1]] + [sc.legend_elements()[0][1]] + \
         list(arrows_dict.values())[2:]
     
     labels = ["Factors:", "Labels:"] + [list(arrows_dict.keys())[0]] + ["Healthy"] + \
-        [list(arrows_dict.keys())[1]] + ["Diabetis"] + \
+        [list(arrows_dict.keys())[1]] + ["Diabetes"] + \
         list(arrows_dict.keys())[2:]
 
 
     leg = axi[1].legend(
         hatches,
         labels,
         loc="lower center",
@@ -370,14 +348,16 @@
         markerscale=0.6,
         handlelength=1.3,
         columnspacing=0.8,
         handletextpad=0.5,
         handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
         # markerfirst=False 
     )
+    for lh in leg.legendHandles: 
+        lh.set_alpha(1)
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
 
     axi[2].set_yticks([])
     axi[2].set_xticks([])
```

### Comparing `feature_clock-0.0.2/test/test_pima_autoencoder.py` & `feature_clock-0.0.3/test/test_pima_autoencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from matplotlib import gridspec, pyplot as plt
 import numpy as np
 import pandas as pd
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
 def make_legend_arrow(legend, orig_handle,
@@ -16,15 +16,15 @@
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_pima_data(method="tsne", drop_labels=True, file: str=""):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/diabetes.csv"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
@@ -109,15 +109,15 @@
     # for ax in axi:
     #     for a in ax:
     #         a.axis('off') 
     plt.savefig(f"plots/paper/pima_network/plot_pimaAll_nn_{dataset_i}.pdf")
 
 
 def test_between_all_2():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/emb_6.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_6.csv")
 
     fig_size = ((7.125-0.17)/2, ((7.125-0.17)/2.5)/1.618)
 
     fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=1000, facecolor="w",edgecolor="k",)
     spec2 = gridspec.GridSpec(ncols=2, nrows=1, figure=fig, 
                      left=0.04, right=1.04, top=0.565, bottom=0.07)
     ax1 = fig.add_subplot(spec2[0])
@@ -156,15 +156,15 @@
         arrow_width=0.1
     )
 
     hatches = [plt.plot([],marker="", ls="")[0]]*4 + arrows[0:3] + \
         [sc.legend_elements()[0][0]] + arrows[3:6] + \
         [sc.legend_elements()[0][1]] + arrows[6:] + [plt.plot([],marker="", ls="")[0]]*2
     labels = ["Factors:", " ", " ", "Labels: "] + arrow_labels[0:3] + \
-        ["No diabetes"] + arrow_labels[3:6] + \
+        ["Healthy"] + arrow_labels[3:6] + \
         ["Diabetes"] + arrow_labels[6:] + [" ", " "]
     leg = ax1.legend(
         hatches, labels,
         loc="lower center",
         bbox_to_anchor=(1.02, 1.09),
         fontsize=7,
         ncol=4,
@@ -187,20 +187,17 @@
     ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
 
 
     # second plot
     axis_array = [ax2_11, ax2_12, ax2_13, ax2_21, ax2_22, ax2_23, ax2_31, ax2_32, ax2_33]
 
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/emb_6.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_6.csv")
     standard_embedding[:,0], standard_embedding[:,1] = 1 * standard_embedding[:,0], 7 * standard_embedding[:,1]
     for (i, o), axi in zip(enumerate(obs), axis_array):
-        if o == "Species":
-            break
-
         im = axi.scatter(
             standard_embedding[:, 0],
             standard_embedding[:, 1],
             marker=".",
             s=1,
             c=X_new[o],
             cmap="jet",
@@ -210,14 +207,16 @@
         axi.set_xticks([])
         axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         axi.xaxis.set_label_coords(x=0.5, y=-0.02)
         if o == "SkinThickness":
             o = "SkinThick."
         elif o == "BloodPressure":
             o = "BloodPr."
+        elif o == "Outcome":
+            o = "Labels"
         axi.set_title(o, size=5, pad=-9)
 
     ax2_21.set_ylabel("Dim2", size=8)
     ax2_32.set_xlabel("Dim1", size=8)
 
     ax2_21.yaxis.set_label_coords(0, 0.5)
     ax2_32.xaxis.set_label_coords(0.5, -0.07)
@@ -227,15 +226,15 @@
     cbar.outline.set_visible(False)
 
     plt.savefig("plots/paper/pima_network/pima_global_autoencoder.pdf")
 
 
 
 def test_between_all_new():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/emb_1_e-5.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_1_e-5.csv")
 
     fig_size = ((7.125-0.17)/2, ((7.125-0.17)/2.5)/1.618)
 
     fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=1000, facecolor="w",edgecolor="k",)
     spec2 = gridspec.GridSpec(ncols=2, nrows=1, figure=fig, 
                      left=0.04, right=1.04, top=0.565, bottom=0.07)
     ax1 = fig.add_subplot(spec2[0])
@@ -274,15 +273,15 @@
         arrow_width=0.1
     )
 
     hatches = [plt.plot([],marker="", ls="")[0]]*4 + arrows[0:3] + \
         [sc.legend_elements()[0][0]] + arrows[3:6] + \
         [sc.legend_elements()[0][1]] + arrows[6:] + [plt.plot([],marker="", ls="")[0]]*2
     labels = ["Factors:", " ", " ", "Labels: "] + arrow_labels[0:3] + \
-        ["No diabetes"] + arrow_labels[3:6] + \
+        ["Healthy"] + arrow_labels[3:6] + \
         ["Diabetes"] + arrow_labels[6:] + [" ", " "]
     leg = ax1.legend(
         hatches, labels,
         loc="lower center",
         bbox_to_anchor=(1.02, 1.09),
         fontsize=7,
         ncol=4,
@@ -305,15 +304,15 @@
     ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
 
 
     # second plot
     axis_array = [ax2_11, ax2_12, ax2_13, ax2_21, ax2_22, ax2_23, ax2_31, ax2_32, ax2_33]
 
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/emb_1_e-5.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/emb_1_e-5.csv")
     standard_embedding[:,0], standard_embedding[:,1] = 1 * standard_embedding[:,0], 7 * standard_embedding[:,1]
     for (i, o), axi in zip(enumerate(obs), axis_array):
         if o == "Species":
             break
 
         im = axi.scatter(
             standard_embedding[:, 0],
@@ -328,14 +327,16 @@
         axi.set_xticks([])
         axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         axi.xaxis.set_label_coords(x=0.5, y=-0.02)
         if o == "SkinThickness":
             o = "SkinThick."
         elif o == "BloodPressure":
             o = "BloodPr."
+        elif o == "Outcome":
+            o = "Labels"
         axi.set_title(o, size=5, pad=-9)
 
     ax2_21.set_ylabel("Dim2", size=8)
     ax2_32.set_xlabel("Dim1", size=8)
 
     ax2_21.yaxis.set_label_coords(0, 0.5)
     ax2_32.xaxis.set_label_coords(0.5, -0.07)
```

### Comparing `feature_clock-0.0.2/test/test_pima_nn.py` & `feature_clock-0.0.3/test/test_pima_nn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from matplotlib import pyplot as plt
 import numpy as np
 import pandas as pd
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
 def make_legend_arrow(legend, orig_handle,
@@ -18,15 +18,15 @@
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_pima_data(method="tsne", drop_labels=True, file: str=""):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/diabetes.csv"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
@@ -99,15 +99,15 @@
     # for ax in axi:
     #     for a in ax:
     #         a.axis('off') 
     plt.savefig(f"plots/paper/pima_network/plot_pimaAll_nn_{dataset_i}.pdf")
 
 
 def test_between_all_1():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", file="/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/latent_space_1.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", file="/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_1.csv")
 
     fig, ax = plt.subplots(1, figsize=(3.2325, 3.2325)) #(2.375, 2.375)
     plt.tight_layout()
 
     sc = ax.scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
     colors = [
         'tab:pink', 'tab:green', 'tab:blue', 'tab:olive', 'tab:orange',
@@ -160,15 +160,15 @@
         right=0.96,
         top=0.73,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/pima_network/pima_global_nn_1.pdf")
 
 def test_between_all_2():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/latent_space_2.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="umap", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2.csv")
 
     fig, ax = plt.subplots(1, figsize=(3.2325, 3.2325)) #(2.375, 2.375)
     plt.tight_layout()
 
     sc = ax.scatter(standard_embedding[:,0], standard_embedding[:,1], marker= '.', c=labels, cmap="Accent", zorder=0, alpha=0.3)
 
     colors = [
@@ -221,11 +221,11 @@
         right=0.99,
         top=0.77,
         bottom=0.05,  # wspace=0.21, hspace=0.33
     )
     plt.savefig("plots/paper/pima_network/pima_global_nn_2.pdf")
 
 
-# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/latent_space_1.csv", 1)
+# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_1.csv", 1)
 test_between_all_1()
-# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/latent_space_2.csv", 2)
+# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2.csv", 2)
 test_between_all_2()
```

### Comparing `feature_clock-0.0.2/test/test_pima_nn_2out.py` & `feature_clock-0.0.3/test/test_pima_nn_2out.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from matplotlib import gridspec, pyplot as plt
 import numpy as np
 import pandas as pd
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import umap
 from sklearn.cluster import HDBSCAN
 from sklearn.cluster import KMeans
 from matplotlib.legend_handler import HandlerPatch
 import matplotlib.patches as mpatches
 
 def make_legend_arrow(legend, orig_handle,
@@ -18,15 +18,15 @@
 
 
 def read_data(path):
     return pd.read_csv(path, header=0)
 
 
 def setup_pima_data(method="tsne", drop_labels=True, file: str=""):
-    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/diabetes.csv"
+    file_name = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/diabetes.csv"
     X = read_data(file_name)
     X.rename(columns={"DiabetesPedigreeFunction": "Pedigree"}, inplace=True)
     X = X.dropna()
 
     labels = X["Outcome"]
     if drop_labels:
         X.drop(columns=["Outcome"], inplace=True)
@@ -109,15 +109,15 @@
     # for ax in axi:
     #     for a in ax:
     #         a.axis('off') 
     plt.savefig(f"plots/paper/pima_network/plot_pimaAll_nn_{dataset_i}.pdf")
 
 
 def test_between_all_2():
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/latent_space_2_2out.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2_2out.csv")
 
     fig_size = ((7.125-0.17)/2, ((7.125-0.17)/2.5)/1.618)
 
     fig = plt.figure(constrained_layout=True, figsize=fig_size, dpi=1000, facecolor="w",edgecolor="k",)
     spec2 = gridspec.GridSpec(ncols=2, nrows=1, figure=fig, 
                      left=0.04, right=1.04, top=0.565, bottom=0.07)
     ax1 = fig.add_subplot(spec2[0])
@@ -149,22 +149,22 @@
         standartize_coef=True,
         biggest_arrow_method=True,
         univar_importance=False,
         ax=ax1,
         scale_circle=2,
         move_circle=[0, 2],
         annotate=2.0,
-        arrow_width=0.1
+        arrow_width=0.15
     )
 
     hatches = [plt.plot([],marker="", ls="")[0]]*4 + arrows[0:3] + \
         [sc.legend_elements()[0][0]] + arrows[3:6] + \
         [sc.legend_elements()[0][1]] + arrows[6:] + [plt.plot([],marker="", ls="")[0]]*2
     labels = ["Factors:", " ", " ", "Labels: "] + arrow_labels[0:3] + \
-        ["No diabetes"] + arrow_labels[3:6] + \
+        ["Healthy"] + arrow_labels[3:6] + \
         ["Diabetes"] + arrow_labels[6:] + [" ", " "]
     leg = ax1.legend(
         hatches, labels,
         loc="lower center",
         bbox_to_anchor=(1.02, 1.09),
         fontsize=7,
         ncol=4,
@@ -174,28 +174,30 @@
         handletextpad=0.5,
         handler_map={mpatches.FancyArrow : HandlerPatch(patch_func=make_legend_arrow),},
     )
 
     for vpack in leg._legend_handle_box.get_children()[:1]:
         for hpack in vpack.get_children():
             hpack.get_children()[0].set_width(0)
+    for lh in leg.legendHandles: 
+        lh.set_alpha(1)
 
     ax1.set_yticks([])
     ax1.set_xticks([])
     ax1.set_ylabel("Dim2", size=8)
     ax1.set_xlabel("Dim1", size=8)
     # ax1.set_title("Second hidden layer", size=8)
     ax1.yaxis.set_label_coords(x=-0.01, y=0.5)
     ax1.xaxis.set_label_coords(x=0.5, y=-0.02)
 
 
     # second plot
     axis_array = [ax2_11, ax2_12, ax2_13, ax2_21, ax2_22, ax2_23, ax2_31, ax2_32, ax2_33]
 
-    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/latent_space_2_2out.csv")
+    X_new, obs, standard_embedding, labels, clusters = setup_pima_data(method="", drop_labels=False, file = "/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2_2out.csv")
     standard_embedding[:,0], standard_embedding[:,1] = 1 * standard_embedding[:,0], 7 * standard_embedding[:,1]
     for (i, o), axi in zip(enumerate(obs), axis_array):
         if o == "Species":
             break
 
         im = axi.scatter(
             standard_embedding[:, 0],
@@ -210,14 +212,16 @@
         axi.set_xticks([])
         axi.yaxis.set_label_coords(x=-0.01, y=0.5)
         axi.xaxis.set_label_coords(x=0.5, y=-0.02)
         if o == "SkinThickness":
             o = "SkinThick."
         elif o == "BloodPressure":
             o = "BloodPr."
+        elif o == "Outcome":
+            o = "Labels"
         axi.set_title(o, size=5, pad=-9)
 
     ax2_21.set_ylabel("Dim2", size=8)
     ax2_32.set_xlabel("Dim1", size=8)
 
     ax2_21.yaxis.set_label_coords(0, 0.5)
     ax2_32.xaxis.set_label_coords(0.5, -0.07)
@@ -227,9 +231,9 @@
     cbar.outline.set_visible(False)
 
 
 
     plt.savefig("plots/paper/pima_network/pima_global_nn_last_2out.pdf")
 
 
-# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/latent_space_2.csv", 2)
+# print_pima_all("/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/latent_space_2.csv", 2)
 test_between_all_2()
```

### Comparing `feature_clock-0.0.2/test/test_real_data.py` & `feature_clock-0.0.3/test/test_real_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import scanpy as sp
-from src.nonlinear_clock.plot import NonLinearClock
+from src.feature_clock.plot import NonLinearClock
 import scanpy.external as sce
 import phate
 import pandas as pd
 
 def read_data(path):
     return pd.read_csv(path, sep=";", header=0)
 
 def setup_data(method = "umap"):
-    file_name = '/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/non_lin_visualization/data/E-GEOD-46817-query-results.csv'
+    file_name = '/Users/olga_ovcharenko/Documents/ETH/FS23/ResearchProject/feature_clock_visualization/data/E-GEOD-46817-query-results.csv'
     X = read_data(file_name)
 
     obs = [ 
            "A2058",   "A375",   "C32",  "Malme3M",  "SKMEL28",  "SKMEL5",  "WM2664"
            ]
     
     new_data = X[obs].dropna()
```

