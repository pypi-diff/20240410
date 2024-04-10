# Comparing `tmp/finalytics-0.2.5.tar.gz` & `tmp/finalytics-0.3.0.tar.gz`

## Comparing `finalytics-0.2.5.tar` & `finalytics-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,41 @@
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 finalytics-0.2.5/Cargo.toml
--rw-r--r--   0     1001      127     6148 2024-01-15 09:30:47.000000 finalytics-0.2.5/.DS_Store
--rw-r--r--   0     1001      127     3107 2024-01-15 09:30:47.000000 finalytics-0.2.5/.github/workflows/CI.yml
--rw-r--r--   0     1001      127       63 2024-01-15 09:30:47.000000 finalytics-0.2.5/.gitignore
--rw-r--r--   0     1001      127      241 2024-01-15 09:30:47.000000 finalytics-0.2.5/.readthedocs.yaml
--rw-r--r--   0     1001      127     1073 2024-01-15 09:30:47.000000 finalytics-0.2.5/LICENSE
--rw-r--r--   0     1001      127     5095 2024-01-15 09:30:47.000000 finalytics-0.2.5/README.md
--rwxr-xr-x   0     1001      127     1578 2024-01-15 09:30:47.000000 finalytics-0.2.5/build.sh
--rw-r--r--   0     1001      127      974 2024-01-15 09:30:47.000000 finalytics-0.2.5/conf.py
--rw-r--r--   0     1001      127  3988172 2024-01-15 09:30:47.000000 finalytics-0.2.5/examples/bitcoin_etf_tracker.ipynb
--rw-r--r--   0     1001      127     9282 2024-01-15 09:30:47.000000 finalytics-0.2.5/examples/portfolio_optimization.ipynb
--rw-r--r--   0     1001      127    51767 2024-01-15 09:30:47.000000 finalytics-0.2.5/examples/security_analysis.ipynb
--rw-r--r--   0     1001      127    17579 2024-01-15 09:30:47.000000 finalytics-0.2.5/index.rst
--rw-r--r--   0     1001      127    18555 2024-01-15 09:30:47.000000 finalytics-0.2.5/src/defi.rs
--rw-r--r--   0     1001      127     3287 2024-01-15 09:30:47.000000 finalytics-0.2.5/src/ffi.rs
--rw-r--r--   0     1001      127      656 2024-01-15 09:30:47.000000 finalytics-0.2.5/src/lib.rs
--rw-r--r--   0     1001      127     9648 2024-01-15 09:30:47.000000 finalytics-0.2.5/src/portfolio.rs
--rw-r--r--   0     1001      127     1817 2024-01-15 09:30:47.000000 finalytics-0.2.5/src/symbols.rs
--rw-r--r--   0     1001      127    25612 2024-01-15 09:30:47.000000 finalytics-0.2.5/src/ticker.rs
--rw-r--r--   0     1001      127   116852 2024-01-15 09:30:47.000000 finalytics-0.2.5/Cargo.lock
--rw-r--r--   0     1001      127      384 2024-01-15 09:30:47.000000 finalytics-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 finalytics-0.2.5/PKG-INFO
+-rw-r--r--   0     1001      127     1213 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/Cargo.toml
+-rw-r--r--   0     1001      127    15865 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/fundamentals.rs
+-rw-r--r--   0     1001      127      145 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     5751 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/optimization.rs
+-rw-r--r--   0     1001      127    10803 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/performance.rs
+-rw-r--r--   0     1001      127     4473 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/sentiment.rs
+-rw-r--r--   0     1001      127    15983 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/statistics.rs
+-rw-r--r--   0     1001      127     8696 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/stochastics.rs
+-rw-r--r--   0     1001      127    23743 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/analytics/technicals.rs
+-rw-r--r--   0     1001      127       34 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/charts/mod.rs
+-rw-r--r--   0     1001      127    10755 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/charts/portfolio.rs
+-rw-r--r--   0     1001      127    23418 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/charts/ticker.rs
+-rw-r--r--   0     1001      127     8319 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/data/db.rs
+-rw-r--r--   0     1001      127    27513 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/data/keys.rs
+-rw-r--r--   0     1001      127       41 2024-04-10 08:21:59.000000 finalytics-0.3.0/finalytics/src/data/mod.rs
+-rw-r--r--   0     1001      127 21766144 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/data/sqlite/symbols.db
+-rw-r--r--   0     1001      127     5283 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/data/symbols.rs
+-rw-r--r--   0     1001      127    21572 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/data/ticker.rs
+-rw-r--r--   0     1001      127     1541 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/lib.rs
+-rw-r--r--   0     1001      127       35 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/models/mod.rs
+-rw-r--r--   0     1001      127     4691 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/models/portfolio.rs
+-rw-r--r--   0     1001      127     9138 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/models/ticker.rs
+-rw-r--r--   0     1001      127     1544 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/utils/chart_utils.rs
+-rw-r--r--   0     1001      127     2419 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/utils/date_utils.rs
+-rw-r--r--   0     1001      127       88 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/utils/mod.rs
+-rw-r--r--   0     1001      127     2324 2024-04-10 08:22:00.000000 finalytics-0.3.0/finalytics/src/utils/web_utils.rs
+-rw-r--r--   0     1001      127     9090 2024-04-10 08:21:59.000000 finalytics-0.3.0/README.md
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 finalytics-0.3.0/python/Cargo.toml
+-rw-r--r--   0     1001      127     3352 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/README.md
+-rwxr-xr-x   0     1001      127     1578 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/build.sh
+-rw-r--r--   0     1001      127      974 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/conf.py
+-rw-r--r--   0     1001      127    12047 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/index.rst
+-rw-r--r--   0     1001      127     2689 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/src/ffi.rs
+-rw-r--r--   0     1001      127      424 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/src/lib.rs
+-rw-r--r--   0     1001      127     9402 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/src/portfolio.rs
+-rw-r--r--   0     1001      127     1740 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/src/symbols.rs
+-rw-r--r--   0     1001      127    24521 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/src/ticker.rs
+-rw-r--r--   0     1001      127     2053 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/test.py
+-rw-r--r--   0     1001      127   116852 2024-04-10 08:22:00.000000 finalytics-0.3.0/python/Cargo.lock
+-rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 finalytics-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 finalytics-0.3.0/PKG-INFO
```

### Comparing `finalytics-0.2.5/build.sh` & `finalytics-0.3.0/python/build.sh`

 * *Files identical despite different names*

### Comparing `finalytics-0.2.5/conf.py` & `finalytics-0.3.0/python/conf.py`

 * *Files identical despite different names*

### Comparing `finalytics-0.2.5/index.rst` & `finalytics-0.3.0/python/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -131,32 +131,30 @@
 
             ticker = finalytics.Ticker("AAPL")
             options_chain = ticker.get_options_chain()
 
 
     .. method:: get_news(start: str, end: str, compute_sentiment: bool) -> dict
 
