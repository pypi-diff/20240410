# Comparing `tmp/lumibot-3.3.4.tar.gz` & `tmp/lumibot-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.3.4.tar", last modified: Wed Apr 10 05:23:49 2024, max compression
+gzip compressed data, was "lumibot-3.3.5.tar", last modified: Wed Apr 10 20:58:06 2024, max compression
```

## Comparing `lumibot-3.3.4.tar` & `lumibot-3.3.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.989647 lumibot-3.3.4/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.4/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 05:23:49.989565 lumibot-3.3.4/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.4/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.976252 lumibot-3.3.4/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.977962 lumibot-3.3.4/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    31444 2024-04-10 02:40:39.000000 lumibot-3.3.4/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.978727 lumibot-3.3.4/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    42451 2024-04-10 02:40:36.000000 lumibot-3.3.4/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.4/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    27001 2024-04-10 02:40:36.000000 lumibot-3.3.4/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.980532 lumibot-3.3.4/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.4/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.4/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.4/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6744 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.981775 lumibot-3.3.4/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.4/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28434 2024-04-10 05:16:27.000000 lumibot-3.3.4/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.983460 lumibot-3.3.4/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 04:57:05.000000 lumibot-3.3.4/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.984116 lumibot-3.3.4/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53758 2024-03-31 04:01:24.000000 lumibot-3.3.4/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   149831 2024-04-10 04:58:08.000000 lumibot-3.3.4/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39749 2024-04-10 05:07:07.000000 lumibot-3.3.4/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.985741 lumibot-3.3.4/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.4/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26137 2024-03-31 03:38:08.000000 lumibot-3.3.4/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.4/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15215 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.986009 lumibot-3.3.4/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.986371 lumibot-3.3.4/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.989136 lumibot-3.3.4/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.4/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-10 05:23:49.990122 lumibot-3.3.4/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-10 05:20:37.000000 lumibot-3.3.4/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.988137 lumibot-3.3.4/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.988945 lumibot-3.3.4/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4301 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.3.4/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.296119 lumibot-3.3.5/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.5/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 20:58:06.296043 lumibot-3.3.5/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.5/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.270434 lumibot-3.3.5/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.273005 lumibot-3.3.5/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    31444 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.275425 lumibot-3.3.5/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    42451 2024-04-10 02:40:36.000000 lumibot-3.3.5/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.5/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    27001 2024-04-10 20:52:06.000000 lumibot-3.3.5/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.278881 lumibot-3.3.5/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.5/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.5/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.5/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.281555 lumibot-3.3.5/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.5/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28434 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.284073 lumibot-3.3.5/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.285877 lumibot-3.3.5/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53758 2024-03-31 04:01:24.000000 lumibot-3.3.5/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   149831 2024-04-10 04:58:08.000000 lumibot-3.3.5/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39749 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.289888 lumibot-3.3.5/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.5/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26195 2024-04-10 20:29:05.000000 lumibot-3.3.5/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.5/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15620 2024-04-10 20:12:46.000000 lumibot-3.3.5/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.290401 lumibot-3.3.5/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.290995 lumibot-3.3.5/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.5/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.295686 lumibot-3.3.5/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-10 20:58:06.000000 lumibot-3.3.5/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.5/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-10 20:58:06.296538 lumibot-3.3.5/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-10 20:12:46.000000 lumibot-3.3.5/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.293969 lumibot-3.3.5/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 20:58:06.295486 lumibot-3.3.5/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.3.5/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.3.5/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.5/tests/test_tradingfee.py
```

### Comparing `lumibot-3.3.4/LICENSE` & `lumibot-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/PKG-INFO` & `lumibot-3.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.4
+Version: 3.3.5
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-marshmallow
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
-Requires-Dist: scipy==1.10.1
+Requires-Dist: scipy==1.13.0
 Requires-Dist: ipython
 Requires-Dist: quantstats-lumi>=0.2.0
 Requires-Dist: python-dotenv
 Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
