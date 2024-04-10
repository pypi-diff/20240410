# Comparing `tmp/multicall-0.8.2.tar.gz` & `tmp/multicall-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicall-0.8.2.tar", max compression
+gzip compressed data, was "multicall-0.9.0.tar", max compression
```

## Comparing `multicall-0.8.2.tar` & `multicall-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      116 2023-08-30 22:04:36.650529 multicall-0.8.2/multicall/__init__.py
--rw-r--r--   0        0        0     5132 2024-02-03 22:44:17.233430 multicall-0.8.2/multicall/call.py
--rw-r--r--   0        0        0    21275 2023-09-26 03:14:31.513215 multicall-0.8.2/multicall/constants.py
--rw-r--r--   0        0        0       54 2023-08-30 22:04:36.650529 multicall-0.8.2/multicall/exceptions.py
--rw-r--r--   0        0        0      267 2023-08-30 22:04:36.650529 multicall-0.8.2/multicall/loggers.py
--rw-r--r--   0        0        0     8446 2024-02-03 22:44:17.233430 multicall-0.8.2/multicall/multicall.py
--rw-r--r--   0        0        0     2669 2024-02-03 22:44:17.233430 multicall-0.8.2/multicall/signature.py
--rw-r--r--   0        0        0     3665 2024-02-03 22:49:17.478646 multicall-0.8.2/multicall/utils.py
--rw-r--r--   0        0        0      624 2024-02-03 22:44:29.505643 multicall-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 multicall-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      116 2022-01-29 20:44:41.448800 multicall-0.9.0/multicall/__init__.py
+-rw-r--r--   0        0        0     5132 2024-04-10 16:08:12.589352 multicall-0.9.0/multicall/call.py
+-rw-r--r--   0        0        0    21461 2024-04-10 16:22:28.365786 multicall-0.9.0/multicall/constants.py
+-rw-r--r--   0        0        0       54 2022-05-16 20:41:25.831925 multicall-0.9.0/multicall/exceptions.py
+-rw-r--r--   0        0        0      267 2022-05-16 20:41:25.832091 multicall-0.9.0/multicall/loggers.py
+-rw-r--r--   0        0        0     8470 2024-04-10 16:22:28.366120 multicall-0.9.0/multicall/multicall.py
+-rw-r--r--   0        0        0     2670 2024-04-10 20:14:33.108362 multicall-0.9.0/multicall/signature.py
+-rw-r--r--   0        0        0     3665 2024-04-10 20:14:28.781597 multicall-0.9.0/multicall/utils.py
+-rw-r--r--   0        0        0      585 2024-04-10 20:14:33.110449 multicall-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 multicall-0.9.0/PKG-INFO
```

### Comparing `multicall-0.8.2/multicall/call.py` & `multicall-0.9.0/multicall/call.py`

 * *Files identical despite different names*

### Comparing `multicall-0.8.2/multicall/constants.py` & `multicall-0.9.0/multicall/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,28 +44,30 @@
     Coston2Testnet = 114
     Fuse = 122
     Heco = 128
     Polygon = 137
     Fantom = 250
     Boba = 288
     KCC = 321
+    ZkSync = 324
     OptimismGorli = 420
     Astar = 592
     Metis = 1088
     Moonbeam = 1284
     Moonriver = 1285
     MoonbaseAlphaTestnet = 1287
     Milkomeda = 2001
     Kava = 2222
     FantomTestnet = 4002
     Canto = 7700
     Klaytn = 8217
     Base = 8453
     EvmosTestnet = 9000
     Evmos = 9001
+    Holesky = 17000
     Arbitrum = 42161
     Celo = 42220
     Oasis = 42262
     AvalancheFuji = 43113
     Avax = 43114
     GodwokenTestnet = 71401
     Godwoken = 71402
@@ -139,14 +141,15 @@
     Network.Coston2Testnet: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Fuse: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Heco: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Polygon: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Fantom: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Boba: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.KCC: '0xcA11bde05977b3631167028862bE2a173976CA11',
+    Network.ZkSync: '0x47898B2C52C957663aE9AB46922dCec150a2272c',
     Network.OptimismGorli: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Astar: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Metis: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Moonbeam: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Moonriver: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.MoonbaseAlphaTestnet: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Milkomeda: '0xcA11bde05977b3631167028862bE2a173976CA11',
