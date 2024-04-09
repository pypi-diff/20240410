# Comparing `tmp/fintoolkit-0.0.6.tar.gz` & `tmp/fintoolkit-0.0.7.tar.gz`

## Comparing `fintoolkit-0.0.6.tar` & `fintoolkit-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_black_scholes.py
--rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_cboe_margin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_data.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_famafrench.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_fixed_income.py
--rw-r--r--   0        0        0    17524 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_functional.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_portfolio.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/tests/test_visualization.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/__init__.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/asset_class.py
--rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/black_scholes.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/cboe_margin.py
--rw-r--r--   0        0        0     9720 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/data.py
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/fixed_income.py
--rw-r--r--   0        0        0    53011 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/functional.py
--rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/portfolio.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/toolkit/visualization.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/.gitignore
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 fintoolkit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_black_scholes.py
+-rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_cboe_margin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_data.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_famafrench.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_fixed_income.py
+-rw-r--r--   0        0        0    18014 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_functional.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_portfolio.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/tests/test_visualization.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/__init__.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/asset_class.py
+-rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/black_scholes.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/cboe_margin.py
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/data.py
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/fixed_income.py
+-rw-r--r--   0        0        0    53112 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/functional.py
+-rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/portfolio.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/toolkit/visualization.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/.gitignore
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 fintoolkit-0.0.7/PKG-INFO
```

### Comparing `fintoolkit-0.0.6/tests/test_black_scholes.py` & `fintoolkit-0.0.7/tests/test_black_scholes.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/tests/test_cboe_margin.py` & `fintoolkit-0.0.7/tests/test_cboe_margin.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/tests/test_famafrench.py` & `fintoolkit-0.0.7/tests/test_famafrench.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/tests/test_fixed_income.py` & `fintoolkit-0.0.7/tests/test_fixed_income.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/tests/test_functional.py` & `fintoolkit-0.0.7/tests/test_functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,15 +143,16 @@
         ],
         index=pd.period_range("2000-01", periods=36, freq="M"),
     )
     price_df = pd.concat([unit_price, benchmark_price], axis=1)
 
     def test_periodicity(self):
         for p in ftk.PERIODICITY:
-            s = pd.Series([0], index=pd.period_range("2000-01-01", periods=1, freq=p))
+            s = pd.Series([0], index=pd.period_range(
+                "2000-01-01", periods=1, freq=p))
             self.assertEqual(ftk.periodicity(s), ftk.PERIODICITY[p])
             df = pd.concat([s, s], axis=1)
             self.assertEqual(ftk.periodicity(df), ftk.PERIODICITY[p])
 
     def test_price_return_conversion(self):
         pd.testing.assert_series_equal(ftk.price_to_return(p), r)
         pd.testing.assert_series_equal(ftk.return_to_price(r), p)
@@ -198,15 +199,16 @@
         nky_p.iloc[3] = np.NaN
         jpy_p.iloc[2] = np.NaN
         cad_p.iloc[4] = np.NaN
 
         nky_p.div(jpy_p, axis=0).mul(cad_p, axis=0)
 
         # Expected
-        pd.concat([jpy_p / cad_p, cad_p / jpy_p], axis=1).prod(axis=1)  # All ones
+        pd.concat([jpy_p / cad_p, cad_p / jpy_p],
+                  axis=1).prod(axis=1)  # All ones
         jpy_cad.div(jpy_p, axis=0).iloc[:, 0]  # Ones, with some na
         jpy_cad.div(cad_p, axis=0).iloc[:, 1]
 
         # This SHOULDN'T be ones; reason Pandas auto match column name which is not desirable
         (jpy_cad / cad_jpy)
 
         # JPY depr vs USD, CAD appr vs USD, so CAD appr vs JPY a lot
@@ -226,82 +228,89 @@
             ).iloc[-1],
             0,
         )
 
     def test_compound_return(self):
         self.assertAlmostEqual(ftk.compound_return(p, False), -0.12)
         self.assertAlmostEqual(ftk.compound_return(r, False), -0.12)
