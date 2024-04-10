# Comparing `tmp/lemon_explainer-0.0.2.tar.gz` & `tmp/lemon_explainer-0.0.3.tar.gz`

## Comparing `lemon_explainer-0.0.2.tar` & `lemon_explainer-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,16 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/.DS_Store
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/.gitattributes
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/CITATION.cff
--rw-r--r--   0        0        0    60723 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/example.ipynb
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/requirements.txt
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/lemon/__init__.py
--rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/lemon/explainer.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/lemon/explanation.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/lemon/kernels.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/tests/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/tests/test_explainer.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/.gitignore
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/LICENSE
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 lemon_explainer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/.gitattributes
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/CITATION.cff
+-rw-r--r--   0        0        0    60723 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/example.ipynb
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/lemon/__init__.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/lemon/explainer.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/lemon/explanation.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/lemon/kernels.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/tests/test_explainer.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 lemon_explainer-0.0.3/PKG-INFO
```

### Comparing `lemon_explainer-0.0.2/CITATION.cff` & `lemon_explainer-0.0.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `lemon_explainer-0.0.2/example.ipynb` & `lemon_explainer-0.0.3/example.ipynb`

 * *Files identical despite different names*

### Comparing `lemon_explainer-0.0.2/lemon/explainer.py` & `lemon_explainer-0.0.3/lemon/explainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,48 +25,50 @@
       continuous. Values in these columns MUST be integers.
 
   training_data_stats: {str: float | dict}
       a dict object having the details of training data statistics. For numerical features, this
       describes the standard deviation, for categorical features the frequencies of each category.
 
   sample_size: int
-      Number of samples to generate to train the surrogate model on. More sample means a 
+      Number of samples to generate to train the surrogate model on. More sample means a
       more faithful explanation, but longer running time.
 
   distance_kernel: callable
-      Kernel function to determine the density of samples points around the data instance to be 
+      Kernel function to determine the density of samples points around the data instance to be
       explained. Defaults to uniform kernel, which is likely sufficient for most users.
 
   radius_max: float
-      Maximum radius of the hypersphere, in _normalized_ feature space. In other words, how much 
+      Maximum radius of the hypersphere, in _normalized_ feature space. In other words, how much
       LEMON varies the feature value of each feature to find 'similar' data points, as a percentage
       of the feature range. The lower, the more local the explanation.
 
   random_state: int, RandomState instance or None
-      Controls the randomness of the hypershphere transfer data samples, and samples used for inverse 
+      Controls the randomness of the hypershphere transfer data samples, and samples used for inverse
       transform sampling. Can be used for reproducibility of the explanation.
 
   """
+
   def __init__(
-      self, 
+      self,
       training_data=None,
-      categorical_features=[], 
+      categorical_features=[],
       training_data_stats={},
-      sample_size=5000, 
-      distance_kernel=None, 
-      radius_max=1, 
+      sample_size=5000,
+      distance_kernel=None,
+      radius_max=1,
       random_state=None,
   ):
     self.random_state = check_random_state(random_state)
     np.random.seed(random_state)
 
     self.categorical_features = categorical_features
 
     if training_data is None and len(training_data_stats) > 0:
-      self.training_data = pd.DataFrame([], columns=list(training_data_stats.keys()))
+      self.training_data = pd.DataFrame(
+        [], columns=list(training_data_stats.keys()))
       self.scaler = StandardScaler(with_mean=False)
       self.scaler.scale_ = [
         x for i, x in enumerate(training_data_stats.values())
         if i not in categorical_features
       ]
       self.scaler.mean_ = [
         0 for i, _ in enumerate(training_data_stats.values())
@@ -74,51 +76,66 @@
       ]
 
       dimensions = len(training_data_stats)
     else:
       self.training_data = training_data
 
       self.scaler = StandardScaler(with_mean=False)
-      self.scaler.fit(np.asanyarray(training_data)[:, np.setdiff1d(np.arange(training_data.shape[1]), categorical_features)])
-      
+      self.scaler.fit(
+          np.asanyarray(training_data)[
+              :,
+              np.setdiff1d(
+                  np.arange(
+                      training_data.shape[1]),
+                  categorical_features)])
+
       training_data_stats = {
-        training_data.columns[i]: dict(zip(*np.unique(training_data.iloc[:, i], return_counts=True)))
+        training_data.columns[i]: dict(
+          zip(*np.unique(training_data.iloc[:, i], return_counts=True)))
         for i in categorical_features
       }
-    
+
       dimensions = training_data.shape[1]
 
     n_categorical = len(categorical_features)
     n_numerical = dimensions - n_categorical
 
     if distance_kernel is None:
       distance_kernel = uniform_kernel
-  
-    self.sampling_kernel = self._transform(distance_kernel, n_numerical, radius_max=radius_max)
+
+    self.sampling_kernel = self._transform(
+        distance_kernel, n_numerical, radius_max=radius_max)
     self.sample_size = sample_size
 
     # Create hypersphere samples. The sphere is only computed once for performance and stability,
     # alternatively we can resample the sphere every time `explain_instance` is called, but this
-    # affects running time. My preliminary tests indicate not resampling every time does not 
+    # affects running time. My preliminary tests indicate not resampling every time does not
     # practically affect the resulting explanation much.
-    self.sphere = self._sample_hypersphere(sample_size, n_numerical, categorical_features, training_data_stats)
+    self.sphere = self._sample_hypersphere(
+        sample_size,
+        n_numerical,
+        categorical_features,
+        training_data_stats)
 
   @property
   def surrogate(self):
     """
