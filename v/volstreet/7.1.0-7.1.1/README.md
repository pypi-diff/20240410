# Comparing `tmp/volstreet-7.1.0.tar.gz` & `tmp/volstreet-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.1.0.tar", last modified: Mon Apr  8 03:37:26 2024, max compression
+gzip compressed data, was "volstreet-7.1.1.tar", last modified: Tue Apr  9 03:35:07 2024, max compression
```

## Comparing `volstreet-7.1.0.tar` & `volstreet-7.1.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.316458 volstreet-7.1.0/
--rw-rw-rw-   0        0        0     1293 2024-04-08 03:37:26.315148 volstreet-7.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.1.0/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1104 2024-04-08 03:37:26.317702 volstreet-7.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.141221 volstreet-7.1.0/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.1.0/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.177564 volstreet-7.1.0/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.1.0/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    13980 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.1.0/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.1.0/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.1.0/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.214992 volstreet-7.1.0/volstreet/backtests/
--rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/data_handling.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    47225 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    18739 2024-03-14 09:00:56.000000 volstreet-7.1.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6003 2024-04-08 03:36:49.000000 volstreet-7.1.0/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.238386 volstreet-7.1.0/volstreet/datamodule/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.241378 volstreet-7.1.0/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.272314 volstreet-7.1.0/volstreet/strategies/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    27021 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/strategies/execution.py
--rw-rw-rw-   0        0        0    56666 2024-04-08 03:36:49.000000 volstreet-7.1.0/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0    13100 2024-04-08 03:26:20.000000 volstreet-7.1.0/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    89977 2024-04-06 06:44:48.000000 volstreet-7.1.0/volstreet/strategies/strats.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.289067 volstreet-7.1.0/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26077 2024-04-06 06:58:33.000000 volstreet-7.1.0/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0     9797 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    11666 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/trade_interface/order_placement.py
--rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.1.0/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.300528 volstreet-7.1.0/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     2963 2024-04-06 06:31:33.000000 volstreet-7.1.0/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.1.0/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.1.0/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.312618 volstreet-7.1.0/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.1.0/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.1.0/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.1.0/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.1.0/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:37:26.313648 volstreet-7.1.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2374 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 03:37:26.000000 volstreet-7.1.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.198841 volstreet-7.1.1/
+-rw-rw-rw-   0        0        0     1293 2024-04-09 03:35:07.197834 volstreet-7.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.1.1/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1104 2024-04-09 03:35:07.199929 volstreet-7.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.117453 volstreet-7.1.1/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.1.1/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.137769 volstreet-7.1.1/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.1.1/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.1.1/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.1.1/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    13980 2024-04-06 06:31:33.000000 volstreet-7.1.1/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.1.1/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.1.1/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.1.1/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.153974 volstreet-7.1.1/volstreet/backtests/
+-rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/backtests/data_handling.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.1.1/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    47225 2024-04-06 06:31:33.000000 volstreet-7.1.1/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.1.1/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.1.1/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    19856 2024-04-08 10:59:14.000000 volstreet-7.1.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6003 2024-04-08 03:36:49.000000 volstreet-7.1.1/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.166425 volstreet-7.1.1/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.1.1/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.1.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.1.1/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.167453 volstreet-7.1.1/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.1.1/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.175201 volstreet-7.1.1/volstreet/strategies/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5684 2024-04-03 08:06:51.000000 volstreet-7.1.1/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    27410 2024-04-08 06:26:07.000000 volstreet-7.1.1/volstreet/strategies/execution.py
+-rw-rw-rw-   0        0        0    56830 2024-04-08 12:49:30.000000 volstreet-7.1.1/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0    14746 2024-04-08 14:29:35.000000 volstreet-7.1.1/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    89791 2024-04-08 12:54:07.000000 volstreet-7.1.1/volstreet/strategies/strats.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.182010 volstreet-7.1.1/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.1.1/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26077 2024-04-06 06:58:33.000000 volstreet-7.1.1/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0     9797 2024-04-06 06:31:33.000000 volstreet-7.1.1/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    11666 2024-04-06 06:31:33.000000 volstreet-7.1.1/volstreet/trade_interface/order_placement.py
+-rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.1.1/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.189096 volstreet-7.1.1/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     2963 2024-04-06 06:31:33.000000 volstreet-7.1.1/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.1.1/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.1.1/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.195583 volstreet-7.1.1/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.1.1/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.1.1/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.1.1/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.1.1/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.1.1/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:35:07.196581 volstreet-7.1.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-09 03:35:07.000000 volstreet-7.1.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2374 2024-04-09 03:35:07.000000 volstreet-7.1.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:35:07.000000 volstreet-7.1.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-09 03:35:07.000000 volstreet-7.1.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 03:35:07.000000 volstreet-7.1.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.1.0/PKG-INFO` & `volstreet-7.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.1.0
+Version: 7.1.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.1.0/setup.cfg` & `volstreet-7.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 312e 300d 0a61  rsion = 7.1.0..a
+00000020: 7273 696f 6e20 3d20 372e 312e 310d 0a61  rsion = 7.1.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-7.1.0/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.1.1/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/angel_interface/async_interface.py` & `volstreet-7.1.1/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/angel_interface/base_websocket.py` & `volstreet-7.1.1/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/angel_interface/interface.py` & `volstreet-7.1.1/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/angel_interface/login.py` & `volstreet-7.1.1/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/angel_interface/order_websocket.py` & `volstreet-7.1.1/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/angel_interface/price_websocket.py` & `volstreet-7.1.1/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/angel_interface/smart_connect.py` & `volstreet-7.1.1/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/data_handling.py` & `volstreet-7.1.1/volstreet/backtests/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/database.py` & `volstreet-7.1.1/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/delta_hedging.py` & `volstreet-7.1.1/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/delta_optimizer.py` & `volstreet-7.1.1/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/framework.py` & `volstreet-7.1.1/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.1.1/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/tools.py` & `volstreet-7.1.1/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/trend.py` & `volstreet-7.1.1/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/backtests/underlying_info.py` & `volstreet-7.1.1/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/blackscholes.py` & `volstreet-7.1.1/volstreet/blackscholes.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
 
 def d2(S, K, t, r, sigma):
     return d1(S, K, t, r, sigma) - sigma * np.sqrt(t)
 
 
 def forward_price(S, t, r):