```

### Comparing `lumibot-3.3.4/README.md` & `lumibot-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/__init__.py` & `lumibot-3.3.5/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.3.5/lumibot/backtesting/backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.3.5/lumibot/backtesting/polygon_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/brokers/alpaca.py` & `lumibot-3.3.5/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/brokers/broker.py` & `lumibot-3.3.5/lumibot/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/brokers/ccxt.py` & `lumibot-3.3.5/lumibot/brokers/ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/brokers/interactive_brokers.py` & `lumibot-3.3.5/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/brokers/tradier.py` & `lumibot-3.3.5/lumibot/brokers/tradier.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/alpaca_data.py` & `lumibot-3.3.5/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.3.5/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.3.5/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/ccxt_data.py` & `lumibot-3.3.5/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/data_source.py` & `lumibot-3.3.5/lumibot/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.3.5/lumibot/data_sources/data_source_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/exceptions.py` & `lumibot-3.3.5/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.3.5/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/pandas_data.py` & `lumibot-3.3.5/lumibot/data_sources/pandas_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/tradier_data.py` & `lumibot-3.3.5/lumibot/data_sources/tradier_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/data_sources/yahoo_data.py` & `lumibot-3.3.5/lumibot/data_sources/yahoo_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from lumibot.tools import YahooHelper
 
 
 class YahooData(DataSourceBacktesting):
     SOURCE = "YAHOO"
     MIN_TIMESTEP = "day"
     TIMESTEP_MAPPING = [
-        {"timestep": "day", "representations": ["1D", "day"]},
+        {"timestep": "day", "representations": ["1d", "day"]},
+        {"timestep": "15 minutes", "representations": ["15m", "15 minutes"]},
+        {"timestep": "minute", "representations": ["1m", "1 minute"]},
     ]
 
     def __init__(self, *args, auto_adjust=True, **kwargs):
         super().__init__(*args, **kwargs)
         self.name = "yahoo"
         self.auto_adjust = auto_adjust
         self._data_store = {}
@@ -60,34 +62,37 @@
             logging.warning(
                 f"the exchange parameter is not implemented for YahooData, but {exchange} was passed as the exchange"
             )
 
         if quote is not None:
             logging.warning(f"quote is not implemented for YahooData, but {quote} was passed as the quote")
 
-        self._parse_source_timestep(timestep, reverse=True)
+        interval = self._parse_source_timestep(timestep, reverse=True)
         if asset in self._data_store:
             data = self._data_store[asset]
         else:
             data = YahooHelper.get_symbol_data(
                 asset.symbol,
+                interval=interval,
                 auto_adjust=self.auto_adjust,
                 last_needed_datetime=self.datetime_end,
             )
             if data is None or data.shape[0] == 0:
                 message = f"{self.SOURCE} did not return data for symbol {asset}. Make sure this symbol is valid."
                 logging.error(message)
                 return None
             data = self._append_data(asset, data)
 
-        # Get the last minute of self._datetime to get the current bar
-        dt = self._datetime.replace(hour=23, minute=59, second=59, microsecond=999999)
+        if timestep == "day":
+            # Get the last minute of self._datetime to get the current bar
+            dt = self._datetime.replace(hour=23, minute=59, second=59, microsecond=999999)
+            end = dt - timedelta(days=1)
+        else:
+            end = self._datetime.replace(second=59, microsecond=999999)
 
-        # End should be yesterday because otherwise you can see the future
-        end = dt - timedelta(days=1)
         if timeshift:
             end = end - timeshift
 
         end = self.to_default_timezone(end)
         result_data = data[data.index < end]
 
         result = result_data.tail(length)
@@ -97,19 +102,19 @@
         self, assets, length, timestep=MIN_TIMESTEP, timeshift=None, quote=None, include_after_hours=False
     ):
         """pull broker bars for a list assets"""
 
         if quote is not None:
             logging.warning(f"quote is not implemented for YahooData, but {quote} was passed as the quote")
 
