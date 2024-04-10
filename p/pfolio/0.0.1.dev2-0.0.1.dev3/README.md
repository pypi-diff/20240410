# Comparing `tmp/pfolio-0.0.1.dev2.tar.gz` & `tmp/pfolio-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfolio-0.0.1.dev2.tar", max compression
+gzip compressed data, was "pfolio-0.0.1.dev3.tar", max compression
```

## Comparing `pfolio-0.0.1.dev2.tar` & `pfolio-0.0.1.dev3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11355 2024-04-05 14:48:06.450848 pfolio-0.0.1.dev2/LICENSE
--rw-r--r--   0        0        0      407 2024-04-06 14:00:28.815973 pfolio-0.0.1.dev2/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:44:19.444627 pfolio-0.0.1.dev2/pfolio/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 19:44:39.618232 pfolio-0.0.1.dev2/pfolio/analyses/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 18:48:22.745728 pfolio-0.0.1.dev2/pfolio/analyses/factor_analysis/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 18:48:20.086983 pfolio-0.0.1.dev2/pfolio/analyses/scenario_analysis/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 17:47:37.550178 pfolio-0.0.1.dev2/pfolio/analytics/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 19:47:26.782131 pfolio-0.0.1.dev2/pfolio/analytics/returns.py
--rw-r--r--   0        0        0        0 2024-04-06 19:47:16.665083 pfolio-0.0.1.dev2/pfolio/analytics/risks.py
--rw-r--r--   0        0        0       87 2024-04-07 08:32:09.408511 pfolio-0.0.1.dev2/pfolio/main.py
--rw-r--r--   0        0        0        0 2024-04-06 18:13:09.421752 pfolio-0.0.1.dev2/pfolio/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 18:24:19.905612 pfolio-0.0.1.dev2/pfolio/statistics/__init__.py
--rw-r--r--   0        0        0     2146 2024-04-10 07:24:01.264911 pfolio-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 pfolio-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-05 14:48:06.450848 pfolio-0.0.1.dev3/LICENSE
+-rw-r--r--   0        0        0      447 2024-04-10 08:23:30.270921 pfolio-0.0.1.dev3/README.md
+-rw-r--r--   0        0        0      108 2024-04-10 08:35:08.896316 pfolio-0.0.1.dev3/pfolio/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:44:39.618232 pfolio-0.0.1.dev3/pfolio/analyses/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:48:22.745728 pfolio-0.0.1.dev3/pfolio/analyses/factor_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:48:20.086983 pfolio-0.0.1.dev3/pfolio/analyses/scenario_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:47:37.550178 pfolio-0.0.1.dev3/pfolio/analytics/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:47:26.782131 pfolio-0.0.1.dev3/pfolio/analytics/returns.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:47:16.665083 pfolio-0.0.1.dev3/pfolio/analytics/risks.py
+-rw-r--r--   0        0        0       87 2024-04-07 08:32:09.408511 pfolio-0.0.1.dev3/pfolio/main.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:13:09.421752 pfolio-0.0.1.dev3/pfolio/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:24:19.905612 pfolio-0.0.1.dev3/pfolio/statistics/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 08:43:30.852078 pfolio-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 pfolio-0.0.1.dev3/PKG-INFO
```

### Comparing `pfolio-0.0.1.dev2/LICENSE` & `pfolio-0.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `pfolio-0.0.1.dev2/pyproject.toml` & `pfolio-0.0.1.dev3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "pfolio"
-version = "0.0.1.dev2"
-description = ""
+version = "0.0.1.dev3"
+description = "Portfolio Management Library, including analysis, analytics and optimization"
 license = "Apache-2.0"
 authors = ["Stephen Yau <softwareentrepreneer+pfolio@gmail.com>"]
 readme = "README.md"
 homepage = "https://pfund.ai"
 repository = "https://github.com/PFund-Software-Ltd/pfolio"
 documentation = "https://pfolio-docs.pfund.ai"
 keywords = ["portfolio management", "investment", "analytics", "fundamental analysis"]
 
 [tool.poetry.dependencies]
 python = ">=3.10 <3.13"
-pfund = "^0.0.1.dev9"
-statsmodels = "^0.14.1"
-scikit-learn = "^1.4.2"
+pfund = "^0.0.1.dev10"
+statsmodels = "^0.14.0"
+scikit-learn = "^1.3.1"
 plotly = "^5.20.0"
 seaborn = "^0.13.2"
-pfeed = { version = "^0.0.1.dev9", optional = true, extras = ["df", "data", "boost"] }
+pfeed = { version = "^0.0.1.dev10", optional = true, extras = ["df", "data", "boost"] }
 financedatabase = { version = "^2.2.2", optional = true }
 pymc = { version = "^5.12.0", optional = true }
 pyro-ppl = { version = "^1.9.0", optional = true }
 arviz = { version = "^0.18.0", optional = true }
 cvxpy = { version = "^1.4.2", optional = true }
 skfolio = { version = "^0.1.3", optional = true }
 pyportfolioopt = { version = "^1.5.5", optional = true }
```

