# Comparing `tmp/polars_qt-0.1.3.tar.gz` & `tmp/polars_qt-0.1.4.tar.gz`

## Comparing `polars_qt-0.1.3.tar` & `polars_qt-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 polars_qt-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127     3716 2024-04-10 05:28:13.000000 polars_qt-0.1.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      111 2024-04-10 05:28:13.000000 polars_qt-0.1.3/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-10 05:28:13.000000 polars_qt-0.1.3/.python-version
--rw-r--r--   0     1001      127      645 2024-04-10 05:28:13.000000 polars_qt-0.1.3/Makefile
--rw-r--r--   0     1001      127     1786 2024-04-10 05:28:13.000000 polars_qt-0.1.3/README.md
--rw-r--r--   0     1001      127       38 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/__init__.py
--rw-r--r--   0     1001      127     2898 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/funcs.py
--rw-r--r--   0     1001      127     2105 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/qt.py
--rw-r--r--   0     1001      127     1917 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/strategy.py
--rw-r--r--   0     1001      127     2567 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-10 05:28:13.000000 polars_qt-0.1.3/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-10 05:28:13.000000 polars_qt-0.1.3/rust-toolchain.toml
--rw-r--r--   0     1001      127    13211 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/equity.rs
--rw-r--r--   0     1001      127      649 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/if_then.rs
--rw-r--r--   0     1001      127      319 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/rolling_rank.rs
--rw-r--r--   0     1001      127     7926 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/strategy/boll.rs
--rw-r--r--   0     1001      127      617 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/strategy/mod.rs
--rw-r--r--   0     1001      127     1375 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_equity.py
--rw-r--r--   0     1001      127      867 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_if_then.py
--rw-r--r--   0     1001      127      662 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127     1227 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_strategy.py
--rw-r--r--   0     1001      127    41876 2024-04-10 05:28:25.000000 polars_qt-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127     1773 2024-04-10 05:28:13.000000 polars_qt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 polars_qt-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127     3716 2024-04-10 07:28:54.000000 polars_qt-0.1.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      111 2024-04-10 07:28:54.000000 polars_qt-0.1.4/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-10 07:28:54.000000 polars_qt-0.1.4/.python-version
+-rw-r--r--   0     1001      127      645 2024-04-10 07:28:54.000000 polars_qt-0.1.4/Makefile
+-rw-r--r--   0     1001      127     1786 2024-04-10 07:28:54.000000 polars_qt-0.1.4/README.md
+-rw-r--r--   0     1001      127       38 2024-04-10 07:28:54.000000 polars_qt-0.1.4/polars_qt/__init__.py
+-rw-r--r--   0     1001      127     2898 2024-04-10 07:28:54.000000 polars_qt-0.1.4/polars_qt/funcs.py
+-rw-r--r--   0     1001      127     3349 2024-04-10 07:28:54.000000 polars_qt-0.1.4/polars_qt/qt.py
+-rw-r--r--   0     1001      127     3337 2024-04-10 07:28:54.000000 polars_qt-0.1.4/polars_qt/strategy.py
+-rw-r--r--   0     1001      127     2567 2024-04-10 07:28:54.000000 polars_qt-0.1.4/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-10 07:28:54.000000 polars_qt-0.1.4/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-10 07:28:54.000000 polars_qt-0.1.4/rust-toolchain.toml
+-rw-r--r--   0     1001      127    13211 2024-04-10 07:28:54.000000 polars_qt-0.1.4/src/equity.rs
+-rw-r--r--   0     1001      127      649 2024-04-10 07:28:54.000000 polars_qt-0.1.4/src/if_then.rs
+-rw-r--r--   0     1001      127      319 2024-04-10 07:28:54.000000 polars_qt-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      127     3250 2024-04-10 07:28:54.000000 polars_qt-0.1.4/src/rolling_rank.rs
+-rw-r--r--   0     1001      127     7849 2024-04-10 07:28:54.000000 polars_qt-0.1.4/src/strategy/boll.rs
+-rw-r--r--   0     1001      127     6410 2024-04-10 07:28:54.000000 polars_qt-0.1.4/src/strategy/boll_vol_stop.rs
+-rw-r--r--   0     1001      127      636 2024-04-10 07:28:54.000000 polars_qt-0.1.4/src/strategy/mod.rs
+-rw-r--r--   0     1001      127     1375 2024-04-10 07:28:54.000000 polars_qt-0.1.4/tests/test_equity.py
+-rw-r--r--   0     1001      127      867 2024-04-10 07:28:54.000000 polars_qt-0.1.4/tests/test_if_then.py
+-rw-r--r--   0     1001      127      662 2024-04-10 07:28:54.000000 polars_qt-0.1.4/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127     1663 2024-04-10 07:28:54.000000 polars_qt-0.1.4/tests/test_strategy.py
+-rw-r--r--   0     1001      127    41876 2024-04-10 07:29:08.000000 polars_qt-0.1.4/Cargo.lock
+-rw-r--r--   0     1001      127     1773 2024-04-10 07:28:54.000000 polars_qt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.4/PKG-INFO
```

### Comparing `polars_qt-0.1.3/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.4/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/Makefile` & `polars_qt-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/README.md` & `polars_qt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/polars_qt/funcs.py` & `polars_qt-0.1.4/polars_qt/funcs.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/polars_qt/utils.py` & `polars_qt-0.1.4/polars_qt/utils.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/src/equity.rs` & `polars_qt-0.1.4/src/equity.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/src/if_then.rs` & `polars_qt-0.1.4/src/if_then.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/src/rolling_rank.rs` & `polars_qt-0.1.4/src/rolling_rank.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/src/strategy/boll.rs` & `polars_qt-0.1.4/src/strategy/boll.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
 use pyo3_polars::export::polars_core::utils::CustomIterTools;
 use serde::Deserialize;
 
 #[derive(Deserialize)]
 struct BollKwargs {
+    // window, open_width, stop_width, take_profit_width
     params: (usize, f64, f64, Option<f64>),
     filter_flag: bool,
     delay_open: bool,
     long_signal: f64,
     short_signal: f64,
     close_signal: f64,
 }
 
 #[polars_expr(output_type=Float64)]
 fn boll(inputs: &[Series], kwargs: BollKwargs) -> PolarsResult<Series> {
     let fac = inputs[0].f64()?;
     let middle = inputs[1].f64()?;
-    let std = inputs[2].f64()?;
+    let std_ = inputs[2].f64()?;
     let filter = if kwargs.filter_flag {
         Some(StrategyFilter::from_inputs(inputs, (3, 4, 5, 6))?)
     } else {
         None
     };
-    Ok(impl_boll(fac, middle, std, filter, kwargs).into_series())
+    Ok(impl_boll(fac, middle, std_, filter, kwargs).into_series())
 }
 
 macro_rules! boll_logic_impl {
     (
         $kwargs: expr,
         $fac: expr, $middle: expr, $std: expr,
         $last_signal: expr, $last_fac: expr,
@@ -53,21 +54,21 @@
                     // short open
                     $last_signal = $kwargs.short_signal;
                     open_flag = true;
                 }
                 // == stop condition
                 if (!open_flag) && ($last_signal != $kwargs.close_signal) {
                     // we can skip stop condition if trade is already close or open
-                    if ($last_fac > $kwargs.params.2) && (fac <= $kwargs.params.2)
+                    if (($last_fac > $kwargs.params.2) && (fac <= $kwargs.params.2))
                         $(|| $long_stop.unwrap_or(false))?  // additional stop condition
                         $(|| fac > $m3)?  // profit stop condition
                     {
                         // long stop
                         $last_signal = $kwargs.close_signal;
-                    } else if ($last_fac < -$kwargs.params.2) && (fac >= -$kwargs.params.2)
+                    } else if (($last_fac < -$kwargs.params.2) && (fac >= -$kwargs.params.2))
                         $(|| $short_stop.unwrap_or(false))?
                         $(|| fac < -$m3)?  // profit stop condition
                     {
                         // short stop
                         $last_signal = $kwargs.close_signal;
                     }
                 }