-        self._parse_source_timestep(timestep, reverse=True)
+        interval = self._parse_source_timestep(timestep, reverse=True)
         missing_assets = [asset.symbol for asset in assets if asset not in self._data_store]
 
         if missing_assets:
-            dfs = YahooHelper.get_symbols_data(missing_assets, auto_adjust=self.auto_adjust)
+            dfs = YahooHelper.get_symbols_data(missing_assets, interval=interval, auto_adjust=self.auto_adjust)
             for symbol, df in dfs.items():
                 self._append_data(symbol, df)
 
         result = {}
         for asset in assets:
             result[asset] = self._pull_source_symbol_bars(asset, length, timestep=timestep, timeshift=timeshift)
         return result
```

### Comparing `lumibot-3.3.4/lumibot/entities/asset.py` & `lumibot-3.3.5/lumibot/entities/asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/entities/bar.py` & `lumibot-3.3.5/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/entities/bars.py` & `lumibot-3.3.5/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/entities/data.py` & `lumibot-3.3.5/lumibot/entities/data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/entities/order.py` & `lumibot-3.3.5/lumibot/entities/order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/entities/position.py` & `lumibot-3.3.5/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/entities/trading_fee.py` & `lumibot-3.3.5/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.3.5/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.3.5/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.3.5/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.3.5/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.3.5/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.3.5/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.3.5/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.3.5/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.3.5/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/stock_oco.py` & `lumibot-3.3.5/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/example_strategies/strangle.py` & `lumibot-3.3.5/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/strategies/_strategy.py` & `lumibot-3.3.5/lumibot/strategies/_strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/strategies/strategy.py` & `lumibot-3.3.5/lumibot/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/strategies/strategy_executor.py` & `lumibot-3.3.5/lumibot/strategies/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/__init__.py` & `lumibot-3.3.5/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/black_scholes.py` & `lumibot-3.3.5/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/ccxt_data_store.py` & `lumibot-3.3.5/lumibot/tools/ccxt_data_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/decorators.py` & `lumibot-3.3.5/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/helpers.py` & `lumibot-3.3.5/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/indicators.py` & `lumibot-3.3.5/lumibot/tools/indicators.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import webbrowser
 from datetime import datetime
 from decimal import Decimal
 
 import pandas as pd
 import plotly.graph_objects as go
+import pytz
 import quantstats_lumi as qs
 from plotly.subplots import make_subplots
 
 from lumibot import LUMIBOT_DEFAULT_TIMEZONE
 from lumibot.tools import to_datetime_aware
 
 from .yahoo_helper import YahooHelper as yh
