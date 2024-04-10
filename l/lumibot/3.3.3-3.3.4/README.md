# Comparing `tmp/lumibot-3.3.3.tar.gz` & `tmp/lumibot-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.3.3.tar", last modified: Wed Apr 10 02:41:58 2024, max compression
+gzip compressed data, was "lumibot-3.3.4.tar", last modified: Wed Apr 10 05:23:49 2024, max compression
```

## Comparing `lumibot-3.3.3.tar` & `lumibot-3.3.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.939475 lumibot-3.3.3/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.3/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 02:41:58.939386 lumibot-3.3.3/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.3/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.912180 lumibot-3.3.3/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.914914 lumibot-3.3.3/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    31444 2024-04-10 02:40:39.000000 lumibot-3.3.3/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.917287 lumibot-3.3.3/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    42451 2024-04-10 02:40:36.000000 lumibot-3.3.3/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.3/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    27001 2024-04-10 02:40:36.000000 lumibot-3.3.3/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.921312 lumibot-3.3.3/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.3/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.3/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.3/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6744 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.924392 lumibot-3.3.3/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.3/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28584 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.927191 lumibot-3.3.3/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2469 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.929077 lumibot-3.3.3/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53758 2024-03-31 04:01:24.000000 lumibot-3.3.3/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   149831 2024-04-10 02:40:36.000000 lumibot-3.3.3/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39624 2024-03-19 07:27:52.000000 lumibot-3.3.3/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.932965 lumibot-3.3.3/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.3/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26137 2024-03-31 03:38:08.000000 lumibot-3.3.3/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.3/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15215 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.933412 lumibot-3.3.3/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.934027 lumibot-3.3.3/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.3/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.938967 lumibot-3.3.3/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 02:41:58.000000 lumibot-3.3.3/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-10 02:41:58.000000 lumibot-3.3.3/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-10 02:41:58.000000 lumibot-3.3.3/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-10 02:41:58.000000 lumibot-3.3.3/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-10 02:41:58.000000 lumibot-3.3.3/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.3/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-10 02:41:58.939898 lumibot-3.3.3/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-10 02:40:48.000000 lumibot-3.3.3/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.937270 lumibot-3.3.3/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 02:41:58.938697 lumibot-3.3.3/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4301 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.3.3/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.3/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.989647 lumibot-3.3.4/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.4/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 05:23:49.989565 lumibot-3.3.4/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.4/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.976252 lumibot-3.3.4/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.977962 lumibot-3.3.4/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    31444 2024-04-10 02:40:39.000000 lumibot-3.3.4/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.978727 lumibot-3.3.4/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    42451 2024-04-10 02:40:36.000000 lumibot-3.3.4/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.4/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    27001 2024-04-10 02:40:36.000000 lumibot-3.3.4/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.980532 lumibot-3.3.4/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.4/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.4/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.4/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6744 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.981775 lumibot-3.3.4/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.4/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28434 2024-04-10 05:16:27.000000 lumibot-3.3.4/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.983460 lumibot-3.3.4/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 04:57:05.000000 lumibot-3.3.4/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.984116 lumibot-3.3.4/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53758 2024-03-31 04:01:24.000000 lumibot-3.3.4/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   149831 2024-04-10 04:58:08.000000 lumibot-3.3.4/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39749 2024-04-10 05:07:07.000000 lumibot-3.3.4/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.985741 lumibot-3.3.4/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.4/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26137 2024-03-31 03:38:08.000000 lumibot-3.3.4/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.4/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15215 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.986009 lumibot-3.3.4/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.986371 lumibot-3.3.4/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.4/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.989136 lumibot-3.3.4/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-10 05:23:49.000000 lumibot-3.3.4/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.4/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-10 05:23:49.990122 lumibot-3.3.4/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-10 05:20:37.000000 lumibot-3.3.4/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.988137 lumibot-3.3.4/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-10 05:23:49.988945 lumibot-3.3.4/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4301 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.3.4/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.4/tests/test_tradingfee.py
```

### Comparing `lumibot-3.3.3/LICENSE` & `lumibot-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/PKG-INFO` & `lumibot-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.3
+Version: 3.3.4
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.3.3/README.md` & `lumibot-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/__init__.py` & `lumibot-3.3.4/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.3.4/lumibot/backtesting/backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.3.4/lumibot/backtesting/polygon_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/brokers/alpaca.py` & `lumibot-3.3.4/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/brokers/broker.py` & `lumibot-3.3.4/lumibot/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/brokers/ccxt.py` & `lumibot-3.3.4/lumibot/brokers/ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/brokers/interactive_brokers.py` & `lumibot-3.3.4/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/brokers/tradier.py` & `lumibot-3.3.4/lumibot/brokers/tradier.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/alpaca_data.py` & `lumibot-3.3.4/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.3.4/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.3.4/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/ccxt_data.py` & `lumibot-3.3.4/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/data_source.py` & `lumibot-3.3.4/lumibot/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.3.4/lumibot/data_sources/data_source_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/exceptions.py` & `lumibot-3.3.4/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.3.4/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/pandas_data.py` & `lumibot-3.3.4/lumibot/data_sources/pandas_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/tradier_data.py` & `lumibot-3.3.4/lumibot/data_sources/tradier_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/data_sources/yahoo_data.py` & `lumibot-3.3.4/lumibot/data_sources/yahoo_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/entities/asset.py` & `lumibot-3.3.4/lumibot/entities/asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/entities/bar.py` & `lumibot-3.3.4/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/entities/bars.py` & `lumibot-3.3.4/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/entities/data.py` & `lumibot-3.3.4/lumibot/entities/data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/entities/order.py` & `lumibot-3.3.4/lumibot/entities/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,17 +303,14 @@
         self._raw = None
         self._transmitted = False
         self._error = None
         self.error_message = None
 
         self.quantity = quantity
 
