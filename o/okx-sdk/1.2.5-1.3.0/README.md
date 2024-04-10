# Comparing `tmp/okx-sdk-1.2.5.tar.gz` & `tmp/okx-sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okx-sdk-1.2.5.tar", last modified: Mon Apr  1 08:00:34 2024, max compression
+gzip compressed data, was "okx-sdk-1.3.0.tar", last modified: Wed Apr 10 16:09:56 2024, max compression
```

## Comparing `okx-sdk-1.2.5.tar` & `okx-sdk-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 08:00:34.526127 okx-sdk-1.2.5/
--rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.2.5/LICENSE
--rw-rw-rw-   0        0        0    32037 2024-04-01 08:00:34.524611 okx-sdk-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    30608 2024-03-10 12:44:14.000000 okx-sdk-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 08:00:34.314616 okx-sdk-1.2.5/okx/
--rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.2.5/okx/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.2.5/okx/clients.py
--rw-rw-rw-   0        0        0    22139 2024-03-09 15:24:16.000000 okx-sdk-1.2.5/okx/constants.py
--rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.2.5/okx/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:00:34.455297 okx-sdk-1.2.5/okx/restapi/
--rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.2.5/okx/restapi/Account.py
--rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.2.5/okx/restapi/AlgoTrading.py
--rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.2.5/okx/restapi/BaseClient.py
--rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.2.5/okx/restapi/BlockTrading.py
--rw-rw-rw-   0        0        0     6562 2024-03-09 15:24:05.000000 okx-sdk-1.2.5/okx/restapi/Broker.py
--rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.2.5/okx/restapi/CopyTrading.py
--rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.2.5/okx/restapi/Finance.py
--rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.2.5/okx/restapi/Funding.py
--rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.2.5/okx/restapi/GridTrading.py
--rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.2.5/okx/restapi/PublicData.py
--rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.2.5/okx/restapi/RecurringBuy.py
--rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.2.5/okx/restapi/Rubik.py
--rw-rw-rw-   0        0        0      390 2024-03-08 16:37:22.000000 okx-sdk-1.2.5/okx/restapi/SignalTrading.py
--rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.2.5/okx/restapi/SpreadTrading.py
--rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.2.5/okx/restapi/SubAccount.py
--rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.2.5/okx/restapi/Trading.py
--rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.2.5/okx/restapi/__init__.py
--rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.2.5/okx/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:00:34.496761 okx-sdk-1.2.5/okx/wsapi/
--rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.2.5/okx/wsapi/Factory.py
--rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.2.5/okx/wsapi/PrivateAsync.py
--rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.2.5/okx/wsapi/PublicAsync.py
--rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.2.5/okx/wsapi/__init__.py
--rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.2.5/okx/wsapi/wsutils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:00:34.523612 okx-sdk-1.2.5/okx_sdk.egg-info/
--rw-rw-rw-   0        0        0    32037 2024-04-01 08:00:34.000000 okx-sdk-1.2.5/okx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-04-01 08:00:34.000000 okx-sdk-1.2.5/okx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 08:00:34.000000 okx-sdk-1.2.5/okx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-01 08:00:34.000000 okx-sdk-1.2.5/okx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-01 08:00:34.000000 okx-sdk-1.2.5/okx_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 08:00:34.526127 okx-sdk-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1198 2024-04-01 07:59:24.000000 okx-sdk-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:00:34.522615 okx-sdk-1.2.5/tests/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.2.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/
+-rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0    33352 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    31907 2024-04-10 16:08:46.000000 okx-sdk-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.321192 okx-sdk-1.3.0/okx/
+-rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.3.0/okx/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.3.0/okx/clients.py
+-rw-rw-rw-   0        0        0    22003 2024-04-10 16:05:30.000000 okx-sdk-1.3.0/okx/constants.py
+-rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.3.0/okx/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.461369 okx-sdk-1.3.0/okx/restapi/
+-rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.3.0/okx/restapi/Account.py
+-rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.3.0/okx/restapi/AlgoTrading.py
+-rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.3.0/okx/restapi/BaseClient.py
+-rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.3.0/okx/restapi/BlockTrading.py
+-rw-rw-rw-   0        0        0     6562 2024-03-09 15:24:05.000000 okx-sdk-1.3.0/okx/restapi/Broker.py
+-rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.3.0/okx/restapi/CopyTrading.py
+-rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.3.0/okx/restapi/Finance.py
+-rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.3.0/okx/restapi/Funding.py
+-rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.3.0/okx/restapi/GridTrading.py
+-rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.3.0/okx/restapi/PublicData.py
+-rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.3.0/okx/restapi/RecurringBuy.py
+-rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.3.0/okx/restapi/Rubik.py
+-rw-rw-rw-   0        0        0     5099 2024-04-10 16:05:04.000000 okx-sdk-1.3.0/okx/restapi/SignalTrading.py
+-rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.3.0/okx/restapi/SpreadTrading.py
+-rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.3.0/okx/restapi/SubAccount.py
+-rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.3.0/okx/restapi/Trading.py
+-rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.3.0/okx/restapi/__init__.py
+-rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.3.0/okx/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.502867 okx-sdk-1.3.0/okx/wsapi/
+-rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.3.0/okx/wsapi/Factory.py
+-rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.3.0/okx/wsapi/PrivateAsync.py
+-rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.3.0/okx/wsapi/PublicAsync.py
+-rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.3.0/okx/wsapi/__init__.py
+-rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.3.0/okx/wsapi/wsutils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/okx_sdk.egg-info/
+-rw-rw-rw-   0        0        0    33352 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2024-04-10 16:09:12.000000 okx-sdk-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.3.0/tests/__init__.py
```

### Comparing `okx-sdk-1.2.5/LICENSE` & `okx-sdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/PKG-INFO` & `okx-sdk-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.2.5
+Version: 1.3.0
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -532,15 +532,31 @@
 
 #### Order Book Trading → Signal Bot Trading Client
 
 ```python
 from okx import OkxRestClient
 
 api = OkxRestClient('---API-KEY---', '---API-SECRET---', '---PASS-PHRASE---')
-# TODO
+api.signaltrade.create_signal(signalChanName, signalChanDesc='')
+api.signaltrade.get_signals(signalSourceType, signalChanId='', after='', before='', limit='')
+api.signaltrade.create(signalChanId, lever, investAmt, subOrdType, includeAll='', instIds='', ratio='', entrySettingParam={},exitSettingParam={})
+api.signaltrade.cancel(algoId)
+api.signaltrade.adjust_margin_balance(algoId, type, amt, allowReinvest=False)
+api.signaltrade.amend_tpsl(algoId, exitSettingParam={})
+api.signaltrade.set_instruments(algoId, instIds=[], includeAll=False)
+api.signaltrade.get_order(algoOrdType, algoId)
+api.signaltrade.get_active(algoOrdType, algoId, after='', before='', limit='')
+api.signaltrade.get_history(algoOrdType, algoId, after='', before='', limit='')
+api.signaltrade.get_positions(algoOrdType, algoId)
+api.signaltrade.get_position_history(algoId='', instId='', after='', before='', limit='')
+api.signaltrade.close_position(algoId, instId)
+api.signaltrade.place_sub_order(algoId, instId, side, ordType, sz, px='', reduceOnly=False)
+api.signaltrade.cancel_sub_order(algoId, instId, signalOrdId)
+api.signaltrade.get_sub_orders(algoId, algoOrdType, type='', clOrdId='', state='', signalOrdId='', after='', before='', begin='', end='', limit='')
+api.signaltrade.get_bot_events(algoId, after='', before='', limit='')
 ```
 
 #### Block Trading Client
 
 ```python
 from okx import OkxRestClient
```

