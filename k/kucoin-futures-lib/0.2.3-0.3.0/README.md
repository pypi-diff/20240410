# Comparing `tmp/kucoin_futures_lib-0.2.3.tar.gz` & `tmp/kucoin_futures_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.2.3.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.3.0.tar", max compression
```

## Comparing `kucoin_futures_lib-0.2.3.tar` & `kucoin_futures_lib-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/LICENSE
--rw-r--r--   0        0        0       52 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/README.md
--rw-r--r--   0        0        0      719 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      251 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     1977 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2554 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     1775 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    12789 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     2786 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      455 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/LICENSE
+-rw-r--r--   0        0        0       52 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/README.md
+-rw-r--r--   0        0        0      719 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      251 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     1977 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2554 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     1775 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    12789 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     3079 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      455 2024-04-09 17:06:16.244252 kucoin_futures_lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.3.0/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.2.3/LICENSE` & `kucoin_futures_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/entry.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/handlers/oco.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.3/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.3.0/kucoin_futures_lib/websocket.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,46 +17,52 @@
 
     def __init__(self, token: WsToken):
         self.token = token
 
     async def subscribe(
         self, handler: HandlerABC, timeout: Optional[float] = 60 * 60 * 12
     ) -> None:
-        """Subscribe to the WebSocket topic."""
+        """Subscribe to the WebSocket topic.
+        :param handler: Handler object
+        :param timeout: Timeout in seconds. Default is 12 hours
+        :raises asyncio.TimeoutError: If the timeout is reached
+        """
         ws_client = await KucoinFuturesWsClient.create(
             loop=None,
             client=self.token,
             callback=handler.handle,
             private=handler.private,
         )
         await ws_client.subscribe(handler.topic)
         logger.info("%s subscribed to %s", handler, handler.topic)
         try:
             if timeout:
                 await asyncio.wait_for(handler.done.wait(), timeout)
             else:
                 await handler.done.wait()
         except asyncio.TimeoutError:
-            logger.warning("Timeout reached. Unsubscribing from %s", handler.topic)
             handler.done.set()
+            raise asyncio.TimeoutError(f"Timeout reached for {handler}")
         finally:
+            logger.info("Unsubscribing from %s", handler.topic)
             await ws_client.unsubscribe(handler.topic)
 
     async def listen_for_entry(
         self,
         instrument: str,
         entry_high: float,
         entry_low: float,
         timeout: float = 60 * 60 * 12,
     ) -> None:
         """Listen for the entry price range.
         :param instrument: Instrument symbol
         :param entry_high: Entry high price
         :param entry_low: Entry low price
         :param timeout: timeout in seconds. Default is 12 hours
+        :raises asyncio.TimeoutError: If the timeout is reached
         """
         handler = EntryRangeHandler(
             instrument=instrument, entry_high=entry_high, entry_low=entry_low
         )
         await self.subscribe(handler, timeout)
 
     async def tp_sl_cancel(
```

### Comparing `kucoin_futures_lib-0.2.3/PKG-INFO` & `kucoin_futures_lib-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.2.3
+Version: 0.3.0
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

