# Comparing `tmp/polars_ols-0.2.6.tar.gz` & `tmp/polars_ols-0.2.8.tar.gz`

## Comparing `polars_ols-0.2.6.tar` & `polars_ols-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 polars_ols-0.2.6/Cargo.toml
--rw-r--r--   0     1001      127      116 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.cargo/config.toml
--rw-r--r--   0     1001      127     4460 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      139 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.gitignore
--rw-r--r--   0     1001      127      912 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1067 2024-04-09 18:13:33.000000 polars_ols-0.2.6/LICENSE
--rw-r--r--   0     1001      127      671 2024-04-09 18:13:33.000000 polars_ols-0.2.6/Makefile
--rw-r--r--   0     1001      127    15333 2024-04-09 18:13:33.000000 polars_ols-0.2.6/README.md
--rw-r--r--   0     1001      127    44513 2024-04-09 18:13:33.000000 polars_ols-0.2.6/notebooks/polars_ols_demo.ipynb
--rw-r--r--   0     1001      127     4486 2024-04-09 18:13:33.000000 polars_ols-0.2.6/polars_ols/__init__.py
--rw-r--r--   0     1001      127    15997 2024-04-09 18:13:33.000000 polars_ols-0.2.6/polars_ols/least_squares.py
--rw-r--r--   0     1001      127     3464 2024-04-09 18:13:33.000000 polars_ols-0.2.6/polars_ols/utils.py
--rw-r--r--   0     1001      127       63 2024-04-09 18:13:33.000000 polars_ols-0.2.6/requirements.txt
--rw-r--r--   0     1001      127    14543 2024-04-09 18:13:33.000000 polars_ols-0.2.6/src/expressions.rs
--rw-r--r--   0     1001      127    20829 2024-04-09 18:13:33.000000 polars_ols-0.2.6/src/least_squares.rs
--rw-r--r--   0     1001      127     5579 2024-04-09 18:13:33.000000 polars_ols-0.2.6/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/__init__.py
--rw-r--r--   0     1001      127     7984 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/benchmark.py
--rw-r--r--   0     1001      127       87 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/requirements-test.txt
--rw-r--r--   0     1001      127    25397 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/test_ols.py
--rw-r--r--   0     1001      127    61832 2024-04-09 18:13:33.000000 polars_ols-0.2.6/Cargo.lock
--rw-r--r--   0     1001      127     1865 2024-04-09 18:13:33.000000 polars_ols-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    16041 1970-01-01 00:00:00.000000 polars_ols-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 polars_ols-0.2.8/Cargo.toml
+-rw-r--r--   0     1001      127      116 2024-04-10 11:35:06.000000 polars_ols-0.2.8/.cargo/config.toml
+-rw-r--r--   0     1001      127     4460 2024-04-10 11:35:06.000000 polars_ols-0.2.8/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      139 2024-04-10 11:35:06.000000 polars_ols-0.2.8/.gitignore
+-rw-r--r--   0     1001      127      912 2024-04-10 11:35:06.000000 polars_ols-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1067 2024-04-10 11:35:06.000000 polars_ols-0.2.8/LICENSE
+-rw-r--r--   0     1001      127      671 2024-04-10 11:35:06.000000 polars_ols-0.2.8/Makefile
+-rw-r--r--   0     1001      127    15333 2024-04-10 11:35:06.000000 polars_ols-0.2.8/README.md
+-rw-r--r--   0     1001      127    44513 2024-04-10 11:35:06.000000 polars_ols-0.2.8/notebooks/polars_ols_demo.ipynb
+-rw-r--r--   0     1001      127     4649 2024-04-10 11:35:06.000000 polars_ols-0.2.8/polars_ols/__init__.py
+-rw-r--r--   0     1001      127    16768 2024-04-10 11:35:06.000000 polars_ols-0.2.8/polars_ols/least_squares.py
+-rw-r--r--   0     1001      127     3464 2024-04-10 11:35:06.000000 polars_ols-0.2.8/polars_ols/utils.py
+-rw-r--r--   0     1001      127       63 2024-04-10 11:35:06.000000 polars_ols-0.2.8/requirements.txt
+-rw-r--r--   0     1001      127    17982 2024-04-10 11:35:06.000000 polars_ols-0.2.8/src/expressions.rs
+-rw-r--r--   0     1001      127    20841 2024-04-10 11:35:06.000000 polars_ols-0.2.8/src/least_squares.rs
+-rw-r--r--   0     1001      127     5579 2024-04-10 11:35:06.000000 polars_ols-0.2.8/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-10 11:35:06.000000 polars_ols-0.2.8/tests/__init__.py
+-rw-r--r--   0     1001      127     7984 2024-04-10 11:35:06.000000 polars_ols-0.2.8/tests/benchmark.py
+-rw-r--r--   0     1001      127       87 2024-04-10 11:35:06.000000 polars_ols-0.2.8/tests/requirements-test.txt
+-rw-r--r--   0     1001      127    26724 2024-04-10 11:35:06.000000 polars_ols-0.2.8/tests/test_ols.py
+-rw-r--r--   0     1001      127    61832 2024-04-10 11:35:06.000000 polars_ols-0.2.8/Cargo.lock
+-rw-r--r--   0     1001      127     1865 2024-04-10 11:35:06.000000 polars_ols-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    16041 1970-01-01 00:00:00.000000 polars_ols-0.2.8/PKG-INFO
```

### Comparing `polars_ols-0.2.6/Cargo.toml` & `polars_ols-0.2.8/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars_ols"
-version = "0.2.6"
+version = "0.2.8"
 edition = "2021"
 
 [lib]
 name = "polars_ols"
 crate-type= ["cdylib"]
 
 [dependencies]