-    Surrogate model. 
+    Surrogate model.
 
-    This can be any regression model as long as it exposes 
+    This can be any regression model as long as it exposes
     feature-wise coefficients in `surrogate.coef_`.
-    
+
     """
     try:
       return self._surrogate
     except AttributeError:
-      self._surrogate = Ridge(alpha=self.sample_size, fit_intercept=True, random_state=self.random_state)
+      self._surrogate = Ridge(
+          alpha=self.sample_size,
+          fit_intercept=True,
+          random_state=self.random_state)
       return self._surrogate
 
   @property
   def pipeline(self):
     """
     Pipeline for applying the surrogate model on scaled data.
 
@@ -127,99 +144,120 @@
     """
     try:
       return self._pipeline
     except AttributeError:
       self._pipeline = make_pipeline(MinMaxScaler(), self.surrogate)
       return self._pipeline
 
-  def explain_instance(self, instance, predict_fn, labels=None, surrogate=None):
+  def explain_instance(self, instance, predict_fn,
+                       labels=None, surrogate=None):
     """
     Explain the prediction for the provided instance
 
     Parameters
     ----------
     instance: numpy.array
         The instance to be explained.
 
     prediction_fn: callable
-        any callable function that returns the predicted probability. Typically the `predict_proba` 
+        any callable function that returns the predicted probability. Typically the `predict_proba`
         method from scikit-learn.
 
     labels: Tuple[int, ...]
-        Index of which classes to explain: we calculate the feature contribution towards the prediction 
+        Index of which classes to explain: we calculate the feature contribution towards the prediction
         of a particular class.
 
     surrogate: sklearn.base.RegressorMixin
-        Use a custom surrogate model. This can be any regression model as long as it exposes 
+        Use a custom surrogate model. This can be any regression model as long as it exposes
         feature-wise coefficients in `surrogate.coef_`.