@@ -191,16 +192,14 @@
                 izip!(fac_arr, middle_arr, std_arr)
                     .map(|(fac, middle, std)| {
                         boll_logic_impl!(
                             kwargs, fac, middle, std,
                             last_signal, last_fac,
                             long_open=>last_fac < m,
                             short_open=>last_fac > -m,
-                            // long_open=>|last_fac| (last_fac < m),
-                            // short_open=>|last_fac| (last_fac > -m),
                         )
                     })
                     .collect_trusted()
             }
         }
     }
 }
```

### Comparing `polars_qt-0.1.3/src/strategy/mod.rs` & `polars_qt-0.1.4/src/strategy/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 mod boll;
+mod boll_vol_stop;
 
 use polars::datatypes::BooleanChunked;
 use polars::prelude::*;
 
 pub(super) struct StrategyFilter<'a> {
     long_open: &'a BooleanChunked,
     long_stop: &'a BooleanChunked,
```

### Comparing `polars_qt-0.1.3/tests/test_equity.py` & `polars_qt-0.1.4/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/tests/test_if_then.py` & `polars_qt-0.1.4/tests/test_if_then.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/tests/test_rolling_rank.py` & `polars_qt-0.1.4/tests/test_rolling_rank.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/tests/test_strategy.py` & `polars_qt-0.1.4/tests/test_strategy.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,24 +6,31 @@
 
 def test_boll():
     df = pl.DataFrame({
         'close': [10., 11, 12, 10, 11, 12, 10, 11, 12, 13, 14, 10, 7, 5, 4, 3, 4, 4, 3, 2],
         'short_open_filter': [1] * 11 + [0, 0, 1, 1, 1] + [1] * 4,
     })
     df = df.with_columns([
-        pl.col('close').qt.boll((4, 1)).alias('s1'),
+        pl.col('close').qt.boll((4, 1)).alias('s1'), # base boll
+        # boll with filters
         pl.col('close').qt.boll((4, 1), filters=[
             pl.col('close') > 0, False,  # long open, long stop
             'short_open_filter', False,  # short open, short stop
         ]).alias('s2'),
+        # boll with filters and delay open
         pl.col('close').qt.boll((4, 1), filters=[
             pl.col('close') > 0, False,  # long open, long stop
             'short_open_filter', False,  # short open, short stop
         ], delay_open=True).alias('s3'),
-
+        # boll with fac_vol stop, take profit if close reaches 5 * fac_vol
+        pl.col('close').qt.boll((4, 1, 5), fac_vol=pl.repeat(1, pl.col('close').len())).alias('s4'),
     ])
+    print(df.to_pandas())
     expect1 = pl.Series('s1', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, -1, -1, -1, -1, -1, 0, 0, 0, -1])
     assert_series_equal(df['s1'], expect1)
     expect2 = pl.Series('s2', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, -1, 0, 0, 0, -1])
     assert_series_equal(df['s2'], expect2)
     expect3 = pl.Series('s3', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, -1, -1, -1, 0, 0, 0, -1])
     assert_series_equal(df['s3'], expect3)
+    expect3 = pl.Series('s4', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, -1, -1, 0, 0, -1, 0, 0, 0, -1])
+    assert_series_equal(df['s4'], expect3)
+test_boll()
```

### Comparing `polars_qt-0.1.3/Cargo.lock` & `polars_qt-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -854,15 +854,15 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "itertools",
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
 ]
```

### Comparing `polars_qt-0.1.3/pyproject.toml` & `polars_qt-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.3/PKG-INFO` & `polars_qt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-qt
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Author-email: Teamon9161 <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