@@ -43,31 +44,31 @@
 
 
     """
     df = _df.copy()
     df = df.sort_index(ascending=True)
     df["cum_return"] = (1 + df["return"]).cumprod()
     total_ret = df["cum_return"].iloc[-1]
-    start = datetime.utcfromtimestamp(df.index.values[0].astype("O") / 1e9)
-    end = datetime.utcfromtimestamp(df.index.values[-1].astype("O") / 1e9)
+    start = datetime.fromtimestamp(df.index.values[0].astype("O") / 1e9, pytz.UTC)
+    end = datetime.fromtimestamp(df.index.values[-1].astype("O") / 1e9, pytz.UTC)
     period_years = (end - start).days / 365.25
     if period_years == 0:
         return 0
     CAGR = (total_ret) ** (1 / period_years) - 1
     return CAGR
 
 
 def volatility(_df):
     """Calculate the volatility (standard deviation)
     The dataframe _df must include a column "return" that
     has the return for that time period (eg. daily)
     """
     df = _df.copy()
-    start = datetime.utcfromtimestamp(df.index.values[0].astype("O") / 1e9)
-    end = datetime.utcfromtimestamp(df.index.values[-1].astype("O") / 1e9)
+    start = datetime.fromtimestamp(df.index.values[0].astype("O") / 1e9, pytz.UTC)
+    end = datetime.fromtimestamp(df.index.values[-1].astype("O") / 1e9, pytz.UTC)
     period_years = (end - start).days / 365.25
     if period_years == 0:
         return 0
     ratio_to_annual = df["return"].count() / period_years
     vol = df["return"].std() * math.sqrt(ratio_to_annual)
     return vol
 
@@ -453,15 +454,15 @@
 
     def generate_buysell_plotly_text(row):
         if row["status"] != "canceled" and row["status"] != "new":
             if row["asset.asset_type"] == "option":
                 return (
                     row["status"]
                     + "<br>"
-                    + str(row["filled_quantity"].quantize(Decimal("0.01")).__format__(",f"))
+                    + str(Decimal(row["filled_quantity"]).quantize(Decimal("0.01")).__format__(",f"))
                     + " "
                     + row["symbol"]
                     + " "
                     + row["asset.right"]
                     + " Option"
                     + "<br>"
                     + "Strike: "
@@ -492,15 +493,15 @@
                     + str(Decimal(row["trade_cost"]).quantize(Decimal("0.01")).__format__(",f"))
                     + "<br>"
                 )
             else:
                 return (
                     row["status"]
                     + "<br>"
-                    + str(row["filled_quantity"].quantize(Decimal("0.01")).__format__(",f"))
+                    + str(Decimal(row["filled_quantity"]).quantize(Decimal("0.01")).__format__(",f"))
                     + " "
                     + row["symbol"]
                     + "<br>"
                     + "Price: "
                     + str(Decimal(row["price"]).quantize(Decimal("0.0001")).__format__(",f"))
                     + "<br>"
                     + "Order Type: "
```

### Comparing `lumibot-3.3.4/lumibot/tools/lumibot_time.py` & `lumibot-3.3.5/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/pandas.py` & `lumibot-3.3.5/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/polygon_helper.py` & `lumibot-3.3.5/lumibot/tools/polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/types.py` & `lumibot-3.3.5/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/tools/yahoo_helper.py` & `lumibot-3.3.5/lumibot/tools/yahoo_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import pickle
-from datetime import datetime
+from datetime import datetime, timedelta
 
 import pandas as pd
 import yfinance as yf
 
 from lumibot import LUMIBOT_CACHE_FOLDER, LUMIBOT_DEFAULT_PYTZ
 
 from .helpers import get_lumibot_datetime
@@ -165,18 +165,25 @@
         df = ticker.history(period="7d", auto_adjust=False)
         if df.empty:
             return None
 
         return df["Close"].iloc[-1]
 
     @staticmethod
-    def download_symbol_day_data(symbol):
+    def download_symbol_data(symbol, interval="1d"):
         ticker = yf.Ticker(symbol)
         try:
-            df = ticker.history(period="max", auto_adjust=False)
+            if interval == "1m":
+                # Yahoo only supports 1 minute interval for past 7 days
+                df = ticker.history(interval=interval, start=get_lumibot_datetime() - timedelta(days=7), auto_adjust=False)
+            elif interval == "15m":
+                # Yahoo only supports 15 minute interval for past 60 days
+                df = ticker.history(interval=interval, start=get_lumibot_datetime() - timedelta(days=60), auto_adjust=False)
+            else:
+                df = ticker.history(interval=interval, period="max", auto_adjust=False)
         except Exception as e:
             logging.debug(f"Error while downloading symbol day data for {symbol}, returning empty dataframe for now.")
             logging.debug(e)
             return None
 
         # Adjust the time when we are getting daily stock data to the beginning of the day
         # This way the times line up when backtesting daily data
@@ -196,17 +203,17 @@
                 df.index = df.index.tz_convert(info.get("info").get("exchangeTimezoneName"))
             df.index = df.index.map(lambda t: t.replace(hour=23, minute=59))
 
         df = YahooHelper.process_df(df, asset_info=info)
         return df
 
     @staticmethod
-    def download_symbols_day_data(symbols):
+    def download_symbols_data(symbols, interval="1d"):
         if len(symbols) == 1:
-            item = YahooHelper.download_symbol_day_data(symbols[0])
+            item = YahooHelper.download_symbol_data(symbols[0], interval)
             return {symbols[0]: item}
 
         result = {}
         tickers = yf.Tickers(" ".join(symbols))
         df_yf = tickers.history(
             period="max",
             group_by="ticker",
@@ -232,141 +239,137 @@
         # Caching is disabled or no previous data found
         # or data found not up to date
         data = YahooHelper.download_symbol_info(symbol)
         YahooHelper.dump_pickle_file(symbol, INFO_DATA, data)
         return data
 
     @staticmethod
-    def fetch_symbol_day_data(symbol, caching=True, last_needed_datetime=None):
+    def fetch_symbol_data(symbol, caching=True, last_needed_datetime=None, interval="1d"):
         if caching:
-            cached_data = YahooHelper.check_pickle_file(symbol, DAY_DATA)
+            cached_data = YahooHelper.check_pickle_file(symbol, interval)
             if cached_data:
                 if cached_data.is_up_to_date(last_needed_datetime=last_needed_datetime):
                     return cached_data.data
 
         # Caching is disabled or no previous data found
         # or data found not up to date
-        data = YahooHelper.download_symbol_day_data(symbol)
+        data = YahooHelper.download_symbol_data(symbol, interval)
 
         # Check if the data is empty
         if data is None or data.empty:
             return data
 
-        YahooHelper.dump_pickle_file(symbol, DAY_DATA, data)
+        YahooHelper.dump_pickle_file(symbol, interval, data)
         return data
 
     @staticmethod
-    def fetch_symbols_day_data(symbols, caching=True):
+    def fetch_symbols_data(symbols, interval, caching=True):
         result = {}
         missing_symbols = symbols.copy()
 
         if caching:
             for symbol in symbols:
-                cached_data = YahooHelper.check_pickle_file(symbol, DAY_DATA)
+                cached_data = YahooHelper.check_pickle_file(symbol, interval)
                 if cached_data:
                     if cached_data.is_up_to_date():
                         result[symbol] = cached_data.data
                         missing_symbols.remove(symbol)
 
         if missing_symbols:
-            missing_data = YahooHelper.download_symbols_day_data(missing_symbols)
+            missing_data = YahooHelper.download_symbols_data(missing_symbols, interval)
             for symbol, data in missing_data.items():
                 result[symbol] = data
-                YahooHelper.dump_pickle_file(symbol, DAY_DATA, data)
+                YahooHelper.dump_pickle_file(symbol, interval, data)
 
         return result
 
     # ======Shortcut methods==================================
 
     @staticmethod
     def get_symbol_info(symbol, caching=True):
         return YahooHelper.fetch_symbol_info(symbol, caching=caching)
 
     @staticmethod
-    def get_symbol_day_data(symbol, auto_adjust=True, caching=True, last_needed_datetime=None):
-        result = YahooHelper.fetch_symbol_day_data(symbol, caching=caching, last_needed_datetime=last_needed_datetime)
-        return result
-
-    @staticmethod
     def get_symbol_data(
         symbol,
-        timestep="day",
-        auto_adjust=True,
+        interval="1d",
         caching=True,
+        auto_adjust=False,
         last_needed_datetime=None,
     ):
-        if timestep == "day":
-            return YahooHelper.get_symbol_day_data(
+        if interval in ["1m", "15m", "1d"]:
+            df = YahooHelper.fetch_symbol_data(
                 symbol,
-                auto_adjust=auto_adjust,
+                interval=interval,
                 caching=caching,
                 last_needed_datetime=last_needed_datetime,
             )
+            return YahooHelper.format_df(df, False)
         else:
-            raise ValueError("Unknown timestep %s" % timestep)
+            raise ValueError("Unknown interval %s" % interval)
 
     @staticmethod
-    def get_symbols_day_data(symbols, auto_adjust=True, caching=True):
-        result = YahooHelper.fetch_symbols_day_data(symbols, caching=caching)
+    def get_symbols_data(symbols, interval="1d", auto_adjust=True, caching=True):
+        result = YahooHelper.fetch_symbols_data(symbols, interval=interval, caching=caching)
         for key, df in result.items():
             result[key] = YahooHelper.format_df(df, auto_adjust)
         return result
 
     @staticmethod
-    def get_symbols_data(symbols, timestep="day", auto_adjust=True, caching=True):
-        if timestep == "day":
-            return YahooHelper.get_symbols_day_data(symbols, auto_adjust=auto_adjust, caching=caching)
+    def get_symbols_data(symbols, interval="1d", auto_adjust=True, caching=True):
+        if interval in ["1m", "15m", "1d"]:
+            return YahooHelper.get_symbols_data(symbols, interval=interval, auto_adjust=auto_adjust, caching=caching)
         else:
-            raise ValueError("Unknown timestep %s" % timestep)
+            raise ValueError("Unknown interval %s" % interval)
 
     @staticmethod
     def get_symbol_dividends(symbol, caching=True):
         """https://github.com/ranaroussi/yfinance/blob/main/yfinance/base.py"""