-    return S / np.exp(-r * t)
+    return S * np.exp(r * t)
 
 
 def call(S, K, t, r, sigma):
     e_to_the_minus_rt = np.exp(-r * t)
     D1 = d1(S, K, t, r, sigma)
     D2 = d2(S, K, t, r, sigma)
 
@@ -179,15 +179,15 @@
 
 
 def gamma(S, K, t, r, sigma):
     d_1 = d1(S, K, t, r, sigma)
     return pdf(d_1) / (S * sigma * np.sqrt(t))
 
 
-def theta(S, K, t, r, sigma, flag):
+def theta_nd(S, K, t, r, sigma, flag):
     two_sqrt_t = 2 * np.sqrt(t)
 
     D1 = d1(S, K, t, r, sigma)
     D2 = d2(S, K, t, r, sigma)
 
     first_term = (-S * pdf(D1) * sigma) / two_sqrt_t
 
@@ -196,14 +196,51 @@
         return (first_term - second_term) / 365.0
 
     else:
         second_term = r * K * np.exp(-r * t) * N(-D2)
         return (first_term + second_term) / 365.0
 
 
+def theta_fd(S, K, t, r, sigma, flag, time_jump=1 / 365):
+    """dt (delta t) is the change in time IN YEARS
+    For example, a 1 day change in time would be dt=1/365
+    """
+    five_minutes_in_years = 5 / (60 * 24 * 365)
+
+    price_original = (
+        call(S, K, t, r, sigma)
+        if flag.upper().startswith("C")
+        else put(S, K, t, r, sigma)
+    )
+
+    new_time = t - time_jump
+    new_time = max(new_time, five_minutes_in_years)
+
+    # New spot
+    actual_time_jump = max(t - new_time, 1e-5)
+    S1 = S * np.exp(r * actual_time_jump)
+
+    price_bumped = (
+        call(S1, K, new_time, r, sigma)
+        if flag.upper().startswith("C")
+        else put(S1, K, new_time, r, sigma)
+    )
+    return price_bumped - price_original
+
+
+def theta(S, K, t, r, sigma, flag, **kwargs):
+    try:
+        return theta_fd(S, K, t, r, sigma, flag, **kwargs)
+    except Exception as e:
+        logger.error(
+            f"Error in theta_fd: {e}, S={S}, K={K}, t={t}, r={r}, sigma={sigma}, flag={flag}, kwargs={kwargs}"
+        )
+        return theta_nd(S, K, t, r, sigma, flag)
+
+
 def vega(S, K, t, r, sigma):
     d_1 = d1(S, K, t, r, sigma)
     return S * pdf(d_1) * np.sqrt(t) * 0.01
 
 
 def rho(S, K, t, r, sigma, flag):
     d_2 = d2(S, K, t, r, sigma)