-      Get the news for the ticker for a given time period.
+      Get the latest news for the ticker.
 
       - **Arguments:**
-            - `start` (`str`): The start date of the time period in the format YYYY-MM-DD.
-            - `end` (`str`): The end date of the time period in the format YYYY-MM-DD.
             - `compute_sentiment` (`bool`): Whether to compute the sentiment of the news articles.
 
       - **Returns:**
             - `dict`: A dictionary containing the news articles (and sentiment results if requested).
 
       - **Example:**
 
          .. code-block:: python
 
             import finalytics
 
             ticker = finalytics.Ticker("AAPL")
-            news = ticker.get_news("2020-01-01", "2020-12-31", False)
+            news = ticker.get_news(False)
 
 
     .. method:: get_income_statement() -> DataFrame
 
       Get the Income Statement for the ticker.
 
       - **Returns:**
@@ -255,15 +253,15 @@
       - **Arguments:**
             - `start` (`str`): The start date of the time period in the format YYYY-MM-DD.
             - `end` (`str`): The end date of the time period in the format YYYY-MM-DD.
             - `interval` (`str`): The interval of the data (2m, 5m, 15m, 30m, 1h, 1d, 1wk, 1mo, 3mo).
             - `benchmark` (`str`): The ticker symbol of the benchmark to compare against.
             - `confidence_level` (`float`): The confidence level for the VaR and ES calculations.
             - `risk_free_rate` (`float`): The risk free rate to use in the calculations.
-            - `display_format` (`str`): The format to display the chart in (png, html, notebook, colab).
+            - `display_format` (`str`): The format to display the chart in (png, html, notebook).
 
       - **Example:**
 
          .. code-block:: python
 
             import finalytics
 
@@ -275,15 +273,15 @@
 
       Display the candlestick chart for the ticker.
 
       - **Arguments:**
             - `start` (`str`): The start date of the time period in the format YYYY-MM-DD.
             - `end` (`str`): The end date of the time period in the format YYYY-MM-DD.
             - `interval` (`str`): The interval of the data (2m, 5m, 15m, 30m, 1h, 1d, 1wk, 1mo, 3mo).
-            - `display_format` (`str`): The format to display the chart in (png, html, notebook, colab).
+            - `display_format` (`str`): The format to display the chart in (png, html, notebook).
 
       - **Example:**
 
          .. code-block:: python
 
             import finalytics
 