-        history = YahooHelper.get_symbol_day_data(symbol, caching=caching)
+        history = YahooHelper.get_symbol_data(symbol, caching=caching)
         dividends = history["Dividends"]
         return dividends[dividends != 0].dropna()
 
     @staticmethod
     def get_symbols_dividends(symbols, caching=True):
         result = {}
-        data = YahooHelper.get_symbols_day_data(symbols, caching=caching)
+        data = YahooHelper.get_symbols_data(symbols, caching=caching)
         for symbol, df in data.items():
             dividends = df["Dividends"]
             result[symbol] = dividends[dividends != 0].dropna()
 
         return result
 
     @staticmethod
     def get_symbol_splits(symbol, caching=True):
         """https://github.com/ranaroussi/yfinance/blob/main/yfinance/base.py"""
-        history = YahooHelper.get_symbol_day_data(symbol, caching=caching)
+        history = YahooHelper.get_symbol_data(symbol, caching=caching)
         splits = history["Stock Splits"]
         return splits[splits != 0].dropna()
 
     @staticmethod
     def get_symbols_splits(symbols, caching=True):
         result = {}
-        data = YahooHelper.get_symbols_day_data(symbols, caching=caching)
+        data = YahooHelper.get_symbols_data(symbols, caching=caching)
         for symbol, df in data.items():
             splits = df["Stock Splits"]
             result[symbol] = splits[splits != 0].dropna()
 
         return result
 
     @staticmethod
     def get_symbol_actions(symbol, caching=True):
         """https://github.com/ranaroussi/yfinance/blob/main/yfinance/base.py"""