-        self.assertAlmostEqual(ftk.compound_return(r, False), (1 + r).prod() - 1)
+        self.assertAlmostEqual(ftk.compound_return(
+            r, False), (1 + r).prod() - 1)
         self.assertAlmostEqual(ftk.compound_return(pp, False)[0], -0.12)
         self.assertAlmostEqual(ftk.compound_return(rr, False)[1], -0.12)
 
     def test_skew_kurt(self):
         self.assertAlmostEqual(ftk.skew(r), scipy.stats.skew(r, bias=False))
         self.assertAlmostEqual(
             ftk.skew(r), scipy.stats.skew(r) * np.sqrt((n - 1) * n) / (n - 2)
         )
         np.testing.assert_array_almost_equal(
             ftk.skew(rr), scipy.stats.skew(rr, bias=False)
         )
 
-        self.assertAlmostEqual(ftk.kurt(r), scipy.stats.kurtosis(r, bias=False))
+        self.assertAlmostEqual(
+            ftk.kurt(r), scipy.stats.kurtosis(r, bias=False))
         self.assertAlmostEqual(
             ftk.kurt(r),
-            (n - 1) / (n - 2) / (n - 3) * ((n + 1) * scipy.stats.kurtosis(r) + 6),
+            (n - 1) / (n - 2) / (n - 3) *
+            ((n + 1) * scipy.stats.kurtosis(r) + 6),
         )
         np.testing.assert_array_almost_equal(
             ftk.kurt(rr), scipy.stats.kurtosis(rr, bias=False)
         )
 
     def test_mean(self):
         self.assertAlmostEqual(ftk.arithmetic_mean(r), r.sum() / len(r))
         np.testing.assert_array_almost_equal(
             ftk.arithmetic_mean(rr), rr.sum() / len(rr)
         )
 
-        self.assertAlmostEqual(ftk.geometric_mean(r), scipy.stats.gmean(1 + r) - 1)
+        self.assertAlmostEqual(ftk.geometric_mean(
+            r), scipy.stats.gmean(1 + r) - 1)
         np.testing.assert_array_almost_equal(
             ftk.geometric_mean(rr), scipy.stats.gmean(1 + rr) - 1
         )
 
     def test_descriptive_stats(self):
         self.assertAlmostEqual(ftk.arithmetic_mean(self.unit_price), 0.011, 3)
         self.assertAlmostEqual(ftk.compound_return(self.unit_price), 0.454, 3)
         self.assertAlmostEqual(
             ftk.compound_return(self.unit_price, annualize=True), 0.1329, 4
         )
         self.assertAlmostEqual(ftk.mean_abs_dev(self.unit_price), 0.0252, 4)
-        self.assertAlmostEqual(ftk.variance(self.unit_price), 0.0011 * 36 / 35, 4)
+        self.assertAlmostEqual(ftk.variance(
+            self.unit_price), 0.0011 * 36 / 35, 4)
         self.assertAlmostEqual(ftk.volatility(self.unit_price), 0.0336, 4)
         self.assertAlmostEqual(
             ftk.volatility(self.unit_price, annualize=True),
             0.1149 * np.sqrt(36 / 35),
             4,
         )
         self.assertAlmostEqual(ftk.skew(self.unit_price), -0.25, 2)
         self.assertAlmostEqual(ftk.kurt(self.unit_price), 0.16, 2)
         self.assertAlmostEqual(
             ftk.covariance(self.price_df).iloc[0, 1], 0.001109 * 36 / 35, 6
         )
-        self.assertAlmostEqual(ftk.correlation(self.price_df).iloc[0, 1], 0.995, 3)
+        self.assertAlmostEqual(ftk.correlation(
+            self.price_df).iloc[0, 1], 0.995, 3)
         self.assertAlmostEqual(ftk.sharpe(self.unit_price, 0.0243), 0.93, 2)
 
     def test_relative_risk(self):
         self.assertAlmostEqual(
             ftk.tracking_error(self.unit_price, self.benchmark_price),
             0.00348 * np.sqrt(35 / 36),
             3,
         )
         self.assertAlmostEqual(
             ftk.tracking_error(self.unit_price, self.benchmark_price, True),
             0.0121 * np.sqrt(35 / 36),
             3,
         )
         self.assertAlmostEqual(
-            ftk.information_ratio(self.unit_price, self.benchmark_price), -1.1, 1
+            ftk.information_ratio(
+                self.unit_price, self.benchmark_price), -1.1, 1
         )
 
     def test_regression(self):
         # Regression only, does NOT take into account of risk free rate
         self.assertAlmostEqual(
             ftk.beta(self.unit_price, self.benchmark_price), 0.9814, 3
         )  # vs 0.9812