@@ -375,183 +373,8 @@
       - **Example:**
 
          .. code-block:: python
 
             import finalytics
 
             portfolio = finalytics.Portfolio(["AAPL", "GOOG", "MSFT"], "^GSPC", "2020-01-01", "2021-01-01", "1d", 0.95, 0.02, 1000, "max_sharpe")
-            portfolio.display_portfolio_charts("optimization","html")
-
-
-
-DeFi Module
--------------
-
-This module contains the `DefiPools` and `DefiBalances` classes.
-
-.. class:: DefiPools
-
-   DefiPools is a class that provides information about DeFi liquidity pools.
-
-   .. method:: __init__() -> DefiPools
-
-      Create a new `DefiPools` object.
-
-      - **Returns:**
-            - `DefiPools`: A DefiPools object.
-
-      - **Example:**
-
-         .. code-block:: python
-
-            import finalytics
-
-            defi_pools = finalytics.DefiPools()
-            print(f"Total Value Locked: ${defi_pools.total_value_locked:,.0f}")
-            print(defi_pools.pools_data)
-
-
-   .. method:: search_pools_by_symbol(symbol: str) -> List[str]
-
-      Search the pools data for pools that match the search term.
-
-      - **Arguments:**
-            - `symbol` (`str`): Cryptocurrency symbol.
-
-      - **Returns:**
-            - `List[str]`: List of pools that match the search term.
-
-      - **Example:**
-
-         .. code-block:: python
-
-            import finalytics
-
-            defi_pools = finalytics.DefiPools()
-            print(defi_pools.search_pools_by_symbol("USDC"))
-
-
-   .. method:: display_top_protocols_by_tvl(pool_symbol: str, num_protocols: int, display_format: str)
-
-      Display the top protocols for a given symbol by total value locked.
-
-      - **Arguments:**
-            - `pool_symbol` (`str`): Liquidity pool symbol.
-            - `num_protocols` (`int`): Number of protocols to display.
-            - `display_format` (`str`): Display format for the chart (html, svg, notebook, colab).
-
-      - **Example:**
-
-         .. code-block:: python
-
-            import finalytics
-
-            defi_pools = finalytics.DefiPools()
-            defi_pools.display_top_protocols_by_tvl("USDC-USDT", 20, "html")
-
-
-   .. method:: display_top_protocols_by_apy(pool_symbol: str, num_protocols: int, display_format: str)
-
-      Display the top protocols for a given symbol by APY.
-
-      - **Arguments:**
-            - `pool_symbol` (`str`): Liquidity pool symbol.
-            - `num_protocols` (`int`): Number of protocols to display.
-            - `display_format` (`str`): Display format for the chart (html, svg, notebook, colab).
-
-      - **Example:**
-
-         .. code-block:: python
-
-            import finalytics
-
-            defi_pools = finalytics.DefiPools()
-            defi_pools.display_top_protocols_by_apy("USDC-USDT", 20, "html")
-
-
-   .. method:: display_pool_tvl_history(pool_symbol: str, protocol: str, chain: str, display_format: str)
-
-      Display the total value locked history for a given pool.
-
-      - **Arguments:**
-            - `pool_symbol` (`str`): Liquidity pool symbol.
-            - `protocol` (`str`): Protocol.
-            - `chain` (`str`): Blockchain.
-            - `display_format` (`str`): Display format for the chart (html, svg, notebook, colab).
-
-      - **Example:**
-
-         .. code-block:: python
-
-            import finalytics
-
-            defi_pools = finalytics.DefiPools()
-            defi_pools.display_pool_tvl_history("USDC-USDT", "uniswap-v3", "ethereum", "html")
-
-
-   .. method:: display_pool_apy_history(pool_symbol: str, protocol: str, chain: str, display_format: str)
-
-      Display the APY history for a given pool.
-
-      - **Arguments:**
-            - `pool_symbol` (`str`): Liquidity pool symbol.
-            - `protocol` (`str`): Protocol.
-            - `chain` (`str`): Blockchain.
-            - `display_format` (`str`): Display format for the chart (html, svg, notebook, colab).
-
-      - **Example:**
-
-         .. code-block:: python
-
-            import finalytics
-
-            defi_pools = finalytics.DefiPools()
-            defi_pools.display_pool_apy_history("USDC-USDT", "uniswap-v3", "ethereum", "html")
-
-
-
-.. class:: DefiBalances
-
-   The DefiBalances class enables you to fetch DeFi Users' wallet & protocol balances.
-
-   .. method:: __init__(protocols: List[str], chains: List[str], address: str, display_format: str) -> DefiBalances
-
-      Initializes a new `DefiBalances` object.
-
-      - **Arguments:**
-            - `protocols` (`List[str]`): List of protocols to fetch balances for.
-            - `chains` (`List[str]`): List of chains to fetch balances for.
-            - `address` (`str`): Wallet address to fetch balances for.
-            - `display_format` (`str`): Display format for the chart (html, svg, notebook, colab).
-
-      - **Returns:**
-            - `DefiBalances`: A DefiBalances object.
-
-      - **Example:**
-
-         .. code-block:: python
-
-            import finalytics
-
-            defi_balances = finalytics.DefiBalances(["wallet", "eigenlayer", "blast", "ether.fi"],
-                                                       ["ethereum", "arbitrum"],
-                                                       "0x7ac34681f6aaeb691e150c43ee494177c0e2c183",
-                                                       "html")
-            print(defi_balances.balances)
-
-
-
-.. function:: get_supported_protocols() -> Dict[str, List[str]]
-
-  Fetches the supported protocols and chains for the `DefiBalances` class.
-
-  - **Returns:**
-        - `Dict[str, List[str]]`: Dictionary of protocols and chains.
-
-  - **Example:**
-
-     .. code-block:: python
-
-        import finalytics
-
-        supported_protocols = finalytics.get_supported_protocols()
-        print(supported_protocols)
+            portfolio.display_portfolio_charts("optimization","html")
```

### Comparing `finalytics-0.2.5/src/ffi.rs` & `finalytics-0.3.0/python/src/ffi.rs`

 * *Files 15% similar despite different names*

```diff
@@ -86,27 +86,7 @@
 
         let iframe = jupyter.call_method1("IFrame", (file_path, 1000, 800))?;
 
         jupyter.call_method1("display", (iframe,))?;
         Ok(())
     })
 }