```

### Comparing `polars_ols-0.2.6/.github/workflows/publish_to_pypi.yml` & `polars_ols-0.2.8/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/.pre-commit-config.yaml` & `polars_ols-0.2.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/LICENSE` & `polars_ols-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/Makefile` & `polars_ols-0.2.8/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/README.md` & `polars_ols-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/notebooks/polars_ols_demo.ipynb` & `polars_ols-0.2.8/notebooks/polars_ols_demo.ipynb`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/polars_ols/__init__.py` & `polars_ols-0.2.8/polars_ols/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,17 +112,27 @@
             return self.rls(*features, add_intercept=add_intercept, **kwargs)
         elif kwargs.get("window_size"):
             return self.rolling_ols(*features, add_intercept=add_intercept, **kwargs)
         else:
             return self.least_squares(*features, add_intercept=add_intercept, **kwargs)
 
     def predict(
-        self, *features: pl.Expr, name: Optional[str] = None, add_intercept: bool = False
+        self,
+        *features: pl.Expr,
+        name: Optional[str] = None,
+        add_intercept: bool = False,
+        null_policy: NullPolicy = "zero",
     ) -> pl.Expr:
-        return predict(self._expr, *features, add_intercept=add_intercept, name=name)
+        return predict(
+            self._expr,
+            *features,
+            add_intercept=add_intercept,
+            name=name,
+            null_policy=null_policy,
+        )
 
     def predict_from_formula(self, formula: str, name: Optional[str] = None) -> pl.Expr:
         features, add_intercept = build_expressions_from_patsy_formula(
             formula, include_dependent_variable=False
         )
         has_const = any(f.meta.output_name == "const" for f in features)
         add_intercept &= not has_const
```

### Comparing `polars_ols-0.2.6/polars_ols/least_squares.py` & `polars_ols-0.2.8/polars_ols/least_squares.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,22 @@
     "RollingKwargs",
     # types controlling general modelling behaviour
     "NullPolicy",
     "OutputMode",
     "SolveMethod",
 ]
 
-NullPolicy = Literal["zero", "drop", "drop_y_zero_x", "ignore"]
+NullPolicy = Literal[
+    "zero",  # simply zero fills nulls in both targets & features
+    "drop",  # drops any rows with nulls in fitting and masks associated predictions with nulls
+    "ignore",  # use this option if nulls are already handled upstream
+    "drop_zero",  # drops any rows with nulls in fitting, but then computes predictions
+    # with zero filled features. Use this to allow for extrapolation.
+    "drop_y_zero_x",  # only drops rows with null targets and fill any null features with zero
+]
 OutputMode = Literal["predictions", "residuals", "coefficients"]
 SolveMethod = Literal["qr", "svd", "chol", "lu", "cd"]
 
 _VALID_NULL_POLICIES: Set[NullPolicy] = set(get_args(NullPolicy))
 _VALID_OUTPUT_MODES: Set[OutputMode] = set(get_args(OutputMode))
 _VALID_SOLVE_METHODS: Set[SolveMethod] = set(get_args(SolveMethod)).union({None})
 
@@ -60,16 +67,17 @@
         alpha: Regularization strength. Defaults to 0.0.
         l1_ratio: Mixing parameter for ElasticNet regularization (0 for Ridge, 1 for LASSO).
             Defaults to None (equivalent to Ridge regression).
         max_iter: Maximum number of iterations. Defaults to 1000 iterations.
         tol: Tolerance for convergence criterion. Defaults to 1.e-5.
         positive: Whether to enforce non-negativity constraints on coefficients.
             Defaults to False (no constraint on coefficients).
-        null_policy: Strategy for handling missing data ("zero", "drop", "ignore", "drop_y_zero_x").
-            Defaults to None, where a recommended default algorithm is chosen based on problem
+        null_policy: Strategy for handling missing data. Defaults to "ignore".
+        solve_method: Algorithm used for computing least squares solution.
+            Defaults to None, where a recommended default method is chosen based on problem
             specifics.
     """
 
     alpha: Optional[float] = 0.0
     l1_ratio: Optional[float] = None
     max_iter: Optional[int] = 1_000
     tol: Optional[float] = 1.0e-5
@@ -98,15 +106,15 @@
         half_life: Half-life parameter for exponential forgetting. Defaults to None
             (no forgetting).
         initial_state_covariance: Scalar representing which behaves like an L2 regularization
                                   parameter. Larger values correspond to larger prior uncertainty
                                   around mean vector of state (inversely proportional to strength
                                   of equivalent L2 penalty). Defaults to 10.
         initial_state_mean: Initial mean vector of the state. Defaults to None.
-        null_policy: Strategy for handling missing data ("zero", "drop", "ignore", "drop_y_zero_x").
+        null_policy: Strategy for handling missing data. Defaults to "ignore".
     """
 
     half_life: Optional[float] = None
     initial_state_covariance: Optional[float] = 10.0
     initial_state_mean: Union[Optional[List[float], float]] = None
     null_policy: NullPolicy = "ignore"
 