@@ -315,20 +324,22 @@
             ftk.price_to_return(self.benchmark_price) - self.risk_free_return
         )
 
         self.assertAlmostEqual(ftk.beta(unit_rfr, benchmark_rfr), 0.982, 3)
         self.assertAlmostEqual(ftk.alpha(unit_rfr, benchmark_rfr), -0.00082, 5)
 
         self.assertAlmostEqual(
-            ftk.bull_beta(self.unit_price, self.benchmark_price, self.risk_free_return),
+            ftk.bull_beta(self.unit_price, self.benchmark_price,
+                          self.risk_free_return),
             1.035,
             3,
         )
         self.assertAlmostEqual(
-            ftk.bear_beta(self.unit_price, self.benchmark_price, self.risk_free_return),
+            ftk.bear_beta(self.unit_price, self.benchmark_price,
+                          self.risk_free_return),
             0.948,
             3,
         )
         self.assertAlmostEqual(
             ftk.beta_timing_ratio(
                 self.unit_price, self.benchmark_price, self.risk_free_return
             ),
@@ -373,72 +384,87 @@
 
     def test_drawdown(self):
         # Assuming uninterrupted drawdown definition is used
         self.assertAlmostEqual(ftk.worst_drawdown(self.unit_price), -0.1463, 4)
         self.assertAlmostEqual(
             ftk.calmar(self.unit_price, rfr_annualized=0.0243), 0.74, 2
         )
-        self.assertAlmostEqual(ftk.avg_drawdown(self.unit_price, d=3), -0.056, 3)
+        self.assertAlmostEqual(ftk.avg_drawdown(
+            self.unit_price, d=3), -0.056, 3)
         # ftk.sterling() # Original
         self.assertAlmostEqual(
-            ftk.sterling_modified(self.unit_price, rfr_annualized=0.0243, d=3), 1.92, 2
+            ftk.sterling_modified(
+                self.unit_price, rfr_annualized=0.0243, d=3), 1.92, 2
         )
-        self.assertAlmostEqual(ftk.drawdown_deviation(self.unit_price, d=3), -0.0245, 4)
+        self.assertAlmostEqual(ftk.drawdown_deviation(
+            self.unit_price, d=3), -0.0245, 4)
         self.assertAlmostEqual(
-            ftk.burke_modified(self.unit_price, rfr_annualized=0.0243, d=3), 4.43, 1
+            ftk.burke_modified(
+                self.unit_price, rfr_annualized=0.0243, d=3), 4.43, 1
         )  # vs 4.42
-        self.assertAlmostEqual(ftk.avg_annual_drawdown(self.unit_price), -0.0604, 4)
         self.assertAlmostEqual(
-            ftk.sterling_calmar(self.unit_price, rfr_annualized=0.0243), 1.80, 2
+            ftk.avg_annual_drawdown(self.unit_price), -0.0604, 4)
+        self.assertAlmostEqual(
+            ftk.sterling_calmar(
+                self.unit_price, rfr_annualized=0.0243), 1.80, 2
         )
         self.assertAlmostEqual(ftk.pain_index(self.unit_price), 0.0376, 4)
         self.assertAlmostEqual(ftk.pain(self.unit_price, 0.0243), 2.89, 2)
         self.assertAlmostEqual(ftk.ulcer_index(self.unit_price), 0.0597, 4)
         self.assertAlmostEqual(ftk.martin(self.unit_price, 0.0243), 1.82, 2)
 
         # Max Upturn
         self.assertAlmostEqual(
-            ftk.max_upturn(ftk.price_to_return(self.unit_price).loc["2000"]), 0.2764, 4
+            ftk.max_upturn(ftk.price_to_return(
+                self.unit_price).loc["2000"]), 0.2764, 4
         )
 
     def test_partial_moments(self):
         self.assertAlmostEqual(
             ftk.downside_potential(self.unit_price, mar=0.005), 0.0101, 4
         )
-        self.assertAlmostEqual(ftk.downside_risk(self.unit_price, mar=0.005), 0.0212, 4)
+        self.assertAlmostEqual(ftk.downside_risk(
+            self.unit_price, mar=0.005), 0.0212, 4)
         self.assertAlmostEqual(
-            ftk.downside_risk(self.unit_price, mar=0.005, annualize=True), 0.0733, 4
+            ftk.downside_risk(self.unit_price, mar=0.005,
+                              annualize=True), 0.0733, 4
         )
         self.assertAlmostEqual(
             ftk.upside_potential(self.unit_price, mar=0.005), 0.0161, 4
         )
-        self.assertAlmostEqual(ftk.upside_risk(self.unit_price, mar=0.005), 0.0262, 4)
+        self.assertAlmostEqual(ftk.upside_risk(
+            self.unit_price, mar=0.005), 0.0262, 4)
         self.assertAlmostEqual(
-            ftk.upside_risk(self.unit_price, mar=0.005, annualize=True), 0.0909, 4
+            ftk.upside_risk(self.unit_price, mar=0.005,
+                            annualize=True), 0.0909, 4
         )
         self.assertAlmostEqual(ftk.omega(self.unit_price, mar=0.005), 1.6, 1)
         self.assertAlmostEqual(
             ftk.upside_potential_ratio(self.unit_price, 0.005), 0.22, 2
         )
         self.assertAlmostEqual(
             ftk.variability_skewness(self.unit_price, 0.005), 1.24, 2
         )
-        self.assertAlmostEqual(ftk.sortino(self.unit_price, mar=0.005), 0.97, 2)
+        self.assertAlmostEqual(ftk.sortino(
+            self.unit_price, mar=0.005), 0.97, 2)
 
     def test_value_at_risk(self):
         for alpha in [0.05, 0.95]:
             self.assertAlmostEqual(
                 ftk.var_historical(self.unit_price, alpha), -0.0520, 4
             )
-            self.assertAlmostEqual(ftk.var_normal(self.unit_price, alpha), -0.0443, 4)
-            self.assertAlmostEqual(ftk.var_modified(self.unit_price, alpha), -0.0465, 4)
+            self.assertAlmostEqual(ftk.var_normal(
+                self.unit_price, alpha), -0.0443, 4)
+            self.assertAlmostEqual(ftk.var_modified(
+                self.unit_price, alpha), -0.0465, 4)
             self.assertAlmostEqual(
                 ftk.cvar_historical(self.unit_price, alpha), -0.0625, 4
             )
-            self.assertAlmostEqual(ftk.cvar_normal(self.unit_price, alpha), -0.0584, 4)
+            self.assertAlmostEqual(ftk.cvar_normal(
+                self.unit_price, alpha), -0.0584, 4)
 
     def test_summary(self):
         summary = ftk.summary(
             self.unit_price, self.benchmark_price, self.risk_free_return
         )
 
         self.assertAlmostEqual(summary["Periodic Geometric Mean"], 0.0105, 4)
@@ -458,20 +484,22 @@
         self.assertAlmostEqual(summary["VaR Gaussian (95%)"], -0.0443, 4)
         self.assertAlmostEqual(summary["VaR Modified (95%)"], -0.0465, 4)
 
         self.assertAlmostEqual(summary["Sharpe (2.43%)"], 0.9322, 4)
         self.assertAlmostEqual(summary["Calmar"], 0.7425, 4),
         self.assertAlmostEqual(summary["Sterling Original"], 0.8283, 4)
         self.assertAlmostEqual(summary["Average Annual Drawdown"], -0.0604, 4)
-        self.assertAlmostEqual(summary["Downside Risk (Annualized)"], 0.0663, 4)
+        self.assertAlmostEqual(
+            summary["Downside Risk (Annualized)"], 0.0663, 4)
         self.assertAlmostEqual(summary["Omega Ratio"], 2.3382, 4),
         self.assertAlmostEqual(summary["Sortino Ratio"], 2.0034, 4),
         self.assertAlmostEqual(summary["Annualized Active Return"], -0.0133, 4)
         self.assertAlmostEqual(summary["Annualized Tracking Error"], 0.0122, 4)
-        self.assertAlmostEqual(summary["Annualized Information Ratio"], -1.0921, 4)
+        self.assertAlmostEqual(
+            summary["Annualized Information Ratio"], -1.0921, 4)
         self.assertAlmostEqual(summary["Beta"], 0.98, 2)
         self.assertAlmostEqual(summary["Alpha (Annualized)"], -0.0098, 4)
         self.assertAlmostEqual(summary["Correlation"], 0.9947, 4)
         self.assertAlmostEqual(summary["R-Squared"], 0.9894, 4)
         self.assertAlmostEqual(summary["Treynor Ratio"], 0.111, 3)
-        self.assertAlmostEqual(summary["Up Capture"], 0.9276, 4)
+        self.assertAlmostEqual(summary["Up Capture"], 0.9379, 4)
         self.assertAlmostEqual(summary["Down Capture"], 0.9929, 4)
```

### Comparing `fintoolkit-0.0.6/tests/test_portfolio.py` & `fintoolkit-0.0.7/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/toolkit/asset_class.py` & `fintoolkit-0.0.7/toolkit/asset_class.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/toolkit/black_scholes.py` & `fintoolkit-0.0.7/toolkit/black_scholes.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/toolkit/cboe_margin.py` & `fintoolkit-0.0.7/toolkit/cboe_margin.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/toolkit/data.py` & `fintoolkit-0.0.7/toolkit/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,87 +4,91 @@
     - Ken French’s Data Library
     - Federal Reserve Economic Data
     - Bank of Canada
     - Statistics Canada
     - MSCI
     - Eurekahedge
 """
+from functools import wraps
 import io
 import re
 import datetime
 import urllib
 import requests
 import pandas as pd
 import pandas_datareader as pdr
 import yfinance as yf
 
 
-def today() -> datetime.date:
-    """Today
+def _default_date(func):
 
-    Returns
-    -------
-    datetime.date
-        Today
-    """
-    return datetime.datetime.today().date()
+    @wraps(func)
+    def wrapper(**kwargs):
+        if 'date' not in kwargs:
+            kwargs['date'] = datetime.datetime.today().date()
+        return func(**kwargs)
+
+    wrapper.__doc__ = func.__doc__
+    return wrapper
 
 
-def last_business_day(date=today()):
+@_default_date
+def last_business_day(date: datetime.date = None):
     return (date - datetime.timedelta(days=max(0, date.weekday() - 4)))
 
 
-def end_of_month(date: datetime.date = today(), n: int = 0) -> datetime.date:
+@_default_date
+def end_of_month(date: datetime.date = None, n: int = 0) -> datetime.date:
     """Last day of the month that is `n` months after the specified date.
     Similar to the `EOMONTH` function in Excel.
 
     Parameters
     ----------
     date : datetime.date, optional
-        A date, by default today()
+        A date, by default None (i.e. today)
     n : int, optional
         Number of months, by default 0. A positive value yields a month in the future,
         a negative value yields a month in the past.
 
     Returns
     -------
     datetime.date
         _description_
     """
     year = date.year + (date.month + n) // 12
     month = (date.month + n) % 12 + 1
     return datetime.date(year, month, 1) - datetime.timedelta(days=1)
 
 
-def end_of_quarter(date: datetime.date = today(), n: int = 0) -> datetime.date:
+def end_of_quarter(date: datetime.date = None, n: int = 0) -> datetime.date:
     """Last day of the calendar quarter that is `n` quarters after the specified date.
 
     Parameters
     ----------
     date : datetime.date, optional
-        A date, by default today()
+        A date, by default None (i.e. today)
     n : int, optional
         Number of quarters, by default 0. A positive value yields a quarter in the future,
         a negative value yields a quarter in the past.
 
     Returns
     -------
     datetime.date
         _description_
     """
     return end_of_month(date, 2 - ((date.month - 1) % 3) + 3 * n)
 
 
-def end_of_year(date: datetime.date = today(), n: int = 0) -> datetime.date:
+def end_of_year(date: datetime.date = None, n: int = 0) -> datetime.date:
     """Last date of the calendar year that is `n` years after the specified date.
 
     Parameters
     ----------
     date : datetime.date, optional
-        A date, by default today()
+        A date, by default None (i.e. today)
     n : int, optional
         Number of years, by default 0. A positive value yields a year in the future,
         a negative value yields a year in the past.
 
     Returns
     -------
     datetime.date
@@ -119,32 +123,32 @@
             / 100,
             how="inner",
         )
     return factors.join(rfr, how="inner")
 
 
 # Yahoo