-
-pub fn display_html(plot: Option<Plot>, chart_type: &str) -> Result<(), Box<dyn Error>> {
-    let file_path = format!("{}.html", chart_type);
-
-    if plot != None {
-        let mut plot = plot.clone().unwrap();
-        let layout = plot.layout().clone().width(1000).height(800);
-        plot.set_layout(layout);
-        let html = plot.to_html();
-        std::fs::write(&file_path, html)?;
-    }
-
-    Python::with_gil(|py| {
-        let jupyter = py.import("IPython.display")?;
-
-        // Display the HTML
-        jupyter.call_method1("display_html", (file_path, true))?;
-        Ok(())
-    })
-}
```

### Comparing `finalytics-0.2.5/src/portfolio.rs` & `finalytics-0.3.0/python/src/portfolio.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-use finalytics::analytics::optimization::ObjectiveFunction;
-use finalytics::data::ticker::Interval;
-use finalytics::PortfolioCharts;
-use finalytics::utils::chart_utils::PlotImage;
+use finalytics::prelude::*;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 use tokio::task;
-use crate::ffi::{display_html, display_html_with_iframe, rust_df_to_py_df, rust_series_to_py_series};
+use crate::ffi::{display_html_with_iframe, rust_df_to_py_df, rust_series_to_py_series};
 
 
 #[pyclass]
 #[pyo3(name = "Portfolio")]
 pub struct PyPortfolio {
-    pub portfolio: PortfolioCharts
+    pub portfolio: Portfolio
 }
 
 #[pymethods]
 impl PyPortfolio {
     #[new]
     /// Create a new Portfolio object
     ///
@@ -38,23 +35,25 @@
     /// # Example
     ///
     /// ```
     /// import finalytics
     ///
     /// portfolio = finalytics.Portfolio(["AAPL", "GOOG", "MSFT", "ZN=F"], "^GSPC", "2020-01-01", "2021-01-01", "1d", 0.95, 0.02, 1000, "max_sharpe")
     /// ```
-    pub fn new(ticker_symbols: Vec<String>, benchmark_symbol: String, start_date: String, end_date: String,
+    pub fn new(ticker_symbols: Vec<&str>, benchmark_symbol: String, start_date: String, end_date: String,
                interval: String, confidence_level: f64, risk_free_rate: f64, max_iterations: u64, objective_function: String) -> Self {
         task::block_in_place(move || {
             let interval = Interval::from_str(&interval);
             let objective_function = ObjectiveFunction::from_str(&objective_function);
             let portfolio = tokio::runtime::Runtime::new().unwrap().block_on(
-                PortfolioCharts::new(ticker_symbols, &benchmark_symbol, &start_date, &end_date,
-                                     interval, confidence_level, risk_free_rate, max_iterations,
-                                     objective_function)).unwrap();
+                PortfolioBuilder::new().ticker_symbols(ticker_symbols).benchmark_symbol(&benchmark_symbol)
+                    .start_date(&start_date).end_date(&end_date).interval(interval)
+                    .confidence_level(confidence_level).risk_free_rate(risk_free_rate)
+                    .max_iterations(max_iterations).objective_function(objective_function)
+                    .build()).unwrap();
             PyPortfolio {
                 portfolio
             }
         })
     }
 
     /// get the portfolio optimization results
@@ -152,17 +151,12 @@
                     println!("chart written to {}.png", chart_type);
                 },
                 "notebook" => {
                     if let Err(err) = display_html_with_iframe(Some(chart), &chart_type) {
                         eprintln!("Error displaying HTML with iframe: {:?}", err);
                     }
                 },
