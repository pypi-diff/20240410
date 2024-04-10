# Comparing `tmp/optrabot-0.8.2a0.tar.gz` & `tmp/optrabot-0.8.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrabot-0.8.2a0.tar", max compression
+gzip compressed data, was "optrabot-0.8.2a1.tar", max compression
```

## Comparing `optrabot-0.8.2a0.tar` & `optrabot-0.8.2a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.8.2a0/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.8.2a0/optrabot/__init__.py
--rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.8.2a0/optrabot/alembic/README
--rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.8.2a0/optrabot/alembic/env.py
--rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.8.2a0/optrabot/alembic/script.py.mako
--rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.8.2a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
--rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.8.2a0/optrabot/alembic.ini
--rw-r--r--   0        0        0    11822 2024-03-29 23:18:40.612397 optrabot-0.8.2a0/optrabot/config.py
--rw-r--r--   0        0        0     2804 2024-02-22 12:22:44.564924 optrabot-0.8.2a0/optrabot/crud.py
--rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.8.2a0/optrabot/database.py
--rw-r--r--   0        0        0     2323 2024-02-22 12:22:44.565504 optrabot-0.8.2a0/optrabot/main.py
--rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.8.2a0/optrabot/marketdatatype.py
--rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.8.2a0/optrabot/models.py
--rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.8.2a0/optrabot/optionhelper.py
--rw-r--r--   0        0        0    10416 2024-04-09 12:37:04.558376 optrabot-0.8.2a0/optrabot/optrabot.py
--rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.8.2a0/optrabot/schemas.py
--rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.8.2a0/optrabot/stoplossadjuster.py
--rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.8.2a0/optrabot/tradehelper.py
--rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.8.2a0/optrabot/tradetemplate/__init__.py
--rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.8.2a0/optrabot/tradetemplate/ironfly.py
--rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.8.2a0/optrabot/tradetemplate/putspread.py
--rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.8.2a0/optrabot/tradetemplate/template.py
--rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.8.2a0/optrabot/tradetemplate/templatefactory.py
--rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.8.2a0/optrabot/tradetemplate/templatetrigger.py
--rw-r--r--   0        0        0    35316 2024-04-08 18:36:39.426454 optrabot-0.8.2a0/optrabot/tradinghubclient.py
--rw-r--r--   0        0        0      821 2024-04-09 12:25:34.408407 optrabot-0.8.2a0/pyproject.toml
--rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.8.2a0/PKG-INFO
+-rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.8.2a1/README.md
+-rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.8.2a1/optrabot/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.8.2a1/optrabot/alembic/README
+-rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.8.2a1/optrabot/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.8.2a1/optrabot/alembic/script.py.mako
+-rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.8.2a1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
+-rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.8.2a1/optrabot/alembic.ini
+-rw-r--r--   0        0        0    11822 2024-03-29 23:18:40.612397 optrabot-0.8.2a1/optrabot/config.py
+-rw-r--r--   0        0        0     2804 2024-02-22 12:22:44.564924 optrabot-0.8.2a1/optrabot/crud.py
+-rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.8.2a1/optrabot/database.py
+-rw-r--r--   0        0        0     2323 2024-02-22 12:22:44.565504 optrabot-0.8.2a1/optrabot/main.py
+-rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.8.2a1/optrabot/marketdatatype.py
+-rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.8.2a1/optrabot/models.py
+-rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.8.2a1/optrabot/optionhelper.py
+-rw-r--r--   0        0        0    10487 2024-04-09 12:55:21.942393 optrabot-0.8.2a1/optrabot/optrabot.py
+-rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.8.2a1/optrabot/schemas.py
+-rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.8.2a1/optrabot/stoplossadjuster.py
+-rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.8.2a1/optrabot/tradehelper.py
+-rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.8.2a1/optrabot/tradetemplate/__init__.py
+-rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.8.2a1/optrabot/tradetemplate/ironfly.py
+-rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.8.2a1/optrabot/tradetemplate/putspread.py
+-rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.8.2a1/optrabot/tradetemplate/template.py
+-rw-r--r--   0        0        0     2273 2024-03-19 15:36:19.405141 optrabot-0.8.2a1/optrabot/tradetemplate/templatefactory.py
+-rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.8.2a1/optrabot/tradetemplate/templatetrigger.py
+-rw-r--r--   0        0        0    35316 2024-04-08 18:36:39.426454 optrabot-0.8.2a1/optrabot/tradinghubclient.py
+-rw-r--r--   0        0        0      821 2024-04-09 12:56:48.661345 optrabot-0.8.2a1/pyproject.toml
+-rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.8.2a1/PKG-INFO
```

### Comparing `optrabot-0.8.2a0/README.md` & `optrabot-0.8.2a1/README.md`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/alembic/env.py` & `optrabot-0.8.2a1/optrabot/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/alembic/script.py.mako` & `optrabot-0.8.2a1/optrabot/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py` & `optrabot-0.8.2a1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/alembic.ini` & `optrabot-0.8.2a1/optrabot/alembic.ini`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/config.py` & `optrabot-0.8.2a1/optrabot/config.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/crud.py` & `optrabot-0.8.2a1/optrabot/crud.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/database.py` & `optrabot-0.8.2a1/optrabot/database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/main.py` & `optrabot-0.8.2a1/optrabot/main.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/marketdatatype.py` & `optrabot-0.8.2a1/optrabot/marketdatatype.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/models.py` & `optrabot-0.8.2a1/optrabot/models.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/optionhelper.py` & `optrabot-0.8.2a1/optrabot/optionhelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/optrabot.py` & `optrabot-0.8.2a1/optrabot/optrabot.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 			ibMarketDataType = MarketDataType(ticker.marketDataType)
 			if ibMarketDataType.Value != marketDataType.Value:
 				logger.error("IB returned '{}' data for SPX! Trading is deactivated!", ibMarketDataType.toString())
 				return
 			else:
 				logger.info("Received '{}' market data for SPX as expected.", ibMarketDataType.toString())
 