@@ -120,15 +128,15 @@
 
     Attributes:
         window_size: The size of the rolling window.
         min_periods: The minimum number of observations required to produce estimates.
         use_woodbury: Whether to use Woodbury matrix identity for faster computation.
                       Defaults to True if num_features > 10.
         alpha: L2 Regularization strength. Default is 0.0.
-        null_policy: Strategy for handling missing data ("zero", "drop", "drop_y_zero_x", "ignore").
+        null_policy: Strategy for handling missing data. Defaults to "ignore".
     """
 
     window_size: int = 1_000_000  # defaults to expanding OLS
     min_periods: Optional[int] = None
     use_woodbury: Optional[bool] = None
     alpha: Optional[float] = None  # optional ridge alpha
     null_policy: NullPolicy = "ignore"
@@ -151,15 +159,15 @@
         *features: Variable number of feature expressions.
         sample_weights: Optional expression representing sample weights.
         add_intercept: Whether to add an intercept column.
 
     Returns:
         Tuple containing the pre-processed target, features, and sample weights.
     """
-    target = parse_into_expr(target)
+    target = parse_into_expr(target).cast(pl.Float32)
     features = [f.cast(pl.Float32) for f in features]
     # handle intercept
     if add_intercept:
         if any(f.meta.output_name == "const" for f in features):
             logger.info("feature named 'const' already detected, assuming it is an intercept")
         else:
             features.append(target.fill_null(0.0).mul(0.0).add(1.0).alias("const").cast(pl.Float32))
@@ -231,15 +239,15 @@
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
-            return target - predictions
+            return target / sqrt_w - predictions
 
 
 def compute_recursive_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
@@ -295,15 +303,15 @@
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
-            return target - predictions
+            return target / sqrt_w - predictions
 
 
 def compute_rolling_least_squares(
     target: IntoExpr,
     *features: pl.Expr,
     sample_weights: Optional[pl.Expr] = None,
     add_intercept: bool = False,
@@ -356,15 +364,15 @@
                 is_elementwise=False,
             )
             / sqrt_w
         )  # undo the sqrt(w) scaling implicit in predictions
         if mode == "predictions":
             return predictions
         else:
-            return target - predictions
+            return target / sqrt_w - predictions
 
 
 def compute_least_squares_from_formula(
     formula: str,
     sample_weights: Optional[pl.Expr] = None,
     mode: OutputMode = "predictions",
     **kwargs,
@@ -406,33 +414,37 @@
         mode=mode,
     )
 
 
 def predict(
     coefficients: IntoExpr,
     *features: pl.Expr,
+    null_policy: NullPolicy = "zero",
     add_intercept: bool = False,
     name: Optional[str] = None,
 ) -> pl.Expr:
     """Helper which computes predictions as a product of (aligned) coefficients with features.
 
     Args:
         coefficients: Polars expression returning a coefficients struct.
         *features: variable number of feature expressions.
+        null_policy: specifies how nulls in features are handled. Defaults to zero filling.
         add_intercept: boolean indicating if a constant should be added to features.
         name: optional str defining an alias for computed predictions expression.
 
     Returns:
         polars expression denoting computed predictions.
     """
+    assert null_policy in _VALID_NULL_POLICIES, "'null_policy' must be one of {drop, ignore, zero}"
     if add_intercept:
         if any(f.meta.output_name == "const" for f in features):
             logger.warning("feature named 'const' already detected, assuming it is the intercept")
         else:
             features += (features[-1].fill_null(0.0).mul(0.0).add(1.0).alias("const"),)
 
     return register_plugin_function(
         plugin_path=Path(__file__).parent,
         function_name="predict",
         args=[coefficients, *(f.cast(pl.Float32) for f in features)],
+        kwargs={"null_policy": null_policy},
         is_elementwise=False,
     ).alias(name or "predictions")
```

### Comparing `polars_ols-0.2.6/polars_ols/utils.py` & `polars_ols-0.2.8/polars_ols/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/src/expressions.rs` & `polars_ols-0.2.8/src/expressions.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #![allow(clippy::unit_arg, clippy::unused_unit)]
 
 use ndarray::{Array, Array1, Array2, Axis};
 use polars::datatypes::{DataType, Field, Float32Type};
 use polars::error::{polars_err, PolarsResult};
 use polars::frame::DataFrame;