-                "colab" => {
-                    if let Err(err) = display_html(Some(chart), &chart_type) {
-                        eprintln!("Error displaying HTML: {:?}", err);
-                    }
-                },
                 _ => panic!("display_format must be one of: html, png, notebook or colab")
             }
         })
     }
 }
```

### Comparing `finalytics-0.2.5/src/symbols.rs` & `finalytics-0.3.0/python/src/symbols.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 use std::collections::HashMap;
-use finalytics::data::keys::{AssetClass, Category, Exchange};
-use finalytics::database::db::get_symbols;
+use finalytics::prelude::*;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
 #[pyfunction]
 #[pyo3(name = "get_symbols")]
 /// Fetches ticker symbols that closely match the specified query and asset class
 ///
```

### Comparing `finalytics-0.2.5/src/ticker.rs` & `finalytics-0.3.0/python/src/ticker.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-use pyo3::prelude::*;
 use tokio::task;
-use finalytics::data::ticker::{Interval, Ticker};
-use finalytics::{Financials, TickerCharts, TickerPerformanceStats};
+use pyo3::prelude::*;
 use pyo3::types::PyDict;
-use finalytics::utils::chart_utils::PlotImage;
-use crate::ffi::{rust_df_to_py_df, rust_series_to_py_series, display_html_with_iframe, display_html};
+use finalytics::prelude::*;
+use crate::ffi::{rust_df_to_py_df, rust_series_to_py_series, display_html_with_iframe};
 
 #[pyclass]
 #[pyo3(name = "Ticker")]
 pub struct PyTicker {
     #[pyo3(get, set)]
     pub symbol: String,
     #[pyo3(get, set)]
@@ -39,23 +37,23 @@
     ///
     /// ```
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// print(ticker.symbol, ticker.name, ticker.category, ticker.asset_class, ticker.exchange)
     /// ```
-    pub fn new(symbol: String) -> Self {
+    pub fn new(symbol: &str) -> Self {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(Ticker::new(&symbol)).unwrap();
+            let ticker = TickerBuilder::new().ticker(symbol).unwrap().build().unwrap();
             PyTicker {
-                symbol: ticker.symbol,
-                name: ticker.name,
-                category: ticker.category,
-                asset_class: ticker.asset_class,
-                exchange: ticker.exchange,
+                symbol: ticker.ticker.symbol,
+                name: ticker.ticker.name,
+                category: ticker.ticker.category,
+                asset_class: ticker.ticker.asset_class,
+                exchange: ticker.ticker.exchange,
             }
         })
     }
 
     /// Get the current price of the ticker
     ///
     /// # Returns
@@ -68,17 +66,15 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// current_price = ticker.get_current_price()
     /// ```
     pub fn get_current_price(&self) -> f64 {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Ticker::new(&self.symbol)
-            ).unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
             let current_price = tokio::runtime::Runtime::new().unwrap().block_on(ticker.get_quote()).unwrap();
             current_price
         })
     }
 
     /// Get summary technical and fundamental statistics for the ticker
     ///
@@ -92,17 +88,15 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// summary_stats = ticker.get_summary_stats()
     /// ```
     pub fn get_summary_stats(&self) -> Py<PyDict>  {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Ticker::new(&self.symbol)
-            ).unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
             let ticker_stats = tokio::runtime::Runtime::new().unwrap().block_on(
                 ticker.get_ticker_stats()
             ).unwrap();
             // convert ticker stats to pydict
             Python::with_gil(|py| {
                 let locals = PyDict::new(py);
                 locals.set_item("Symbol", ticker_stats.symbol).unwrap();
@@ -158,20 +152,18 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// ohlcv = ticker.get_price_history("2020-01-01", "2020-12-31", "1d")
     /// ```
     pub fn get_price_history(&self, start: String, end: String, interval: String) -> PyObject {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Ticker::new(&self.symbol)
-            ).unwrap();
             let interval = Interval::from_str(&interval);
             let price_history = tokio::runtime::Runtime::new().unwrap().block_on(
-                ticker.get_chart(&start, &end, interval)
+                TickerBuilder::new().ticker(&self.symbol).unwrap().start_date(&start).end_date(&end)
+                    .interval(interval).build().unwrap().get_chart()
             ).unwrap();
             let df = rust_df_to_py_df(&price_history).unwrap();
             df
         })
     }
 
     /// Get the options chain for the ticker
