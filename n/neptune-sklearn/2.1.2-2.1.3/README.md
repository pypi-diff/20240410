# Comparing `tmp/neptune_sklearn-2.1.2.tar.gz` & `tmp/neptune_sklearn-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_sklearn-2.1.2.tar", max compression
+gzip compressed data, was "neptune_sklearn-2.1.3.tar", max compression
```

## Comparing `neptune_sklearn-2.1.2.tar` & `neptune_sklearn-2.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1352 2024-01-28 17:43:08.891642 neptune_sklearn-2.1.2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-01-28 17:43:08.891642 neptune_sklearn-2.1.2/LICENSE
--rw-r--r--   0        0        0     2626 2024-01-28 17:43:08.891642 neptune_sklearn-2.1.2/README.md
--rw-r--r--   0        0        0     2642 2024-01-28 17:43:17.459645 neptune_sklearn-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     2299 2024-01-28 17:43:08.895642 neptune_sklearn-2.1.2/src/neptune_sklearn/__init__.py
--rw-r--r--   0        0        0    38399 2024-01-28 17:43:08.895642 neptune_sklearn-2.1.2/src/neptune_sklearn/impl/__init__.py
--rw-r--r--   0        0        0      736 2024-01-28 17:43:08.895642 neptune_sklearn-2.1.2/src/neptune_sklearn/impl/version.py
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 neptune_sklearn-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1859 2024-04-10 09:04:02.434693 neptune_sklearn-2.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-10 09:04:02.434693 neptune_sklearn-2.1.3/LICENSE
+-rw-r--r--   0        0        0     2626 2024-04-10 09:04:02.434693 neptune_sklearn-2.1.3/README.md
+-rw-r--r--   0        0        0     2642 2024-04-10 09:04:13.802713 neptune_sklearn-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2299 2024-04-10 09:04:02.434693 neptune_sklearn-2.1.3/src/neptune_sklearn/__init__.py
+-rw-r--r--   0        0        0    39385 2024-04-10 09:04:02.434693 neptune_sklearn-2.1.3/src/neptune_sklearn/impl/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-10 09:04:02.434693 neptune_sklearn-2.1.3/src/neptune_sklearn/impl/version.py
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 neptune_sklearn-2.1.3/PKG-INFO
```

### Comparing `neptune_sklearn-2.1.2/CHANGELOG.md` & `neptune_sklearn-2.1.3/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## neptune-sklearn 2.1.3
+
+### Fixes
+- Monkey patches [`yellowbrick.regression.CooksDistance.draw()`](https://github.com/DistrictDataLabs/yellowbrick/blob/f7a8e950bd31452ea2f5d402a1c5d519cd163fd5/yellowbrick/regressor/influence.py#L184) to remove unsupported `use_line_collection` matplotlib arg ([#28](https://github.com/neptune-ai/neptune-sklearn/pull/28))
+
+### Changes
+- Replaced `print()` with `warnings.warn()` to better capture `stderr`  ([#28](https://github.com/neptune-ai/neptune-sklearn/pull/28))
+
 ## neptune-sklearn 2.1.2
 
 ### Changes
 - Constraining scipy to `<1.12` ([#25](https://github.com/neptune-ai/neptune-sklearn/pull/25))
 
 ## neptune-sklearn 2.1.1
```

### Comparing `neptune_sklearn-2.1.2/LICENSE` & `neptune_sklearn-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_sklearn-2.1.2/README.md` & `neptune_sklearn-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `neptune_sklearn-2.1.2/pyproject.toml` & `neptune_sklearn-2.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 repository = "https://github.com/neptune-ai/neptune-sklearn"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/sklearn"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-sklearn"
 readme = "README.md"
-version = "2.1.2"
+version = "2.1.3"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_sklearn-2.1.2/src/neptune_sklearn/__init__.py` & `neptune_sklearn-2.1.3/src/neptune_sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_sklearn-2.1.2/src/neptune_sklearn/impl/__init__.py` & `neptune_sklearn-2.1.3/src/neptune_sklearn/impl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 except ImportError:
     from neptune.new.types import (
         File,
         FileSeries,
     )
     from neptune.new.utils import stringify_unsupported
 
+from warnings import warn
+
 
 def create_regressor_summary(regressor, X_train, X_test, y_train, y_test, nrows=1000, log_charts=True):
     """Creates scikit-learn regressor summary.
 
     The summary includes:
 
     - all regressor parameters,
@@ -451,15 +453,15 @@
     if X_test is None and y_pred_proba is None:
         raise ValueError("X_test or y_pred_proba is required")
 
     if y_pred_proba is None:
         try:
             y_pred_proba = classifier.predict_proba(X_test)
         except Exception as e:
-            print("This classifier does not provide predictions probabilities. Error: {}".format(e))
+            warn(f"This classifier does not provide predictions probabilities. Error: {e}")
             return
 
     df = pd.DataFrame(data=y_pred_proba, columns=classifier.classes_)
     df = df.head(n=nrows)
 
     return File.as_html(df)
 
@@ -586,15 +588,15 @@
     try:
         fig, ax = plt.subplots()
         plot_learning_curve(regressor, X_train, y_train, ax=ax)
 
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log learning curve chart. Error: {}".format(e))
+        warn(f"Did not log learning curve chart. Error: {e}")
 
     return chart
 
 
 def create_feature_importance_chart(regressor, X_train, y_train):
     """Creates feature importance chart.
 
@@ -629,15 +631,15 @@
         visualizer = FeatureImportances(regressor, is_fitted=True, ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.finalize()
 
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log feature importance chart. Error: {}".format(e))
+        warn(f"Did not log feature importance chart. Error: {e}")
 
     return chart
 
 
 def create_residuals_chart(regressor, X_train, X_test, y_train, y_test):
     """Creates residuals chart.
 
@@ -674,15 +676,15 @@
         visualizer = ResidualsPlot(regressor, is_fitted=True, ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.score(X_test, y_test)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log residuals chart. Error: {}".format(e))
+        warn(f"Did not log residuals chart. Error: {e}")
 
     return chart
 
 
 def create_prediction_error_chart(regressor, X_train, X_test, y_train, y_test):
     """Creates prediction error chart.
 
@@ -719,19 +721,55 @@
         visualizer = PredictionError(regressor, is_fitted=True, ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.score(X_test, y_test)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log prediction error chart. Error: {}".format(e))
+        warn(f"Did not log prediction error chart. Error: {e}")
 
     return chart
 
 
+def _monkey_draw(self):
+    """
+    Monkey patches `yellowbrick.regressor.CooksDistance.draw()`
+    to remove unsupported matplotlib argument `use_line_collection`.
+
+    Draws a stem plot where each stem is the Cook's Distance of the instance at the
+    index specified by the x axis. Optionaly draws a threshold line.
+    """
+    # Draw a stem plot with the influence for each instance
+    _, _, baseline = self.ax.stem(
+        self.distance_,
+        linefmt=self.linefmt,
+        markerfmt=self.markerfmt,
+        # use_line_collection=True
+    )
+
+    # No padding on either side of the instance index
+    self.ax.set_xlim(0, len(self.distance_))
+
+    # Draw the threshold for most influential points
+    if self.draw_threshold:
+        label = r"{:0.2f}% > $I_t$ ($I_t=\frac {{4}} {{n}}$)".format(self.outlier_percentage_)
+        self.ax.axhline(
+            self.influence_threshold_,
+            ls="--",
+            label=label,
+            c=baseline.get_color(),
+            lw=baseline.get_linewidth(),
+        )
+
+    return self.ax
+
+
+CooksDistance.draw = _monkey_draw
+
+
 def create_cooks_distance_chart(regressor, X_train, y_train):
     """Creates cooks distance chart.
 
     Args:
         regressor (`regressor`): Fitted sklearn regressor object
         X_train (`ndarray`): Training data matrix
         y_train (`ndarray`): The regression target for training
@@ -761,15 +799,15 @@
         fig, ax = plt.subplots()
         visualizer = CooksDistance(ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log cooks distance chart. Error: {}".format(e))
+        warn(f"Did not log cooks distance chart. Error: {e}")
 
     return chart
 
 
 def create_classification_report_chart(classifier, X_train, X_test, y_train, y_test):
     """Creates classification report chart.
 
@@ -808,15 +846,15 @@
         visualizer = ClassificationReport(classifier, support=True, is_fitted=True, ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.score(X_test, y_test)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log Classification Report chart. Error: {}".format(e))
+        warn(f"Did not log Classification Report chart. Error: {e}")
 
     return chart
 
 
 def create_confusion_matrix_chart(classifier, X_train, X_test, y_train, y_test):
     """Creates confusion matrix.
 
@@ -855,15 +893,15 @@
         visualizer = ConfusionMatrix(classifier, is_fitted=True, ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.score(X_test, y_test)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log Confusion Matrix chart. Error: {}".format(e))
+        warn(f"Did not log Confusion Matrix chart. Error: {e}")
 
     return chart
 
 
 def create_roc_auc_chart(classifier, X_train, X_test, y_train, y_test):
     """Creates ROC-AUC chart.
 
@@ -900,15 +938,15 @@
         visualizer = ROCAUC(classifier, is_fitted=True, ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.score(X_test, y_test)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log ROC-AUC chart. Error {}".format(e))
+        warn(f"Did not log ROC-AUC chart. Error {e}")
 
     return chart
 
 
 def create_precision_recall_chart(classifier, X_test, y_test, y_pred_proba=None):
     """Creates precision-recall chart.
 
@@ -939,27 +977,27 @@
 
     chart = None
 
     if y_pred_proba is None:
         try:
             y_pred_proba = classifier.predict_proba(X_test)
         except Exception as e:
-            print(
-                "Did not log Precision-Recall chart: this classifier does not provide predictions probabilities."
-                "Error {}".format(e)
+            warn(
+                f"""Did not log Precision-Recall chart: this classifier does not provide predictions probabilities.
+                Error {e}"""
             )
             return chart
 
     try:
         fig, ax = plt.subplots()
         plot_precision_recall(y_test, y_pred_proba, ax=ax)
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log Precision-Recall chart. Error {}".format(e))
+        warn(f"Did not log Precision-Recall chart. Error {e}")
 
     return chart
 
 
 def create_class_prediction_error_chart(classifier, X_train, X_test, y_train, y_test):
     """Creates class prediction error chart.
 
@@ -998,15 +1036,15 @@
         visualizer = ClassPredictionError(classifier, is_fitted=True, ax=ax)
         visualizer.fit(X_train, y_train)
         visualizer.score(X_test, y_test)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log Class Prediction Error chart. Error {}".format(e))
+        warn(f"Did not log Class Prediction Error chart. Error {e}")
 
     return chart
 
 
 def get_cluster_labels(model, X, nrows=1000, **kwargs):
     """Logs the index of the cluster label each sample belongs to.
 
@@ -1084,15 +1122,15 @@
         fig, ax = plt.subplots()
         visualizer = KElbowVisualizer(model, k=k, ax=ax)
         visualizer.fit(X)
         visualizer.finalize()
         chart = File.as_image(fig)
         plt.close(fig)
     except Exception as e:
-        print("Did not log KMeans elbow chart. Error {}".format(e))
+        warn(f"Did not log KMeans elbow chart. Error {e}")
 
     return chart
 
 
 def create_silhouette_chart(model, X, **kwargs):
     """Creates silhouette coefficients charts for KMeans clusterer.
 
@@ -1136,10 +1174,10 @@
             fig, ax = plt.subplots()
             visualizer = SilhouetteVisualizer(model, is_fitted=True, ax=ax)
             visualizer.fit(X)
             visualizer.finalize()
             charts.append(File.as_image(fig))
             plt.close(fig)
         except Exception as e:
-            print("Did not log Silhouette Coefficients chart. Error {}".format(e))
+            warn(f"Did not log Silhouette Coefficients chart. Error {e}")
 
     return FileSeries(charts)
```

### Comparing `neptune_sklearn-2.1.2/src/neptune_sklearn/impl/version.py` & `neptune_sklearn-2.1.3/src/neptune_sklearn/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_sklearn-2.1.2/PKG-INFO` & `neptune_sklearn-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-sklearn
-Version: 2.1.2
+Version: 2.1.3
 Summary: Neptune.ai scikit-learn integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