-use polars::prelude::{FillNullStrategy, IndexOrder, IntoSeries, NamedFromOwned, Series};
+use polars::prelude::{
+    BooleanChunked, FillNullStrategy, IndexOrder, IntoSeries, NamedFrom, NamedFromOwned, Series,
+};
 use pyo3_polars::derive::polars_expr;
 use serde::Deserialize;
 use std::str::FromStr;
 
 use crate::least_squares::{
     solve_elastic_net, solve_ols, solve_recursive_least_squares, solve_ridge, solve_rolling_ols,
     SolveMethod,
@@ -45,21 +47,22 @@
     x
 }
 
 /// Convert a slice of polars series into target & feature ndarray objects.
 pub fn convert_polars_to_ndarray(
     inputs: &[Series],
     null_policy: &NullPolicy,
+    is_valid: Option<&BooleanChunked>,
 ) -> (Array1<f32>, Array2<f32>) {
     let m = inputs.len();
     assert!(m > 1, "must pass at least 2 series");
 
     // handle nulls according to the specified null policy
     let mut filtered_inputs = Vec::new();
-    handle_nulls(inputs, null_policy, &mut filtered_inputs);
+    handle_nulls(inputs, null_policy, is_valid, &mut filtered_inputs);
 
     // prepare targets & features ndarrays. assume first series is targets and rest are features.
     let y = filtered_inputs[0]
         .f32()
         .expect("Failed to convert polars series to f32 array")
         .to_ndarray()
         .expect("Failed to convert f32 series to ndarray")
@@ -96,84 +99,145 @@
             .collect::<Vec<Series>>(),
     )
     .unwrap();
     // Convert DataFrame to a Series of struct dtype
     df.into_struct("coefficients").into_series()
 }
 
-/// Computes linear predictions and returns a polars series.
-fn make_predictions(features: &Array2<f32>, coefficients: &Array1<f32>, name: &str) -> Series {
-    Series::from_vec(name, features.dot(coefficients).to_vec())
+fn mask_predictions(predictions: Vec<f32>, is_valid_mask: &BooleanChunked) -> Vec<Option<f32>> {
+    is_valid_mask
+        .iter()
+        .zip(&predictions)
+        // apply validity mask to predictions
+        .map(|(valid, &prediction)| {
+            if valid.unwrap_or(false) {
+                Some(prediction)
+            } else {
+                None
+            }
+        })
+        .collect()
+}
+
+/// Computes linear predictions and returns a Polars series.
+///
+/// # Arguments
+/// * `features` - A 2D array representing the features.
+/// * `coefficients` - A 1D array representing the coefficients.
+/// * `is_valid_mask` - An optional BooleanChunked series representing the validity mask.
+/// * `name` - A string specifying the name of the resulting series.
+///
+/// # Returns
+/// A Polars Series containing the computed predictions.
+fn make_predictions(
+    features: &Array2<f32>,
+    coefficients: &Array1<f32>,
+    is_valid_mask: Option<&BooleanChunked>,
+    name: &str,
+) -> Series {
+    // compute dot product of (zero-filled) features with coefficients
+    let predictions = features.dot(coefficients).to_vec();
+    if let Some(is_valid) = is_valid_mask {
+        // is_valid mask has been passed: when true retain values and otherwise mask with None.
+        let masked_predictions: Vec<Option<f32>> = mask_predictions(predictions, is_valid);
+        Series::new(name, &masked_predictions)
+    } else {
+        // no mask is provided, return predictions as-is
+        Series::from_vec(name, predictions)
+    }
 }
 
 fn convert_option_vec_to_array1(opt_vec: Option<Vec<f32>>) -> Option<Array1<f32>> {
     opt_vec.map(Array1::from)
 }
 
 #[derive(Debug, PartialEq)]
 pub enum NullPolicy {
     Zero,
-    DropYZeroX,
     Drop,
     Ignore,
+    DropZero,
+    DropYZeroX,
 }
 
 impl FromStr for NullPolicy {
     type Err = ();
 
     fn from_str(input: &str) -> Result<NullPolicy, Self::Err> {
         match input {
             "zero" => Ok(NullPolicy::Zero),
             "drop" => Ok(NullPolicy::Drop),
             "ignore" => Ok(NullPolicy::Ignore),
             "drop_y_zero_x" => Ok(NullPolicy::DropYZeroX),
+            "drop_zero" => Ok(NullPolicy::DropZero),
             _ => Err(()),
         }
     }
 }
 
+fn compute_is_valid_mask(inputs: &[Series], null_policy: &NullPolicy) -> Option<BooleanChunked> {
+    match null_policy {
+        // Compute the intersection of all non-null rows across input series
+        NullPolicy::Drop | NullPolicy::DropZero => {
+            let is_valid_mask = inputs[0].is_not_null();
+            Some(
+                inputs[1..]
+                    .iter()
+                    .fold(is_valid_mask, |acc, s| acc & s.is_not_null()),
+            )
+        }
+        // Compute non-null mask based on the first input series (i.e. targets)
+        NullPolicy::DropYZeroX => Some(inputs[0].is_not_null()),
+        _ => None,
+    }
+}
+
 /// Handles null values in the input series based on the specified null policy.
 ///
 /// # Arguments
 ///
 /// * `inputs` - A slice of input series to be processed.
 /// * `null_policy` - The null handling policy to be applied.
+/// * `is_valid_mask` - A boolean array which specifies, based on the chosen null policy,
+///                     which row samples are valid.
 /// * `outputs` - A mutable reference to a vector of series where null values have been handled
 ///               according to the specified policy. If no null handling is required
 ///               (NullPolicy::Ignore), `outputs` will contain a reference to the original `inputs`
-fn handle_nulls(inputs: &[Series], null_policy: &NullPolicy, outputs: &mut Vec<Series>) {
+fn handle_nulls(
+    inputs: &[Series],
+    null_policy: &NullPolicy,
+    is_valid_mask: Option<&BooleanChunked>,
+    outputs: &mut Vec<Series>,
+) {
     match null_policy {
         NullPolicy::Zero => {
             // Zero out any nulls across all input series
             outputs.extend(
                 inputs
                     .iter()
                     .map(|s| s.fill_null(FillNullStrategy::Zero).unwrap()),
             );
         }
         NullPolicy::DropYZeroX => {
             // Compute non-null mask based on the first input series (i.e. targets)
-            let is_valid = inputs[0].is_not_null();
+            let is_valid_mask = is_valid_mask.unwrap();
             // Apply mask to all series, then additionally fill any remaining nulls with zero
             outputs.extend(inputs.iter().map(|s| {
-                s.filter(&is_valid)
+                s.filter(is_valid_mask)
                     .expect("Failed to filter input series with targets not-null mask!")
                     .fill_null(FillNullStrategy::Zero)
                     .unwrap()
             }));
         }
-        NullPolicy::Drop => {
+        NullPolicy::Drop | NullPolicy::DropZero => {
             // Compute the intersection of all non-null rows across input series
-            let is_valid = inputs[0].is_not_null();
-            let is_valid = inputs[1..]
-                .iter()
-                .fold(is_valid, |acc, s| acc & s.is_not_null());
+            let is_valid_mask = is_valid_mask.unwrap();
             // Apply mask to all input series
             outputs.extend(inputs.iter().map(|s| {
-                s.filter(&is_valid)
+                s.filter(is_valid_mask)
                     .expect("Failed to filter input series with common not-null mask!")
             }));
         }
         // For `Ignore`, simply assign inputs to outputs
         // this approach of working with references should avoid copying unnecessarily
         NullPolicy::Ignore => outputs.extend_from_slice(inputs),
     }
@@ -203,14 +267,19 @@
     window_size: usize,
     min_periods: Option<usize>,
     use_woodbury: Option<bool>,
     alpha: Option<f32>,
     null_policy: Option<String>,
 }
 
+#[derive(Deserialize)]
+pub struct PredictKwargs {
+    null_policy: Option<String>,
+}
+
 pub trait HasNullPolicy {
     fn get_null_policy(&self) -> NullPolicy;
 }
 
 macro_rules! impl_has_null_policy {
     ($($struct:ident),*) => {
         $(
@@ -220,15 +289,15 @@
                     .expect("Invalid null_policy detected!")).unwrap_or(NullPolicy::Ignore)
                 }
             }
         )*
     };
 }
 