-def get_yahoo(ticker: str) -> pd.Series:
+def get_yahoo(ticker: str = "^GSPC") -> pd.Series:
     """Download the historical adjusted closing price of a security with
     ticker `ticker`.
 
     Args:
-        ticker (str): Yahoo! ticker of the security
+        ticker (str): Yahoo! ticker of the security, by default "^GSPC", i.e. S&P 500
 
     Returns:
         pd.Series: Time series of the prices of the security
     """
     t = yf.Ticker(ticker)
     # Some securities e.g. crypto trades on weekends
     s = t.history(period="max")["Close"]
     s.name = ticker
     return s
 
 
-def get_yahoo_bulk(tickers: list, period: str = "max") -> pd.DataFrame:
+def get_yahoo_bulk(tickers: list = ["^GSPC"], period: str = "max") -> pd.DataFrame:
     """Download the historical adjusted closing price of multiple securities
     with ticker in the `tickers` list.
 
     Parameters
     ----------
     tickers : list
         List of Yahoo! tickers
@@ -152,31 +156,31 @@
         Length of track record to download, by default 'max'
 
     Returns
     -------
     pd.DataFrame
         Time series of the prices of the securities
     """
-    # Columns are already the tickers
-    return yf.download(" ".join(tickers), period=period)["Adj Close"].asfreq("B")
+    # Columns are already the tickers, note some securities like crypto trades in non-business days
+    return yf.download(" ".join(tickers), period=period)["Adj Close"]
 
 
 def get_msci(
-        codes: list,
-        end_date: str = last_business_day().strftime("%Y%m%d"),
+        codes: list = [990100],
+        end_date: str = None,
         fx: str = "USD",
         variant: str = "STRD",
         freq: str = "END_OF_MONTH",
         ror: bool = True) -> pd.DataFrame:
     """Download the historical index value of multiple indexes.
 
     Parameters
     ----------
     codes : list
-        List of MSCI index code.
+        List of MSCI index code, by default [990100], i.e. MSCI World
         See https://www.msci.com/our-solutions/indexes/index-resources/index-tools
     end_date : str, optional
         As of date, by default get_last_business_day().strftime("%Y%m%d")
     fx : str, optional
         Currency, by default "USD"
     variant : str, optional
         Index Level ('STRD' for Price, 'NETR' for Net, 'GRTR' for Gross), by default "STRD"
@@ -186,14 +190,16 @@
         Convert from index value to return, by default True
 
     Returns
     -------
     pd.DataFrame
         Time series of the index values. Index is DatetimeIndex (freq=None).
     """
