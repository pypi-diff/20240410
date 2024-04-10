# Comparing `tmp/coinpaprika_async-3.0.3.tar.gz` & `tmp/coinpaprika_async-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinpaprika_async-3.0.3.tar", last modified: Mon Apr  8 22:52:53 2024, max compression
+gzip compressed data, was "coinpaprika_async-3.1.0.tar", max compression
```

## Comparing `coinpaprika_async-3.0.3.tar` & `coinpaprika_async-3.1.0.tar`

### file list

```diff
@@ -1,59 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.458334 coinpaprika_async-3.0.3/
--rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.3/LICENSE
--rw-rw-rw-   0        0        0     2191 2024-04-08 22:52:53.457336 coinpaprika_async-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.3/README.md
--rw-rw-rw-   0        0        0      364 2024-04-08 22:09:42.000000 coinpaprika_async-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      139 2024-04-08 22:52:53.460336 coinpaprika_async-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-04-08 22:17:29.000000 coinpaprika_async-3.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.324319 coinpaprika_async-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.357296 coinpaprika_async-3.0.3/src/coinpaprika_async/
--rw-rw-rw-   0        0        0      485 2024-04-08 22:14:45.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-08 22:06:50.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.373290 coinpaprika_async-3.0.3/src/coinpaprika_async/api/
--rw-rw-rw-   0        0        0      245 2023-06-20 18:10:10.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/__init__.py
--rw-rw-rw-   0        0        0      235 2023-06-18 16:35:59.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coinpaprika_api.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.381394 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/__init__.py
--rw-rw-rw-   0        0        0     5954 2023-06-21 22:20:04.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/api.py
--rw-rw-rw-   0        0        0     3033 2023-06-20 18:29:31.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.392600 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:33:51.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/__init__.py
--rw-rw-rw-   0        0        0      897 2024-04-08 22:40:55.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/api.py
--rw-rw-rw-   0        0        0     1322 2024-04-08 22:41:52.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.400392 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:50.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/__init__.py
--rw-rw-rw-   0        0        0      828 2023-06-20 20:00:00.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/api.py
--rw-rw-rw-   0        0        0      351 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.406419 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:39.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/__init__.py
--rw-rw-rw-   0        0        0      307 2023-06-18 14:55:02.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/api.py
--rw-rw-rw-   0        0        0      408 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.414399 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/__init__.py
--rw-rw-rw-   0        0        0     3200 2024-04-08 22:06:10.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/api.py
--rw-rw-rw-   0        0        0     1457 2023-06-20 17:52:21.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.430347 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/
--rw-rw-rw-   0        0        0       62 2023-06-18 14:49:03.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-06-20 17:03:43.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/http_async_client.py
--rw-rw-rw-   0        0        0      217 2023-06-20 17:03:37.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/http_models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.435332 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-06-20 20:01:10.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/api.py
--rw-rw-rw-   0        0        0      569 2023-06-20 18:13:19.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.442332 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:37:29.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/__init__.py
--rw-rw-rw-   0        0        0      769 2023-06-20 20:05:47.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/api.py
--rw-rw-rw-   0        0        0      241 2023-06-20 20:03:04.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/models.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.448347 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/__init__.py
--rw-rw-rw-   0        0        0     2482 2023-06-20 18:32:49.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/api.py
--rw-rw-rw-   0        0        0     1056 2023-06-20 17:15:14.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/models.py
--rw-rw-rw-   0        0        0     1478 2024-04-08 22:10:59.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/coinpaprika_async_client.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.455334 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/
--rw-rw-rw-   0        0        0     2191 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1693 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.450332 coinpaprika_async-3.0.3/src/tests/
--rw-rw-rw-   0        0        0     2289 2024-04-08 22:37:24.000000 coinpaprika_async-3.0.3/src/tests/test_client.py
+-rw-r--r--   0        0        0      537 2024-04-10 19:15:12.474999 coinpaprika_async-3.1.0/coinpaprika_async_client/__init__.py
+-rw-r--r--   0        0        0      125 2024-04-10 07:39:36.455175 coinpaprika_async-3.1.0/coinpaprika_async_client/__version__.py
+-rw-r--r--   0        0        0       62 2024-04-10 19:16:23.702687 coinpaprika_async-3.1.0/coinpaprika_async_client/client/__init__.py
+-rw-r--r--   0        0        0     1415 2024-04-10 19:16:10.754193 coinpaprika_async-3.1.0/coinpaprika_async_client/client/coinpaprika_async_client.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:52.763805 coinpaprika_async-3.1.0/coinpaprika_async_client/coins/__init__.py
+-rw-r--r--   0        0        0     6492 2024-04-10 19:17:36.999935 coinpaprika_async-3.1.0/coinpaprika_async_client/coins/api.py
+-rw-r--r--   0        0        0     3032 2024-04-10 08:05:34.426767 coinpaprika_async-3.1.0/coinpaprika_async_client/coins/models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:33:51.447490 coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/__init__.py
+-rw-r--r--   0        0        0     1166 2024-04-10 19:17:11.487434 coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/api.py
+-rw-r--r--   0        0        0     1322 2024-04-08 22:41:52.869451 coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/models.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:50.315267 coinpaprika_async-3.1.0/coinpaprika_async_client/key/__init__.py
+-rw-r--r--   0        0        0      993 2024-04-10 19:18:22.652039 coinpaprika_async-3.1.0/coinpaprika_async_client/key/api.py
+-rw-r--r--   0        0        0      351 2023-06-20 16:48:12.366887 coinpaprika_async-3.1.0/coinpaprika_async_client/key/models.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:39.258082 coinpaprika_async-3.1.0/coinpaprika_async_client/market/__init__.py
+-rw-r--r--   0        0        0      453 2024-04-10 19:18:38.537515 coinpaprika_async-3.1.0/coinpaprika_async_client/market/api.py
+-rw-r--r--   0        0        0      408 2023-06-20 16:48:12.366887 coinpaprika_async-3.1.0/coinpaprika_async_client/market/models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:28:26.393731 coinpaprika_async-3.1.0/coinpaprika_async_client/misc/__init__.py
+-rw-r--r--   0        0        0     3417 2024-04-10 19:18:49.157594 coinpaprika_async-3.1.0/coinpaprika_async_client/misc/api.py
+-rw-r--r--   0        0        0     1457 2023-06-20 17:52:21.337155 coinpaprika_async-3.1.0/coinpaprika_async_client/misc/models.py
+-rw-r--r--   0        0        0       62 2024-04-10 19:00:09.499127 coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/__init__.py
+-rw-r--r--   0        0        0     2803 2024-04-10 12:02:51.311704 coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/http_async_client.py
+-rw-r--r--   0        0        0      217 2023-06-20 17:03:37.194237 coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/http_models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:28:26.393731 coinpaprika_async-3.1.0/coinpaprika_async_client/people/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-10 19:19:06.254703 coinpaprika_async-3.1.0/coinpaprika_async_client/people/api.py
+-rw-r--r--   0        0        0      569 2023-06-20 18:13:19.881849 coinpaprika_async-3.1.0/coinpaprika_async_client/people/models.py
+-rw-r--r--   0        0        0       43 2023-06-18 16:37:29.668193 coinpaprika_async-3.1.0/coinpaprika_async_client/tags/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-10 19:19:13.806061 coinpaprika_async-3.1.0/coinpaprika_async_client/tags/api.py
+-rw-r--r--   0        0        0      241 2023-06-20 20:03:04.015456 coinpaprika_async-3.1.0/coinpaprika_async_client/tags/models.py
+-rw-r--r--   0        0        0       43 2023-06-17 19:19:52.763805 coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/__init__.py
+-rw-r--r--   0        0        0     2747 2024-04-10 19:19:22.052321 coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/api.py
+-rw-r--r--   0        0        0     1056 2023-06-20 17:15:14.018308 coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/models.py
+-rw-r--r--   0        0        0     1084 2023-05-21 17:45:15.267559 coinpaprika_async-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1220 2024-04-10 20:32:44.638165 coinpaprika_async-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1346 2024-04-10 11:51:13.154098 coinpaprika_async-3.1.0/README.md
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 coinpaprika_async-3.1.0/PKG-INFO
```

### Comparing `coinpaprika_async-3.0.3/LICENSE` & `coinpaprika_async-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.3/PKG-INFO` & `coinpaprika_async-3.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,67 @@
-Metadata-Version: 2.1
-Name: coinpaprika_async
-Version: 3.0.3
-Summary: An asynchronous client for the coinpaprika API.
-Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
-Author: DroidZed
-Author-email: droid.zed77@outlook.com
-License: MIT
-Keywords: coinpaprika_async,api,cryptocurrency,async,httpx,client
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx
-
-<div align="center">
-<h1 style="font-size:50px;">Coinpaprika Async Client</h1>
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coinpaprika-async)
-
-</div>
-
-## 1. Usage
-
-This library provides convenient and modern way to use [coinpaprika.com](https://api.coinpaprika.com/) API in Python.
-
-[Coinpaprika](https://coinpaprika.com/) delivers full market data to the world of crypto: coin prices, volumes, market caps, ATHs, return rates and more.
-
-## 2. Requirements
-
-```sh
-pip install coinpaprika_async
-```
-
-Or:
-
-```sh
-pipenv install coinpaprika_async
-```
-
-## 3. Getting started
-
-Each top-level path has their own endpoint class now:
-
-
-- `GET` /coins `->` `CoinsEndpoint`
-- `GET` /exchanges `->` `ExchangesEndpoint`
-- `GET` /key `->` `KeyEndpoint`
-- `GET` /global `->` `MarketEndpoint`
-- `GET` /search + /price-converter `->` `MiscelanousEndpoints`
-- `GET` /people `->` `PeopleEndpoint`
-- `GET` /tags `->` `TagsEndpoint`
-- `GET` /tickers `->` `TickersEndpoint`
-
-
-## 4 Examples:
-
-Check out the [examples](./examples) directory.
-
-## 5. Tests
-
-```test
-pip install -r requirements-dev.txt
-
-pytest tests/test_client.py
-```
-
-## 6. License
-CoinpaprikaAPI is available under the MIT license. See the LICENSE file for more info.
+Metadata-Version: 2.1
+Name: coinpaprika-async
+Version: 3.1.0
+Summary: An asynchronous library for interacting with the Coinpaprika.com API, written with httpx in Python.
+Author: DroidZed
+Author-email: 41507665+DroidZed@users.noreply.github.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
+Description-Content-Type: text/markdown
+
+<div align="center">
+<h1 style="font-size:50px;">Coinpaprika Async Client</h1>
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coinpaprika-async)
+
+</div>
+
+## 1. Usage
+
+This library provides convenient and modern way to use [coinpaprika.com](https://api.coinpaprika.com/) API in Python.
+
+[Coinpaprika](https://coinpaprika.com/) delivers full market data to the world of crypto: coin prices, volumes, market caps, ATHs, return rates and more.
+
+## 2. Requirements
+
+```sh
+pip install coinpaprika_async
+```
+
+Or:
+
+```sh
+poetry add coinpaprika_async
+```
+
+## 3. Getting started
+
+Each top-level path has their own endpoint class now:
+
+
+- `GET` /coins `->` `CoinsEndpoint`
+- `GET` /exchanges `->` `ExchangesEndpoint`
+- `GET` /key `->` `KeyEndpoint`
+- `GET` /global `->` `MarketEndpoint`
+- `GET` /search + /price-converter `->` `MiscelanousEndpoints`
+- `GET` /people `->` `PeopleEndpoint`
+- `GET` /tags `->` `TagsEndpoint`
+- `GET` /tickers `->` `TickersEndpoint`
+
+
+## 4 Examples:
+
+Check out the [examples](./examples) directory.
+
+## 5. Tests
+
+```sh
+py -m pytest -vs .
+```
+
+## 6. License
+CoinpaprikaAPI is available under the MIT license. See the LICENSE file for more info.
+
```

### Comparing `coinpaprika_async-3.0.3/README.md` & `coinpaprika_async-3.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```sh
 pip install coinpaprika_async
 ```
 
 Or:
 
 ```sh
-pipenv install coinpaprika_async
+poetry add coinpaprika_async
 ```
 
 ## 3. Getting started
 
 Each top-level path has their own endpoint class now:
 
 
@@ -41,15 +41,13 @@
 
 ## 4 Examples:
 
 Check out the [examples](./examples) directory.
 
 ## 5. Tests
 
-```test
-pip install -r requirements-dev.txt
-
-pytest tests/test_client.py
+```sh
+py -m pytest -vs .
 ```
 
 ## 6. License
 CoinpaprikaAPI is available under the MIT license. See the LICENSE file for more info.
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/api.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/coins/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,93 @@
-from ..networking_layer import Result
-from ..coinpaprika_api import CoinpaprikaAPI
+from ..client import CoinPaprikaAsyncClient
+
+from ..networking_layer import Result, ApiError
+
 from .models import *
 
 
-class CoinsEndpoint(CoinpaprikaAPI):
-    async def get_all(self):
-        res = await self.internal.call_api("coins")
+class CoinsEndpoint:
+
+    def __init__(self) -> None:
+        self.__internal = CoinPaprikaAsyncClient()
+
+    async def get_all(self) -> ApiError | list[CoinItem]:
+        res = await self.__internal.call_api("coins")
 
         if res.Error:
             return res.Error
 
         return [CoinItem(**e) for e in res.Data]
 
-    async def coin_by_id(self, coin_id: str):
-        return await self.internal.call_api(f"coins/{coin_id}")
+    async def coin_by_id(self, coin_id: str) -> Result:
+        return await self.__internal.call_api(f"coins/{coin_id}")
 
-    async def tweets_of_coin(self, coin_id: str):
+    async def tweets_of_coin(
+        self, coin_id: str
+    ) -> ApiError | list[TwitterCoinItem]:
         """Returns the last 50 timeline tweets from the official Twitter profile for a given coin.
 
         Args:
             coin_id: Required id for the coin
         """
-        res = await self.internal.call_api(f"coins/{coin_id}/twitter")
+        res = await self.__internal.call_api(f"coins/{coin_id}/twitter")
 
         if res.Error:
             return res.Error
 
         return [TwitterCoinItem(**e) for e in res.Data]
 
-    async def events_of_coin(self, coin_id: str):
+    async def events_of_coin(
+        self, coin_id: str
+    ) -> ApiError | list[EventCoinItem]:
         """Returns events for a given coin.
 
         Args:
             coin_id: Required id for the coin
         """
-        res = await self.internal.call_api(f"coins/{coin_id}/events")
+        res = await self.__internal.call_api(f"coins/{coin_id}/events")
 
         if res.Error:
             return res.Error
 
-        return [EventCointItem(**e) for e in res.Data]
+        return [EventCoinItem(**e) for e in res.Data]
 
-    async def exchanges_of_coin(self, coin_id: str):
+    async def exchanges_of_coin(
+        self, coin_id: str
+    ) -> ApiError | list[ExchangeCoinItem]:
         """Returns exchanges where a given coin is traded.
 
         Args:
             coin_id:  Required id for the coin
         """
-        res = await self.internal.call_api(f"coins/{coin_id}/exchanges")
+        res = await self.__internal.call_api(f"coins/{coin_id}/exchanges")
 
         if res.Error:
             return res.Error
 
         return [
             ExchangeCoinItem(
                 fiats=[Fiat(**f) for f in e["fiats"]],
                 id=e["id"],
                 name=e["name"],
                 adjusted_volume_24h_share=e["adjusted_volume_24h_share"],
             )
             for e in res.Data
         ]
 
-    async def markets_of_coin(self, coin_id: str, quotes: str = "USD"):
+    async def markets_of_coin(
+        self, coin_id: str, quotes: str = "USD"
+    ) -> ApiError | list[MarketCoinItem]:
         """Returns all available markets for a given coin.
 
         Args:
             coin_id: Required id for the coin
             quotes: Comma separated list of quotes to return. Currently allowed values: BTC, ETH, USD, EUR, PLN, KRW, GBP, CAD, JPY, RUB, TRY, NZD, AUD, CHF, UAH, HKD, SGD, NGN, PHP, MXN, BRL, THB, CLP, CNY, CZK, DKK, HUF, IDR, ILS, INR, MYR, NOK, PKR, SEK, TWD, ZAR, VND, BOB, COP, PEN, ARS and ISK.
         """
-        res = await self.internal.call_api(
+        res = await self.__internal.call_api(
             f"coins/{coin_id}/markets", quotes=quotes
         )
 
         if res.Error:
             return res.Error
 
         return [
@@ -94,69 +108,75 @@
                 base_currency_id=m["base_currency_id"],
                 exchange_id=m["exchange_id"],
                 adjusted_volume_24h_share=m["adjusted_volume_24h_share"],
             )
             for m in res.Data
         ]
 
-    async def latest_ohlcv(self, coin_id: str, quote: str = "usd"):
+    async def latest_ohlcv(
+        self, coin_id: str, quote: str = "usd"
+    ) -> ApiError | list[CandleItem]:
         """Returns Open/High/Low/Close values with volume and market capitalization for the last full day.
 
         Args:
             coin_id: Required id for the coin
             quote: returned data quote (available values: usd & btc).
         """
-        res = await self.internal.call_api(
+        res = await self.__internal.call_api(
             f"coins/{coin_id}/ohlcv/latest",
             quote=quote,
         )
 
-        return self.__candle_handler(res)
+        return await self.__candle_handler(res)
 
     async def historical_ohlcv(
         self,
         coin_id: str,
         start: str,
         end: Optional[str] = None,
         limit: Optional[int] = None,
         interval: Optional[str] = None,
         quote: Optional[str] = None,
-    ):
+    ) -> ApiError | list[CandleItem]:
         """Returns Open/High/Low/Close values with volume and market capitalization for any date range. If the end date is the current day, data can change with every request until actual close of the day at 23:59:59"
 
         Args:
             coin_id: Required id for the coin
             start: start point for historical data. Supported formats: RFC3999, Simple date (yyyy-mm-dd) & Unix timestamp (in seconds)
             end: end point for ohlcv (max 1 year). Supported formats: same as start date.
             limit: limit of result rows (max 366)
             interval: returned OHLCV point interval (available values: 15m, 30m, 1h, 6h, 12h, 24h)
             quote: returned data quote (available values: usd & btc)
         """
-        res = await self.internal.call_api(
+        res = await self.__internal.call_api(
             f"coins/{coin_id}/ohlcv/historical",
             start=start,
             end=end,
             limit=limit,
             interval=interval,
             quote=quote,
         )
-        return self.__candle_handler(res)
+        return await self.__candle_handler(res)
 
-    async def ohlcv_of_today(self, coin_id: str, quote: str = "usd"):
+    async def ohlcv_of_today(
+        self, coin_id: str, quote: str = "usd"
+    ) -> ApiError | list[CandleItem]:
         """Returns Open/High/Low/Close values with volume and market capitalization for the current day. Data can change every each request until actual close of the day at 23:59:59.
 
         Args:
             coin_id: Required id for the coin
             quote: returned data quote (available values: usd & btc)
         """
-        res = await self.internal.call_api(
+        res = await self.__internal.call_api(
             f"coins/{coin_id}/ohlcv/today",
             quote=quote,
         )
 
-        return self.__candle_handler(res)
+        return await self.__candle_handler(res)
 
-    async def __candle_handler(self, result: Result):
+    async def __candle_handler(
+        self, result: Result
+    ) -> ApiError | list[CandleItem]:
         if result.Error:
             return result.Error
 
         return [CandleItem(**c) for c in result.Data]
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/models.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/coins/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     status_link: str
     status_id: str
     media_link: str
     youtube_link: str
 
 
 @dataclass
-class EventCointItem:
+class EventCoinItem:
     id: str
     date: datetime
     date_to: str
     name: str
     description: str
     is_conference: bool
     link: str
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/api.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,45 @@
-from typing import Optional, Any
+from typing import Any
+
+from ..client import CoinPaprikaAsyncClient
+
+from ..networking_layer import ApiError
 
-from ..coinpaprika_api import CoinpaprikaAPI
 from .models import *
 
 
-class ExchangesEndpoint(CoinpaprikaAPI):
-    async def exchange_list(self, **params):
-        res = await self.internal.call_api("exchanges", **params)
+class ExchangesEndpoint:
+
+    def __init__(self) -> None:
+        self.__internal = CoinPaprikaAsyncClient()
+
+    async def exchange_list(self, **params: Any) -> ApiError | list[Exchange]:
+        res = await self.__internal.call_api("exchanges", **params)
 
         if res.Error:
             return res.Error
 
         return [Exchange(**data) for data in res.Data]
 
-    async def exchange(self, exchange_id: str, **params):
-        res = await self.internal.call_api(f"exchanges/{exchange_id}", **params)
+    async def get_exchange(
+        self, exchange_id: str, **params: Any
+    ) -> ApiError | Exchange:
+        res = await self.__internal.call_api(
+            f"exchanges/{exchange_id}", **params
+        )
 
         if res.Error:
             return res.Error
 
         return Exchange(**res.Data)
 
-    async def exchange_markets(self, exchange_id: str, **params):
-        res = await self.internal.call_api(
+    async def exchange_markets(
+        self, exchange_id: str, **params: Any
+    ) -> ApiError | ExchangeMarket:
+        res = await self.__internal.call_api(
             f"exchanges/{exchange_id}/markets", **params
         )
 
         if res.Error:
             return res.Error
 
         return ExchangeMarket(**res.Data)
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/models.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/exchanges/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/api.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/key/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 from typing import Dict, Any
-from ..coinpaprika_api import CoinpaprikaAPI
+
+from ..client import CoinPaprikaAsyncClient
+
+from ..networking_layer import ApiError
+
 from .models import KeyInfo, APIUsage, CurrentMonthUsage
 
 
-class KeyEndpoint(CoinpaprikaAPI):
-    async def get_key_info(self):
-        res = await self.internal.call_api("key/info")
+class KeyEndpoint:
+
+    def __init__(self) -> None:
+        self.__internal = CoinPaprikaAsyncClient()
+
+    async def get_key_info(self) -> ApiError | KeyInfo:
+        res = await self.__internal.call_api("key/info")
 
         if res.Error:
             return res.Error
 
         data: Dict[str, Any] = res.Data
 
         return KeyInfo(
             plan=data["plan"],
             plan_started_at=data["plan_started_at"],
             plan_status=data["plan_status"],
             portal_url=data["portal_url"],
             usage=APIUsage(
                 message=data["message"],
                 current_month=CurrentMonthUsage(
-                    requests_left=data["requests_left"], requests_made=data["requests_made"]
+                    requests_left=data["requests_left"],
+                    requests_made=data["requests_made"],
                 ),
             ),
         )
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/api.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/misc/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from typing import Optional, Any, Dict, List
-from ..coinpaprika_api import CoinpaprikaAPI
+
+from ..client import CoinPaprikaAsyncClient
+
+from ..networking_layer import ApiError
+
 from .models import *
 
 
-class MiscellaneousEndpoints(CoinpaprikaAPI):
-    async def people(self, person_id: str):
-        res = await self.internal.call_api(f"people/{person_id}")
+class MiscellaneousEndpoints:
+
+    def __init__(self) -> None:
+        self.__internal = CoinPaprikaAsyncClient()
+
+    async def people(self, person_id: str) -> ApiError | list[PeopleItem]:
+        res = await self.__internal.call_api(f"people/{person_id}")
 
         if res.Error:
             return res.Error
 
         data: List[Dict[str, Any]] = res.Data
 
         return [
@@ -32,15 +40,15 @@
 
     async def search(
         self,
         q: str,
         categories: Optional[str] = None,
         modifier: Optional[str] = None,
         limit: Optional[int] = 6,
-    ):
+    ) -> ApiError | list[SearchResult]:
         """Returns currencies, exchanges, icos, people, tags on coinpaprika.com for a given search query.
 
         Available on the following API plans:
 
            * Free
            * Starter
            * Pro
@@ -52,15 +60,15 @@
             categories: Available options: currencies|exchanges|icos|people|tags.
             modifier: Available options: symbol_search - search only by symbol (works for currencies only).
             limit: Limit of results per category (max 250) Defaults to 6.
 
         Returns:
             A list of the search result items.
         """
-        res = await self.internal.call_api(
+        res = await self.__internal.call_api(
             "search",
             q=q,
             c=categories,
             modifier=modifier,
             limit=limit,
         )
         if res.Error:
@@ -80,16 +88,16 @@
         ]
 
     async def price_converter(
         self,
         base_currency_id: str,
         quote_currency_id: str,
         amount: Optional[int] = 0,
-    ):
-        res = await self.internal.call_api(
+    ) -> ApiError | ConvertResult:
+        res = await self.__internal.call_api(
             "price-converter",
             base_currency_id=base_currency_id,
             quote_currency_id=quote_currency_id,
             amount=amount,
         )
 
         if res.Error:
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/models.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/misc/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/http_async_client.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/networking_layer/http_async_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,21 @@
         Raises:
             RequestError: If there was an error in the request.
         """
         try:
             async with AsyncClient() as client:
                 request_method = getattr(client, method)
                 if method in {"get", "delete"}:
-                    response = await request_method(url, headers=headers, params=url_params)
+                    response = await request_method(
+                        url, headers=headers, params=url_params
+                    )
                 else:
-                    response = await request_method(url, headers=headers, params=url_params, timeout=timeout)
+                    response = await request_method(
+                        url, headers=headers, params=url_params, timeout=timeout
+                    )
                 response.raise_for_status()
                 return Result(Data=response.json(), Error=None)
         except HTTPStatusError as exec:
             return Result(Error=ApiError(**exec.response.json()), Data=None)
 
     async def get(
         self,
@@ -61,8 +65,10 @@
             headers: Optional headers to include in the request.
             url_params: Optional URL parameters to include in the request.
             timeout: Optional number to indicate the timeout limit for the query.
 
         Returns:
             The JSON response body as a dictionary or list, or a RequestError if there was an error.
         """
-        return await self.send_request("get", url, headers=headers, url_params=url_params, timeout=timeout)
+        return await self.send_request(
+            "get", url, headers=headers, url_params=url_params, timeout=timeout
+        )
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/models.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/people/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/api.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/tags/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 from typing import Dict, List, Any, Optional
-from ..coinpaprika_api import CoinpaprikaAPI
+
+from ..client import CoinPaprikaAsyncClient
+
+from ..networking_layer import ApiError
+
 from .models import *
 
 
-class TagsEndpoint(CoinpaprikaAPI):
-    async def tags(self, additional_fields: Optional[str] = None):
-        res = await self.internal.call_api("tags", additional_fields=additional_fields)
+class TagsEndpoint:
+
+    def __init__(self) -> None:
+        self.__internal = CoinPaprikaAsyncClient()
+
+    async def tags(
+        self, additional_fields: Optional[str] = None
+    ) -> ApiError | list[Tag]:
+        res = await self.__internal.call_api(
+            "tags", additional_fields=additional_fields
+        )
 
         if res.Error:
             return res.Error
 
         data: List[Dict[str, Any]] = res.Data
 
         return [Tag(**t) for t in data]
 
-    async def tag(self, tag_id: str, additional_fields: Optional[str] = None):
-        res = await self.internal.call_api(f"tags/{tag_id}", additional_fields=additional_fields)
+    async def tag(
+        self, tag_id: str, additional_fields: Optional[str] = None
+    ) -> ApiError | Tag:
+        res = await self.__internal.call_api(
+            f"tags/{tag_id}", additional_fields=additional_fields
+        )
 
         if res.Error:
             return res.Error
 
         data: Dict[str, Any] = res.Data
 
         return Tag(**data)
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/api.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from typing import Optional, List, Dict, Any
-from ..coinpaprika_api import CoinpaprikaAPI
+
+from ..client import CoinPaprikaAsyncClient
+
+from ..networking_layer import ApiError
+
 from .models import *
 
 
-class TickersEndpoint(CoinpaprikaAPI):
-    async def tickers(self, quotes: str = "USD"):
-        res = await self.internal.call_api("tickers", quotes=quotes)
+class TickersEndpoint:
+
+    def __init__(self) -> None:
+        self.__internal = CoinPaprikaAsyncClient()
+
+    async def tickers(self, quotes: str = "USD") -> ApiError | list[TickerItem]:
+        res = await self.__internal.call_api("tickers", quotes=quotes)
         if res.Error:
             return res.Error
 
         data: List[Dict[str, Any]] = res.Data
 
         return [
             TickerItem(
@@ -24,16 +32,20 @@
                 first_data_at=tc["first_data_at"],
                 last_updated=tc["last_updated"],
                 quotes={t: Quote(**v) for t, v in tc["quotes"]},
             )
             for tc in data
         ]
 
-    async def ticker_by_coin(self, coin_id: str, quotes: str = "USD"):
-        res = await self.internal.call_api(f"tickers/{coin_id}", quotes=quotes)
+    async def ticker_by_coin(
+        self, coin_id: str, quotes: str = "USD"
+    ) -> ApiError | list[TickerItem]:
+        res = await self.__internal.call_api(
+            f"tickers/{coin_id}", quotes=quotes
+        )
 
         if res.Error:
             return res.Error
 
         data: List[Dict[str, Any]] = res.Data
 
         return [
@@ -57,16 +69,16 @@
         self,
         coin_id: str,
         start: str,
         end: str = "NOW",
         limit: Optional[int] = 1000,
         quotes: str = "USD",
         interval: str = "5m",
-    ):
-        res = await self.internal.call_api(
+    ) -> ApiError | list[HistoryTickerItem]:
+        res = await self.__internal.call_api(
             f"tickers/{coin_id}/historical",
             start=start,
             end=end,
             limit=limit,
             interval=interval,
             quotes=quotes,
         )
```

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/models.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/tickers/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.3/src/coinpaprika_async/coinpaprika_async_client.py` & `coinpaprika_async-3.1.0/coinpaprika_async_client/client/coinpaprika_async_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-from typing import Optional, Any
+from typing import Any, Optional
 
-from .api.networking_layer import HttpAsyncClient
+from ..networking_layer import HttpAsyncClient, Result
 
 
 class CoinPaprikaAsyncClient:
     """
     ### An async client for interacting with Coinpaprika's API backend.
-
     """
 
     __FREE_API_URL = "https://api.coinpaprika.com/v1"
 
     __PRO_API_URL = "https://api-pro.coinpaprika.com/v1"
 
     def __init__(
         self,
         http: HttpAsyncClient = HttpAsyncClient(),
         api_key: Optional[str] = None,
-    ):
+    ) -> None:
         self._http_client = http
         self._is_paid = api_key != None
         self._api_key = api_key
 
-    async def call_api(self, path: str, **query_params):
+    async def call_api(self, path: str, **query_params: Any) -> Result:
         uri = self.__create_api_uri(path)
         headers = self.__create_headers()
 
         return await self._http_client.get(
             uri, headers=headers, url_params=query_params, timeout=20
         )
 
-    def __create_api_uri(self, path: str):
+    def __create_api_uri(self, path: str) -> str:
         return (
             f"{self.__FREE_API_URL}/{path}"
             if not self._is_paid
             else f"{self.__PRO_API_URL}/{path}"
         )
 
-    def __create_headers(self):
+    def __create_headers(self) -> dict[str, Any | str]:
+
+        headers: dict[str, Any | str] = {
+            "Accept": "application/json",
+            "User-Agent": "coinpaprika_async-async/python",
+        }
+
         if self._is_paid:
-            return {
-                "Accept": "application/json",
-                "User-Agent": "coinpaprika_async-async/python",
-                "Authorization": self._api_key,
-            }
-        else:
-            return {
-                "Accept": "application/json",
-                "User-Agent": "coinpaprika_async-async/python",
-            }
+            headers["Authorization"] = self._api_key
+
+        return headers
```