### Comparing `pfolio-0.0.1.dev2/PKG-INFO` & `pfolio-0.0.1.dev3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pfolio
-Version: 0.0.1.dev2
-Summary: 
+Version: 0.0.1.dev3
+Summary: Portfolio Management Library, including analysis, analytics and optimization
 Home-page: https://pfund.ai
 License: Apache-2.0
 Keywords: portfolio management,investment,analytics,fundamental analysis
 Author: Stephen Yau
 Author-email: softwareentrepreneer+pfolio@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,35 +22,37 @@
 Requires-Dist: cvxpy (>=1.4.2,<2.0.0) ; extra == "portfolio"
 Requires-Dist: empyrial (>=2.1.4,<3.0.0) ; extra == "temporary"
 Requires-Dist: empyrical-reloaded (>=0.5.9,<0.6.0) ; extra == "temporary"
 Requires-Dist: ffn (>=1.0.1,<2.0.0)
 Requires-Dist: financedatabase (>=2.2.2,<3.0.0) ; extra == "data"
 Requires-Dist: financetoolkit (>=1.8.5,<2.0.0) ; extra == "temporary"
 Requires-Dist: finquant (>=0.7.0,<0.8.0) ; extra == "temporary"
-Requires-Dist: pfeed[boost,data,df] (>=0.0.1.dev9,<0.0.2) ; extra == "data"
-Requires-Dist: pfund (>=0.0.1.dev9,<0.0.2)
+Requires-Dist: pfeed[boost,data,df] (>=0.0.1.dev10,<0.0.2) ; extra == "data"
+Requires-Dist: pfund (>=0.0.1.dev10,<0.0.2)
 Requires-Dist: plotly (>=5.20.0,<6.0.0)
 Requires-Dist: pyfolio-reloaded (>=0.9.5,<0.10.0) ; extra == "temporary"
 Requires-Dist: pymc (>=5.12.0,<6.0.0) ; extra == "bayesian"
 Requires-Dist: pyportfolioopt (>=1.5.5,<2.0.0) ; extra == "portfolio"
 Requires-Dist: pyro-ppl (>=1.9.0,<2.0.0) ; extra == "bayesian"
 Requires-Dist: quantstats (>=0.0.62,<0.0.63)
 Requires-Dist: riskfolio-lib (>=6.0.0,<7.0.0) ; extra == "portfolio"
 Requires-Dist: rsome (>=1.2.6,<2.0.0) ; extra == "temporary"
-Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: scikit-learn (>=1.3.1,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: skfolio (>=0.1.3,<0.2.0) ; extra == "portfolio"
-Requires-Dist: statsmodels (>=0.14.1,<0.15.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: thepassiveinvestor (>=1.2.2,<2.0.0) ; extra == "temporary"
 Project-URL: Documentation, https://pfolio-docs.pfund.ai
 Project-URL: Repository, https://github.com/PFund-Software-Ltd/pfolio
 Description-Content-Type: text/markdown
 
 # pfolio
 
+> **still designing, NOT WORKING YET**
+
 It is a wrapper of the existing portfolio management packages, eventually it will be a true package on its own.
 
 
 > Ultimate Goal: It will be the backend of an open-source version of a portfolio analysis tool, like Two Sigma's Venn, or Bloomberg's PORT.
 
 Refereces: \
 [Portfolio Visualizer](https://www.portfoliovisualizer.com) \
```