-    
+
     """
     if surrogate is not None:
       self._surrogate = surrogate
-  
-    # Create transfer dataset by perturbing the original instance with the hypersphere samples
+
+    # Create transfer dataset by perturbing the original instance with the
+    # hypersphere samples
     X_transfer = self._samples_around(instance, self.categorical_features)
-    
+
     if isinstance(self.training_data, pd.DataFrame):
       prediction = predict_fn(pd.DataFrame(instance).T)
-      y_transfer = predict_fn(pd.DataFrame(X_transfer, columns=self.training_data.columns))
+      y_transfer = predict_fn(
+          pd.DataFrame(
+              X_transfer,
+              columns=self.training_data.columns))
     else:
-      prediction = predict_fn(np.array(instance).reshape(1,-1))
+      prediction = predict_fn(np.array(instance).reshape(1, -1))
       y_transfer = predict_fn(X_transfer)
 
+    if y_transfer.ndim == 1:  # Single-output model
+      prediction = prediction[..., None]
+      y_transfer = y_transfer[..., None]
+
+    # infer model type
     if labels is None:
-      prediction_index = np.argmax(prediction)
-      labels = (prediction_index,)
+      if prediction.sum() == 1:
+        # outputs probabilities: classification model, explain predicted class
+        prediction_index = np.argmax(prediction)
+        labels = (prediction_index,)
+      else:
+        # other: (multi-output) regression, explain all targets
+        labels = tuple([*np.arange(prediction.shape[-1])])
 
     for index in self.categorical_features:
       # single one-hot encoded feature for categorical
-      X_transfer[:,index] = (X_transfer[:,index] == instance.values[index]).astype(int)
+      X_transfer[:, index] = (X_transfer[:, index] ==
+                              instance.values[index]).astype(int)
 
     def explain_label(label):
-      self.pipeline.fit(X_transfer, y_transfer[:,label])
-      certainty = prediction[:,label]
-      score = self.pipeline.score(X_transfer, y_transfer[:,label])
+      self.pipeline.fit(X_transfer, y_transfer[:, label])
+      certainty = prediction[:, label]
+      score = self.pipeline.score(X_transfer, y_transfer[:, label])
 
       return Explanation(
         instance,
         self.surrogate,
         label=label,
         label_certainty=certainty,
         local_faithfulness=score
       )
 
     return [explain_label(label) for label in labels]
-  
+
   def _samples_around(self, instance, categorical_features):
-    instance = np.array(instance).reshape(1,-1)
-    
+    instance = np.array(instance).reshape(1, -1)
+
     if categorical_features is not None:
-      numeric_idx = [i for i in range(instance.shape[1]) if i not in categorical_features]
+      numeric_idx = [
+          i for i in range(
+              instance.shape[1]) if i not in categorical_features]
       sphere = np.copy(self.sphere)
-      sphere[:, numeric_idx] = self.scaler.inverse_transform(sphere[:, numeric_idx])
-      sphere[:, numeric_idx] = sphere[:, numeric_idx].astype('float') + instance[:, numeric_idx]
+      sphere[:, numeric_idx] = self.scaler.inverse_transform(
+        sphere[:, numeric_idx])
+      sphere[:, numeric_idx] = sphere[:, numeric_idx].astype(
+        'float') + instance[:, numeric_idx]
       X_transfer = sphere
     else:
       numeric_idx = [i for i in range(instance.shape[1])]
       X_transfer = self.scaler.inverse_transform(self.sphere) + instance
 
     return X_transfer
 
-  def _sample_hypersphere(self, sample_size, n_numerical, categorical_features=[], training_data_stats={}):
+  def _sample_hypersphere(self, sample_size, n_numerical,
+                          categorical_features=[], training_data_stats={}):
     """
     Sample from `distance_kernel`-distributed hypersphere.
 
-    Generates samples on a n-dimensional hypersphere distributed according to `distance_kernel` 
-    provided in the initializer. This sphere is later scaled and translated into the feature 
+    Generates samples on a n-dimensional hypersphere distributed according to `distance_kernel`
+    provided in the initializer. This sphere is later scaled and translated into the feature
     space of the training data set.
-    
+
     Parameters
     ----------
     sample_size: int
-        Number of samples to generate to train the surrogate model on. More sample means a 
+        Number of samples to generate to train the surrogate model on. More sample means a
         more faithful explanation, but longer running time.
 
     n_numerical: int
         Number of numerical features, equal to the number of numerical features in the original training dataset.
 
     categorical_features : list
         list of indices corresponding to the categorical columns. Everything else will be considered