-impl_has_null_policy!(OLSKwargs, RLSKwargs, RollingKwargs);
+impl_has_null_policy!(OLSKwargs, RLSKwargs, RollingKwargs, PredictKwargs);
 
 fn _get_least_squares_coefficients(
     targets: &Array1<f32>,
     features: &Array2<f32>,
     kwargs: OLSKwargs,
 ) -> Array1<f32> {
     let alpha = kwargs.alpha.unwrap_or(0.0);
@@ -259,36 +328,55 @@
         )
     }
 }
 
 #[polars_expr(output_type=Float32)]
 fn least_squares(inputs: &[Series], kwargs: OLSKwargs) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
-    let (y_fit, x_fit) = convert_polars_to_ndarray(inputs, &null_policy);
+    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let (y_fit, x_fit) = convert_polars_to_ndarray(inputs, &null_policy, is_valid.as_ref());
     let coefficients = _get_least_squares_coefficients(&y_fit, &x_fit, kwargs);
 
     if matches!(null_policy, NullPolicy::Ignore | NullPolicy::Zero) {
         // absent additional filtering: features for fitting is the same as for prediction
-        Ok(make_predictions(&x_fit, &coefficients, inputs[0].name()))
-    } else {
-        // ensure that predictions:
-        // 1. broadcast to the same shape as original inputs (no drop) &
-        // 2. always produce valid values in the presence of nulls (zero fill)
-        let x_predict = construct_features_array(&inputs[1..], true);
         Ok(make_predictions(
-            &x_predict,
+            &x_fit,
             &coefficients,
+            is_valid.as_ref(),
             inputs[0].name(),
         ))
+    } else {
+        // ensure that predictions broadcast to the same shape as original inputs (don't drop rows)
+        let x_predict = construct_features_array(&inputs[1..], true);
+        if null_policy == NullPolicy::Drop {
+            // if null policy is drop: mask invalid rows with is_valid BooleanChunked
+            Ok(make_predictions(
+                &x_predict,
+                &coefficients,
+                is_valid.as_ref(),
+                inputs[0].name(),
+            ))
+        } else {
+            // Otherwise always produce valid predictions as dot product of zero-filled features w/
+            // estimated coefficients.
+            Ok(make_predictions(
+                &x_predict,
+                &coefficients,
+                None,
+                inputs[0].name(),
+            ))
+        }
     }
 }
 
 #[polars_expr(output_type_func=coefficients_struct_dtype)]
 fn least_squares_coefficients(inputs: &[Series], kwargs: OLSKwargs) -> PolarsResult<Series> {
-    let (y, x) = convert_polars_to_ndarray(inputs, &kwargs.get_null_policy());
+    let null_policy = kwargs.get_null_policy();
+    let is_valid = compute_is_valid_mask(inputs, &null_policy);
+    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy, is_valid.as_ref());
     // force into 1 x K 2-d array, so that we can return a series of struct
     let coefficients = _get_least_squares_coefficients(&y, &x, kwargs).insert_axis(Axis(0));
     // let series = coefficients_to_series_list(&coefficients);
     let series = coefficients_to_struct_series(&coefficients);
     Ok(series.with_name("coefficients"))
 }
 