-        history = YahooHelper.get_symbol_day_data(symbol, caching=caching)
+        history = YahooHelper.get_symbol__data(symbol, caching=caching)
         actions = history[["Dividends", "Stock Splits"]]
         return actions[actions != 0].dropna(how="all").fillna(0)
 
     @staticmethod
     def get_symbols_actions(symbols, caching=True):
         result = {}
-        data = YahooHelper.get_symbols_day_data(symbols, caching=caching)
+        data = YahooHelper.get_symbols__data(symbols, caching=caching)
         for symbol, df in data.items():
             actions = df[["Dividends", "Stock Splits"]]
             result[symbol] = actions[actions != 0].dropna(how="all").fillna(0)
 
         return result
 
     @staticmethod
```

### Comparing `lumibot-3.3.4/lumibot/traders/trader.py` & `lumibot-3.3.5/lumibot/traders/trader.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.3.5/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot/trading_builtins/safe_list.py` & `lumibot-3.3.5/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot.egg-info/PKG-INFO` & `lumibot-3.3.5/lumibot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.4
+Version: 3.3.5
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-marshmallow
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
-Requires-Dist: scipy==1.10.1
+Requires-Dist: scipy==1.13.0
 Requires-Dist: ipython
 Requires-Dist: quantstats-lumi>=0.2.0
 Requires-Dist: python-dotenv
 Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