### Comparing `okx-sdk-1.2.5/README.md` & `okx-sdk-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -512,15 +512,31 @@
 
 #### Order Book Trading → Signal Bot Trading Client
 
 ```python
 from okx import OkxRestClient
 
 api = OkxRestClient('---API-KEY---', '---API-SECRET---', '---PASS-PHRASE---')
-# TODO
+api.signaltrade.create_signal(signalChanName, signalChanDesc='')
+api.signaltrade.get_signals(signalSourceType, signalChanId='', after='', before='', limit='')
+api.signaltrade.create(signalChanId, lever, investAmt, subOrdType, includeAll='', instIds='', ratio='', entrySettingParam={},exitSettingParam={})
+api.signaltrade.cancel(algoId)
+api.signaltrade.adjust_margin_balance(algoId, type, amt, allowReinvest=False)
+api.signaltrade.amend_tpsl(algoId, exitSettingParam={})
+api.signaltrade.set_instruments(algoId, instIds=[], includeAll=False)
+api.signaltrade.get_order(algoOrdType, algoId)
+api.signaltrade.get_active(algoOrdType, algoId, after='', before='', limit='')
+api.signaltrade.get_history(algoOrdType, algoId, after='', before='', limit='')
+api.signaltrade.get_positions(algoOrdType, algoId)
+api.signaltrade.get_position_history(algoId='', instId='', after='', before='', limit='')
+api.signaltrade.close_position(algoId, instId)
+api.signaltrade.place_sub_order(algoId, instId, side, ordType, sz, px='', reduceOnly=False)
+api.signaltrade.cancel_sub_order(algoId, instId, signalOrdId)
+api.signaltrade.get_sub_orders(algoId, algoOrdType, type='', clOrdId='', state='', signalOrdId='', after='', before='', begin='', end='', limit='')
+api.signaltrade.get_bot_events(algoId, after='', before='', limit='')
 ```
 
 #### Block Trading Client
 
 ```python
 from okx import OkxRestClient
```