@@ -298,15 +386,15 @@
     kwargs: RLSKwargs,
 ) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
     assert!(
         matches!(null_policy, NullPolicy::Ignore | NullPolicy::Zero),
         "null policies which drop rows are not yet supported for RLS"
     );
-    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy);
+    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy, None);
     let initial_state_mean = convert_option_vec_to_array1(kwargs.initial_state_mean);
     let coefficients = solve_recursive_least_squares(
         &y,
         &x,
         kwargs.half_life,
         kwargs.initial_state_covariance,
         initial_state_mean,
@@ -318,15 +406,15 @@
 #[polars_expr(output_type=Float32)]
 fn recursive_least_squares(inputs: &[Series], kwargs: RLSKwargs) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
     assert!(
         matches!(null_policy, NullPolicy::Ignore | NullPolicy::Zero),
         "null policies which drop rows are not yet supported for RLS"
     );
-    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy);
+    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy, None);
     let coefficients = solve_recursive_least_squares(
         &y,
         &x,
         kwargs.half_life,
         kwargs.initial_state_covariance,
         None,
     );
@@ -340,15 +428,15 @@
     kwargs: RollingKwargs,
 ) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
     assert!(
         matches!(null_policy, NullPolicy::Ignore | NullPolicy::Zero),
         "null policies which drop rows are not yet supported for rolling least squares"
     );