+    if end_date is None:
+        end_date = last_business_day().strftime("%Y%m%d")
     url = f'https://app2-nv.msci.com/products/service/index/indexmaster/downloadLevelData?output=INDEX_LEVELS&currency_symbol={fx}&index_variant={variant}&start_date=19691231&end_date={end_date}&data_frequency={freq}&baseValue=false&index_codes={",".join(map(str, codes))}'
     df = pd.read_excel(url, thousands=',', parse_dates=[
                        0], skiprows=6, skipfooter=19).set_index('Date')
     if ror:
         df = df.pct_change().to_period('M')
     return df
 
@@ -205,21 +211,21 @@
     -------
     pd.DataFrame
         Time series of the monthly returns. Index is PeriodIndex.
     """
     return pd.read_csv("https://www.eurekahedge.com/df/Eurekahedge_indices.zip", parse_dates=['Date'], index_col=[0, 1, 2], na_values=' ').squeeze().unstack().T.to_period('M') / 100.0
 
 
-def get_statcan_bulk(ids: list, n: int = 25) -> pd.DataFrame:
+def get_statcan_bulk(ids: list = [2062815], n: int = 25) -> pd.DataFrame:
     """Download the historical data from Statisticas Canada
 
     Parameters
     ----------
     ids : list
-        List of vectors (10 digits without leading "V")
+        List of vectors, by default [2062815]. (Vector number is a 10-digit number without leading "V")
     n : int, optional
         Number of months, by default 24
 
     Returns
     -------
     pd.DataFrame
         Column names are ids. Index is DatetimeIndex (freq=None).