@@ -228,29 +266,37 @@
     training_data_stats: {str: float | dict}
         a dict object having the details of training data statistics. For this method, only info
         about the categorical features is used: the frequencies of each category.
 
     """
     sphere = np.random.normal(size=(sample_size, n_numerical))
     sphere = normalize(sphere)
-    sphere *= self.sampling_kernel(np.random.uniform(size=sample_size)).reshape(-1,1)
+    sphere *= self.sampling_kernel(
+      np.random.uniform(size=sample_size)).reshape(-1, 1)
 
     for index in categorical_features:
       descriptor = training_data_stats[self.training_data.columns[index]]
       categories = list(descriptor.keys())
       frequencies = np.array(list(descriptor.values()))
-      values = self.random_state.choice(categories, size=sample_size, replace=True, p=frequencies / float(sum(frequencies)))
-      sphere = np.c_[sphere[:,0:index], values, sphere[:, index:]]
+      values = self.random_state.choice(
+          categories,
+          size=sample_size,
+          replace=True,
+          p=frequencies /
+          float(
+              sum(frequencies)))
+      sphere = np.c_[sphere[:, 0:index], values, sphere[:, index:]]
 
     return sphere
-  
-  def _transform(self, kernel, n_numerical, sample_size=5000, radius_max=1, adjust=True): 
+
+  def _transform(self, kernel, n_numerical, sample_size=5000,
+                 radius_max=1, adjust=True):
     """
     Inverse transform sampling
-    
+
     Generate samples distributed according to the distribution described by the `kernel` function,
     adjusted for sampling within a hypersphere ($x^{n-1}$).
 
     Parameters
     ----------
     kernel: callable
         Original PDF to sample from.
@@ -258,15 +304,15 @@
     n_numerical: int
         Number of (numerical) dimensions to adjust for hypersphere sampling.
 
     sample_size: int
         Number of samples to invert the distribution function.
 
     radius_max: float
-        Maximum radius of the hypersphere, in _normalized_ feature space. In other words, how much 
+        Maximum radius of the hypersphere, in _normalized_ feature space. In other words, how much
         LEMON varies the feature value of each feature to find similar data points, as a percentage
         of the feature range. The lower, the more local the explanation.
 
     """
     if adjust:
       pdf = lambda x: kernel(x) * (x ** (n_numerical - 1))
     else:
```

### Comparing `lemon_explainer-0.0.2/lemon/explanation.py` & `lemon_explainer-0.0.3/lemon/explanation.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,48 +10,50 @@
 
   Parameters
   ----------
   instance: pandas.DataFrame, numpy.array
       The instance that is explained.
 
   surrogate: sklearn.base.RegressorMixin
-      The fitted surrogate model. This can be any regression model as long as it exposes 
+      The fitted surrogate model. This can be any regression model as long as it exposes
       feature-wise coefficients in `surrogate.coef_`.
 
   local_faithfulness: float
-      Local faithfulness of the surrogate, or the sklearn score with respect to the 
+      Local faithfulness of the surrogate, or the sklearn score with respect to the
       reference model to be explained.
 
   label: int
       The class label this explanation explains. Typically the predicted label by the model
       for this instance.
 
   label_certainty: float
       The predicted probability for the prediction of this instance.
 
   """
-  def __init__(self, instance, surrogate, label, label_certainty, local_faithfulness):
+
+  def __init__(self, instance, surrogate, label,
+               label_certainty, local_faithfulness):
     # TODO: check if surrogate is fitted and has coef_
     self.instance = instance
     self.surrogate = surrogate
     self.label = label
     self.label_certainty = label_certainty
     self.local_faithfulness = local_faithfulness
 
   @property
   def feature_contribution(self):
-     """
-     Returns a score for each feature that indicates how much it contributed to the final prediction. 
-     
-     More precisely, it shows the sensitivity of the feature: a small change in an important feature's 
-     value results in a relatively large change in prediction. 
-
-     """
-     # TODO: return feature contribution for other types of models.
-     return self.surrogate.coef_
+    """
+    Returns a score for each feature that indicates how much it contributed to the final prediction.
+
+    More precisely, it shows the sensitivity of the feature: a small change in an important feature's
+    value results in a relatively large change in prediction.
+
+    """
+    # TODO: return feature contribution for other types of models.
+    return self.surrogate.coef_
 
   def plot(self, normalize=True, absolute_value=False):
     """
     Plot feature contribution as vertical bar chart.
 
     """
     if not isinstance(self.instance, pd.Series):
@@ -67,37 +69,38 @@
 
     feature_contribution = self.feature_contribution
 
     if absolute_value:
       feature_contribution = np.abs(feature_contribution)
     if normalize:
       feature_contribution /= np.sum(np.abs(feature_contribution))