-    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy);
+    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy, None);
     let coefficients = solve_rolling_ols(
         &y,
         &x,
         kwargs.window_size,
         kwargs.min_periods,
         kwargs.use_woodbury,
         kwargs.alpha,
@@ -360,15 +448,15 @@
 #[polars_expr(output_type=Float32)]
 fn rolling_least_squares(inputs: &[Series], kwargs: RollingKwargs) -> PolarsResult<Series> {
     let null_policy = kwargs.get_null_policy();
     assert!(
         matches!(null_policy, NullPolicy::Ignore | NullPolicy::Zero),
         "null policies which drop rows are not yet supported for rolling least Squares"
     );
-    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy);
+    let (y, x) = convert_polars_to_ndarray(inputs, &null_policy, None);
     let coefficients = solve_rolling_ols(
         &y,
         &x,
         kwargs.window_size,
         kwargs.min_periods,
         kwargs.use_woodbury,
         kwargs.alpha,
@@ -377,24 +465,35 @@
     Ok(Series::from_vec(inputs[0].name(), predictions.to_vec()))
 }
 
 /// This function provides a convenience expression to multiply fitted coefficients with features,
 /// which may be particularly useful in case predicting on test data
 /// (otherwise use direct prediction functions).
 #[polars_expr(output_type=Float32)]
-fn predict(inputs: &[Series]) -> PolarsResult<Series> {
+fn predict(inputs: &[Series], kwargs: PredictKwargs) -> PolarsResult<Series> {
+    let null_policy = kwargs.get_null_policy();
     // The first input is always assumed to be the coefficient struct, and the remaining
     // input series are assumed to be an equivalent number of features.
     let coefficients_df: DataFrame = inputs[0]
         .struct_()
         .expect("the first input series to predict function must be of dtype struct!")
         .clone()
         .unnest();
-    // features are always zero filled in the context of predictions, whereas coefficients may
-    // embed more complex null processing steps.
-    let features = construct_features_array(&inputs[1..], true);
+    // compute predictions assuming zero filled features
+    let features = construct_features_array(&inputs[1..], null_policy != NullPolicy::Ignore);
     let coefficients: Array2<f32> = coefficients_df
         .to_ndarray::<Float32Type>(IndexOrder::C)
         .unwrap();
-    let predictions = (&features * &coefficients).sum_axis(Axis(1));
-    Ok(Series::from_vec(inputs[0].name(), predictions.to_vec()))
+    let predictions = (&features * &coefficients).sum_axis(Axis(1)).to_vec();
+
+    if null_policy == NullPolicy::Drop {
+        // If user has opted for "Drop" policy: mask predictions
+        let is_valid = compute_is_valid_mask(inputs, &null_policy).unwrap();
+        Ok(Series::new(
+            inputs[0].name(),
+            mask_predictions(predictions, &is_valid),
+        ))
+    } else {
+        // Otherwise, simply return predictions
+        Ok(Series::from_vec(inputs[0].name(), predictions))
+    }
 }
```

### Comparing `polars_ols-0.2.6/src/least_squares.rs` & `polars_ols-0.2.8/src/least_squares.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-use std::cmp::max;
 use faer::linalg::solvers::SolverCore;
 use faer::prelude::*;
 use faer::Side;
 use faer_ext::{IntoFaer, IntoNdarray};
 use ndarray::{array, s, Array, Array1, Array2, ArrayView1, Axis, NewAxis};
+use std::cmp::max;
 use std::str::FromStr;
 
 #[cfg(target_os = "macos")]
 use ndarray_linalg::LeastSquaresSvd;
 
-
 /// Invert square matrix input using either Cholesky or LU decomposition
 pub fn inv(array: &Array2<f32>, use_cholesky: bool) -> Array2<f32> {
     let m = array.view().into_faer();
     if use_cholesky {
         match m.cholesky(Side::Lower) {
             Ok(cholesky) => {
                 return cholesky.inverse().as_ref().into_ndarray().to_owned();
@@ -51,15 +50,14 @@
             "lu" => Ok(SolveMethod::LU),
             "cd" => Ok(SolveMethod::CD),
             _ => Err(()),
         }
     }
 }
 
-
 /// Solves ridge regression using Singular Value Decomposition (SVD).
 ///
 /// # Arguments
 ///
 /// * `y` - Target vector.
 /// * `x` - Feature matrix.
 /// * `alpha` - Ridge parameter.
@@ -99,29 +97,28 @@
         .slice(s![.., 0])
         .into_owned();
     let d = &s / (&s * &s + alpha);
     let d_ut_y = &d * &u_t_y;
     v.dot(&d_ut_y)
 }
 
-
 #[cfg(not(target_os = "macos"))]
 fn solve_ols_svd(y: &Array1<f32>, x: &Array2<f32>) -> Array1<f32> {
     // TODO: try to compute w/ LAPACK SVD. Must handle BLAS dependency on linux & windows OS
     //      either use ndarray-linalg or directly call sgelsd from lapack crate..
     solve_ridge_svd(y, x, f32::EPSILON, None)
 }
 
 #[cfg(target_os = "macos")]
 fn solve_ols_svd(y: &Array1<f32>, x: &Array2<f32>) -> Array1<f32> {
-    x.least_squares(y).expect("Failed to compute LAPACK SVD solution!").solution
+    x.least_squares(y)
+        .expect("Failed to compute LAPACK SVD solution!")
+        .solution
 }
 
-
-
 /// Solves an ordinary least squares problem using either QR (faer) or LAPACK SVD
 /// Inputs: features (2d ndarray), targets (1d ndarray), and an optional enum denoting solve method
 /// Outputs: 1-d OLS coefficients
 pub fn solve_ols(
     y: &Array1<f32>,
     x: &Array2<f32>,
     solve_method: Option<SolveMethod>,
@@ -186,15 +183,14 @@
         .solve(&xty.slice(s![.., NewAxis]).into_faer())
         .as_ref()
         .into_ndarray()
         .slice(s![.., 0])
         .into_owned()
 }
 
-
 /// Solves a ridge regression problem of the form: ||y - x B|| + alpha * ||B||
 /// Inputs: features (2d ndarray), targets (1d ndarray), ridge alpha scalar
 pub fn solve_ridge(
     y: &Array1<f32>,
     x: &Array2<f32>,
     alpha: f32,
     solve_method: Option<SolveMethod>,
```

### Comparing `polars_ols-0.2.6/src/lib.rs` & `polars_ols-0.2.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/tests/benchmark.py` & `polars_ols-0.2.8/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/tests/test_ols.py` & `polars_ols-0.2.8/tests/test_ols.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from statsmodels.regression.rolling import RollingOLS
 
 from polars_ols import (
     OLSKwargs,
     compute_least_squares,
     compute_least_squares_from_formula,
 )
-from polars_ols.least_squares import SolveMethod
+from polars_ols.least_squares import NullPolicy, SolveMethod
 
 
 @contextmanager
 def timer(msg: Optional[str] = None, precision: int = 3) -> float:
     start = time.perf_counter()
     end = start
     yield lambda: end - start
@@ -135,15 +135,16 @@
                 pl.col("x1"), pl.col("x2"), null_policy="ignore", mode="coefficients"
             )
         )
         .unnest("coefficients"),
     )
 
 