-			logger.debug("Ticker data: {}", ticker)	
+			logger.debug("Ticker data: Last={} Close={} Market Price={}", ticker.last, ticker.close, ticker.marketPrice())	
 			spxPrice = ticker.close
 			if util.isNan(spxPrice):
 				logger.debug("IB returned no SPX price but just NaN value for last price. Trading is deactivated!")
 			else:
 				break # no more loop required
 
 		if util.isNan(spxPrice):
```

### Comparing `optrabot-0.8.2a0/optrabot/schemas.py` & `optrabot-0.8.2a1/optrabot/schemas.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/stoplossadjuster.py` & `optrabot-0.8.2a1/optrabot/stoplossadjuster.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/tradehelper.py` & `optrabot-0.8.2a1/optrabot/tradehelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/tradetemplate/template.py` & `optrabot-0.8.2a1/optrabot/tradetemplate/template.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/tradetemplate/templatefactory.py` & `optrabot-0.8.2a1/optrabot/tradetemplate/templatefactory.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/tradetemplate/templatetrigger.py` & `optrabot-0.8.2a1/optrabot/tradetemplate/templatetrigger.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/optrabot/tradinghubclient.py` & `optrabot-0.8.2a1/optrabot/tradinghubclient.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.8.2a0/pyproject.toml` & `optrabot-0.8.2a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optrabot"
-version = "0.8.2a0"
+version = "0.8.2a1"
 description = "QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account."
 authors = ["QuantX GmbH"]
 readme = "README.md"
 license = "MIT"
 homepage = "http://www.optrabot.com"
 keywords = ["tws"]
 packages =  [{include = "optrabot"}]
```

### Comparing `optrabot-0.8.2a0/PKG-INFO` & `optrabot-0.8.2a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optrabot
-Version: 0.8.2a0
+Version: 0.8.2a1
 Summary: QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account.
 Home-page: http://www.optrabot.com
 License: MIT
 Keywords: tws
 Author: QuantX GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

