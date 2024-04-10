# Comparing `tmp/xchangelib-0.0.5.tar.gz` & `tmp/xchangelib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchangelib-0.0.5.tar", last modified: Fri Apr  5 22:59:20 2024, max compression
+gzip compressed data, was "xchangelib-0.0.6.tar", last modified: Wed Apr 10 08:03:44 2024, max compression
```

## Comparing `xchangelib-0.0.5.tar` & `xchangelib-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.759057 xchangelib-0.0.5/
--rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-04-05 22:58:16.000000 xchangelib-0.0.5/LICENSE
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-05 22:59:20.758352 xchangelib-0.0.5/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-04-05 22:58:16.000000 xchangelib-0.0.5/README.md
--rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-04-05 22:58:16.000000 xchangelib-0.0.5/pyproject.toml
--rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-04-05 22:59:20.759279 xchangelib-0.0.5/setup.cfg
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.746240 xchangelib-0.0.5/src/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.751584 xchangelib-0.0.5/src/xchangelib/
--rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/__init__.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.746538 xchangelib-0.0.5/src/xchangelib/docs/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.755574 xchangelib-0.0.5/src/xchangelib/docs/source/
--rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/docs/source/conf.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.756395 xchangelib-0.0.5/src/xchangelib/examples/
--rw-r--r--   0 rohanv     (501) staff       (20)     3414 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/examples/example_bot.py
--rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/service_pb2.py
--rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/service_pb2_grpc.py
--rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/setup.py
--rw-r--r--   0 rohanv     (501) staff       (20)    14298 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/xchange_client.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.757418 xchangelib-0.0.5/src/xchangelib.egg-info/
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/SOURCES.txt
--rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/dependency_links.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/requires.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/top_level.txt
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.265513 xchangelib-0.0.6/
+-rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-04-10 08:02:54.000000 xchangelib-0.0.6/LICENSE
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-10 08:03:44.264645 xchangelib-0.0.6/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-04-10 08:02:54.000000 xchangelib-0.0.6/README.md
+-rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-04-10 08:02:54.000000 xchangelib-0.0.6/pyproject.toml
+-rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-04-10 08:03:44.265750 xchangelib-0.0.6/setup.cfg
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.248309 xchangelib-0.0.6/src/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.256552 xchangelib-0.0.6/src/xchangelib/
+-rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/__init__.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.248969 xchangelib-0.0.6/src/xchangelib/docs/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.261261 xchangelib-0.0.6/src/xchangelib/docs/source/
+-rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/docs/source/conf.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.262379 xchangelib-0.0.6/src/xchangelib/examples/
+-rw-r--r--   0 rohanv     (501) staff       (20)     3414 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/examples/example_bot.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/service_pb2.py
+-rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/service_pb2_grpc.py
+-rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/setup.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    14296 2024-04-10 08:02:54.000000 xchangelib-0.0.6/src/xchangelib/xchange_client.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-10 08:03:44.263584 xchangelib-0.0.6/src/xchangelib.egg-info/
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/SOURCES.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/dependency_links.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/requires.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-04-10 08:03:44.000000 xchangelib-0.0.6/src/xchangelib.egg-info/top_level.txt
```

### Comparing `xchangelib-0.0.5/LICENSE` & `xchangelib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.5/PKG-INFO` & `xchangelib-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xchangelib-0.0.5/pyproject.toml` & `xchangelib-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchangelib"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Rohan Voddhi", email="rohan.voddhi@gmail.com" },
 ]
 description = "A client library for interacting with xchange-v3"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ['setuptools>=69.0','protobuf==5.26.0', 'grpcio==1.62.1']
```

### Comparing `xchangelib-0.0.5/src/xchangelib/docs/source/conf.py` & `xchangelib-0.0.6/src/xchangelib/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.5/src/xchangelib/examples/example_bot.py` & `xchangelib-0.0.6/src/xchangelib/examples/example_bot.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.5/src/xchangelib/service_pb2.py` & `xchangelib-0.0.6/src/xchangelib/service_pb2.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.5/src/xchangelib/service_pb2_grpc.py` & `xchangelib-0.0.6/src/xchangelib/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.5/src/xchangelib/xchange_client.py` & `xchangelib-0.0.6/src/xchangelib/xchange_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 from dataclasses import dataclass, field
 from collections import defaultdict
 from typing import Optional
 import time
 
 
-__version__ = "0.0.0"
+__version__ = "0.0.6"
 
 logging.basicConfig(level=logging.INFO)
 _LOGGER = logging.getLogger("xchange-client")
 _LOGGER.setLevel(logging.INFO)
 
 
 @dataclass
@@ -110,19 +110,19 @@
             order_request = utc_bot_pb2.NewOrderRequest(symbol=symbol, id=str(self.order_id), market=market_order_msg,
                                                         side=side)
         else:
             limit_order_msg = utc_bot_pb2.LimitOrder(qty=qty, px=px)
             order_request = utc_bot_pb2.NewOrderRequest(symbol=symbol, id=str(self.order_id), limit=limit_order_msg,
                                                         side=side)
         request = utc_bot_pb2.ClientMessageToExchange(new_order=order_request)
-        await self.call.write(request)
-        self.open_orders[str(self.order_id)] = [order_request, qty, is_market]
+        key = str(self.order_id)
         self.order_id += 1
-        return str(self.order_id - 1)
-
+        await self.call.write(request)
+        self.open_orders[key] = [order_request, qty, is_market]
+        return key
     async def place_swap_order(self, swap: str, qty: int) -> None:
         """
         Places a swap request with the exchange.
         :param swap: Name of the swap
         :param qty: Quantity of swaps to execute
         :return:
         """
```

### Comparing `xchangelib-0.0.5/src/xchangelib.egg-info/PKG-INFO` & `xchangelib-0.0.6/src/xchangelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