@@ -230,70 +236,80 @@
     data = [pd.DataFrame(json[i]["object"]["vectorDataPoint"]).set_index(
         "refPer")["value"] for i in range(len(json))]
     df = pd.concat(data, axis=1, keys=ids)
     df.index = pd.to_datetime(df.index)
     return df.sort_index()
 
 
-def get_fred_bulk(ids: list = [], start: datetime.date = end_of_month(n=-25), end: datetime.date = today()) -> pd.DataFrame:
+def get_fred_bulk(ids: list = ["SOFR"], start_date: datetime.date = None, end_date: datetime.date = None) -> pd.DataFrame:
     """Download the historical Federal Reserve Economic Data (FRED) from Frederal Reserver Bank of St. Louis
 
     Parameters
     ----------
     ids : list, optional
-        List of series Ids, by default []
+        List of series Ids, by default ["SOFR"], i.e. Secured Overnight Financing Rate
     start : datetime.date, optional
         Start date, by default 2 years before today
     end : datetime.date, optional
         End date, by default today
 
     Returns
     -------
     pd.DataFrame
         Index is DatetimeIndex (freq='ME')
     """
-    df = pdr.DataReader(['SOFR', 'T10YIE'], 'fred', start, end)
+    if start_date is None:
+        start_date = end_of_month(n=-25)
+    if end_date is None:
+        end_date = datetime.datetime.today()
+    df = pdr.DataReader(ids, 'fred', start_date, end_date)
     return df.groupby(pd.Grouper(freq="ME")).last()
 
 