```

### Comparing `lumibot-3.3.4/lumibot.egg-info/SOURCES.txt` & `lumibot-3.3.5/lumibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/lumibot.egg-info/requires.txt` & `lumibot-3.3.5/lumibot.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 flask-sqlalchemy
 flask-marshmallow
 flask-security
 marshmallow-sqlalchemy
 email_validator
 bcrypt
 pytest
-scipy==1.10.1
+scipy==1.13.0
 ipython
 quantstats-lumi>=0.2.0
 python-dotenv
 ccxt==4.2.85
 termcolor
 jsonpickle
 apscheduler==3.10.4
```

### Comparing `lumibot-3.3.4/pyproject.toml` & `lumibot-3.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/setup.cfg` & `lumibot-3.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/setup.py` & `lumibot-3.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.3.4",
+    version="3.3.5",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
@@ -31,15 +31,15 @@
         "flask-sqlalchemy",
         "flask-marshmallow",
         "flask-security",
         "marshmallow-sqlalchemy",
         "email_validator",
         "bcrypt",
         "pytest",
-        "scipy==1.10.1",  # Newer versions of scipy are currently causing issues
+        "scipy==1.13.0",  # Newer versions of scipy are currently causing issues
         "ipython",  # required for quantstats, but not in their dependency list for some reason
         "quantstats-lumi>=0.2.0",
         "python-dotenv",  # Secret Storage
         "ccxt==4.2.85",
         "termcolor",
         "jsonpickle",
         "apscheduler==3.10.4",
```

### Comparing `lumibot-3.3.4/tests/backtest/test_example_strategies.py` & `lumibot-3.3.5/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.3.5/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/backtest/test_polygon.py` & `lumibot-3.3.5/tests/backtest/test_polygon.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/backtest/test_strategy_executor.py` & `lumibot-3.3.5/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/backtest/test_yahoo.py` & `lumibot-3.3.5/tests/backtest/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_alpaca.py` & `lumibot-3.3.5/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_alpaca_old.py` & `lumibot-3.3.5/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_asset.py` & `lumibot-3.3.5/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_backtesting_broker.py` & `lumibot-3.3.5/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_ccxt.py` & `lumibot-3.3.5/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_ccxt_store.py` & `lumibot-3.3.5/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_interactive_brokers.py` & `lumibot-3.3.5/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_order.py` & `lumibot-3.3.5/tests/test_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class TestOrderBasics:
     def test_side_must_be_one_of(self):
         assert Order(asset=Asset("SPY"), quantity=10, side="buy", strategy='abc').side == 'buy'
         assert Order(asset=Asset("SPY"), quantity=10, side="sell", strategy='abc').side == 'sell'
 
-        with pytest.raises(ValueError):
-            Order(asset=Asset("SPY"), quantity=10, side="unknown", strategy='abc')
-
     def test_is_option(self):
         # Standard stock order
         asset = Asset("SPY")
         order = Order(asset=asset, quantity=10, side="buy", strategy='abc')
         assert not order.is_option()
 
         # Option order
```

### Comparing `lumibot-3.3.4/tests/test_polygon_helper.py` & `lumibot-3.3.5/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_strategy_methods.py` & `lumibot-3.3.5/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.4/tests/test_tradier.py` & `lumibot-3.3.5/tests/test_tradier.py`

 * *Files identical despite different names*

