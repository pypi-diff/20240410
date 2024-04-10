# Comparing `tmp/dualPredictor-0.0.7.tar.gz` & `tmp/dualPredictor-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualPredictor-0.0.7.tar", last modified: Sat Mar 23 10:01:05 2024, max compression
+gzip compressed data, was "dualPredictor-0.0.8.tar", last modified: Wed Apr 10 11:34:04 2024, max compression
```

## Comparing `dualPredictor-0.0.7.tar` & `dualPredictor-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:01:05.229679 dualPredictor-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-23 10:00:55.000000 dualPredictor-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-03-23 10:01:05.229679 dualPredictor-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-03-23 10:00:55.000000 dualPredictor-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:01:05.229679 dualPredictor-0.0.7/dualPredictor/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-23 10:00:55.000000 dualPredictor-0.0.7/dualPredictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-23 10:00:55.000000 dualPredictor-0.0.7/dualPredictor/dual_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-03-23 10:00:55.000000 dualPredictor-0.0.7/dualPredictor/model_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:01:05.229679 dualPredictor-0.0.7/dualPredictor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-03-23 10:01:05.000000 dualPredictor-0.0.7/dualPredictor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-23 10:01:05.000000 dualPredictor-0.0.7/dualPredictor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 10:01:05.000000 dualPredictor-0.0.7/dualPredictor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 10:01:05.000000 dualPredictor-0.0.7/dualPredictor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-23 10:01:05.000000 dualPredictor-0.0.7/dualPredictor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 10:01:05.229679 dualPredictor-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-23 10:00:55.000000 dualPredictor-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:34:04.022487 dualPredictor-0.0.8/dualPredictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/dualPredictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/dualPredictor/dual_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/dualPredictor/model_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/dualPredictor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 11:34:01.000000 dualPredictor-0.0.8/setup.py
```

### Comparing `dualPredictor-0.0.7/LICENSE` & `dualPredictor-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dualPredictor-0.0.7/dualPredictor/dual_model.py` & `dualPredictor-0.0.8/dualPredictor/dual_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     def __init__(self, model_type='lasso', metric='youden_index',default_cut_off=0.5):
         self.model_type = model_type
         self.metric=metric
         self.default_cut_off = default_cut_off
         self.model = None
         self.optimal_cut_off = None
         self.y_label_true_=None
+        self.metrics=None
+        self.cutoffs=None
 
         if model_type == 'lasso':
             self.model = LassoCV(cv=5)
         elif model_type == 'ridge':
             self.model = RidgeCV(cv=5)
         elif model_type == 'ols':
             self.model = LinearRegression()
@@ -31,15 +33,15 @@
         y_label_true = (y < self.default_cut_off).astype(int)
         self.y_label_true_=y_label_true
         # error hadnling for the user input default cut_off
         if self.default_cut_off >= np.max(y):
                     raise ValueError("The default cut-off must be smaller than the maximum value of y.")
 
         # Tune the optimal cut-off
-        cut_offs = np.linspace(self.default_cut_off, max(y) * 0.9, 100)
+        cut_offs = np.linspace(self.default_cut_off, max(y), 55)
         metrics = []
 
         for cut_off in cut_offs:
             y_pred = (self.model.predict(X) < cut_off).astype(int)
             if self.metric == 'f1_score':
                 metric_value = fbeta_score(y_label_true, y_pred,beta=1)
             elif self.metric == 'f2_score':
@@ -51,23 +53,33 @@
 
             metrics.append(metric_value)
 
         max_metric = max(metrics)
         max_indices = [i for i, x in enumerate(metrics) if x == max_metric]
         middle_index = max_indices[len(max_indices) // 2]
         self.optimal_cut_off = cut_offs[middle_index]
+        self.metrics=metrics
+        self.cutoffs=cut_offs
 
         return self
 
     def predict(self, X):
         grade_predictions = self.model.predict(X)
         class_predictions = (grade_predictions < self.optimal_cut_off).astype(int)
         return grade_predictions, class_predictions
 
     @property
+    def metrics_(self):
+        return self.metrics
+
+    @property
+    def cutoffs_(self):
+        return self.cutoffs
+
+    @property
     def alpha_(self):
         return self.model.alpha_
 
     @property
     def coef_(self):
         return self.model.coef_
```

### Comparing `dualPredictor-0.0.7/dualPredictor/model_plot.py` & `dualPredictor-0.0.8/dualPredictor/model_plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -102,7 +102,26 @@
     for i, coef in enumerate(sorted_coef):
         ax.text(coef, i, str(coef), va="center")
 
     # Add a title to the plot
     ax.set_title(f"Feature Coefficient Plot - {num_of_features} features")
 
     return fig
+
+def plot_cutoff_tuning(cutoffs,metrics, xlabel="Cutoff", ylabel="Metric"):
+    """Plots the results of cutoff tuning.
+
+    Args:
+        dual_clf: A DualModel object.
+        title: The title of the plot.
+        xlabel: The label for the x-axis.
+        ylabel: The label for the y-axis.
+    """
+
+    # Plot the results
+    plt.figure(figsize=(7, 3.5), dpi=500)
+    plt.plot(cutoffs, metrics, label=f'{ylabel}', color='blue')
+    plt.title("Cutoff Tuning Plot")
+    plt.xlabel(xlabel)
+    plt.ylabel(ylabel)
+    plt.legend()
+    plt.show()
```

### Comparing `dualPredictor-0.0.7/setup.py` & `dualPredictor-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dualPredictor",
-    version="0.0.7",
+    version="0.0.8",
     author="Dong",
     author_email="no@email.com",
     description="A Python package for simultaneous regression and binary classification for educational analytics.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/098765d/dualPredictor.git",
     packages=find_packages(),
```