-def get_us_yield_curve(year: int = today().year, n: int = 2) -> pd.DataFrame:
+def get_us_yield_curve(year: int = 0, n: int = 2) -> pd.DataFrame:
     """Download the historical Treasury Par Yield Curve Rates
 
     Parameters
     ----------
     year : int, optional
         Year, by default the current year
     n : int, optional
         Number of years, by default 2
 
     Returns
     -------
     pd.DataFrame
         Index is DatetimeIndex (freq=None)
     """
+    if year == 0:
+        year = datetime.datetime.today().year
     data = [pd.read_csv(
         f"https://home.treasury.gov/resource-center/data-chart-center/interest-rates/daily-treasury-rates.csv/{y}/all?type=daily_treasury_yield_curve&_format=csv", index_col=0) for y in range(year, year - n, -1)]
     df = pd.concat(data, axis=0)
     df.index = pd.to_datetime(df.index)
     return df.sort_index()
 
 
-def get_boc_bulk(ids: list, start: datetime.date = end_of_month(n=-25), end: datetime.date = end_of_month()) -> pd.DataFrame:
+def get_boc_bulk(ids: list = ["V80691342"], start_date: datetime.date = None, end_date: datetime.date = None) -> pd.DataFrame:
     """Download the historical data from Bank of Canada
 
     Parameters
     ----------
     ids : list
-        List of series names
+        List of series names, by default ["V80691342"], i.e. 1 month Treasury bill
     start : datetime.date, optional
         Start date, by default end_of_month(n=-25)
     end : datetime.date, optional
         End date, by default end_of_month()
 
     Returns
     -------
     pd.DataFrame
         _description_
     """
-    url = f'https://www.bankofcanada.ca/valet/observations/{urllib.parse.quote(",".join(ids))}/csv?start_date={start.strftime("%Y-%m-%d")}&end_date={end.strftime("%Y-%m-%d")}'
+    if start_date is None:
+        start_date = end_of_month(n=-25)
+    if end_date is None:
+        end_date = end_of_month()
+    url = f'https://www.bankofcanada.ca/valet/observations/{urllib.parse.quote(",".join(ids))}/csv?start_date={start_date.strftime("%Y-%m-%d")}&end_date={end_date.strftime("%Y-%m-%d")}'
     csv = requests.get(url, verify=False)
     return pd.read_csv(io.StringIO(csv.text.split('"OBSERVATIONS"\r\n')[1]), parse_dates=["date"]).set_index("date").loc[:, ids]