-def test_fit_missing_data_predictions_and_residuals():
+@pytest.mark.parametrize("null_policy", ["drop", "drop_zero", "drop_y_zero_x"])
+def test_fit_missing_data_predictions_and_residuals(null_policy: NullPolicy):
     df = _make_data()
     rng = np.random.default_rng(0)
 
     def insert_nulls(val):
         return None if rng.random() < 0.1 else val
 
     df = df.with_columns(
@@ -155,44 +156,67 @@
         # compute desired behaviour for "drop" in numpy:
         x, y = (
             df.select("x1", "x2").to_numpy(),
             df.select("y").to_numpy().flatten(),
         )  # notice implicit null -> nan converting to numpy
 
         # 1) compute mask, drop invalid rows, compute coefficients
-        is_valid = ~np.isnan(x).any(axis=1) & ~np.isnan(y)
-        x_fit, y_fit = x[is_valid, :], y[is_valid]
+        if null_policy == "drop_y_zero_x":
+            # drop_y will only drop rows based on the target
+            is_valid = ~np.isnan(y)
+            x_fit, y_fit = np.nan_to_num(x[is_valid, :]), y[is_valid]
+        else:
+            # drop or drop_zero will drop any invalid row in fitting
+            is_valid = ~np.isnan(x).any(axis=1) & ~np.isnan(y)
+            x_fit, y_fit = x[is_valid, :], y[is_valid]
+
         coef = np.linalg.lstsq(x_fit, y_fit, rcond=None)[0]
 
-        # in order to broadcast (valid) predictions to the dimensions of original data; we must
-        # use the original (un-dropped) x. most reasonable behaviour for linear models is:
-        # a) always produce predictions, even for cases where target was null
-        # (allows extrapolation) &
-        # b) for residuals, by default, one wants to retain nulls of targets
-        # Thus the logic below:
+        # in order to broadcast (valid) predictions/residuals to the dimensions of original data; we
+        # use the original (un-dropped) x for computing predictions.
+        # The behaviours which are provided for handling nulls in prediction context:
+        # a) null_policy="drop": ensure predictions are always masked to null
+        #                        if any feature or target is null.
+        # b) null_policy="drop_zero": using coefficients estimated from dropped data, always produce
+        #                             valid predictions by zero filling features
+        #                             (this allows extrapolation).
+        # c) null_policy="drop_y_zero_x": similar to "drop_zero" but where coefficients have been
+        #                                 estimated based on the validity of y alone.
         is_nan_x = np.isnan(x)
         x_predict = x.copy()
         x_predict[is_nan_x] = 0.0  # fill x nans with zero
         predictions_expected = x_predict @ coef
+
+        # if user selected "drop" ensure that predictions are masked based on
+        # validity of both features & targets.
+        if null_policy == "drop":
+            predictions_expected[~is_valid] = np.nan
+        # otherwise, if "drop_zero" / "drop_y_zero_x", compute predictions based on zero-filled
+        # features which allows extrapolation.
+
     with timer("polars-ols w/ null_policy", precision=5):
         predictions = df.select(
             predictions=pl.col("y").least_squares.ols(
-                pl.col("x1"), pl.col("x2"), null_policy="drop", mode="predictions"
+                pl.col("x1"), pl.col("x2"), null_policy=null_policy, mode="predictions"
             )
         )
 
     assert np.allclose(
-        predictions.to_numpy().flatten(), predictions_expected.flatten(), rtol=1.0e-4, atol=1.0e-4
+        predictions.to_numpy().flatten(),
+        predictions_expected.flatten(),
+        rtol=1.0e-4,
+        atol=1.0e-4,
+        equal_nan=True,
     )
 
     # check residuals logic
     residuals_expected = y - predictions_expected  # no need to copy y
     residuals = df.select(
         residuals=pl.col("y").least_squares.ols(
-            pl.col("x1"), pl.col("x2"), null_policy="drop", mode="residuals"
+            pl.col("x1"), pl.col("x2"), null_policy=null_policy, mode="residuals"
         )
     )
     assert np.allclose(
         residuals.to_numpy().flatten(), residuals_expected, rtol=1.0e-4, atol=1.0e-4, equal_nan=True
     )
 
 
@@ -713,15 +737,18 @@
 
     # compute predictions as a rust expression
     predictions = (
         df_test.lazy()
         .join(df_coefficients, on="group")
         .select(
             pl.col("coefficients").least_squares.predict(
-                pl.col("x1"), pl.col("x2"), name="predictions"
+                pl.col("x1"),
+                pl.col("x2"),
+                name="predictions",
+                null_policy="zero",
             )
         )
         .collect()
         .to_numpy()
         .flatten()
     )
```

### Comparing `polars_ols-0.2.6/Cargo.lock` & `polars_ols-0.2.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1586,15 +1586,15 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ols"
-version = "0.2.6"
+version = "0.2.8"
 dependencies = [
  "approx",
  "faer",
  "faer-ext",
  "jemallocator",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `polars_ols-0.2.6/pyproject.toml` & `polars_ols-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.6/PKG-INFO` & `polars_ols-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-ols
-Version: 0.2.6
+Version: 0.2.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Requires-Dist: numpy ; extra == 'dev'
 Requires-Dist: pytest >=7.4.1 ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
```