@@ -167,23 +170,24 @@
     Network.ArbitrumGorli: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Sepolia: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Aurora: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Harmony: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.PulseChain: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.PulseChainTestnet: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Base: '0xcA11bde05977b3631167028862bE2a173976CA11',
+    Network.Holesky: '0xcA11bde05977b3631167028862bE2a173976CA11',
 }
 
 # With default AsyncBaseProvider settings, some dense calls will fail
 #   due to aiohttp.TimeoutError where they would otherwise succeed.
 AIOHTTP_TIMEOUT = ClientTimeout(int(os.environ.get("AIOHTTP_TIMEOUT", 30)))
 
 # Parallelism
 user_choice = max(1, int(os.environ.get("MULTICALL_PROCESSES", 1)))
 parallelism_capacity = max(1, os.cpu_count() - 1)
 NUM_PROCESSES = min(user_choice, parallelism_capacity)
 
-NO_STATE_OVERRIDE = [ Network.Gnosis, Network.Harmony, Network.Moonbeam, Network.Moonriver, Network.Kovan, Network.Fuse ]
+NO_STATE_OVERRIDE = [ Network.Gnosis, Network.Harmony, Network.Moonbeam, Network.Moonriver, Network.Kovan, Network.Fuse, Network.ZkSync ]
 
 # NOTE: If we run too many async calls at once, we'll have memory issues.
 #       Feel free to increase this with the "MULTICALL_CALL_SEMAPHORE" env var if you know what you're doing.
 ASYNC_SEMAPHORE = int(os.environ.get("MULTICALL_CALL_SEMAPHORE", 1000))
```

### Comparing `multicall-0.8.2/multicall/multicall.py` & `multicall-0.9.0/multicall/multicall.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,18 +81,18 @@
         if calls is None:
             calls = self.calls
         
         async with _get_semaphore():
             try:
                 args = await run_in_subprocess(get_args, calls, self.require_success)
                 if self.require_success is True:
-                    _, outputs = await self.aggregate.coroutine(args)
+                    self.block_id, outputs = await self.aggregate.coroutine(args)
                     outputs = await run_in_subprocess(unpack_aggregate_outputs, outputs)
                 else:
-                    _, _, outputs = await self.aggregate.coroutine(args)
+                    self.block_id, _, outputs = await self.aggregate.coroutine(args)
                 outputs = await gather([
                     run_in_subprocess(Call.decode_output, output, call.signature, call.returns, success)
                     for call, (success, output) in zip(calls, outputs)
                 ])
                 logger.debug(f"coroutine {id} finished")
                 return outputs
             except Exception as e:
```

### Comparing `multicall-0.8.2/multicall/signature.py` & `multicall-0.9.0/multicall/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import lru_cache
 from typing import Any, List, Optional, Tuple
 
 # For eth_abi versions < 2.2.0, `decode` and `encode` have not yet been added.
-# As we require web3 ^5.27, we require eth_abi compatability with eth_abi v2.0.0b6 and greater.
+# As we require web3 >=5.27, we require eth_abi compatability with eth_abi v2.0.0b6 and greater.
 try:
     from eth_abi import decode, encode
 except ImportError: 
     from eth_abi import encode_abi as encode, decode_abi as decode
 
 from eth_typing.abi import Decodable, TypeStr
 from eth_utils import function_signature_to_4byte_selector
```

### Comparing `multicall-0.8.2/multicall/utils.py` & `multicall-0.9.0/multicall/utils.py`

 * *Files identical despite different names*

### Comparing `multicall-0.8.2/pyproject.toml` & `multicall-0.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 [tool.poetry]
 name = "multicall"
-version = "0.8.2"
+version = "0.9.0"
 description = "aggregate results from multiple ethereum contract calls"
 authors = ["banteg"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<4"
 # These web3.py versions have a busted async provider and cannot be used in any multithreaded applications
-web3 = "^5.27,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2"
-eth_retry = "^0.1.8"
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-flake8 = "^5.0"
-black = "^22.8"
-joblib = "^1.2"
+web3 = ">=5.27,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2"
+eth_retry = ">=0.1.8"
 
 [tool.poetry.group.dev.dependencies]
-eth-brownie = "^1.19.3"
+pytest = ">=6.2.5"
+ruff = ">=0.3.5"
+joblib = ">=1.2"
+# eth-brownie = ">=1.19.3"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