-      
+
     contribution = pd.Series(feature_contribution, index=self.instance.index)
     contribution = contribution.iloc[contribution.abs().argsort()]
     fig, _ = plt.subplots()
     contribution.plot.barh(
       color=['#ff5a42' if c < 0 else '#007cff' for c in contribution],
     )
     plt.axvline(x=0, color='black', linewidth=1)
 
-    fig.suptitle("Feature contribution (LEMON)", x=0, y=1, ha='left', va='top', fontweight='bold')
+    fig.suptitle("Feature contribution (LEMON)", x=0, y=1,
+                 ha='left', va='top', fontweight='bold')
     offsetY = transforms.ScaledTranslation(0, -0.3, fig.dpi_scale_trans)
-    plt.title("Shows the sensitivity of a feature: a small change in an important feature's value results in a relatively large change in prediction.", 
+    plt.title("Shows the sensitivity of a feature: a small change in an important feature's value results in a relatively large change in prediction.",
               x=0, y=1, ha='left', va='top', fontsize=13, color='#5e6e8a', transform=fig.transFigure + offsetY, wrap=True)
-    
+
     plt.tight_layout()
 
   def as_list(self):
     """
     Convenience method with similar interface to LIME.
 
     """
     return self.feature_contribution
-  
+
   def show_in_notebook(self):
     """
     Convenience method with similar interface to LIME.
 
     """
     self.plot()
     plt.show()
```

### Comparing `lemon_explainer-0.0.2/tests/test_explainer.py` & `lemon_explainer-0.0.3/tests/test_explainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from unittest import TestCase
 import numpy as np
 import pandas as pd
 from scipy.stats import ks_1samp, uniform, truncnorm
 from lemon import LemonExplainer
 from lemon.kernels import uniform_kernel, gaussian_kernel
 from sklearn.compose import make_column_selector, make_column_transformer
-from sklearn.datasets import load_iris, load_wine
+from sklearn.datasets import load_iris, load_wine, load_linnerud
 from sklearn.ensemble import RandomForestClassifier, HistGradientBoostingClassifier
+from sklearn.multioutput import MultiOutputRegressor
+from sklearn.linear_model import LinearRegression
 from sklearn.pipeline import make_pipeline
-from sklearn.preprocessing import OrdinalEncoder
+from sklearn.preprocessing import OrdinalEncoder, StandardScaler
 from scipy.special import gammainccinv
 from functools import partial
 
 
-# chosen by fair dice roll. 
+# chosen by fair dice roll.
 # guaranteed to be random.
 random_state = 4
 
 
 class TestExplainer(TestCase):
   def setUp(self):
     data = load_iris(as_frame=True)
@@ -32,15 +34,15 @@
     self.y = y
     self.clf = clf
 
   def test_sample_hypersphere_uniform(self):
     for dimensions in np.linspace(2, 50, 10).astype(int):
       for radius_max in np.linspace(0.25, 1.0, 10):
         X = np.array([
-          np.array([-1 for d in range(0, dimensions)]), 
+          np.array([-1 for d in range(0, dimensions)]),
           np.array([1 for d in range(0, dimensions)])
         ])
         explainer = LemonExplainer(X, radius_max=radius_max)
 
         sphere = explainer._sample_hypersphere(10000, dimensions)
         distances = np.linalg.norm(sphere, axis=1) / radius_max
 
@@ -49,193 +51,270 @@
         test = ks_1samp(distances * distances**(dimensions - 1), uniform.cdf)
         assert test.statistic < 0.05
 
   def test_sample_hypersphere_size(self):
     for dimensions in np.linspace(2, 50, 10).astype(int):
       for radius_max in np.linspace(0.25, 1.0, 10):
         X = np.array([
-          np.array([-1 for d in range(0, dimensions)]), 
+          np.array([-1 for d in range(0, dimensions)]),
           np.array([1 for d in range(0, dimensions)])
         ])
         explainer = LemonExplainer(X, radius_max=radius_max)
-        
+
         sphere = explainer._sample_hypersphere(10000, dimensions)
         distances = np.linalg.norm(sphere, axis=1)
 
         # All samples should fall strictly within the specified maximum radius
         assert np.isclose(radius_max, np.max(distances), rtol=1e-02)
         assert np.max(distances) < radius_max
 
   def test_sample_hypersphere_uniform_circle(self):
     for dimensions in np.linspace(2, 50, 10).astype(int):
       for radius_max in np.linspace(0.25, 1.0, 10):
         X = np.array([
-          np.array([-1 for d in range(0, dimensions)]), 
+          np.array([-1 for d in range(0, dimensions)]),
           np.array([1 for d in range(0, dimensions)])
         ])
         explainer = LemonExplainer(X, radius_max=radius_max)
-        
+
         sphere = explainer._sample_hypersphere(10000, dimensions)
         axis_aligned_variance = np.var(sphere, axis=0)
-        difference = np.abs(np.min(axis_aligned_variance) - np.max(axis_aligned_variance))
+        difference = np.abs(
+            np.min(axis_aligned_variance) -
+            np.max(axis_aligned_variance))
 
-        # All samples should have the same distribution in each direction (rotational symmetry)
+        # All samples should have the same distribution in each direction
+        # (rotational symmetry)
         assert difference < 1e-02
 
   def test_sample_hypersphere_gaussian_circle(self):
     for dimensions in np.linspace(2, 50, 10).astype(int):
       for radius_max in np.linspace(0.25, 1.0, 10):
         X = np.array([
-          np.array([-1 for d in range(0, dimensions)]), 
+          np.array([-1 for d in range(0, dimensions)]),
           np.array([1 for d in range(0, dimensions)])
         ])
         p = 0.99
-        kernel_width = 1 / (2*gammainccinv(dimensions / 2, (1 - p)))
+        kernel_width = 1 / (2 * gammainccinv(dimensions / 2, (1 - p)))
         kernel = lambda x: gaussian_kernel(x, kernel_width)
-        explainer = LemonExplainer(X, distance_kernel=kernel, radius_max=radius_max)
-        
+        explainer = LemonExplainer(
+            X, distance_kernel=kernel, radius_max=radius_max)
+
         sphere = explainer._sample_hypersphere(10000, dimensions)
         axis_aligned_variance = np.var(sphere, axis=0)
-        difference = np.abs(np.min(axis_aligned_variance) - np.max(axis_aligned_variance))
+        difference = np.abs(
+            np.min(axis_aligned_variance) -
+            np.max(axis_aligned_variance))
 
-        # All samples should have the same distribution in each direction (rotational symmetry)
+        # All samples should have the same distribution in each direction
+        # (rotational symmetry)
         assert difference < 1e-02
 
   def test_transform_uniform(self):
     for dimensions in np.linspace(2, 50, 10).astype(int):
       for radius_max in np.linspace(0.25, 1.0, 10):
         X = np.array([
-          np.array([-1 for d in range(0, dimensions)]), 
+          np.array([-1 for d in range(0, dimensions)]),
           np.array([1 for d in range(0, dimensions)])
         ])
         explainer = LemonExplainer(X, radius_max=radius_max)
         kernel = uniform_kernel
-        sampling_kernel = explainer._transform(kernel, dimensions, 5000, radius_max, adjust=False)
+        sampling_kernel = explainer._transform(
+            kernel, dimensions, 5000, radius_max, adjust=False)
 
         samples = sampling_kernel(np.random.uniform(size=50000)) / radius_max
 
         # Samples should be uniformly distributed
         test = ks_1samp(samples, uniform.cdf)
         assert test.statistic < 0.05
 
   def test_transform_normal(self):
     for dimensions in np.linspace(2, 50, 10).astype(int):
       for radius_max in np.linspace(0.25, 1.0, 10):
         X = np.array([
-          np.array([-1 for d in range(0, dimensions)]), 
+          np.array([-1 for d in range(0, dimensions)]),
           np.array([1 for d in range(0, dimensions)])
         ])
         explainer = LemonExplainer(X, radius_max=radius_max)
-        
+
         p = 0.99
-        kernel_width = 1 / (2*gammainccinv(dimensions / 2, (1 - p)))
+        kernel_width = 1 / (2 * gammainccinv(dimensions / 2, (1 - p)))
         kernel = lambda x: gaussian_kernel(x, kernel_width=kernel_width)
 
-        sampling_kernel = explainer._transform(kernel, dimensions, 5000, radius_max, adjust=False)
+        sampling_kernel = explainer._transform(
+            kernel, dimensions, 5000, radius_max, adjust=False)
         samples = sampling_kernel(np.random.uniform(size=50000)) / radius_max
-        
+
         # Samples should be (truncated)normally distributed
-        cdf = partial(truncnorm.cdf, a=0, b=1/(kernel_width / radius_max), scale=kernel_width / radius_max)
+        cdf = partial(truncnorm.cdf, a=0, b=1 / (kernel_width /
+                      radius_max), scale=kernel_width / radius_max)
         test = ks_1samp(samples, cdf)
         assert test.statistic < 0.05
 
   def test_explain_instance(self):
     explainer = LemonExplainer(self.X, random_state=random_state)
 
     rf_fi = self.clf.feature_importances_
 
     lemon_fi = np.mean([
-      explainer.explain_instance(instance, self.clf.predict_proba)[0].feature_contribution
+      explainer.explain_instance(instance, self.clf.predict_proba)[
+          0].feature_contribution
       for _, instance in self.X.iterrows()
     ], axis=0)
     lemon_fi /= np.sum(np.abs(lemon_fi))
     lemon_fi = np.abs(lemon_fi)
 
-    # Mean important features should be roughly proportional to random forest feature importance
-    assert(np.array_equal(np.argsort(rf_fi), np.argsort(lemon_fi)))
+    # Mean important features should be roughly proportional to random forest
+    # feature importance
+    assert (np.array_equal(np.argsort(rf_fi), np.argsort(lemon_fi)))
 
   def test_explain_instance_scaling_invariant(self):
     # Unscaled
     explainer = LemonExplainer(self.X, random_state=random_state)
 
     lemon_fi = np.mean([
-      explainer.explain_instance(instance, self.clf.predict_proba)[0].feature_contribution
+      explainer.explain_instance(instance, self.clf.predict_proba)[
+          0].feature_contribution
       for _, instance in self.X.iterrows()
     ], axis=0)
     lemon_fi /= np.sum(np.abs(lemon_fi))
     lemon_fi = np.abs(lemon_fi)
-    
+
     # Scaled
     data = load_iris(as_frame=True)
     X_scaled = data.data
     X_scaled.loc[:, 'petal width (cm)'] *= 1000
     y = pd.Series(np.array(data.target_names)[data.target])
     y.name = "Class"
 
     clf_scaled = RandomForestClassifier(random_state=random_state)
     clf_scaled.fit(X_scaled, y)
     explainer_scaled = LemonExplainer(X_scaled, random_state=random_state)
 
     lemon_fi_scaled = np.mean([
-      explainer_scaled.explain_instance(instance, clf_scaled.predict_proba)[0].feature_contribution
+      explainer_scaled.explain_instance(instance, clf_scaled.predict_proba)[
+          0].feature_contribution
       for _, instance in X_scaled.iterrows()
     ], axis=0)
     lemon_fi_scaled /= np.sum(np.abs(lemon_fi_scaled))
     lemon_fi_scaled = np.abs(lemon_fi_scaled)
 
-    # Scaling features should have have no effect on which feature is most important
+    # Scaling features should have have no effect on which feature is most
+    # important
     assert np.allclose(lemon_fi, lemon_fi_scaled, rtol=0.01, atol=0.01)
 
   def test_explain_instance_plot(self):
     explainer = LemonExplainer(self.X, random_state=random_state)
 
     instance = self.X.iloc[-1, :]
     exp = explainer.explain_instance(instance, self.clf.predict_proba)[0]
 
     exp.show_in_notebook()
 
+
 class TestExplainerCategorical(TestCase):
   def setUp(self):
     data = load_wine(as_frame=True)
     X = data.data
     X.loc[:, 'ash'] = pd.cut(X.loc[:, 'ash'], 4)
     y = pd.Series(np.array(data.target_names)[data.target])
     y.name = "Class"
 
     self.categorical_features = [2]
     ordinal_encoder = make_column_transformer(
       (
-        OrdinalEncoder(handle_unknown="use_encoded_value", unknown_value=np.nan),
+        OrdinalEncoder(
+            handle_unknown="use_encoded_value",
+            unknown_value=np.nan),
         make_column_selector(dtype_include="category"),
       ),
       remainder="passthrough",
       verbose_feature_names_out=False,
     )
 
     clf = make_pipeline(
-      ordinal_encoder, HistGradientBoostingClassifier(categorical_features=self.categorical_features, random_state=random_state)
+      ordinal_encoder, HistGradientBoostingClassifier(
+          categorical_features=self.categorical_features, random_state=random_state)
     )
     clf.fit(X, y)
 
     self.X = X
     self.y = y
     self.clf = clf
 
   def test_explain_instance_plot(self):
-    explainer = LemonExplainer(self.X, radius_max=0.5, categorical_features=self.categorical_features, random_state=random_state)
+    explainer = LemonExplainer(
+        self.X,
+        radius_max=0.5,
+        categorical_features=self.categorical_features,
+        random_state=random_state)
 
     instance = self.X.iloc[120, :]
     exp = explainer.explain_instance(instance, self.clf.predict_proba)[0]
 
     exp.show_in_notebook()
 
   def test_explain_instance_without_training_data(self):
     stats = {
-      column: dict(zip(*np.unique(self.X[column], return_counts=True))) if i in self.categorical_features else self.X[column].std(ddof=0)
+      column: dict(
+          zip(
+              *
+              np.unique(
+                  self.X[column],
+                  return_counts=True))) if i in self.categorical_features else self.X[column].std(
+        ddof=0)
       for i, column in enumerate(self.X.columns)
-    } 
-    explainer = LemonExplainer(training_data_stats=stats, radius_max=0.5, categorical_features=self.categorical_features, random_state=random_state)
+    }
+    explainer = LemonExplainer(
+        training_data_stats=stats,
+        radius_max=0.5,
+        categorical_features=self.categorical_features,
+        random_state=random_state)
 
     instance = self.X.iloc[120, :]
     exp = explainer.explain_instance(instance, self.clf.predict_proba)[0]
 