@@ -186,52 +178,46 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// options_chain = ticker.get_options_chain()
     /// ```
     pub fn get_options_chain(&self) -> PyObject {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Ticker::new(&self.symbol)
-            ).unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
             let options_chain = tokio::runtime::Runtime::new().unwrap().block_on(
                 ticker.get_options()
             ).unwrap().chain;
             let df = rust_df_to_py_df(&options_chain).unwrap();
             df
         })
     }
 
-    /// Get the news for the ticker for a given time period
+    /// Get the latest news for the given ticker
     ///
     /// # Arguments
     ///
-    /// * `start` - `str` - The start date of the time period in the format YYYY-MM-DD
-    /// * `end` - `str` - The end date of the time period in the format YYYY-MM-DD
     /// * `compute_sentiment` - `bool` - Whether to compute the sentiment of the news articles (set to false to speed up the process)
     ///
     /// # Returns
     ///
     /// `dict` - A dictionary containing the news articles (and sentiment results if requested)
     ///
     /// # Example
     ///
     /// ```
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
-    /// news = ticker.get_news("2020-01-01", "2020-12-31", False)
+    /// news = ticker.get_news(False)
     /// ```
-    pub fn get_news(&self, start: String, end: String, compute_sentiment: bool) -> PyObject {
+    pub fn get_news(&self, compute_sentiment: bool) -> PyObject {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Ticker::new(&self.symbol)
-            ).unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
             let news = tokio::runtime::Runtime::new().unwrap().block_on(
-                ticker.get_news(&start, &end, compute_sentiment)
+                ticker.get_news(compute_sentiment)
             ).unwrap();
 
             Python::with_gil(|py| {
                 let locals = PyDict::new(py);
                 for (i, article) in news.iter().enumerate() {
                     let article_dict = PyDict::new(py);
                     article_dict.set_item("Title", article.title.clone()).unwrap();
@@ -263,18 +249,17 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// income_statement = ticker.get_income_statement()
     /// ```
     pub fn get_income_statement(&self) -> PyObject {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Financials::new(&self.symbol)
-            ).unwrap();
-            let income_statement = ticker.format_income_statement().unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
+            let income_statement = tokio::runtime::Runtime::new().unwrap().block_on(
+                ticker.income_statement()).unwrap();
             let df = rust_df_to_py_df(&income_statement).unwrap();
             df
         })
     }
 
     /// Get the Balance Sheet for the ticker
     ///
@@ -288,18 +273,17 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// balance_sheet = ticker.get_balance_sheet()
     /// ```
     pub fn get_balance_sheet(&self) -> PyObject {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Financials::new(&self.symbol)
-            ).unwrap();
-            let balance_sheet = ticker.format_balance_sheet().unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
+            let balance_sheet = tokio::runtime::Runtime::new().unwrap().block_on(
+                ticker.balance_sheet()).unwrap();
             let df = rust_df_to_py_df(&balance_sheet).unwrap();
             df
         })
     }
 
     /// Get the Cashflow Statement for the ticker
     ///
@@ -313,18 +297,17 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// cashflow_statement = ticker.get_cashflow_statement()
     /// ```
     pub fn get_cashflow_statement(&self) -> PyObject {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Financials::new(&self.symbol)
-            ).unwrap();
-            let cashflow_statement = ticker.format_cashflow_statement().unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
+            let cashflow_statement = tokio::runtime::Runtime::new().unwrap().block_on(
+                ticker.cashflow_statement()).unwrap();
             let df = rust_df_to_py_df(&cashflow_statement).unwrap();
             df
         })
     }
 
     /// Get the Financial Ratios for the ticker
     ///
@@ -338,18 +321,17 @@
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// financial_ratios = ticker.get_financial_ratios()
     /// ```
     pub fn get_financial_ratios(&self) -> PyObject {
         task::block_in_place(move || {
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                Financials::new(&self.symbol)
-            ).unwrap();
-            let ratios = ticker.compute_ratios().unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().build().unwrap();
+            let ratios = tokio::runtime::Runtime::new().unwrap().block_on(
+                ticker.financial_ratios()).unwrap();
             let df = rust_df_to_py_df(&ratios).unwrap();
             df
         })
     }
 
     /// Compute the performance statistics for the ticker
     ///