-        # setting the side
-        if side not in [BUY, SELL]:
-            raise ValueError("Side must be either sell or buy, got %r instead" % side)
         self.side = side
 
         self._set_type(
             limit_price,
             stop_price,
             take_profit_price,
             stop_loss_price,
```

### Comparing `lumibot-3.3.3/lumibot/entities/position.py` & `lumibot-3.3.4/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/entities/trading_fee.py` & `lumibot-3.3.4/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.3.4/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.3.4/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.3.4/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,22 +43,27 @@
                 symbol=buy_symbol,
                 asset_type="option",
                 expiration=expiry,
                 strike=strike,
                 right="call",
             )
 
-            # Bracket order
+            # Create order
             order = self.create_order(
                 asset,
                 10,
-                "buy",
+                "buy_to_open",
             )
+            
+            # Submit order
             self.submit_order(order)
 
+            # Log a message
+            self.log_message(f"Bought {order.quantity} of {asset}")
+
 
 if __name__ == "__main__":
     is_live = False
 
     if is_live:
         from credentials import INTERACTIVE_BROKERS_CONFIG
```

### Comparing `lumibot-3.3.3/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.3.4/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.3.4/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.3.4/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.3.4/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.3.4/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.3.4/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/stock_oco.py` & `lumibot-3.3.4/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/example_strategies/strangle.py` & `lumibot-3.3.4/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/strategies/_strategy.py` & `lumibot-3.3.4/lumibot/strategies/_strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/strategies/strategy.py` & `lumibot-3.3.4/lumibot/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/strategies/strategy_executor.py` & `lumibot-3.3.4/lumibot/strategies/strategy_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,18 @@
                 self.strategy.log_message(
                     f"Trading iteration ended at {end_str}, next check in time is {dt_str}. Took {runtime:.2f}s", color="blue"
                 )
 
             else:
                 self.strategy.log_message(f"Trading iteration ended at {end_str}", color="blue")
         except Exception as e:
+            # If backtesting, raise the exception
+            if self.broker.IS_BACKTESTING_BROKER:
+                raise e
+
             # Log the error
             self.strategy.log_message(
                 f"An error occurred during the on_trading_iteration lifecycle method: {e}", color="red"
             )
 
             # Log the traceback
             self.strategy.log_message(traceback.format_exc(), color="red")
```

### Comparing `lumibot-3.3.3/lumibot/tools/__init__.py` & `lumibot-3.3.4/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/black_scholes.py` & `lumibot-3.3.4/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/ccxt_data_store.py` & `lumibot-3.3.4/lumibot/tools/ccxt_data_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/decorators.py` & `lumibot-3.3.4/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/helpers.py` & `lumibot-3.3.4/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/indicators.py` & `lumibot-3.3.4/lumibot/tools/indicators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/lumibot_time.py` & `lumibot-3.3.4/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/pandas.py` & `lumibot-3.3.4/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/polygon_helper.py` & `lumibot-3.3.4/lumibot/tools/polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/types.py` & `lumibot-3.3.4/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/tools/yahoo_helper.py` & `lumibot-3.3.4/lumibot/tools/yahoo_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/traders/trader.py` & `lumibot-3.3.4/lumibot/traders/trader.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.3.4/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot/trading_builtins/safe_list.py` & `lumibot-3.3.4/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot.egg-info/PKG-INFO` & `lumibot-3.3.4/lumibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.3
+Version: 3.3.4
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.3.3/lumibot.egg-info/SOURCES.txt` & `lumibot-3.3.4/lumibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/lumibot.egg-info/requires.txt` & `lumibot-3.3.4/lumibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/pyproject.toml` & `lumibot-3.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/setup.cfg` & `lumibot-3.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/setup.py` & `lumibot-3.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.3.3",
+    version="3.3.4",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
```

### Comparing `lumibot-3.3.3/tests/backtest/test_example_strategies.py` & `lumibot-3.3.4/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.3.4/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/backtest/test_polygon.py` & `lumibot-3.3.4/tests/backtest/test_polygon.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/backtest/test_strategy_executor.py` & `lumibot-3.3.4/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/backtest/test_yahoo.py` & `lumibot-3.3.4/tests/backtest/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_alpaca.py` & `lumibot-3.3.4/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_alpaca_old.py` & `lumibot-3.3.4/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_asset.py` & `lumibot-3.3.4/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_backtesting_broker.py` & `lumibot-3.3.4/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_ccxt.py` & `lumibot-3.3.4/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_ccxt_store.py` & `lumibot-3.3.4/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_interactive_brokers.py` & `lumibot-3.3.4/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_order.py` & `lumibot-3.3.4/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_polygon_helper.py` & `lumibot-3.3.4/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_strategy_methods.py` & `lumibot-3.3.4/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.3/tests/test_tradier.py` & `lumibot-3.3.4/tests/test_tradier.py`

 * *Files identical despite different names*