### Comparing `okx-sdk-1.2.5/okx/__init__.py` & `okx-sdk-1.3.0/okx/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/clients.py` & `okx-sdk-1.3.0/okx/clients.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/constants.py` & `okx-sdk-1.3.0/okx/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,31 +119,31 @@
 GRID_COMPUTE_MARGIN_BALANCE = '/api/v5/tradingBot/grid/compute-margin-balance'
 GRID_MARGIN_BALANCE = '/api/v5/tradingBot/grid/margin-balance'
 GRID_AI_PARAM = '/api/v5/tradingBot/grid/ai-param'
 GRID_MIN_INVESTMENT = '/api/v5/tradingBot/grid/min-investment'
 GRID_RSI_BACK_TESTING = '/api/v5/tradingBot/public/rsi-back-testing'
 
 # Order Book Trading >> Signal Trading Endpoints
-SIGNAL_CREATE_SIGNAL = '/api/v5/tradingBot/signal/create-signal'  # TODO
-SIGNAL_SIGNALS = '/api/v5/tradingBot/signal/signals'  # TODO
-SIGNAL_ORDER_ALGO = '/api/v5/tradingBot/signal/order-algo'  # TODO
-SIGNAL_STOP_ORDER_ALGO = '/api/v5/tradingBot/signal/stop-order-algo'  # TODO
-SIGNAL_MARGIN_BALANCE = '/api/v5/tradingBot/signal/margin-balance'  # TODO
-SIGNAL_AMEND_TPSL = '/api/v5/tradingBot/signal/amendTPSL'  # TODO
-SIGNAL_SET_INSTRUMENTS = '/api/v5/tradingBot/signal/set-instruments'  # TODO
-SIGNAL_ORDERS_ALGO_DETAILS_01 = '/api/v5/tradingBot/signal/orders-algo-details'  # TODO
-SIGNAL_ORDERS_ALGO_DETAILS_02 = '/api/v5/tradingBot/signal/orders-algo-details'  # TODO
-SIGNAL_ORDERS_ALGO_HISTORY = '/api/v5/tradingBot/signal/orders-algo-history'  # TODO
-SIGNAL_POSITIONS = '/api/v5/tradingBot/signal/positions'  # TODO
-SIGNAL_POSITIONS_HISTORY = '/api/v5/tradingBot/signal/positions-history'  # TODO
-SIGNAL_CLOSE_POSITION = '/api/v5/tradingBot/signal/close-position'  # TODO
-SIGNAL_SUB_ORDER = '/api/v5/tradingBot/signal/sub-order'  # TODO
-SIGNAL_CANCEL_SUB_ORDER = '/api/v5/tradingBot/signal/cancel-sub-order'  # TODO
-SIGNAL_SUB_ORDERS = '/api/v5/tradingBot/signal/sub-orders'  # TODO
-SIGNAL_EVENT_HISTORY = '/api/v5/tradingBot/signal/event-history'  # TODO
+SIGNAL_CREATE_SIGNAL = '/api/v5/tradingBot/signal/create-signal'
+SIGNAL_SIGNALS = '/api/v5/tradingBot/signal/signals'
+SIGNAL_ORDER_ALGO = '/api/v5/tradingBot/signal/order-algo'
+SIGNAL_STOP_ORDER_ALGO = '/api/v5/tradingBot/signal/stop-order-algo'
+SIGNAL_MARGIN_BALANCE = '/api/v5/tradingBot/signal/margin-balance'
+SIGNAL_AMEND_TPSL = '/api/v5/tradingBot/signal/amendTPSL'
+SIGNAL_SET_INSTRUMENTS = '/api/v5/tradingBot/signal/set-instruments'
+SIGNAL_ORDERS_ALGO_DETAILS_01 = '/api/v5/tradingBot/signal/orders-algo-details'
+SIGNAL_ORDERS_ALGO_DETAILS_02 = '/api/v5/tradingBot/signal/orders-algo-details'
+SIGNAL_ORDERS_ALGO_HISTORY = '/api/v5/tradingBot/signal/orders-algo-history'
+SIGNAL_POSITIONS = '/api/v5/tradingBot/signal/positions'
+SIGNAL_POSITIONS_HISTORY = '/api/v5/tradingBot/signal/positions-history'
+SIGNAL_CLOSE_POSITION = '/api/v5/tradingBot/signal/close-position'
+SIGNAL_SUB_ORDER = '/api/v5/tradingBot/signal/sub-order'
+SIGNAL_CANCEL_SUB_ORDER = '/api/v5/tradingBot/signal/cancel-sub-order'
+SIGNAL_SUB_ORDERS = '/api/v5/tradingBot/signal/sub-orders'
+SIGNAL_EVENT_HISTORY = '/api/v5/tradingBot/signal/event-history'
 
 # Order Book Trading >> Recurring Buy Endpoints
 RECURRING_ORDER_ALGO = '/api/v5/tradingBot/recurring/order-algo'
 RECURRING_AMEND_ORDER_ALGO = '/api/v5/tradingBot/recurring/amend-order-algo'
 RECURRING_STOP_ORDER_ALGO = '/api/v5/tradingBot/recurring/stop-order-algo'
 RECURRING_ORDERS_ALGO_PENDING = '/api/v5/tradingBot/recurring/orders-algo-pending'
 RECURRING_ORDERS_ALGO_HISTORY = '/api/v5/tradingBot/recurring/orders-algo-history'