```

### Comparing `volstreet-7.1.0/volstreet/config.py` & `volstreet-7.1.1/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/database_connection.py` & `volstreet-7.1.1/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/datamodule/analysis.py` & `volstreet-7.1.1/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/datamodule/archive.py` & `volstreet-7.1.1/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/datamodule/eod_client.py` & `volstreet-7.1.1/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/datamodule/gambling.py` & `volstreet-7.1.1/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/datamodule/intraday_data.py` & `volstreet-7.1.1/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/datamodule/stockmock.py` & `volstreet-7.1.1/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/datamodule/trading_assistance.py` & `volstreet-7.1.1/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/dealingroom.py` & `volstreet-7.1.1/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/decorators.py` & `volstreet-7.1.1/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/discord_bot.py` & `volstreet-7.1.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/exceptions.py` & `volstreet-7.1.1/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.1.1/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/parallelization.py` & `volstreet-7.1.1/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/performance_tracking.py` & `volstreet-7.1.1/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/strategies/error_handling.py` & `volstreet-7.1.1/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/strategies/execution.py` & `volstreet-7.1.1/volstreet/strategies/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,26 +514,31 @@
             )
             self.strategies.append(strategy)
 
     @wait_for_login
     def continuously_handle_open_orders(self):
         while not self.session_terminated:
             try:
-                with order_placement_lock:
-                    order_book = fetch_book("orderbook", from_api=True)
-                    if not order_book:
-                        continue
-                    open_orders = get_open_orders(order_book, statuses=["open"])
+                order_placement_lock.acquire()
+                order_book = fetch_book("orderbook", from_api=True)
+                if not order_book:
+                    continue
+                open_orders = get_open_orders(order_book, statuses=["open"])
 
-                    if open_orders.size > 0:
-                        logger.info(f"Modifying open orders at {current_time()}...")
-                        modify_orders(open_orders)
+                if open_orders.size > 0:
+                    logger.info(f"Modifying open orders at {current_time()}...")
+                    modify_orders(open_orders)
             except Exception as e:
                 logger.error(f"Error in continuously handling open orders: {e}")
-            sleep(3)
+            # In Python, the "finally" block is guaranteed to be executed regardless of how the try block is exited.
+            # This includes situations where the try block is exited due to a return, break, or continue statement,
+            # or even if an exception is raised. Hence, the lock gets released in the "finally" block.
+            finally:
+                order_placement_lock.release()
+                sleep(3)
 
 
 def run_client(
     client: Client,
     websockets: bool = True,
     process_manager: Manager = None,
     notifier_level="INFO",
```

### Comparing `volstreet-7.1.0/volstreet/strategies/helpers.py` & `volstreet-7.1.1/volstreet/strategies/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             order_tag=order_tag,
             webhook_url=notifier_url,
         )
         self.update_active_qty_and_premium(quantity_in_shares, avg_price)
 
     def update_active_qty_and_premium(self, adjustment_qty: int, avg_price: float):
         self.active_qty = self.active_qty + adjustment_qty
-        self.premium_received = self.premium_received - (adjustment_qty * avg_price)
+        self.premium_received += adjustment_qty * avg_price
 
 
 class PositionMonitor:
     def __init__(self, underlying: Index, **kwargs):
         self.underlying = underlying
         self.instrument = None
         self.position_active = False
@@ -790,17 +790,21 @@
             self.prospective_calls, True
         )
         put_greeks = self.prepare_greek_frame_with_options(self.prospective_puts, False)
         all_greeks = np.concatenate([call_greeks, put_greeks])
         # At this point all_greeks has the following columns:
         # [strike, ltp, delta, gamma, theta, vega, option]
 