@@ -374,18 +356,19 @@
     /// ticker = finalytics.Ticker("AAPL")
     /// performance_stats = ticker.compute_performance_stats("2020-01-01", "2020-12-31", "1d", "^GSPC", 0.95, 0.02)
     /// ```
     pub fn compute_performance_stats(&self, start: String, end: String, interval: String, benchmark: String,
                                      confidence_level: f64, risk_free_rate: f64) -> PyObject {
         task::block_in_place(move || {
             let interval = Interval::from_str(&interval);
-            let ticker = tokio::runtime::Runtime::new().unwrap().block_on(
-                TickerPerformanceStats::new(&self.symbol, &benchmark, &start, &end, interval, confidence_level, risk_free_rate)
-            ).unwrap();
-            let performance_stats = ticker.compute_stats().unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().start_date(&start).end_date(&end)
+                .interval(interval).benchmark_symbol(&benchmark).confidence_level(confidence_level)
+                .risk_free_rate(risk_free_rate).build().unwrap();
+            let performance_stats = tokio::runtime::Runtime::new().unwrap().block_on(
+                ticker.performance_stats()).unwrap();
             // convert ticker performance stats struct to pydict
             Python::with_gil(|py| {
                 let locals = PyDict::new(py);
                 locals.set_item("Symbol", performance_stats.ticker_symbol).unwrap();
                 locals.set_item("Benchmark", performance_stats.benchmark_symbol).unwrap();
                 locals.set_item("Start Date", performance_stats.start_date).unwrap();
                 locals.set_item("End Date", performance_stats.end_date).unwrap();
@@ -422,33 +405,33 @@
     ///
     /// * `start` - `str` - The start date of the time period in the format YYYY-MM-DD
     /// * `end` - `str` - The end date of the time period in the format YYYY-MM-DD
     /// * `interval` - `str` - The interval of the data (2m, 5m, 15m, 30m, 1h, 1d, 1wk, 1mo, 3mo)
     /// * `benchmark` - `str` - The ticker symbol of the benchmark to compare against
     /// * `confidence_level` - `float` - The confidence level for the VaR and ES calculations
     /// * `risk_free_rate` - `float` - The risk free rate to use in the calculations
-    /// * `display_format` - `str` - The format to display the chart in (png, html, notebook, colab)
+    /// * `display_format` - `str` - The format to display the chart in (png, html, notebook)
     ///
     /// # Example
     ///
     /// ```
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// ticker.display_performance_chart("2020-01-01", "2020-12-31", "1d", "^GSPC", 0.95, 0.02, "html")
     /// ```
     pub fn display_performance_chart(&self, start: String, end: String, interval: String, benchmark: String,
                                      confidence_level: f64, risk_free_rate: f64, display_format: String)  {
         task::block_in_place(move || {
             let interval = Interval::from_str(&interval);
-            let chart = TickerCharts::new(&self.symbol,  &start,
-                                          &end, interval, &benchmark, confidence_level, risk_free_rate).unwrap();
-
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().start_date(&start).end_date(&end)
+                .interval(interval).benchmark_symbol(&benchmark).confidence_level(confidence_level)
+                .risk_free_rate(risk_free_rate).build().unwrap();
             let performance_chart = tokio::runtime::Runtime::new().unwrap().block_on(
-                chart.performance_chart()).unwrap();
+                ticker.performance_chart()).unwrap();
 
             match display_format.as_str() {
                 "png" => {
                     performance_chart.to_png("ticker_performance_chart.png",  1500, 1200, 1.0);
                     println!("Chart Saved to ticker_performance_chart.png");
                 },
                 "html" => {
@@ -456,51 +439,45 @@
                     println!("Chart Saved to ticker_performance_chart.html");
                 },
                 "notebook" => {
                     if let Err(err) = display_html_with_iframe(Some(performance_chart), "performance_chart") {
                         eprintln!("Error displaying HTML with iframe: {:?}", err);
                     }
                 },
-                "colab" => {
-                    if let Err(err) = display_html(Some(performance_chart), "performance_chart") {
-                        eprintln!("Error displaying HTML: {:?}", err);
-                    }
-                },
                 _ => {
-                    println!("Invalid output format. Please choose either 'png', 'html', notebook or colab");
+                    println!("Invalid output format. Please choose either 'png', 'html', or 'notebook'");
                 }
             }
         })
     }
 
     /// Display the candlestick chart for the ticker
     ///
     /// # Arguments
     ///
     /// * `start` - `str` - The start date of the time period in the format YYYY-MM-DD
     /// * `end` - `str` - The end date of the time period in the format YYYY-MM-DD
     /// * `interval` - `str` - The interval of the data (2m, 5m, 15m, 30m, 1h, 1d, 1wk, 1mo, 3mo)
-    /// * `display_format` - `str` - The format to display the chart in (png, html, notebook, colab)
+    /// * `display_format` - `str` - The format to display the chart in (png, html, notebook)
     ///
     /// # Example
     ///
     /// ```
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// ticker.display_candlestick_chart("2020-01-01", "2020-12-31", "1d", "html")
     /// ```
     pub fn display_candlestick_chart(&self, start: String, end: String, interval: String, display_format: String)  {
         task::block_in_place(move || {
             let interval = Interval::from_str(&interval);
-            let chart = TickerCharts::new(&self.symbol,  &start,
-                                          &end, interval, "", 0.0, 0.0).unwrap();
-
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().start_date(&start).end_date(&end)
+                .interval(interval).build().unwrap();
             let candlestick_chart = tokio::runtime::Runtime::new().unwrap().block_on(
-                chart.candlestick_chart()).unwrap();
+                ticker.candlestick_chart()).unwrap();
 
             match display_format.as_str() {
                 "png" => {
                     candlestick_chart.to_png("candlestick_chart.png",  1500, 1200, 1.0);
                     println!("Chart Saved to candlestick_chart.png")
                 },
                 "html" => {
@@ -508,55 +485,48 @@
                     println!("Chart Saved to candlestick_chart.html");
                 },
                 "notebook" => {
                     if let Err(err) = display_html_with_iframe(Some(candlestick_chart), "candlestick_chart") {
                         eprintln!("Error displaying HTML with iframe: {:?}", err);
                     }
                 },
-                "colab" => {
-                    if let Err(err) = display_html(Some(candlestick_chart), "candlestick_chart") {
-                        eprintln!("Error displaying HTML: {:?}", err);
-                    }
-                },
                 _ => {
-                    println!("Invalid output format. Please choose either 'png', 'html', 'notebook' or 'colab'");
+                    println!("Invalid output format. Please choose either 'png', 'html' or 'notebook'");
                 }
             }
         })
     }
 
     /// Display the options volatility surface, smile and term structure charts for the ticker
     ///
     /// # Arguments
     ///
     /// * `risk_free_rate` - `float` - The risk free rate to use in the calculations
     /// * `chart_type` - `str` - The type of options volatility chart to display (surface, smile, term_structure)
-    /// * `display_format` - `str` - The format to display the chart in (png, html, notebook, colab)
+    /// * `display_format` - `str` - The format to display the chart in (png, html, notebook)
     ///
     /// # Example
     ///
     /// ```
     /// import finalytics
     ///
     /// ticker = finalytics.Ticker("AAPL")
     /// ticker.display_options_chart(0.02, "surface", "html")
     /// ```
     pub fn display_options_chart(&self, risk_free_rate: f64, chart_type: String,  display_format: String)  {
         task::block_in_place(move || {
-            let interval = Interval::from_str("1d");
-            let chart = TickerCharts::new(&self.symbol,  "",
-                                          "", interval, "", 0.0, risk_free_rate).unwrap();
+            let ticker = TickerBuilder::new().ticker(&self.symbol).unwrap().risk_free_rate(risk_free_rate).build().unwrap();
 
             let options_chart = tokio::runtime::Runtime::new().unwrap().block_on(
-                chart.options_volatility_charts()).unwrap();
+                ticker.volatility_charts()).unwrap();
 
             let plot = match chart_type.as_str() {
-                "surface" => options_chart.get(0).unwrap().clone(),
-                "smile" => options_chart.get(1).unwrap().clone(),
-                "term_structure" => options_chart.get(2).unwrap().clone(),
+                "surface" => options_chart.get("Volatility Surface").unwrap().clone(),
+                "smile" => options_chart.get("Volatility Smile").unwrap().clone(),
+                "term_structure" => options_chart.get("Volatility Term Structure").unwrap().clone(),
                 _ => panic!("Invalid chart type. Please choose either 'surface', 'smile' or 'term_structure'"),
             };
 
             match display_format.as_str() {
                 "png" => {
                     plot.to_png(format!("{}.png", chart_type).as_str(),  1500, 1200, 1.0);
                     println!("{}.png", chart_type);
@@ -566,21 +536,16 @@
                     println!("{}.html", chart_type);
                 },
                 "notebook" => {
                     if let Err(err) = display_html_with_iframe(Some(plot), &chart_type) {
                         eprintln!("Error displaying HTML with iframe: {:?}", err);
                     }
                 },
-                "colab" => {
-                    if let Err(err) = display_html(Some(plot), &chart_type) {
-                        eprintln!("Error displaying HTML: {:?}", err);
-                    }
-                },
                 _ => {
-                    println!("Invalid output format. Please choose either 'png', 'html', 'notebook' or 'colab'");
+                    println!("Invalid output format. Please choose either 'png', 'html' or 'notebook'");
                 }
             }
 
         })
     }
 }
```

### Comparing `finalytics-0.2.5/Cargo.lock` & `finalytics-0.3.0/python/Cargo.lock`

 * *Files identical despite different names*