```

### Comparing `fintoolkit-0.0.6/toolkit/fixed_income.py` & `fintoolkit-0.0.7/toolkit/fixed_income.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/toolkit/functional.py` & `fintoolkit-0.0.7/toolkit/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,15 +815,16 @@
 
     Returns
     -------
     float | pd.Series
         Downside Risk
     """
     dr = np.sqrt(
-        ((mar - timeseries[timeseries < mar]) ** 2).sum() / (len(timeseries) - ddof)
+        ((mar - timeseries[timeseries < mar])
+         ** 2).sum() / (len(timeseries) - ddof)
     )
     if annualize:
         dr *= np.sqrt(periodicity(timeseries))
     return dr
 
 
 @_requirereturn
@@ -849,15 +850,16 @@
 
     Returns
     -------
     float | pd.Series
         Upside Risk
     """
     ur = np.sqrt(
-        ((timeseries[timeseries > mar] - mar) ** 2).sum() / (len(timeseries) - ddof)
+        ((timeseries[timeseries > mar] - mar)
+         ** 2).sum() / (len(timeseries) - ddof)
     )
     if annualize:
         ur *= np.sqrt(periodicity(timeseries))
     return ur
 
 
 def omega(timeseries: pd.Series | pd.DataFrame, mar: float = 0) -> float:
@@ -1094,15 +1096,16 @@
         3. Simple regression on `n` portfolios (i.e. timeseries is a DataFrame, benchmark is a Series)
         Return type is a DataFrame of shape (4, n). Index types are (float, float, float, float).
         4. Multiple regression on `n` portfolios (i.e. timeseries is a DataFrame, benchmark is a DataFrame)
         Return type is a DataFrame of shape (4, n). Index types (float, Series, float, float).
     """
     if isinstance(timeseries, pd.DataFrame):
         return timeseries.aggregate(lambda x: regress(x, benchmark, rfr_periodic))
-    result = sm.OLS(timeseries - rfr_periodic, sm.add_constant(benchmark)).fit()
+    result = sm.OLS(timeseries - rfr_periodic,
+                    sm.add_constant(benchmark)).fit()
     a = result.params.iloc[0]
     b = result.params.iloc[1:].squeeze()  # Series
     r2 = result.rsquared
     r2adj = result.rsquared_adj
     return pd.Series([a, b, r2, r2adj], index=['alpha', 'betas', 'r2', 'r2adj'])
 
 
@@ -1139,15 +1142,15 @@
         Return type is a Series of shape (k,).
         4. Multiple regression on `k` portfolios (i.e. timeseries is a DataFrame, benchmark is a DataFrame) against `m` benchmarks/factors
         Return type is a Series of shape (k,). Each value is another Series of shape (m,)
 
     Note
     ----
     Benchmark should be already NET of risk-free rate, so this method works for multi-factor analysis
-    """    
+    """
     return regress(timeseries, benchmark, rfr_periodic).iloc[1]
 
 
 @_requirereturn
 @_requirebenchmark
 def alpha(
     timeseries: pd.Series | pd.DataFrame,
@@ -1715,15 +1718,15 @@
 
     Returns
     -------
     float | pd.Series
         Up-market capture ratio
     """
     up = benchmark >= 0
-    return compound_return(timeseries[up]) / compound_return(benchmark[up])
+    return compound_return(timeseries[up], annualize=True) / compound_return(benchmark[up], annualize=True)
 
 
 @_requirereturn
 @_requirebenchmark
 def down_capture(
     timeseries: pd.Series | pd.DataFrame, benchmark: pd.Series | pd.DataFrame
 ) -> float | pd.Series:
@@ -1739,15 +1742,15 @@
 
     Returns
     -------
     float | pd.Series
         Down-market capture ratio
     """
     down = benchmark < 0
-    return compound_return(timeseries[down]) / compound_return(benchmark[down])
+    return compound_return(timeseries[down], annualize=True) / compound_return(benchmark[down], annualize=True)
 
 
 def carino(r: float, b: float) -> float:
     """Smoothing algorithm for multi-period attribution
 
     Parameters
     ----------
```

### Comparing `fintoolkit-0.0.6/toolkit/portfolio.py` & `fintoolkit-0.0.7/toolkit/portfolio.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/.gitignore` & `fintoolkit-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/README.md` & `fintoolkit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.6/pyproject.toml` & `fintoolkit-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fintoolkit"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Chris Cheng", email="kc1116@gmail.com" },
 ]
 description = "Financial Toolkit"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fintoolkit-0.0.6/PKG-INFO` & `fintoolkit-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fintoolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Financial Toolkit
 Project-URL: Homepage, https://github.com/chris-kc-cheng/financial-toolkit
 Project-URL: Bug Tracker, https://github.com/chris-kc-cheng/financial-toolkit/issues
 Author-email: Chris Cheng <kc1116@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