-        # Hardcoded gamma scaler 1000 since we are optimizing theta which is very high relative to gamma
-        all_greeks[:, 3] = all_greeks[:, 3] * 1000
+        # Gamma scaling
+        # Minimum of the ratios of absolute-theta/gamma. Dividing by 2 just for safety.
+        # Preliminary study shows dividing does not matter all that much
+        g_scaler = min(abs(all_greeks[:, 4]) / all_greeks[:, 3]) / 2
+        all_greeks[:, 3] = all_greeks[:, 3] * g_scaler
 
+        # Solving the optimization problem
         prob, weights = delta_neutral_optimization_lp(
             all_greeks[:, 2:6]
         )  # Using delta, gamma, theta, vega
 
         if prob.status != 1:
             logger.warning(
                 f"Optimization failed with status {LpStatus[prob.status]}. "
@@ -924,14 +928,15 @@
 
         date = current_time().strftime("%Y-%m-%d")
         file_path = f"{ActiveSession.obj.userId}\\{self.underlying.name}_delta_data\\{date}.json"
 
         position_status = {
             "timestamp": current_time(),
             "underlying": self.underlying.name,
+            "underlying_price": self.underlying.fetch_ltp(),
             "expiry": self.expiry,
             "base_exposure_qty": self.base_exposure_qty,
             "active_call_options": [
                 {
                     "strike": option.strike,
                     "option_type": option.option_type.value,
                     "active_qty": option.active_qty,
@@ -950,20 +955,20 @@
                     "current_ltp": option.current_ltp,
                     "current_greeks": option.current_greeks.as_dict(),
                 }
                 for option in self.active_put_options
             ],
             "aggregate_greeks": self.aggregate_greeks().as_dict(),
             "total_premium_received": sum(
-                [option.premium_received for option in self.active_options]
+                [option.premium_received for option in self.all_options]
             ),
             "total_premium_outstanding": sum(
                 [option.premium_outstanding for option in self.active_options]
             ),
-            "mtm": sum([option.mtm for option in self.active_options]),
+            "mtm": sum([option.mtm for option in self.all_options]),
             "exit_triggers": self.exit_triggers,
         }
 
         load_combine_save_json_data(position_status, file_path, default_structure=list)
 
 
 def generate_optimized_result(
@@ -1389,17 +1394,15 @@
     if tasks_to_perform is None:
         tasks_to_perform = []
 
     # Determining the next timestamp
     if isinstance(interval_minutes, int):
         next_timestamp = (time_now + timedelta(minutes=interval_minutes)).replace(
             second=0, microsecond=0
-        ) - timedelta(
-            seconds=2
-        )  # 2 seconds buffer
+        )
     elif isinstance(interval_minutes, float):
         next_timestamp = time_now + timedelta(minutes=interval_minutes)
     else:
         raise ValueError("Invalid interval_minutes value")
     next_timestamp = min(
         next_timestamp,
         current_time().replace(
```

### Comparing `volstreet-7.1.0/volstreet/strategies/optimization.py` & `volstreet-7.1.1/volstreet/strategies/optimization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 from scipy.optimize import minimize, dual_annealing
 import numpy as np
 from volstreet import logger, OptimizationError
 from pulp import LpProblem, LpMaximize, LpVariable, lpSum, lpDot, LpStatus, value
 
 
-def delta_neutral_optimization_lp(greeks: np.ndarray) -> tuple[LpProblem, np.ndarray]:
-
-    logger.info(f"Starting delta neutral optimization for greeks: {greeks}")
-
+def generate_base_problem(greeks: np.ndarray) -> tuple[LpProblem, dict]:
     call_greeks = greeks[np.argwhere(greeks[:, 0] > 0).flatten()]
     put_greeks = greeks[np.argwhere(greeks[:, 0] < 0).flatten()]
 
-    call_delta = call_greeks[:, 0]
-    call_gamma = call_greeks[:, 1]
-    call_theta = call_greeks[:, 2]
-
-    put_delta = put_greeks[:, 0]
-    put_gamma = put_greeks[:, 1]
-    put_theta = put_greeks[:, 2]
-
-    # Create a new LP problem
-    prob = LpProblem("Delta_Neutral_Optimization", LpMaximize)
+    call_deltas = call_greeks[:, 0]
+    call_gammas = call_greeks[:, 1]
+    call_thetas = call_greeks[:, 2]
+
+    put_deltas = put_greeks[:, 0]
+    put_gammas = put_greeks[:, 1]
+    put_thetas = put_greeks[:, 2]
 
     # Define decision variables
     x = [
         LpVariable(f"call_{i}", cat="Continuous", upBound=1, lowBound=-1)
         for i in range(len(call_greeks))
     ]
     y = [
@@ -37,64 +31,115 @@
         for i in range(len(x))
     ]
     abs_y = [
         LpVariable(f"abs_put_{i}", cat="Continuous", upBound=1, lowBound=0)
         for i in range(len(y))
     ]
 
-    call_total_delta = lpDot(x, call_delta)
-    call_total_theta = lpDot(x, call_theta)
-    call_total_gamma = lpDot(x, call_gamma)
-
-    put_total_delta = lpDot(y, put_delta)
-    put_total_theta = lpDot(y, put_theta)
-    put_total_gamma = lpDot(y, put_gamma)
-
-    # Set objective function
-    prob += lpSum(
-        [(call_total_theta + put_total_theta), (call_total_gamma + put_total_gamma)]
-    )
-
-    # Add constraints
+    call_total_delta = lpDot(x, call_deltas)
+    call_total_theta = lpDot(x, call_thetas)
+    call_total_gamma = lpDot(x, call_gammas)
+
+    put_total_delta = lpDot(y, put_deltas)
+    put_total_theta = lpDot(y, put_thetas)
+    put_total_gamma = lpDot(y, put_gammas)
 
-    # DELTA CONSTRAINTS
-    prob += lpSum([call_total_delta, put_total_delta]) <= 0.005  # Delta constraint
-    prob += lpSum([call_total_delta, put_total_delta]) >= -0.005  # Delta constraint
+    # Create a new LP problem
+    prob = LpProblem("Optimization", LpMaximize)
 
     # QUANTITY CONSTRAINTS
-    prob += lpSum(x) == 0  # Total quantity of calls should be 0
-    prob += lpSum(y) == 0  # Total quantity of puts should be 0
 
+    # Linking abs_x and x
     for i in range(len(x)):
         prob += abs_x[i] >= x[i]
         prob += abs_x[i] >= -x[i]
 
+    # Linking abs_y and y
     for i in range(len(y)):
         prob += abs_y[i] >= y[i]
         prob += abs_y[i] >= -y[i]
 
+    prob += lpSum(x) == 0  # Total quantity of calls should be 0
+    prob += lpSum(y) == 0  # Total quantity of puts should be 0
     prob += lpSum(abs_x) >= 1.99  # Total abs quantity of calls should be 2
     prob += lpSum(abs_x) <= 2  # Total abs quantity of calls should be 2
-
     prob += lpSum(abs_y) >= 1.99  # Total abs quantity of puts should be 2
     prob += lpSum(abs_y) <= 2  # Total abs quantity of puts should be 2
 
+    vars_dict = {
+        "call": {
+            "weights": x,
+            "deltas": call_deltas,
+            "gammas": call_gammas,
+            "thetas": call_thetas,
+            "total_delta": call_total_delta,
+            "total_theta": call_total_theta,
+            "total_gamma": call_total_gamma,
+        },
+        "put": {
+            "weights": y,
+            "deltas": put_deltas,
+            "gammas": put_gammas,
+            "thetas": put_thetas,
+            "total_delta": put_total_delta,
+            "total_theta": put_total_theta,
+            "total_gamma": put_total_gamma,
+        },
+    }
+
+    return prob, vars_dict
+
+
+def delta_neutral_optimization_lp(greeks: np.ndarray) -> tuple[LpProblem, np.ndarray]:
+    logger.info(f"Starting delta neutral optimization for greeks: {greeks}")
+
+    prob, vars_dict = generate_base_problem(greeks)
+
+    call_total_delta = vars_dict["call"]["total_delta"]
+    call_total_theta = vars_dict["call"]["total_theta"]
+    call_total_gamma = vars_dict["call"]["total_gamma"]
+
+    put_total_delta = vars_dict["put"]["total_delta"]
+    put_total_theta = vars_dict["put"]["total_theta"]
+    put_total_gamma = vars_dict["put"]["total_gamma"]
+
+    # Set objective function
+    prob += lpSum(
+        [(call_total_theta + put_total_theta), (call_total_gamma + put_total_gamma)]
+    )
+
+    # Add constraints
+
+    # DELTA CONSTRAINTS
+    prob += lpSum([call_total_delta, put_total_delta]) <= 0.005  # Delta constraint
+    prob += lpSum([call_total_delta, put_total_delta]) >= -0.005  # Delta constraint
+
+    # THETA POSITIVE AND GAMMA NEGATIVE
+    prob += lpSum([call_total_theta, put_total_theta]) >= 0  # Theta constraint
+    prob += lpSum([call_total_gamma, put_total_gamma]) <= 0  # Gamma constraint
+
     # GAMMA CONSTRAINT
+    call_gammas = vars_dict["call"]["gammas"]
+    put_gammas = vars_dict["put"]["gammas"]
 
     # Hardcoded that our gamma should be less than the 25th percentile of the gamma values
-    gamma_percentile_25_call = np.percentile(call_gamma, 25)
-    gamma_percentile_25_put = np.percentile(put_gamma, 25)
-    total_threshold = gamma_percentile_25_call + gamma_percentile_25_put
-    prob += -1 * lpSum([call_total_gamma, put_total_gamma]) <= total_threshold
+    gamma_percentile_25_call = np.percentile(call_gammas, 25)
+    gamma_percentile_25_put = np.percentile(put_gammas, 25)
+    total_threshold = (
+        gamma_percentile_25_call + gamma_percentile_25_put
+    ) * -1  # Negative to mimic sell position
+
+    # We should try to outperform the 25th percentile gamma
+    prob += lpSum([call_total_gamma, put_total_gamma]) >= total_threshold
 
     # Solve the problem
     prob.solve()
 
-    call_weights = np.array([v.varValue for v in x])
-    put_weights = np.array([v.varValue for v in y])
+    call_weights = np.array([v.varValue for v in vars_dict["call"]["weights"]])
+    put_weights = np.array([v.varValue for v in vars_dict["put"]["weights"]])
 
     combined_weights = np.concatenate([call_weights, put_weights])
 
     logger.info(
         f"Status of optimization: {LpStatus[prob.status]}, "
         f"Objective value: {value(prob.objective)}. "
         f"Call Delta, Theta, Gamma: {value(call_total_delta)}, {value(call_total_theta)}, {value(call_total_gamma)}. "
```

### Comparing `volstreet-7.1.0/volstreet/strategies/strats.py` & `volstreet-7.1.1/volstreet/strategies/strats.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,16 +353,20 @@
         delta_position.update_underlying()
         delta_position.set_recommended_qty(target_delta, optimized)
         delta_position.adjust_recommended_qty()
         delta_position.enter_positions()
         delta_position.reset_trigger_flags()
 
         def interruption_condition():
-            return abs(delta_position.aggregate_greeks().delta) > 0.07 * base_qty_shares
             # Hard coded 7% of base qty shares as the threshold for interruption
+            condition_1 = (
+                abs(delta_position.aggregate_greeks().delta) > 0.07 * base_qty_shares
+            )
+            condition_2 = False  # todo: Add a condition that always maximizes Theta
+            return condition_1 or condition_2
 
         # Delta hedging begins here
         while not any(delta_position.exit_triggers.values()):
             sleep_until_next_action(
                 delta_interval_minutes,
                 exit_time,
                 special_condition=interruption_condition,
@@ -573,48 +577,44 @@
     # Loading current position
     buy_strangle, buy_quantity_in_lots = load_current_strangle(
         underlying_str=underlying.name,
         user_id=ActiveSession.obj.userId,
         file_appendix="overnight_positions",
     )
 
+    notifier(
+        f"{underlying.name} Exiting current position {buy_strangle}",
+        notification_url,
+        "INFO",
+    )
+
     trade_info_dict = {
         "Date": current_time().strftime("%d-%m-%Y %H:%M:%S"),
         "Underlying": underlying.name,
     }
 
     call_buy_avg, put_buy_avg = np.nan, np.nan
     call_sell_avg, put_sell_avg = np.nan, np.nan
 
     # Placing orders
     if buy_strangle is None and sell_strangle is None:
-        notifier(f"{underlying.name} No trade required.", notification_url, "INFO")
+        notifier(f"{underlying.name} No trade possible.", notification_url, "INFO")
     elif sell_strangle is None:  # only exiting current position
-        notifier(
-            f"{underlying.name} Exiting current position on {buy_strangle}.",
-            notification_url,
-            "INFO",
-        )
         execution_details = execute_instructions(
             {
                 buy_strangle: {
                     "action": Action.BUY,
                     "quantity_in_lots": buy_quantity_in_lots,
                     "order_tag": strategy_tag,
                 }
             }
         )
         call_buy_avg, put_buy_avg = execution_details[buy_strangle]
 
     elif buy_strangle is None:  # only entering new position
-        notifier(
-            f"{underlying.name} Entering new position on {buy_strangle}.",
-            notification_url,
-            "INFO",
-        )
         execution_details = execute_instructions(
             {
                 sell_strangle: {
                     "action": Action.SELL,
                     "quantity_in_lots": quantity_in_lots,
                     "order_tag": strategy_tag,
                 }
@@ -633,19 +633,14 @@
             call_buy_avg, put_buy_avg, call_sell_avg, put_sell_avg = (
                 call_ltp,
                 put_ltp,
                 call_ltp,
                 put_ltp,
             )
         else:
-            notifier(
-                f"{underlying.name} Buying {buy_strangle} and selling {sell_strangle}.",
-                notification_url,
-                "INFO",
-            )
             execution_details = execute_instructions(
                 {
                     buy_strangle: {
                         "action": Action.BUY,
                         "quantity_in_lots": buy_quantity_in_lots,
                         "order_tag": strategy_tag,
                     },
@@ -2147,15 +2142,15 @@
             hedge_instrument = Option(
                 strike=hedge_strike,
                 option_type=hedge_option_type,
                 underlying=underlying.name,
                 expiry=underlying.current_expiry,
             )
             instructions[hedge_instrument] = {
-                "action": ~action,
+                "action": Action.SELL,
                 "quantity_in_lots": quantity_in_lots,
                 "order_tag": strategy_tag + " hedge",
             }
 
         else:
             hedge_strike = np.nan
             hedge_instrument = 0
@@ -2231,15 +2226,15 @@
                 "quantity_in_lots": quantity_in_lots,
                 "order_tag": strategy_tag,
                 "square_off_order": True,
             }
         }
         if execute_hedge:
             instructions[hedge_instrument] = {
-                "action": action,
+                "action": Action.BUY,
                 "quantity_in_lots": quantity_in_lots,
                 "order_tag": strategy_tag,
                 "square_off_order": True,
             }
 
         execution_details = execute_instructions(instructions)
         call_exit_price, put_exit_price = execution_details[atm_synthetic_fut]
```

### Comparing `volstreet-7.1.0/volstreet/trade_interface/instruments.py` & `volstreet-7.1.1/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/trade_interface/order_execution.py` & `volstreet-7.1.1/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/trade_interface/order_placement.py` & `volstreet-7.1.1/volstreet/trade_interface/order_placement.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/trade_interface/underlyings.py` & `volstreet-7.1.1/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/utils/change_config.py` & `volstreet-7.1.1/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/utils/communication.py` & `volstreet-7.1.1/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/utils/core.py` & `volstreet-7.1.1/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/utils/data_io.py` & `volstreet-7.1.1/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/utils/scrip_processing.py` & `volstreet-7.1.1/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/vectorized_blackscholes.py` & `volstreet-7.1.1/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/vslogging/formatters.py` & `volstreet-7.1.1/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/vslogging/logging_config.json` & `volstreet-7.1.1/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/vslogging/logging_setup.py` & `volstreet-7.1.1/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet/vslogging/parsing.py` & `volstreet-7.1.1/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.0/volstreet.egg-info/PKG-INFO` & `volstreet-7.1.1/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.1.0
+Version: 7.1.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.1.0/volstreet.egg-info/SOURCES.txt` & `volstreet-7.1.1/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