```

### Comparing `okx-sdk-1.2.5/okx/exceptions.py` & `okx-sdk-1.3.0/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/Account.py` & `okx-sdk-1.3.0/okx/restapi/Account.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/AlgoTrading.py` & `okx-sdk-1.3.0/okx/restapi/AlgoTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/BaseClient.py` & `okx-sdk-1.3.0/okx/restapi/BaseClient.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/BlockTrading.py` & `okx-sdk-1.3.0/okx/restapi/BlockTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/Broker.py` & `okx-sdk-1.3.0/okx/restapi/Broker.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/CopyTrading.py` & `okx-sdk-1.3.0/okx/restapi/CopyTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/Finance.py` & `okx-sdk-1.3.0/okx/restapi/Finance.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/Funding.py` & `okx-sdk-1.3.0/okx/restapi/Funding.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/GridTrading.py` & `okx-sdk-1.3.0/okx/restapi/GridTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/PublicData.py` & `okx-sdk-1.3.0/okx/restapi/PublicData.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/RecurringBuy.py` & `okx-sdk-1.3.0/okx/restapi/RecurringBuy.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/Rubik.py` & `okx-sdk-1.3.0/okx/restapi/Rubik.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/SpreadTrading.py` & `okx-sdk-1.3.0/okx/restapi/SpreadTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/SubAccount.py` & `okx-sdk-1.3.0/okx/restapi/SubAccount.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/Trading.py` & `okx-sdk-1.3.0/okx/restapi/Trading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/restapi/__init__.py` & `okx-sdk-1.3.0/okx/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/utils.py` & `okx-sdk-1.3.0/okx/utils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/wsapi/Factory.py` & `okx-sdk-1.3.0/okx/wsapi/Factory.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/wsapi/PrivateAsync.py` & `okx-sdk-1.3.0/okx/wsapi/PrivateAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/wsapi/PublicAsync.py` & `okx-sdk-1.3.0/okx/wsapi/PublicAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx/wsapi/wsutils.py` & `okx-sdk-1.3.0/okx/wsapi/wsutils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/okx_sdk.egg-info/PKG-INFO` & `okx-sdk-1.3.0/okx_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.2.5
+Version: 1.3.0
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -532,15 +532,31 @@
 
 #### Order Book Trading → Signal Bot Trading Client
 
 ```python
 from okx import OkxRestClient
 
 api = OkxRestClient('---API-KEY---', '---API-SECRET---', '---PASS-PHRASE---')
-# TODO
+api.signaltrade.create_signal(signalChanName, signalChanDesc='')
+api.signaltrade.get_signals(signalSourceType, signalChanId='', after='', before='', limit='')
+api.signaltrade.create(signalChanId, lever, investAmt, subOrdType, includeAll='', instIds='', ratio='', entrySettingParam={},exitSettingParam={})
+api.signaltrade.cancel(algoId)
+api.signaltrade.adjust_margin_balance(algoId, type, amt, allowReinvest=False)
+api.signaltrade.amend_tpsl(algoId, exitSettingParam={})
+api.signaltrade.set_instruments(algoId, instIds=[], includeAll=False)
+api.signaltrade.get_order(algoOrdType, algoId)
+api.signaltrade.get_active(algoOrdType, algoId, after='', before='', limit='')
+api.signaltrade.get_history(algoOrdType, algoId, after='', before='', limit='')
+api.signaltrade.get_positions(algoOrdType, algoId)
+api.signaltrade.get_position_history(algoId='', instId='', after='', before='', limit='')
+api.signaltrade.close_position(algoId, instId)
+api.signaltrade.place_sub_order(algoId, instId, side, ordType, sz, px='', reduceOnly=False)
+api.signaltrade.cancel_sub_order(algoId, instId, signalOrdId)
+api.signaltrade.get_sub_orders(algoId, algoOrdType, type='', clOrdId='', state='', signalOrdId='', after='', before='', begin='', end='', limit='')
+api.signaltrade.get_bot_events(algoId, after='', before='', limit='')
 ```
 
 #### Block Trading Client
 
 ```python
 from okx import OkxRestClient
```

### Comparing `okx-sdk-1.2.5/okx_sdk.egg-info/SOURCES.txt` & `okx-sdk-1.3.0/okx_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.2.5/setup.py` & `okx-sdk-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
     
-VERSION = '1.2.5'
+VERSION = '1.3.0'
 DESCRIPTION = 'Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python'
 
 setuptools.setup(
     name="okx-sdk",
     version=VERSION,
     author="Burak Öner",
     author_email="info@burakoner.com",
```