-    exp.show_in_notebook()
+    exp.show_in_notebook()
+
+
+class TestExplainerRegression(TestCase):
+  def setUp(self):
+    data = load_linnerud(as_frame=True)
+    X = data.data
+    y = data.target
+    y.name = "Target"
+
+    regr = make_pipeline(
+        StandardScaler(),
+        MultiOutputRegressor(
+            LinearRegression()))
+    regr.fit(X, y)
+
+    self.X = X
+    self.y = y
+    self.regr = regr
+
+  def test_explain_instance_plot(self):
+    explainer = LemonExplainer(
+        self.X,
+        radius_max=0.5,
+        random_state=random_state)
+
+    instance = self.X.iloc[10, :]
+    exp = explainer.explain_instance(instance, self.regr.predict)[0]
+
+    exp.show_in_notebook()
+
+  def test_explain_instance_without_training_data(self):
+    stats = {
+      column: self.X[column].std(ddof=0)
+      for i, column in enumerate(self.X.columns)
+    }
+    explainer = LemonExplainer(
+        training_data_stats=stats,
+        radius_max=0.5,
+        random_state=random_state)
+
+    instance = self.X.iloc[10, :]
+    exp = explainer.explain_instance(instance, self.regr.predict)[0]
+
+    exp.show_in_notebook()
```

### Comparing `lemon_explainer-0.0.2/.gitignore` & `lemon_explainer-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lemon_explainer-0.0.2/LICENSE` & `lemon_explainer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon_explainer-0.0.2/README.md` & `lemon_explainer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lemon_explainer-0.0.2/pyproject.toml` & `lemon_explainer-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemon-explainer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Dennis Collaris", email="d.collaris@me.com" },
 ]
 description = "Explaining the predictions of any machine learning model"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "BSD-2-Clause"
@@ -24,8 +24,11 @@
 dependencies = [
     "numpy",
     "pandas",
     "matplotlib"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/iamDecode/lemon"
+"Homepage" = "https://github.com/iamDecode/lemon"
+
+[tool.hatch.build.targets.wheel]
+packages = ["lemon"]
```

### Comparing `lemon_explainer-0.0.2/PKG-INFO` & `lemon_explainer-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lemon-explainer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Explaining the predictions of any machine learning model
 Project-URL: Homepage, https://github.com/iamDecode/lemon
 Author-email: Dennis Collaris <d.collaris@me.com>
 License-Expression: BSD-2-Clause
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

