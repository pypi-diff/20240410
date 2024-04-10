# Comparing `tmp/pfund-0.0.1.dev7.tar.gz` & `tmp/pfund-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfund-0.0.1.dev7.tar", max compression
+gzip compressed data, was "pfund-0.0.1.dev8.tar", max compression
```

## Comparing `pfund-0.0.1.dev7.tar` & `pfund-0.0.1.dev8.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0    11355 2024-02-06 15:08:56.890856 pfund-0.0.1.dev7/LICENSE
--rw-r--r--   0        0        0    11039 2024-04-07 04:39:43.468423 pfund-0.0.1.dev7/README.md
--rw-r--r--   0        0        0      321 2024-04-02 10:11:02.227146 pfund-0.0.1.dev7/pfund/CONTRIBUTING.md
--rw-r--r--   0        0        0      952 2024-04-03 07:01:02.777543 pfund-0.0.1.dev7/pfund/__init__.py
--rw-r--r--   0        0        0      155 2024-01-30 15:01:45.803425 pfund-0.0.1.dev7/pfund/accounts/__init__.py
--rw-r--r--   0        0        0      743 2024-01-30 15:01:45.806625 pfund-0.0.1.dev7/pfund/accounts/account_base.py
--rw-r--r--   0        0        0     1000 2024-01-30 15:01:45.807227 pfund-0.0.1.dev7/pfund/accounts/account_crypto.py
--rw-r--r--   0        0        0      615 2024-01-30 15:01:45.809008 pfund-0.0.1.dev7/pfund/accounts/account_ib.py
--rw-r--r--   0        0        0     2599 2024-03-15 10:53:53.937479 pfund-0.0.1.dev7/pfund/adapter.py
--rw-r--r--   0        0        0       52 2024-04-05 07:01:21.159840 pfund-0.0.1.dev7/pfund/analyzer.py
--rw-r--r--   0        0        0      156 2024-01-30 15:01:45.809984 pfund-0.0.1.dev7/pfund/balances/__init__.py
--rw-r--r--   0        0        0     1390 2024-01-30 15:01:45.811449 pfund-0.0.1.dev7/pfund/balances/balance_base.py
--rw-r--r--   0        0        0      449 2024-01-30 15:01:45.811748 pfund-0.0.1.dev7/pfund/balances/balance_crypto.py
--rw-r--r--   0        0        0      953 2024-01-30 15:01:45.812044 pfund-0.0.1.dev7/pfund/balances/balance_ib.py
--rw-r--r--   0        0        0      149 2024-01-30 15:01:45.812406 pfund-0.0.1.dev7/pfund/brokers/__init__.py
--rw-r--r--   0        0        0     3114 2024-01-30 15:01:45.815600 pfund-0.0.1.dev7/pfund/brokers/broker_backtest.py
--rw-r--r--   0        0        0      609 2024-02-04 14:35:55.856380 pfund-0.0.1.dev7/pfund/brokers/broker_base.py
--rw-r--r--   0        0        0    13203 2024-02-25 11:13:12.191532 pfund-0.0.1.dev7/pfund/brokers/broker_crypto.py
--rw-r--r--   0        0        0     3793 2024-02-04 14:36:28.703645 pfund-0.0.1.dev7/pfund/brokers/broker_live.py
--rw-r--r--   0        0        0       41 2024-01-30 15:01:45.817494 pfund-0.0.1.dev7/pfund/brokers/ib/__init__.py
--rw-r--r--   0        0        0    10473 2024-01-30 15:01:45.821478 pfund-0.0.1.dev7/pfund/brokers/ib/broker_ib.py
--rw-r--r--   0        0        0    12505 2024-01-30 15:01:45.821940 pfund-0.0.1.dev7/pfund/brokers/ib/ib_api.py
--rw-r--r--   0        0        0     5565 2024-01-30 15:01:45.822316 pfund-0.0.1.dev7/pfund/brokers/ib/ib_client.py
--rw-r--r--   0        0        0     9434 2024-01-30 15:01:45.822738 pfund-0.0.1.dev7/pfund/brokers/ib/ib_wrapper.py
--rw-r--r--   0        0        0       66 2024-02-09 08:16:05.819131 pfund-0.0.1.dev7/pfund/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-02-09 08:11:30.211353 pfund-0.0.1.dev7/pfund/cli/commands/__init__.py
--rw-r--r--   0        0        0     2995 2024-03-15 11:27:53.965076 pfund-0.0.1.dev7/pfund/cli/commands/config.py
--rw-r--r--   0        0        0     1379 2024-03-14 14:02:23.158906 pfund-0.0.1.dev7/pfund/cli/commands/docker_compose.py
--rw-r--r--   0        0        0      482 2024-02-14 07:33:56.424587 pfund-0.0.1.dev7/pfund/cli/main.py
--rw-r--r--   0        0        0     1968 2024-02-16 03:08:17.961892 pfund-0.0.1.dev7/pfund/config/bybit/config.yml
--rw-r--r--   0        0        0      213 2024-01-30 15:01:45.824270 pfund-0.0.1.dev7/pfund/config/bybit/lot_sizes_inverse.yml
--rw-r--r--   0        0        0     6131 2024-01-30 15:01:45.824581 pfund-0.0.1.dev7/pfund/config/bybit/lot_sizes_linear.yml
--rw-r--r--   0        0        0    13804 2024-01-30 15:01:45.824913 pfund-0.0.1.dev7/pfund/config/bybit/lot_sizes_option.yml
--rw-r--r--   0        0        0    10101 2024-01-30 15:01:45.825238 pfund-0.0.1.dev7/pfund/config/bybit/lot_sizes_spot.yml
--rw-r--r--   0        0        0      178 2024-01-30 15:01:45.825531 pfund-0.0.1.dev7/pfund/config/bybit/pdt_matchings_inverse.yml
--rw-r--r--   0        0        0     6765 2024-01-30 15:01:45.825785 pfund-0.0.1.dev7/pfund/config/bybit/pdt_matchings_linear.yml
--rw-r--r--   0        0        0        3 2024-01-30 15:01:45.826011 pfund-0.0.1.dev7/pfund/config/bybit/pdt_matchings_option.yml
--rw-r--r--   0        0        0    10720 2024-01-30 15:01:45.826379 pfund-0.0.1.dev7/pfund/config/bybit/pdt_matchings_spot.yml
--rw-r--r--   0        0        0      257 2024-01-30 15:01:45.826793 pfund-0.0.1.dev7/pfund/config/bybit/tick_sizes_inverse.yml
--rw-r--r--   0        0        0     7181 2024-01-30 15:01:45.827089 pfund-0.0.1.dev7/pfund/config/bybit/tick_sizes_linear.yml
--rw-r--r--   0        0        0    12304 2024-01-30 15:01:45.827403 pfund-0.0.1.dev7/pfund/config/bybit/tick_sizes_option.yml
--rw-r--r--   0        0        0    11241 2024-01-30 15:01:45.827703 pfund-0.0.1.dev7/pfund/config/bybit/tick_sizes_spot.yml
--rw-r--r--   0        0        0     2024 2024-04-05 06:07:27.237219 pfund-0.0.1.dev7/pfund/config/configuration.py
--rw-r--r--   0        0        0      563 2024-01-30 15:01:45.828458 pfund-0.0.1.dev7/pfund/config/ib/config.yml
--rw-r--r--   0        0        0     2810 2024-04-05 13:05:59.130620 pfund-0.0.1.dev7/pfund/config/logging.yml
--rw-r--r--   0        0        0     4697 2024-04-05 14:37:42.574104 pfund-0.0.1.dev7/pfund/config_handler.py
--rw-r--r--   0        0        0       65 2024-01-30 15:01:45.829160 pfund-0.0.1.dev7/pfund/const/__init__.py
--rw-r--r--   0        0        0     1686 2024-01-30 15:01:45.830903 pfund-0.0.1.dev7/pfund/const/_zmq_routes.py
--rw-r--r--   0        0        0     1033 2024-04-06 09:32:57.827190 pfund-0.0.1.dev7/pfund/const/commons.py
--rw-r--r--   0        0        0      955 2024-04-05 14:37:15.302051 pfund-0.0.1.dev7/pfund/const/paths.py
--rw-r--r--   0        0        0     1646 2024-04-06 09:33:58.489623 pfund-0.0.1.dev7/pfund/data_tools/data_tool_base.py
--rw-r--r--   0        0        0     9564 2024-04-05 09:10:12.990507 pfund-0.0.1.dev7/pfund/data_tools/data_tool_pandas.py
--rw-r--r--   0        0        0      171 2024-01-30 15:01:45.833717 pfund-0.0.1.dev7/pfund/datas/__init__.py
--rw-r--r--   0        0        0     6716 2024-01-30 15:01:45.838564 pfund-0.0.1.dev7/pfund/datas/data_bar.py
--rw-r--r--   0        0        0      480 2024-01-30 15:01:45.838818 pfund-0.0.1.dev7/pfund/datas/data_base.py
--rw-r--r--   0        0        0     1455 2024-01-30 15:01:45.839101 pfund-0.0.1.dev7/pfund/datas/data_quote.py
--rw-r--r--   0        0        0     1291 2024-01-30 15:01:45.839333 pfund-0.0.1.dev7/pfund/datas/data_tick.py
--rw-r--r--   0        0        0     1845 2024-01-30 15:01:45.839539 pfund-0.0.1.dev7/pfund/datas/data_time_based.py
--rw-r--r--   0        0        0     3105 2024-03-17 07:02:17.135272 pfund-0.0.1.dev7/pfund/datas/resolution.py
--rw-r--r--   0        0        0     1647 2024-01-30 15:01:45.839977 pfund-0.0.1.dev7/pfund/datas/timeframe.py
--rw-r--r--   0        0        0      207 2024-01-30 15:01:45.840501 pfund-0.0.1.dev7/pfund/engines/__init__.py
--rw-r--r--   0        0        0    13392 2024-04-08 11:30:36.424423 pfund-0.0.1.dev7/pfund/engines/backtest_engine.py
--rw-r--r--   0        0        0     4148 2024-04-06 11:27:49.172639 pfund-0.0.1.dev7/pfund/engines/base_engine.py
--rw-r--r--   0        0        0      602 2024-02-05 14:57:27.586210 pfund-0.0.1.dev7/pfund/engines/test_engine.py
--rw-r--r--   0        0        0     8220 2024-04-06 11:35:13.967858 pfund-0.0.1.dev7/pfund/engines/trade_engine.py
--rw-r--r--   0        0        0     1018 2024-04-06 11:30:25.760953 pfund-0.0.1.dev7/pfund/engines/train_engine.py
--rw-r--r--   0        0        0      120 2024-01-30 15:01:45.844589 pfund-0.0.1.dev7/pfund/errors.py
--rw-r--r--   0        0        0        0 2024-01-30 15:01:45.844855 pfund-0.0.1.dev7/pfund/exchanges/__init__.py
--rw-r--r--   0        0        0      258 2024-01-30 15:01:45.848467 pfund-0.0.1.dev7/pfund/exchanges/bybit/__init__.py
--rw-r--r--   0        0        0    17337 2024-04-05 11:01:26.265498 pfund-0.0.1.dev7/pfund/exchanges/bybit/exchange.py
--rw-r--r--   0        0        0    11498 2024-01-30 15:01:45.852818 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api.py
--rw-r--r--   0        0        0     9650 2024-01-30 15:01:45.853371 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse
--rw-r--r--   0        0        0   164823 2024-01-30 15:01:45.854380 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear
--rw-r--r--   0        0        0   227045 2024-01-30 15:01:45.855347 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option
--rw-r--r--   0        0        0    99033 2024-01-30 15:01:45.855940 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot
--rw-r--r--   0        0        0    15516 2024-01-30 15:01:45.856319 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse
--rw-r--r--   0        0        0   262316 2024-01-30 15:01:45.857183 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear
--rw-r--r--   0        0        0   395202 2024-01-30 15:01:45.858710 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option
--rw-r--r--   0        0        0   155302 2024-01-30 15:01:45.860232 pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot
--rw-r--r--   0        0        0       86 2024-01-30 15:01:45.861200 pfund-0.0.1.dev7/pfund/exchanges/bybit/types.py
--rw-r--r--   0        0        0    18581 2024-01-30 15:01:45.861449 pfund-0.0.1.dev7/pfund/exchanges/bybit/ws_api.py
--rw-r--r--   0        0        0    20498 2024-02-16 06:27:07.662274 pfund-0.0.1.dev7/pfund/exchanges/exchange_base.py
--rw-r--r--   0        0        0     4112 2024-01-30 15:01:45.862894 pfund-0.0.1.dev7/pfund/exchanges/rest_api_base.py
--rw-r--r--   0        0        0    26589 2024-01-30 15:01:45.865158 pfund-0.0.1.dev7/pfund/exchanges/ws_api_base.py
--rw-r--r--   0        0        0      481 2024-01-30 15:01:45.876419 pfund-0.0.1.dev7/pfund/externals/ibapi/__init__.py
--rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.902207 pfund-0.0.1.dev7/pfund/externals/ibapi/account_summary_tags.py
--rw-r--r--   0        0        0   149406 2024-01-30 15:01:45.902893 pfund-0.0.1.dev7/pfund/externals/ibapi/client.py
--rw-r--r--   0        0        0     2297 2024-01-30 15:01:45.903103 pfund-0.0.1.dev7/pfund/externals/ibapi/comm.py
--rw-r--r--   0        0        0      892 2024-01-30 15:01:45.903285 pfund-0.0.1.dev7/pfund/externals/ibapi/commission_report.py
--rw-r--r--   0        0        0     7841 2024-01-30 15:01:45.903569 pfund-0.0.1.dev7/pfund/externals/ibapi/common.py
--rw-r--r--   0        0        0     3755 2024-01-30 15:01:45.903915 pfund-0.0.1.dev7/pfund/externals/ibapi/connection.py
--rw-r--r--   0        0        0     6642 2024-01-30 15:01:45.904226 pfund-0.0.1.dev7/pfund/externals/ibapi/contract.py
--rw-r--r--   0        0        0    59604 2024-01-30 15:01:45.904561 pfund-0.0.1.dev7/pfund/externals/ibapi/decoder.py
--rw-r--r--   0        0        0      520 2024-01-30 15:01:45.904809 pfund-0.0.1.dev7/pfund/externals/ibapi/enum_implem.py
--rw-r--r--   0        0        0     1635 2024-01-30 15:01:45.905010 pfund-0.0.1.dev7/pfund/externals/ibapi/errors.py
--rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.905259 pfund-0.0.1.dev7/pfund/externals/ibapi/execution.py
--rw-r--r--   0        0        0     2211 2024-01-30 15:01:45.905484 pfund-0.0.1.dev7/pfund/externals/ibapi/ibapi.pyproj
--rw-r--r--   0        0        0     6366 2024-01-30 15:01:45.905865 pfund-0.0.1.dev7/pfund/externals/ibapi/message.py
--rw-r--r--   0        0        0      507 2024-01-30 15:01:45.906062 pfund-0.0.1.dev7/pfund/externals/ibapi/news.py
--rw-r--r--   0        0        0      358 2024-01-30 15:01:45.906261 pfund-0.0.1.dev7/pfund/externals/ibapi/object_implem.py
--rw-r--r--   0        0        0     9369 2024-01-30 15:01:45.906706 pfund-0.0.1.dev7/pfund/externals/ibapi/order.py
--rw-r--r--   0        0        0     8243 2024-01-30 15:01:45.907140 pfund-0.0.1.dev7/pfund/externals/ibapi/order_condition.py
--rw-r--r--   0        0        0      943 2024-01-30 15:01:45.907503 pfund-0.0.1.dev7/pfund/externals/ibapi/order_state.py
--rw-r--r--   0        0        0    19630 2024-01-30 15:01:45.907745 pfund-0.0.1.dev7/pfund/externals/ibapi/orderdecoder.py
--rw-r--r--   0        0        0     1625 2024-01-30 15:01:45.907978 pfund-0.0.1.dev7/pfund/externals/ibapi/reader.py
--rw-r--r--   0        0        0     2020 2024-01-30 15:01:45.908359 pfund-0.0.1.dev7/pfund/externals/ibapi/scanner.py
--rw-r--r--   0        0        0     5580 2024-01-30 15:01:45.908580 pfund-0.0.1.dev7/pfund/externals/ibapi/server_versions.py
--rw-r--r--   0        0        0      553 2024-01-30 15:01:45.908832 pfund-0.0.1.dev7/pfund/externals/ibapi/softdollartier.py
--rw-r--r--   0        0        0      714 2024-01-30 15:01:45.909202 pfund-0.0.1.dev7/pfund/externals/ibapi/tag_value.py
--rw-r--r--   0        0        0     3876 2024-01-30 15:01:45.909614 pfund-0.0.1.dev7/pfund/externals/ibapi/ticktype.py
--rw-r--r--   0        0        0     4130 2024-01-30 15:01:45.909848 pfund-0.0.1.dev7/pfund/externals/ibapi/utils.py
--rw-r--r--   0        0        0    31944 2024-01-30 15:01:45.910151 pfund-0.0.1.dev7/pfund/externals/ibapi/wrapper.py
--rw-r--r--   0        0        0      200 2024-01-30 15:01:45.910543 pfund-0.0.1.dev7/pfund/indicators/__init__.py
--rw-r--r--   0        0        0     2827 2024-04-05 14:16:41.897924 pfund-0.0.1.dev7/pfund/indicators/indicator_base.py
--rw-r--r--   0        0        0     4205 2024-01-30 15:01:45.915035 pfund-0.0.1.dev7/pfund/indicators/ta_indicator.py
--rw-r--r--   0        0        0     2139 2024-01-30 15:01:45.915296 pfund-0.0.1.dev7/pfund/indicators/talib_indicator.py
--rw-r--r--   0        0        0      458 2024-04-07 08:48:35.477337 pfund-0.0.1.dev7/pfund/investment_profile.py
--rw-r--r--   0        0        0      159 2024-02-09 08:17:15.066455 pfund-0.0.1.dev7/pfund/main.py
--rw-r--r--   0        0        0      396 2024-01-30 15:01:45.921058 pfund-0.0.1.dev7/pfund/managers/__init__.py
--rw-r--r--   0        0        0      997 2024-02-04 11:33:27.199191 pfund-0.0.1.dev7/pfund/managers/base_manager.py
--rw-r--r--   0        0        0     7659 2024-01-30 15:01:45.927572 pfund-0.0.1.dev7/pfund/managers/connection_manager.py
--rw-r--r--   0        0        0    13773 2024-01-30 15:01:45.927876 pfund-0.0.1.dev7/pfund/managers/data_manager.py
--rw-r--r--   0        0        0    12813 2024-01-30 15:01:45.928588 pfund-0.0.1.dev7/pfund/managers/order_manager.py
--rw-r--r--   0        0        0     3893 2024-01-30 15:01:45.929260 pfund-0.0.1.dev7/pfund/managers/portfolio_manager.py
--rw-r--r--   0        0        0      175 2024-01-30 15:01:45.930796 pfund-0.0.1.dev7/pfund/managers/risk_manager.py
--rw-r--r--   0        0        0     8106 2024-02-04 11:33:27.188479 pfund-0.0.1.dev7/pfund/managers/strategy_manager.py
--rw-r--r--   0        0        0     8711 2024-04-07 14:29:00.794577 pfund-0.0.1.dev7/pfund/mixins/backtest.py
--rw-r--r--   0        0        0      236 2024-02-08 07:22:22.864364 pfund-0.0.1.dev7/pfund/models/__init__.py
--rw-r--r--   0        0        0     5016 2024-04-07 14:29:17.258234 pfund-0.0.1.dev7/pfund/models/model_backtest.py
--rw-r--r--   0        0        0    18985 2024-04-07 11:40:41.678552 pfund-0.0.1.dev7/pfund/models/model_base.py
--rw-r--r--   0        0        0     2032 2024-02-23 07:37:29.786952 pfund-0.0.1.dev7/pfund/models/model_meta.py
--rw-r--r--   0        0        0     2659 2024-01-30 15:01:45.939461 pfund-0.0.1.dev7/pfund/models/pytorch_model.py
--rw-r--r--   0        0        0     1188 2024-01-30 15:01:45.939751 pfund-0.0.1.dev7/pfund/models/sklearn_model.py
--rw-r--r--   0        0        0      138 2024-01-30 15:01:45.940227 pfund-0.0.1.dev7/pfund/orders/__init__.py
--rw-r--r--   0        0        0    10415 2024-01-30 15:01:45.943085 pfund-0.0.1.dev7/pfund/orders/order_base.py
--rw-r--r--   0        0        0     1531 2024-01-30 15:01:45.943516 pfund-0.0.1.dev7/pfund/orders/order_crypto.py
--rw-r--r--   0        0        0      230 2024-01-30 15:01:45.943750 pfund-0.0.1.dev7/pfund/orders/order_ib.py
--rw-r--r--   0        0        0      781 2024-01-30 15:01:45.943960 pfund-0.0.1.dev7/pfund/orders/order_statuses.py
--rw-r--r--   0        0        0      150 2024-01-30 15:01:45.944152 pfund-0.0.1.dev7/pfund/orders/order_time_in_force.py
--rw-r--r--   0        0        0     3501 2024-04-02 14:32:03.715956 pfund-0.0.1.dev7/pfund/plogging/__init__.py
--rw-r--r--   0        0        0     3269 2024-02-14 09:55:02.600095 pfund-0.0.1.dev7/pfund/plogging/config.py
--rw-r--r--   0        0        0      409 2024-01-30 15:01:45.920021 pfund-0.0.1.dev7/pfund/plogging/filters.py
--rw-r--r--   0        0        0      578 2024-01-30 15:01:45.920250 pfund-0.0.1.dev7/pfund/plogging/formatter.py
--rw-r--r--   0        0        0     1538 2024-01-30 15:01:45.920455 pfund-0.0.1.dev7/pfund/plogging/handlers.py
--rw-r--r--   0        0        0      155 2024-04-07 08:29:14.055235 pfund-0.0.1.dev7/pfund/portfolio.py
--rw-r--r--   0        0        0      165 2024-01-30 15:01:45.944846 pfund-0.0.1.dev7/pfund/positions/__init__.py
--rw-r--r--   0        0        0     1300 2024-01-30 15:01:45.950043 pfund-0.0.1.dev7/pfund/positions/position_base.py
--rw-r--r--   0        0        0     3655 2024-01-30 15:01:45.950417 pfund-0.0.1.dev7/pfund/positions/position_crypto.py
--rw-r--r--   0        0        0     2304 2024-01-30 15:01:45.950721 pfund-0.0.1.dev7/pfund/positions/position_ib.py
--rw-r--r--   0        0        0      155 2024-01-30 15:01:45.952029 pfund-0.0.1.dev7/pfund/products/__init__.py
--rw-r--r--   0        0        0     1593 2024-01-30 15:01:45.958189 pfund-0.0.1.dev7/pfund/products/product_base.py
--rw-r--r--   0        0        0     3275 2024-01-30 15:01:45.958561 pfund-0.0.1.dev7/pfund/products/product_crypto.py
--rw-r--r--   0        0        0     2334 2024-01-30 15:01:45.958836 pfund-0.0.1.dev7/pfund/products/product_ib.py
--rw-r--r--   0        0        0       71 2024-01-30 15:01:45.959095 pfund-0.0.1.dev7/pfund/risk_monitor.py
--rw-r--r--   0        0        0       82 2024-01-30 15:01:45.959597 pfund-0.0.1.dev7/pfund/strategies/__init__.py
--rw-r--r--   0        0        0      241 2024-04-07 08:19:32.706134 pfund-0.0.1.dev7/pfund/strategies/allocation_strategy.py
--rw-r--r--   0        0        0      393 2024-04-07 08:17:21.167790 pfund-0.0.1.dev7/pfund/strategies/diversification_strategy.py
--rw-r--r--   0        0        0      225 2024-04-07 08:13:37.900582 pfund-0.0.1.dev7/pfund/strategies/hedging_strategy.py
--rw-r--r--   0        0        0      384 2024-04-07 08:19:25.707439 pfund-0.0.1.dev7/pfund/strategies/optimization_strategy.py
--rw-r--r--   0        0        0     1326 2024-04-07 08:25:28.806424 pfund-0.0.1.dev7/pfund/strategies/portfolio_strategy.py
--rw-r--r--   0        0        0      233 2024-04-07 08:13:09.996763 pfund-0.0.1.dev7/pfund/strategies/rebalancing_strategy.py
--rw-r--r--   0        0        0     2682 2024-04-07 14:29:23.602709 pfund-0.0.1.dev7/pfund/strategies/strategy_backtest.py
--rw-r--r--   0        0        0    24691 2024-04-07 11:40:34.659660 pfund-0.0.1.dev7/pfund/strategies/strategy_base.py
--rw-r--r--   0        0        0      930 2024-04-05 18:16:14.568282 pfund-0.0.1.dev7/pfund/strategies/strategy_meta.py
--rw-r--r--   0        0        0      241 2024-04-06 11:12:13.515286 pfund-0.0.1.dev7/pfund/types/backtest.py
--rw-r--r--   0        0        0     1212 2024-04-06 09:36:38.856874 pfund-0.0.1.dev7/pfund/types/common_literals.py
--rw-r--r--   0        0        0      509 2024-04-06 09:57:47.537645 pfund-0.0.1.dev7/pfund/types/core.py
--rw-r--r--   0        0        0      306 2024-04-07 08:48:23.503775 pfund-0.0.1.dev7/pfund/universe.py
--rw-r--r--   0        0        0     2455 2024-02-25 13:48:46.475416 pfund-0.0.1.dev7/pfund/utils/aliases.py
--rw-r--r--   0        0        0      591 2024-01-30 15:01:45.966245 pfund-0.0.1.dev7/pfund/utils/envs.py
--rw-r--r--   0        0        0     5268 2024-04-05 13:22:38.753674 pfund-0.0.1.dev7/pfund/utils/utils.py
--rw-r--r--   0        0        0     4033 2024-01-30 15:01:45.966936 pfund-0.0.1.dev7/pfund/zeromq.py
--rw-r--r--   0        0        0     1813 2024-04-09 13:32:46.564362 pfund-0.0.1.dev7/pyproject.toml
--rw-r--r--   0        0        0    12386 1970-01-01 00:00:00.000000 pfund-0.0.1.dev7/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-02-06 15:08:56.890856 pfund-0.0.1.dev8/LICENSE
+-rw-r--r--   0        0        0    11039 2024-04-07 04:39:43.468423 pfund-0.0.1.dev8/README.md
+-rw-r--r--   0        0        0      260 2024-04-09 15:18:33.828194 pfund-0.0.1.dev8/pfund/CONTRIBUTING.md
+-rw-r--r--   0        0        0      952 2024-04-03 07:01:02.777543 pfund-0.0.1.dev8/pfund/__init__.py
+-rw-r--r--   0        0        0      155 2024-01-30 15:01:45.803425 pfund-0.0.1.dev8/pfund/accounts/__init__.py
+-rw-r--r--   0        0        0      743 2024-01-30 15:01:45.806625 pfund-0.0.1.dev8/pfund/accounts/account_base.py
+-rw-r--r--   0        0        0     1000 2024-01-30 15:01:45.807227 pfund-0.0.1.dev8/pfund/accounts/account_crypto.py
+-rw-r--r--   0        0        0      615 2024-01-30 15:01:45.809008 pfund-0.0.1.dev8/pfund/accounts/account_ib.py
+-rw-r--r--   0        0        0     2599 2024-03-15 10:53:53.937479 pfund-0.0.1.dev8/pfund/adapter.py
+-rw-r--r--   0        0        0       52 2024-04-05 07:01:21.159840 pfund-0.0.1.dev8/pfund/analyzer.py
+-rw-r--r--   0        0        0      156 2024-01-30 15:01:45.809984 pfund-0.0.1.dev8/pfund/balances/__init__.py
+-rw-r--r--   0        0        0     1390 2024-01-30 15:01:45.811449 pfund-0.0.1.dev8/pfund/balances/balance_base.py
+-rw-r--r--   0        0        0      449 2024-01-30 15:01:45.811748 pfund-0.0.1.dev8/pfund/balances/balance_crypto.py
+-rw-r--r--   0        0        0      953 2024-01-30 15:01:45.812044 pfund-0.0.1.dev8/pfund/balances/balance_ib.py
+-rw-r--r--   0        0        0      149 2024-01-30 15:01:45.812406 pfund-0.0.1.dev8/pfund/brokers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-01-30 15:01:45.815600 pfund-0.0.1.dev8/pfund/brokers/broker_backtest.py
+-rw-r--r--   0        0        0      609 2024-02-04 14:35:55.856380 pfund-0.0.1.dev8/pfund/brokers/broker_base.py
+-rw-r--r--   0        0        0    13203 2024-02-25 11:13:12.191532 pfund-0.0.1.dev8/pfund/brokers/broker_crypto.py
+-rw-r--r--   0        0        0     3793 2024-02-04 14:36:28.703645 pfund-0.0.1.dev8/pfund/brokers/broker_live.py
+-rw-r--r--   0        0        0       41 2024-01-30 15:01:45.817494 pfund-0.0.1.dev8/pfund/brokers/ib/__init__.py
+-rw-r--r--   0        0        0    10473 2024-01-30 15:01:45.821478 pfund-0.0.1.dev8/pfund/brokers/ib/broker_ib.py
+-rw-r--r--   0        0        0    12505 2024-01-30 15:01:45.821940 pfund-0.0.1.dev8/pfund/brokers/ib/ib_api.py
+-rw-r--r--   0        0        0     5565 2024-01-30 15:01:45.822316 pfund-0.0.1.dev8/pfund/brokers/ib/ib_client.py
+-rw-r--r--   0        0        0     9434 2024-01-30 15:01:45.822738 pfund-0.0.1.dev8/pfund/brokers/ib/ib_wrapper.py
+-rw-r--r--   0        0        0       66 2024-02-09 08:16:05.819131 pfund-0.0.1.dev8/pfund/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:11:30.211353 pfund-0.0.1.dev8/pfund/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2995 2024-03-15 11:27:53.965076 pfund-0.0.1.dev8/pfund/cli/commands/config.py
+-rw-r--r--   0        0        0     1379 2024-03-14 14:02:23.158906 pfund-0.0.1.dev8/pfund/cli/commands/docker_compose.py
+-rw-r--r--   0        0        0      482 2024-02-14 07:33:56.424587 pfund-0.0.1.dev8/pfund/cli/main.py
+-rw-r--r--   0        0        0     1968 2024-02-16 03:08:17.961892 pfund-0.0.1.dev8/pfund/config/bybit/config.yml
+-rw-r--r--   0        0        0      213 2024-01-30 15:01:45.824270 pfund-0.0.1.dev8/pfund/config/bybit/lot_sizes_inverse.yml
+-rw-r--r--   0        0        0     6131 2024-01-30 15:01:45.824581 pfund-0.0.1.dev8/pfund/config/bybit/lot_sizes_linear.yml
+-rw-r--r--   0        0        0    13804 2024-01-30 15:01:45.824913 pfund-0.0.1.dev8/pfund/config/bybit/lot_sizes_option.yml
+-rw-r--r--   0        0        0    10101 2024-01-30 15:01:45.825238 pfund-0.0.1.dev8/pfund/config/bybit/lot_sizes_spot.yml
+-rw-r--r--   0        0        0      178 2024-01-30 15:01:45.825531 pfund-0.0.1.dev8/pfund/config/bybit/pdt_matchings_inverse.yml
+-rw-r--r--   0        0        0     6765 2024-01-30 15:01:45.825785 pfund-0.0.1.dev8/pfund/config/bybit/pdt_matchings_linear.yml
+-rw-r--r--   0        0        0        3 2024-01-30 15:01:45.826011 pfund-0.0.1.dev8/pfund/config/bybit/pdt_matchings_option.yml
+-rw-r--r--   0        0        0    10720 2024-01-30 15:01:45.826379 pfund-0.0.1.dev8/pfund/config/bybit/pdt_matchings_spot.yml
+-rw-r--r--   0        0        0      257 2024-01-30 15:01:45.826793 pfund-0.0.1.dev8/pfund/config/bybit/tick_sizes_inverse.yml
+-rw-r--r--   0        0        0     7181 2024-01-30 15:01:45.827089 pfund-0.0.1.dev8/pfund/config/bybit/tick_sizes_linear.yml
+-rw-r--r--   0        0        0    12304 2024-01-30 15:01:45.827403 pfund-0.0.1.dev8/pfund/config/bybit/tick_sizes_option.yml
+-rw-r--r--   0        0        0    11241 2024-01-30 15:01:45.827703 pfund-0.0.1.dev8/pfund/config/bybit/tick_sizes_spot.yml
+-rw-r--r--   0        0        0     2024 2024-04-05 06:07:27.237219 pfund-0.0.1.dev8/pfund/config/configuration.py
+-rw-r--r--   0        0        0      563 2024-01-30 15:01:45.828458 pfund-0.0.1.dev8/pfund/config/ib/config.yml
+-rw-r--r--   0        0        0     2810 2024-04-05 13:05:59.130620 pfund-0.0.1.dev8/pfund/config/logging.yml
+-rw-r--r--   0        0        0     4697 2024-04-05 14:37:42.574104 pfund-0.0.1.dev8/pfund/config_handler.py
+-rw-r--r--   0        0        0       65 2024-01-30 15:01:45.829160 pfund-0.0.1.dev8/pfund/const/__init__.py
+-rw-r--r--   0        0        0     1686 2024-01-30 15:01:45.830903 pfund-0.0.1.dev8/pfund/const/_zmq_routes.py
+-rw-r--r--   0        0        0     1033 2024-04-06 09:32:57.827190 pfund-0.0.1.dev8/pfund/const/commons.py
+-rw-r--r--   0        0        0      955 2024-04-05 14:37:15.302051 pfund-0.0.1.dev8/pfund/const/paths.py
+-rw-r--r--   0        0        0     1646 2024-04-06 09:33:58.489623 pfund-0.0.1.dev8/pfund/data_tools/data_tool_base.py
+-rw-r--r--   0        0        0     9564 2024-04-05 09:10:12.990507 pfund-0.0.1.dev8/pfund/data_tools/data_tool_pandas.py
+-rw-r--r--   0        0        0      171 2024-01-30 15:01:45.833717 pfund-0.0.1.dev8/pfund/datas/__init__.py
+-rw-r--r--   0        0        0     6716 2024-01-30 15:01:45.838564 pfund-0.0.1.dev8/pfund/datas/data_bar.py
+-rw-r--r--   0        0        0      480 2024-01-30 15:01:45.838818 pfund-0.0.1.dev8/pfund/datas/data_base.py
+-rw-r--r--   0        0        0     1455 2024-01-30 15:01:45.839101 pfund-0.0.1.dev8/pfund/datas/data_quote.py
+-rw-r--r--   0        0        0     1291 2024-01-30 15:01:45.839333 pfund-0.0.1.dev8/pfund/datas/data_tick.py
+-rw-r--r--   0        0        0     1845 2024-01-30 15:01:45.839539 pfund-0.0.1.dev8/pfund/datas/data_time_based.py
+-rw-r--r--   0        0        0     3105 2024-03-17 07:02:17.135272 pfund-0.0.1.dev8/pfund/datas/resolution.py
+-rw-r--r--   0        0        0     1647 2024-01-30 15:01:45.839977 pfund-0.0.1.dev8/pfund/datas/timeframe.py
+-rw-r--r--   0        0        0      207 2024-01-30 15:01:45.840501 pfund-0.0.1.dev8/pfund/engines/__init__.py
+-rw-r--r--   0        0        0    13392 2024-04-08 11:30:36.424423 pfund-0.0.1.dev8/pfund/engines/backtest_engine.py
+-rw-r--r--   0        0        0     4148 2024-04-06 11:27:49.172639 pfund-0.0.1.dev8/pfund/engines/base_engine.py
+-rw-r--r--   0        0        0      602 2024-02-05 14:57:27.586210 pfund-0.0.1.dev8/pfund/engines/test_engine.py
+-rw-r--r--   0        0        0     8220 2024-04-06 11:35:13.967858 pfund-0.0.1.dev8/pfund/engines/trade_engine.py
+-rw-r--r--   0        0        0     1018 2024-04-06 11:30:25.760953 pfund-0.0.1.dev8/pfund/engines/train_engine.py
+-rw-r--r--   0        0        0      120 2024-01-30 15:01:45.844589 pfund-0.0.1.dev8/pfund/errors.py
+-rw-r--r--   0        0        0        0 2024-01-30 15:01:45.844855 pfund-0.0.1.dev8/pfund/exchanges/__init__.py
+-rw-r--r--   0        0        0      258 2024-01-30 15:01:45.848467 pfund-0.0.1.dev8/pfund/exchanges/bybit/__init__.py
+-rw-r--r--   0        0        0    17337 2024-04-05 11:01:26.265498 pfund-0.0.1.dev8/pfund/exchanges/bybit/exchange.py
+-rw-r--r--   0        0        0    11498 2024-01-30 15:01:45.852818 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api.py
+-rw-r--r--   0        0        0     9650 2024-01-30 15:01:45.853371 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse
+-rw-r--r--   0        0        0   164823 2024-01-30 15:01:45.854380 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear
+-rw-r--r--   0        0        0   227045 2024-01-30 15:01:45.855347 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option
+-rw-r--r--   0        0        0    99033 2024-01-30 15:01:45.855940 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot
+-rw-r--r--   0        0        0    15516 2024-01-30 15:01:45.856319 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse
+-rw-r--r--   0        0        0   262316 2024-01-30 15:01:45.857183 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear
+-rw-r--r--   0        0        0   395202 2024-01-30 15:01:45.858710 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option
+-rw-r--r--   0        0        0   155302 2024-01-30 15:01:45.860232 pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot
+-rw-r--r--   0        0        0       86 2024-01-30 15:01:45.861200 pfund-0.0.1.dev8/pfund/exchanges/bybit/types.py
+-rw-r--r--   0        0        0    18581 2024-01-30 15:01:45.861449 pfund-0.0.1.dev8/pfund/exchanges/bybit/ws_api.py
+-rw-r--r--   0        0        0    20498 2024-02-16 06:27:07.662274 pfund-0.0.1.dev8/pfund/exchanges/exchange_base.py
+-rw-r--r--   0        0        0     4112 2024-01-30 15:01:45.862894 pfund-0.0.1.dev8/pfund/exchanges/rest_api_base.py
+-rw-r--r--   0        0        0    26589 2024-01-30 15:01:45.865158 pfund-0.0.1.dev8/pfund/exchanges/ws_api_base.py
+-rw-r--r--   0        0        0      481 2024-01-30 15:01:45.876419 pfund-0.0.1.dev8/pfund/externals/ibapi/__init__.py
+-rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.902207 pfund-0.0.1.dev8/pfund/externals/ibapi/account_summary_tags.py
+-rw-r--r--   0        0        0   149406 2024-01-30 15:01:45.902893 pfund-0.0.1.dev8/pfund/externals/ibapi/client.py
+-rw-r--r--   0        0        0     2297 2024-01-30 15:01:45.903103 pfund-0.0.1.dev8/pfund/externals/ibapi/comm.py
+-rw-r--r--   0        0        0      892 2024-01-30 15:01:45.903285 pfund-0.0.1.dev8/pfund/externals/ibapi/commission_report.py
+-rw-r--r--   0        0        0     7841 2024-01-30 15:01:45.903569 pfund-0.0.1.dev8/pfund/externals/ibapi/common.py
+-rw-r--r--   0        0        0     3755 2024-01-30 15:01:45.903915 pfund-0.0.1.dev8/pfund/externals/ibapi/connection.py
+-rw-r--r--   0        0        0     6642 2024-01-30 15:01:45.904226 pfund-0.0.1.dev8/pfund/externals/ibapi/contract.py
+-rw-r--r--   0        0        0    59604 2024-01-30 15:01:45.904561 pfund-0.0.1.dev8/pfund/externals/ibapi/decoder.py
+-rw-r--r--   0        0        0      520 2024-01-30 15:01:45.904809 pfund-0.0.1.dev8/pfund/externals/ibapi/enum_implem.py
+-rw-r--r--   0        0        0     1635 2024-01-30 15:01:45.905010 pfund-0.0.1.dev8/pfund/externals/ibapi/errors.py
+-rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.905259 pfund-0.0.1.dev8/pfund/externals/ibapi/execution.py
+-rw-r--r--   0        0        0     2211 2024-01-30 15:01:45.905484 pfund-0.0.1.dev8/pfund/externals/ibapi/ibapi.pyproj
+-rw-r--r--   0        0        0     6366 2024-01-30 15:01:45.905865 pfund-0.0.1.dev8/pfund/externals/ibapi/message.py
+-rw-r--r--   0        0        0      507 2024-01-30 15:01:45.906062 pfund-0.0.1.dev8/pfund/externals/ibapi/news.py
+-rw-r--r--   0        0        0      358 2024-01-30 15:01:45.906261 pfund-0.0.1.dev8/pfund/externals/ibapi/object_implem.py
+-rw-r--r--   0        0        0     9369 2024-01-30 15:01:45.906706 pfund-0.0.1.dev8/pfund/externals/ibapi/order.py
+-rw-r--r--   0        0        0     8243 2024-01-30 15:01:45.907140 pfund-0.0.1.dev8/pfund/externals/ibapi/order_condition.py
+-rw-r--r--   0        0        0      943 2024-01-30 15:01:45.907503 pfund-0.0.1.dev8/pfund/externals/ibapi/order_state.py
+-rw-r--r--   0        0        0    19630 2024-01-30 15:01:45.907745 pfund-0.0.1.dev8/pfund/externals/ibapi/orderdecoder.py
+-rw-r--r--   0        0        0     1625 2024-01-30 15:01:45.907978 pfund-0.0.1.dev8/pfund/externals/ibapi/reader.py
+-rw-r--r--   0        0        0     2020 2024-01-30 15:01:45.908359 pfund-0.0.1.dev8/pfund/externals/ibapi/scanner.py
+-rw-r--r--   0        0        0     5580 2024-01-30 15:01:45.908580 pfund-0.0.1.dev8/pfund/externals/ibapi/server_versions.py
+-rw-r--r--   0        0        0      553 2024-01-30 15:01:45.908832 pfund-0.0.1.dev8/pfund/externals/ibapi/softdollartier.py
+-rw-r--r--   0        0        0      714 2024-01-30 15:01:45.909202 pfund-0.0.1.dev8/pfund/externals/ibapi/tag_value.py
+-rw-r--r--   0        0        0     3876 2024-01-30 15:01:45.909614 pfund-0.0.1.dev8/pfund/externals/ibapi/ticktype.py
+-rw-r--r--   0        0        0     4130 2024-01-30 15:01:45.909848 pfund-0.0.1.dev8/pfund/externals/ibapi/utils.py
+-rw-r--r--   0        0        0    31944 2024-01-30 15:01:45.910151 pfund-0.0.1.dev8/pfund/externals/ibapi/wrapper.py
+-rw-r--r--   0        0        0      200 2024-01-30 15:01:45.910543 pfund-0.0.1.dev8/pfund/indicators/__init__.py
+-rw-r--r--   0        0        0     2827 2024-04-05 14:16:41.897924 pfund-0.0.1.dev8/pfund/indicators/indicator_base.py
+-rw-r--r--   0        0        0     4205 2024-01-30 15:01:45.915035 pfund-0.0.1.dev8/pfund/indicators/ta_indicator.py
+-rw-r--r--   0        0        0     2139 2024-01-30 15:01:45.915296 pfund-0.0.1.dev8/pfund/indicators/talib_indicator.py
+-rw-r--r--   0        0        0      458 2024-04-07 08:48:35.477337 pfund-0.0.1.dev8/pfund/investment_profile.py
+-rw-r--r--   0        0        0      159 2024-02-09 08:17:15.066455 pfund-0.0.1.dev8/pfund/main.py
+-rw-r--r--   0        0        0      396 2024-01-30 15:01:45.921058 pfund-0.0.1.dev8/pfund/managers/__init__.py
+-rw-r--r--   0        0        0      997 2024-02-04 11:33:27.199191 pfund-0.0.1.dev8/pfund/managers/base_manager.py
+-rw-r--r--   0        0        0     7659 2024-01-30 15:01:45.927572 pfund-0.0.1.dev8/pfund/managers/connection_manager.py
+-rw-r--r--   0        0        0    13773 2024-01-30 15:01:45.927876 pfund-0.0.1.dev8/pfund/managers/data_manager.py
+-rw-r--r--   0        0        0    12813 2024-01-30 15:01:45.928588 pfund-0.0.1.dev8/pfund/managers/order_manager.py
+-rw-r--r--   0        0        0     3893 2024-01-30 15:01:45.929260 pfund-0.0.1.dev8/pfund/managers/portfolio_manager.py
+-rw-r--r--   0        0        0      175 2024-01-30 15:01:45.930796 pfund-0.0.1.dev8/pfund/managers/risk_manager.py
+-rw-r--r--   0        0        0     8106 2024-02-04 11:33:27.188479 pfund-0.0.1.dev8/pfund/managers/strategy_manager.py
+-rw-r--r--   0        0        0     8711 2024-04-07 14:29:00.794577 pfund-0.0.1.dev8/pfund/mixins/backtest.py
+-rw-r--r--   0        0        0      236 2024-02-08 07:22:22.864364 pfund-0.0.1.dev8/pfund/models/__init__.py
+-rw-r--r--   0        0        0     5016 2024-04-07 14:29:17.258234 pfund-0.0.1.dev8/pfund/models/model_backtest.py
+-rw-r--r--   0        0        0    18985 2024-04-07 11:40:41.678552 pfund-0.0.1.dev8/pfund/models/model_base.py
+-rw-r--r--   0        0        0     2032 2024-02-23 07:37:29.786952 pfund-0.0.1.dev8/pfund/models/model_meta.py
+-rw-r--r--   0        0        0     2659 2024-01-30 15:01:45.939461 pfund-0.0.1.dev8/pfund/models/pytorch_model.py
+-rw-r--r--   0        0        0     1188 2024-01-30 15:01:45.939751 pfund-0.0.1.dev8/pfund/models/sklearn_model.py
+-rw-r--r--   0        0        0      138 2024-01-30 15:01:45.940227 pfund-0.0.1.dev8/pfund/orders/__init__.py
+-rw-r--r--   0        0        0    10415 2024-01-30 15:01:45.943085 pfund-0.0.1.dev8/pfund/orders/order_base.py
+-rw-r--r--   0        0        0     1531 2024-01-30 15:01:45.943516 pfund-0.0.1.dev8/pfund/orders/order_crypto.py
+-rw-r--r--   0        0        0      230 2024-01-30 15:01:45.943750 pfund-0.0.1.dev8/pfund/orders/order_ib.py
+-rw-r--r--   0        0        0      781 2024-01-30 15:01:45.943960 pfund-0.0.1.dev8/pfund/orders/order_statuses.py
+-rw-r--r--   0        0        0      150 2024-01-30 15:01:45.944152 pfund-0.0.1.dev8/pfund/orders/order_time_in_force.py
+-rw-r--r--   0        0        0     3501 2024-04-02 14:32:03.715956 pfund-0.0.1.dev8/pfund/plogging/__init__.py
+-rw-r--r--   0        0        0     3269 2024-02-14 09:55:02.600095 pfund-0.0.1.dev8/pfund/plogging/config.py
+-rw-r--r--   0        0        0      409 2024-01-30 15:01:45.920021 pfund-0.0.1.dev8/pfund/plogging/filters.py
+-rw-r--r--   0        0        0      578 2024-01-30 15:01:45.920250 pfund-0.0.1.dev8/pfund/plogging/formatter.py
+-rw-r--r--   0        0        0     1538 2024-01-30 15:01:45.920455 pfund-0.0.1.dev8/pfund/plogging/handlers.py
+-rw-r--r--   0        0        0      155 2024-04-07 08:29:14.055235 pfund-0.0.1.dev8/pfund/portfolio.py
+-rw-r--r--   0        0        0      165 2024-01-30 15:01:45.944846 pfund-0.0.1.dev8/pfund/positions/__init__.py
+-rw-r--r--   0        0        0     1300 2024-01-30 15:01:45.950043 pfund-0.0.1.dev8/pfund/positions/position_base.py
+-rw-r--r--   0        0        0     3655 2024-01-30 15:01:45.950417 pfund-0.0.1.dev8/pfund/positions/position_crypto.py
+-rw-r--r--   0        0        0     2304 2024-01-30 15:01:45.950721 pfund-0.0.1.dev8/pfund/positions/position_ib.py
+-rw-r--r--   0        0        0      155 2024-01-30 15:01:45.952029 pfund-0.0.1.dev8/pfund/products/__init__.py
+-rw-r--r--   0        0        0     1593 2024-01-30 15:01:45.958189 pfund-0.0.1.dev8/pfund/products/product_base.py
+-rw-r--r--   0        0        0     3275 2024-01-30 15:01:45.958561 pfund-0.0.1.dev8/pfund/products/product_crypto.py
+-rw-r--r--   0        0        0     2334 2024-01-30 15:01:45.958836 pfund-0.0.1.dev8/pfund/products/product_ib.py
+-rw-r--r--   0        0        0       71 2024-01-30 15:01:45.959095 pfund-0.0.1.dev8/pfund/risk_monitor.py
+-rw-r--r--   0        0        0       82 2024-01-30 15:01:45.959597 pfund-0.0.1.dev8/pfund/strategies/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-07 08:19:32.706134 pfund-0.0.1.dev8/pfund/strategies/allocation_strategy.py
+-rw-r--r--   0        0        0      393 2024-04-07 08:17:21.167790 pfund-0.0.1.dev8/pfund/strategies/diversification_strategy.py
+-rw-r--r--   0        0        0      225 2024-04-07 08:13:37.900582 pfund-0.0.1.dev8/pfund/strategies/hedging_strategy.py
+-rw-r--r--   0        0        0      384 2024-04-07 08:19:25.707439 pfund-0.0.1.dev8/pfund/strategies/optimization_strategy.py
+-rw-r--r--   0        0        0     1326 2024-04-07 08:25:28.806424 pfund-0.0.1.dev8/pfund/strategies/portfolio_strategy.py
+-rw-r--r--   0        0        0      233 2024-04-07 08:13:09.996763 pfund-0.0.1.dev8/pfund/strategies/rebalancing_strategy.py
+-rw-r--r--   0        0        0     2682 2024-04-07 14:29:23.602709 pfund-0.0.1.dev8/pfund/strategies/strategy_backtest.py
+-rw-r--r--   0        0        0    24691 2024-04-07 11:40:34.659660 pfund-0.0.1.dev8/pfund/strategies/strategy_base.py
+-rw-r--r--   0        0        0      930 2024-04-05 18:16:14.568282 pfund-0.0.1.dev8/pfund/strategies/strategy_meta.py
+-rw-r--r--   0        0        0      241 2024-04-06 11:12:13.515286 pfund-0.0.1.dev8/pfund/types/backtest.py
+-rw-r--r--   0        0        0     1212 2024-04-06 09:36:38.856874 pfund-0.0.1.dev8/pfund/types/common_literals.py
+-rw-r--r--   0        0        0      509 2024-04-06 09:57:47.537645 pfund-0.0.1.dev8/pfund/types/core.py
+-rw-r--r--   0        0        0      306 2024-04-07 08:48:23.503775 pfund-0.0.1.dev8/pfund/universe.py
+-rw-r--r--   0        0        0     2455 2024-02-25 13:48:46.475416 pfund-0.0.1.dev8/pfund/utils/aliases.py
+-rw-r--r--   0        0        0      591 2024-01-30 15:01:45.966245 pfund-0.0.1.dev8/pfund/utils/envs.py
+-rw-r--r--   0        0        0     5268 2024-04-05 13:22:38.753674 pfund-0.0.1.dev8/pfund/utils/utils.py
+-rw-r--r--   0        0        0     4033 2024-01-30 15:01:45.966936 pfund-0.0.1.dev8/pfund/zeromq.py
+-rw-r--r--   0        0        0     2032 2024-04-09 15:16:40.648825 pfund-0.0.1.dev8/pyproject.toml
+-rw-r--r--   0        0        0    12939 1970-01-01 00:00:00.000000 pfund-0.0.1.dev8/PKG-INFO
```

### Comparing `pfund-0.0.1.dev7/LICENSE` & `pfund-0.0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/README.md` & `pfund-0.0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/__init__.py` & `pfund-0.0.1.dev8/pfund/__init__.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/accounts/account_base.py` & `pfund-0.0.1.dev8/pfund/accounts/account_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/accounts/account_crypto.py` & `pfund-0.0.1.dev8/pfund/accounts/account_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/accounts/account_ib.py` & `pfund-0.0.1.dev8/pfund/accounts/account_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/adapter.py` & `pfund-0.0.1.dev8/pfund/adapter.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/balances/balance_base.py` & `pfund-0.0.1.dev8/pfund/balances/balance_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/balances/balance_ib.py` & `pfund-0.0.1.dev8/pfund/balances/balance_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/broker_backtest.py` & `pfund-0.0.1.dev8/pfund/brokers/broker_backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/broker_base.py` & `pfund-0.0.1.dev8/pfund/brokers/broker_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/broker_crypto.py` & `pfund-0.0.1.dev8/pfund/brokers/broker_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/broker_live.py` & `pfund-0.0.1.dev8/pfund/brokers/broker_live.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/ib/broker_ib.py` & `pfund-0.0.1.dev8/pfund/brokers/ib/broker_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/ib/ib_api.py` & `pfund-0.0.1.dev8/pfund/brokers/ib/ib_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/ib/ib_client.py` & `pfund-0.0.1.dev8/pfund/brokers/ib/ib_client.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/brokers/ib/ib_wrapper.py` & `pfund-0.0.1.dev8/pfund/brokers/ib/ib_wrapper.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/cli/commands/config.py` & `pfund-0.0.1.dev8/pfund/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/cli/commands/docker_compose.py` & `pfund-0.0.1.dev8/pfund/cli/commands/docker_compose.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/config.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/config.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/lot_sizes_linear.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/lot_sizes_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/lot_sizes_option.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/lot_sizes_option.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/lot_sizes_spot.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/lot_sizes_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/pdt_matchings_linear.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/pdt_matchings_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/pdt_matchings_spot.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/pdt_matchings_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/tick_sizes_linear.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/tick_sizes_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/tick_sizes_option.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/tick_sizes_option.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/bybit/tick_sizes_spot.yml` & `pfund-0.0.1.dev8/pfund/config/bybit/tick_sizes_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/configuration.py` & `pfund-0.0.1.dev8/pfund/config/configuration.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/ib/config.yml` & `pfund-0.0.1.dev8/pfund/config/ib/config.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config/logging.yml` & `pfund-0.0.1.dev8/pfund/config/logging.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/config_handler.py` & `pfund-0.0.1.dev8/pfund/config_handler.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/const/_zmq_routes.py` & `pfund-0.0.1.dev8/pfund/const/_zmq_routes.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/const/commons.py` & `pfund-0.0.1.dev8/pfund/const/commons.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/const/paths.py` & `pfund-0.0.1.dev8/pfund/const/paths.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/data_tools/data_tool_base.py` & `pfund-0.0.1.dev8/pfund/data_tools/data_tool_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/data_tools/data_tool_pandas.py` & `pfund-0.0.1.dev8/pfund/data_tools/data_tool_pandas.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/datas/data_bar.py` & `pfund-0.0.1.dev8/pfund/datas/data_bar.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/datas/data_quote.py` & `pfund-0.0.1.dev8/pfund/datas/data_quote.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/datas/data_tick.py` & `pfund-0.0.1.dev8/pfund/datas/data_tick.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/datas/data_time_based.py` & `pfund-0.0.1.dev8/pfund/datas/data_time_based.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/datas/resolution.py` & `pfund-0.0.1.dev8/pfund/datas/resolution.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/datas/timeframe.py` & `pfund-0.0.1.dev8/pfund/datas/timeframe.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/engines/backtest_engine.py` & `pfund-0.0.1.dev8/pfund/engines/backtest_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/engines/base_engine.py` & `pfund-0.0.1.dev8/pfund/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/engines/test_engine.py` & `pfund-0.0.1.dev8/pfund/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/engines/trade_engine.py` & `pfund-0.0.1.dev8/pfund/engines/trade_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/engines/train_engine.py` & `pfund-0.0.1.dev8/pfund/engines/train_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/exchange.py` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/exchange.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api.py` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/bybit/ws_api.py` & `pfund-0.0.1.dev8/pfund/exchanges/bybit/ws_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/exchange_base.py` & `pfund-0.0.1.dev8/pfund/exchanges/exchange_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/rest_api_base.py` & `pfund-0.0.1.dev8/pfund/exchanges/rest_api_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/exchanges/ws_api_base.py` & `pfund-0.0.1.dev8/pfund/exchanges/ws_api_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/account_summary_tags.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/account_summary_tags.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/client.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/client.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/comm.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/comm.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/commission_report.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/commission_report.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/common.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/common.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/connection.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/connection.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/contract.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/contract.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/decoder.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/decoder.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/enum_implem.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/enum_implem.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/errors.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/errors.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/execution.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/execution.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/ibapi.pyproj` & `pfund-0.0.1.dev8/pfund/externals/ibapi/ibapi.pyproj`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/message.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/message.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/order.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/order.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/order_condition.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/order_condition.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/order_state.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/order_state.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/orderdecoder.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/orderdecoder.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/reader.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/reader.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/scanner.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/scanner.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/server_versions.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/server_versions.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/softdollartier.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/softdollartier.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/tag_value.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/tag_value.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/ticktype.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/ticktype.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/utils.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/utils.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/externals/ibapi/wrapper.py` & `pfund-0.0.1.dev8/pfund/externals/ibapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/indicators/indicator_base.py` & `pfund-0.0.1.dev8/pfund/indicators/indicator_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/indicators/ta_indicator.py` & `pfund-0.0.1.dev8/pfund/indicators/ta_indicator.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/indicators/talib_indicator.py` & `pfund-0.0.1.dev8/pfund/indicators/talib_indicator.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/managers/base_manager.py` & `pfund-0.0.1.dev8/pfund/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/managers/connection_manager.py` & `pfund-0.0.1.dev8/pfund/managers/connection_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/managers/data_manager.py` & `pfund-0.0.1.dev8/pfund/managers/data_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/managers/order_manager.py` & `pfund-0.0.1.dev8/pfund/managers/order_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/managers/portfolio_manager.py` & `pfund-0.0.1.dev8/pfund/managers/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/managers/strategy_manager.py` & `pfund-0.0.1.dev8/pfund/managers/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/mixins/backtest.py` & `pfund-0.0.1.dev8/pfund/mixins/backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/models/model_backtest.py` & `pfund-0.0.1.dev8/pfund/models/model_backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/models/model_base.py` & `pfund-0.0.1.dev8/pfund/models/model_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/models/model_meta.py` & `pfund-0.0.1.dev8/pfund/models/model_meta.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/models/pytorch_model.py` & `pfund-0.0.1.dev8/pfund/models/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/models/sklearn_model.py` & `pfund-0.0.1.dev8/pfund/models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/orders/order_base.py` & `pfund-0.0.1.dev8/pfund/orders/order_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/orders/order_crypto.py` & `pfund-0.0.1.dev8/pfund/orders/order_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/orders/order_statuses.py` & `pfund-0.0.1.dev8/pfund/orders/order_statuses.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/plogging/__init__.py` & `pfund-0.0.1.dev8/pfund/plogging/__init__.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/plogging/config.py` & `pfund-0.0.1.dev8/pfund/plogging/config.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/plogging/formatter.py` & `pfund-0.0.1.dev8/pfund/plogging/formatter.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/plogging/handlers.py` & `pfund-0.0.1.dev8/pfund/plogging/handlers.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/positions/position_base.py` & `pfund-0.0.1.dev8/pfund/positions/position_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/positions/position_crypto.py` & `pfund-0.0.1.dev8/pfund/positions/position_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/positions/position_ib.py` & `pfund-0.0.1.dev8/pfund/positions/position_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/products/product_base.py` & `pfund-0.0.1.dev8/pfund/products/product_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/products/product_crypto.py` & `pfund-0.0.1.dev8/pfund/products/product_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/products/product_ib.py` & `pfund-0.0.1.dev8/pfund/products/product_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/strategies/portfolio_strategy.py` & `pfund-0.0.1.dev8/pfund/strategies/portfolio_strategy.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/strategies/strategy_backtest.py` & `pfund-0.0.1.dev8/pfund/strategies/strategy_backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/strategies/strategy_base.py` & `pfund-0.0.1.dev8/pfund/strategies/strategy_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/strategies/strategy_meta.py` & `pfund-0.0.1.dev8/pfund/strategies/strategy_meta.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/types/common_literals.py` & `pfund-0.0.1.dev8/pfund/types/common_literals.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/utils/aliases.py` & `pfund-0.0.1.dev8/pfund/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/utils/envs.py` & `pfund-0.0.1.dev8/pfund/utils/envs.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/utils/utils.py` & `pfund-0.0.1.dev8/pfund/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pfund/zeromq.py` & `pfund-0.0.1.dev8/pfund/zeromq.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev7/pyproject.toml` & `pfund-0.0.1.dev8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 [tool.poetry]
 name = "pfund"
-version = "0.0.1.dev7"
+version = "0.0.1.dev8"
 description = "A Complete Algo-Trading Framework for Machine Learning, enabling trading across TradFi, CeFi and DeFi. Supports Vectorized and Event-Driven Backtesting, Paper and Live Trading"
 license = "Apache-2.0"
 authors = ["Stephen Yau <softwareentrepreneer+pfund@gmail.com>"]
 readme = "README.md"
 homepage = "https://pfund.ai"
 repository = "https://github.com/PFund-Software-Ltd/pfund"
 documentation = "https://pfund-docs.pfund.ai"
 keywords = ["trading", "algo-trading", "stocks", "cryptos", "cryptocurrencies", "TradFi", "CeFi", "DeFi", "portfolio management", "investment", "backtesting", "machine learning"]
 
 [tool.poetry.dependencies]
 python = ">=3.10 <3.13"
-pfeed = "^0.0.1.dev7"
+python-dotenv = "^1.0.1"
 pyyaml = "^6.0.1"
 rich = "^13.7.0"
+click = "^8.1.7"
 schedule = "^1.2.1"
+platformdirs = "^4.2.0"
+requests = "^2.31.0"
 websocket-client = "^1.7.0"
 python-telegram-bot = "^20.7"
-click = "^8.1.7"
-platformdirs = "^4.2.0"
 gitpython = "^3.1.43"
+pfeed = { version = "^0.0.1.dev8", optional = true, extras=["df", "boost"] }
+psutil = { version = "^5.9.8", optional = true }
+orjson = { version = "^3.9.14", optional = true }
+pyzmq = { version = "^25.1.2", optional = true }
+ta = { version = "^0.11.0", optional = true }
+scikit-learn = { version = "^1.4.0", optional = true }
+torch = { version = "^2.1.2", optional = true }
+mlflow = { version = "^2.11.3", optional = true }
+
+[tool.poetry.extras]
+data = ["pfeed", "psutil", "orjson", "pyzmq"]
+ml = ["ta", "scikit-learn", "torch", "mlflow"]
 
 [tool.poetry.scripts]
 pfund = "pfund.main:run_cli"
 
-[tool.poetry.group.pyodide-incompatible.dependencies]
-psutil = "^5.9.8"
-orjson = "^3.9.14"
-ta = "^0.11.0"
-pyzmq = "^25.1.2"
-
-[tool.poetry.group.ml]
-optional = true
-
-[tool.poetry.group.ml.dependencies]
-torch = "^2.1.2"
-scikit-learn = "^1.4.0"
-mlflow = "^2.11.3"
-
-[tool.poetry.group.dev]
-optional = true
-
 [tool.poetry.group.dev.dependencies]
 pfeed = {path = "../pfeed", develop = true}
 pybit = "^5.6.2"
 ta-lib = "^0.4.28"
 pytest = "^8.0.0"
 pre-commit = "^3.6.1"
 bandit = "^1.7.7"
@@ -54,17 +50,14 @@
 faker = "^24.4.0"
 tox = "^4.14.2"
 mypy = "^1.9.0"
 ruff = "^0.3.5"
 pytest-mock = "^3.14.0"
 pytest-cov = "^5.0.0"
 
-[tool.poetry.group.doc]
-optional = true
-
 [tool.poetry.group.doc.dependencies]
 jupyter-book = "^1.0.0"
 notebook = "^7.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pfund-0.0.1.dev7/PKG-INFO` & `pfund-0.0.1.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 Metadata-Version: 2.1
 Name: pfund
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: A Complete Algo-Trading Framework for Machine Learning, enabling trading across TradFi, CeFi and DeFi. Supports Vectorized and Event-Driven Backtesting, Paper and Live Trading
 Home-page: https://pfund.ai
 License: Apache-2.0
 Keywords: trading,algo-trading,stocks,cryptos,cryptocurrencies,TradFi,CeFi,DeFi,portfolio management,investment,backtesting,machine learning
 Author: Stephen Yau
 Author-email: softwareentrepreneer+pfund@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: data
+Provides-Extra: ml
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: gitpython (>=3.1.43,<4.0.0)
-Requires-Dist: pfeed (>=0.0.1.dev7,<0.0.2)
+Requires-Dist: mlflow (>=2.11.3,<3.0.0) ; extra == "ml"
+Requires-Dist: orjson (>=3.9.14,<4.0.0) ; extra == "data"
+Requires-Dist: pfeed[boost,df] (>=0.0.1.dev8,<0.0.2) ; extra == "data"
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0) ; extra == "data"
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-telegram-bot (>=20.7,<21.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: pyzmq (>=25.1.2,<26.0.0) ; extra == "data"
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.0,<2.0.0) ; extra == "ml"
+Requires-Dist: ta (>=0.11.0,<0.12.0) ; extra == "ml"
+Requires-Dist: torch (>=2.1.2,<3.0.0) ; extra == "ml"
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Project-URL: Documentation, https://pfund-docs.pfund.ai
 Project-URL: Repository, https://github.com/PFund-Software-Ltd/pfund
 Description-Content-Type: text/markdown
 
 # PFund: Algo-Trading Framework for Machine Learning, TradFi, CeFi and DeFi ready.
```

