# Comparing `tmp/synthetix-0.1.5.tar.gz` & `tmp/synthetix-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetix-0.1.5.tar", last modified: Tue Apr  2 20:10:32 2024, max compression
+gzip compressed data, was "synthetix-0.1.6.tar", last modified: Wed Apr 10 20:24:07 2024, max compression
```

## Comparing `synthetix-0.1.5.tar` & `synthetix-0.1.6.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.623297 synthetix-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 20:10:19.000000 synthetix-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-02 20:10:32.623297 synthetix-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-02 20:10:19.000000 synthetix-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:10:32.623297 synthetix-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-02 20:10:19.000000 synthetix-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.607297 synthetix-0.1.5/synthetix/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.607297 synthetix-0.1.5/synthetix/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/1/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/1/CannonRegistry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/10/
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/10/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/420/
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/420/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.611297 synthetix-0.1.5/synthetix/contracts/deployments/421614/
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/421614/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.615297 synthetix-0.1.5/synthetix/contracts/deployments/8453/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/USDC.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/8453/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/contracts/deployments/84532/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116830 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/MintableToken.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   102340 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/Pyth.json
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/84532/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/contracts/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/core/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/perps/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/perps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37923 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/perps/perps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/pyth/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/spot/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/spot/spot.py
--rw-r--r--   0 runner    (1001) docker     (127)    20714 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-02 20:10:19.000000 synthetix-0.1.5/synthetix/utils/wei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/synthetix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 20:10:32.000000 synthetix-0.1.5/synthetix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:10:32.619297 synthetix-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_perps_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_spot_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_susd.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-02 20:10:19.000000 synthetix-0.1.5/tests/test_synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 20:23:51.000000 synthetix-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-10 20:24:07.187604 synthetix-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-10 20:23:51.000000 synthetix-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:24:07.187604 synthetix-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 20:23:51.000000 synthetix-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.171604 synthetix-0.1.6/synthetix/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/deployments/1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/1/CannonRegistry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/deployments/10/
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.179604 synthetix-0.1.6/synthetix/contracts/deployments/420/
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.179604 synthetix-0.1.6/synthetix/contracts/deployments/421614/
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/421614/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.179604 synthetix-0.1.6/synthetix/contracts/deployments/8453/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/contracts/deployments/84532/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/MintableToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/Pyth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/perps/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/perps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37923 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/perps/perps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/pyth/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/spot/spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/synthetix/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/utils/wei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/synthetix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_perps_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_spot_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_susd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_synthetix.py
```

### Comparing `synthetix-0.1.5/PKG-INFO` & `synthetix-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.5
+Version: 0.1.6
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.5/README.md` & `synthetix-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/setup.py` & `synthetix-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="synthetix",
-    version="0.1.5",
+    version="0.1.6",
     description="Synthetix protocol SDK",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Synthetix DAO",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `synthetix-0.1.5/synthetix/constants.py` & `synthetix-0.1.6/synthetix/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/contracts.py` & `synthetix-0.1.6/synthetix/contracts/contracts.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/1/CannonRegistry.json` & `synthetix-0.1.6/synthetix/contracts/deployments/1/CannonRegistry.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/10/PerpsV2MarketData.json` & `synthetix-0.1.6/synthetix/contracts/deployments/10/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/10/USDProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/10/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/10/WETH.json` & `synthetix-0.1.6/synthetix/contracts/deployments/10/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/10/sUSD.json` & `synthetix-0.1.6/synthetix/contracts/deployments/10/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/AccountProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/CoreProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsAccountProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsMarketProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2Market.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/PerpsV2MarketData.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/SpotMarketProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/USDProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/WETH.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/420/sUSD.json` & `synthetix-0.1.6/synthetix/contracts/deployments/420/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/421614/WETH.json` & `synthetix-0.1.6/synthetix/contracts/deployments/421614/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/AccountProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/CoreProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsAccountProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/PerpsMarketProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/SpotMarketProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/USDC.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/USDC.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/USDProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/8453/WETH.json` & `synthetix-0.1.6/synthetix/contracts/deployments/8453/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/AccountProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/AccountProxy.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'address'": "'0x9EB560Cc26c2766929A41F8e46E87bd4b8b145d9'"}*

```diff
@@ -803,15 +803,15 @@
             ],
             "name": "transferFrom",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "address": "0xa88694d0025dd96194D1B0237fDEbf7D1D34B02F",
+    "address": "0x9EB560Cc26c2766929A41F8e46E87bd4b8b145d9",
     "contractName": "",
     "deployTxnHash": "",
     "deployedOn": "invoke.init_account",
     "gasCost": "0",
     "gasUsed": 0,
     "highlight": true,
     "sourceName": ""
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/CoreProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/CoreProxy.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444374439964158%*

 * *Differences: {"'abi'": "{142: {'inputs': {delete: [7]}}, 143: {'inputs': {delete: [7]}}}",*

 * * "'address'": "'0x764F4C95FDA0D6f8114faC54f6709b1B45f919a1'"}*

```diff
@@ -3042,20 +3042,14 @@
                     "type": "int128"
                 },
                 {
                     "indexed": false,
                     "internalType": "uint256",
                     "name": "depositedCollateralValue",
                     "type": "uint256"
-                },
-                {
-                    "indexed": false,
-                    "internalType": "uint256",
-                    "name": "reportedDebt",
-                    "type": "uint256"
                 }
             ],
             "name": "MarketUsdDeposited",
             "type": "event"
         },
         {
             "anonymous": false,
@@ -3097,20 +3091,14 @@
                     "type": "int128"
                 },
                 {
                     "indexed": false,
                     "internalType": "uint256",
                     "name": "depositedCollateralValue",
                     "type": "uint256"
-                },
-                {
-                    "indexed": false,
-                    "internalType": "uint256",
-                    "name": "reportedDebt",
-                    "type": "uint256"
                 }
             ],
             "name": "MarketUsdWithdrawn",
             "type": "event"
         },
         {
             "anonymous": false,
@@ -5284,15 +5272,15 @@
                     "type": "int256"
                 }
             ],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "address": "0xF4Df9Dd327Fd30695d478c3c8a2fffAddcdD0d31",
+    "address": "0x764F4C95FDA0D6f8114faC54f6709b1B45f919a1",
     "contractName": "",
     "deployTxnHash": "",
     "deployedOn": "invoke.upgrade_core_proxy",
     "gasCost": "0",
     "gasUsed": 0,
     "highlight": true,
     "sourceName": ""
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/MintableToken.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/MintableToken.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8181818181818182%*

 * *Differences: {"'address'": "'0xc43708f8987Df3f3681801e5e640667D86Ce3C30'",*

 * * "'deployTxnHash'": "'0x0cc8970d5bc56b2196fd8bc2008fe8c2c1bf3d23ba0b4d818dc85df201914141'",*

 * * "'gasCost'": "'1000291'",*

 * * "'gasUsed'": '774845'}*

```diff
@@ -368,24 +368,24 @@
                     "type": "uint256"
                 }
             ],
             "name": "Transfer",
             "type": "event"
         }
     ],
-    "address": "0x69980C3296416820623b3e3b30703A74e2320bC8",
+    "address": "0xc43708f8987Df3f3681801e5e640667D86Ce3C30",
     "constructorArgs": [
         "0x48914229deDd5A9922f44441ffCCfC2Cb7856Ee9",
         "Fake USD Coin",
         "fUSDC",
         "6",
         "0"
     ],
     "contractName": "MintableToken",
-    "deployTxnHash": "0xb5c336c0978bf00ca0b676958c6bd4708669ec6c38a068a3af9a65ce58692546",
+    "deployTxnHash": "0x0cc8970d5bc56b2196fd8bc2008fe8c2c1bf3d23ba0b4d818dc85df201914141",
     "deployedOn": "contract.MintableToken",
-    "gasCost": "1500000254",
-    "gasUsed": 774833,
+    "gasCost": "1000291",
+    "gasUsed": 774845,
     "highlight": true,
     "linkedLibraries": {},
     "sourceName": "src/MintableToken.sol"
 }
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsAccountProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsAccountProxy.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'address'": "'0xc8eE218577545D5b38443C0eB5d7B9E4140085F2'"}*

```diff
@@ -803,15 +803,15 @@
             ],
             "name": "transferFrom",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "address": "0x87f578681CDE29F0701E7274708E1A67Ee9eEf94",
+    "address": "0xc8eE218577545D5b38443C0eB5d7B9E4140085F2",
     "contractName": "",
     "deployTxnHash": "",
     "deployedOn": "invoke.init_account",
     "gasCost": "0",
     "gasUsed": 0,
     "highlight": true,
     "sourceName": ""
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/PerpsMarketProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsMarketProxy.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.942823026646556%*

 * *Differences: {"'abi'": "{165: {'inputs': {delete: [1]}, 'name': 'MaxMarketValueSet'}, 175: {'name': "*

 * *          "'getMaxMarketValue', 'outputs': {delete: [0]}}, 184: {'inputs': {delete: [1]}, 'name': "*

 * *          "'setMaxMarketValue'}, insert: [(86, OrderedDict([('inputs', "*

 * *          "[OrderedDict([('internalType', 'uint128'), ('name', 'accountId'), ('type', "*

 * *          "'uint128')]), OrderedDict([('internalType', 'uint128'), ('name', 'marketId'), ('type', "*

 * *          "'uint128')])]), ('name', 'getOpenPositionSize'), (' […]*

```diff
@@ -1384,14 +1384,38 @@
         },
         {
             "inputs": [
                 {
                     "internalType": "uint128",
                     "name": "accountId",
                     "type": "uint128"
+                },
+                {
+                    "internalType": "uint128",
+                    "name": "marketId",
+                    "type": "uint128"
+                }
+            ],
+            "name": "getOpenPositionSize",
+            "outputs": [
+                {
+                    "internalType": "int128",
+                    "name": "positionSize",
+                    "type": "int128"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
+                    "name": "accountId",
+                    "type": "uint128"
                 }
             ],
             "name": "getRequiredMargins",
             "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "requiredInitialMargin",
@@ -2177,14 +2201,38 @@
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "uint128",
+                    "name": "marketId",
+                    "type": "uint128"
+                },
+                {
+                    "internalType": "uint128",
+                    "name": "settlementStrategyId",
+                    "type": "uint128"
+                }
+            ],
+            "name": "getSettlementRewardCost",
+            "outputs": [
+                {
+                    "internalType": "uint256",
+                    "name": "",
+                    "type": "uint256"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
                     "name": "accountId",
                     "type": "uint128"
                 },
                 {
                     "internalType": "uint128",
                     "name": "marketId",
                     "type": "uint128"
@@ -2898,14 +2946,51 @@
                     "indexed": true,
                     "internalType": "uint128",
                     "name": "accountId",
                     "type": "uint128"
                 },
                 {
                     "indexed": false,
+                    "internalType": "int256",
+                    "name": "availableMargin",
+                    "type": "int256"
+                },
+                {
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "requiredMaintenanceMargin",
+                    "type": "uint256"
+                },
+                {
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "liquidationReward",
+                    "type": "uint256"
+                },
+                {
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "flagReward",
+                    "type": "uint256"
+                }
+            ],
+            "name": "AccountFlaggedForLiquidation",
+            "type": "event"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
+                {
+                    "indexed": true,
+                    "internalType": "uint128",
+                    "name": "accountId",
+                    "type": "uint128"
+                },
+                {
+                    "indexed": false,
                     "internalType": "uint256",
                     "name": "reward",
                     "type": "uint256"
                 },
                 {
                     "indexed": false,
                     "internalType": "bool",
@@ -3235,23 +3320,36 @@
                     "type": "uint128"
                 },
                 {
                     "indexed": false,
                     "internalType": "uint256",
                     "name": "maxMarketSize",
                     "type": "uint256"
+                }
+            ],
+            "name": "MaxMarketSizeSet",
+            "type": "event"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
+                {
+                    "indexed": true,
+                    "internalType": "uint128",
+                    "name": "marketId",
+                    "type": "uint128"
                 },
                 {
                     "indexed": false,
                     "internalType": "uint256",
                     "name": "maxMarketValue",
                     "type": "uint256"
                 }
             ],
-            "name": "MaxMarketSizesSet",
+            "name": "MaxMarketValueSet",
             "type": "event"
         },
         {
             "anonymous": false,
             "inputs": [
                 {
                     "indexed": true,
@@ -3595,21 +3693,35 @@
             "inputs": [
                 {
                     "internalType": "uint128",
                     "name": "marketId",
                     "type": "uint128"
                 }
             ],
-            "name": "getMaxMarketSizes",
+            "name": "getMaxMarketSize",
             "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "maxMarketSize",
                     "type": "uint256"
-                },
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
+                    "name": "marketId",
+                    "type": "uint128"
+                }
+            ],
+            "name": "getMaxMarketValue",
+            "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "maxMarketValue",
                     "type": "uint256"
                 }
             ],
             "stateMutability": "view",
@@ -3848,22 +3960,35 @@
                     "name": "marketId",
                     "type": "uint128"
                 },
                 {
                     "internalType": "uint256",
                     "name": "maxMarketSize",
                     "type": "uint256"
+                }
+            ],
+            "name": "setMaxMarketSize",
+            "outputs": [],
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
+                    "name": "marketId",
+                    "type": "uint128"
                 },
                 {
                     "internalType": "uint256",
                     "name": "maxMarketValue",
                     "type": "uint256"
                 }
             ],
-            "name": "setMaxMarketSizes",
+            "name": "setMaxMarketValue",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
@@ -4540,15 +4665,15 @@
             ],
             "name": "updateReferrerShare",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "address": "0xE6C5f05C415126E6b81FCc3619f65Db2fCAd58D0",
+    "address": "0xf53Ca60F031FAf0E347D44FbaA4870da68250c8d",
     "contractName": "",
     "deployTxnHash": "",
     "deployedOn": "invoke.upgrade_proxy",
     "gasCost": "0",
     "gasUsed": 0,
     "highlight": true,
     "sourceName": ""
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/Pyth.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/Pyth.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'address'": "'0xF9e9e905d3745F5E0B803a179E17328CFe03B56d'",*

 * * "'deployTxnHash'": "''",*

 * * "'gasCost'": "'0'",*

 * * "'gasUsed'": '0'}*

```diff
@@ -151,19 +151,19 @@
             "type": "function"
         },
         {
             "stateMutability": "payable",
             "type": "receive"
         }
     ],
-    "address": "0xBf01fE835b3315968bbc094f50AE3164e6d3D969",
+    "address": "0xF9e9e905d3745F5E0B803a179E17328CFe03B56d",
     "constructorArgs": [
         "0xA2aa501b19aff244D90cc15a4Cf739D2725B5729"
     ],
     "contractName": "PythERC7412Wrapper",
-    "deployTxnHash": "0x872050a196959b8c0b255bcbb0fe55f67117ce8ad54c15e6280e4fbebfe0377b",
+    "deployTxnHash": "",
     "deployedOn": "contract.PythERC7412Wrapper",
-    "gasCost": "1500000254",
-    "gasUsed": 1109617,
+    "gasCost": "0",
+    "gasUsed": 0,
     "linkedLibraries": {},
     "sourceName": "contracts/PythERC7412Wrapper.sol"
 }
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/SpotMarketProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/SpotMarketProxy.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8319357092941999%*

 * *Differences: {"'abi'": "{insert: [(39, OrderedDict([('inputs', [OrderedDict([('internalType', 'uint128'), "*

 * *          "('name', 'synthMarketId'), ('type', 'uint128')])]), ('name', "*

 * *          "'getNominatedMarketOwner'), ('outputs', [OrderedDict([('internalType', 'address'), "*

 * *          "('name', 'marketOwner'), ('type', 'address')])]), ('stateMutability', 'view'), ('type', "*

 * *          "'function')])), (40, OrderedDict([('inputs', [OrderedDict([('internalType', 'uint128'), "*

 * *          "('name', 'synthMarketId'), ('type' […]*

```diff
@@ -588,14 +588,62 @@
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "uint128",
+                    "name": "synthMarketId",
+                    "type": "uint128"
+                }
+            ],
+            "name": "getNominatedMarketOwner",
+            "outputs": [
+                {
+                    "internalType": "address",
+                    "name": "marketOwner",
+                    "type": "address"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
+                    "name": "synthMarketId",
+                    "type": "uint128"
+                }
+            ],
+            "name": "getPriceData",
+            "outputs": [
+                {
+                    "internalType": "bytes32",
+                    "name": "buyFeedId",
+                    "type": "bytes32"
+                },
+                {
+                    "internalType": "bytes32",
+                    "name": "sellFeedId",
+                    "type": "bytes32"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "strictPriceStalenessTolerance",
+                    "type": "uint256"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
                     "name": "marketId",
                     "type": "uint128"
                 }
             ],
             "name": "getSynth",
             "outputs": [
                 {
@@ -1299,14 +1347,33 @@
         },
         {
             "inputs": [
                 {
                     "internalType": "uint128",
                     "name": "marketId",
                     "type": "uint128"
+                }
+            ],
+            "name": "getMarketSkew",
+            "outputs": [
+                {
+                    "internalType": "int256",
+                    "name": "marketSkew",
+                    "type": "int256"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
+                    "name": "marketId",
+                    "type": "uint128"
                 },
                 {
                     "internalType": "uint256",
                     "name": "usdAmount",
                     "type": "uint256"
                 },
                 {
@@ -2862,14 +2929,38 @@
         },
         {
             "inputs": [
                 {
                     "internalType": "uint128",
                     "name": "marketId",
                     "type": "uint128"
+                }
+            ],
+            "name": "getWrapper",
+            "outputs": [
+                {
+                    "internalType": "address",
+                    "name": "wrapCollateralType",
+                    "type": "address"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "maxWrappableAmount",
+                    "type": "uint256"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
+                {
+                    "internalType": "uint128",
+                    "name": "marketId",
+                    "type": "uint128"
                 },
                 {
                     "internalType": "address",
                     "name": "wrapCollateralType",
                     "type": "address"
                 },
                 {
@@ -3838,15 +3929,16 @@
             ],
             "name": "setFeatureFlagDenyAll",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "address": "0xA4fE63F8ea9657990eA8E05Ebfa5C19a7D4d7337",
+    "address": "0xaD2fE7cd224c58871f541DAE01202F93928FEF72",
     "contractName": "",
     "deployTxnHash": "",
     "deployedOn": "invoke.upgradeSpotMarketProxy",
     "gasCost": "0",
     "gasUsed": 0,
+    "highlight": true,
     "sourceName": ""
 }
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/USDProxy.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/USDProxy.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'address'": "'0x682f0d17feDC62b2a0B91f8992243Bf44cAfeaaE'"}*

```diff
@@ -819,15 +819,15 @@
                     "type": "bool"
                 }
             ],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "address": "0xa89163A087fe38022690C313b5D4BBF12574637f",
+    "address": "0x682f0d17feDC62b2a0B91f8992243Bf44cAfeaaE",
     "contractName": "",
     "deployTxnHash": "",
     "deployedOn": "invoke.init_usd",
     "gasCost": "0",
     "gasUsed": 0,
     "highlight": true,
     "sourceName": ""
```

### Comparing `synthetix-0.1.5/synthetix/contracts/deployments/84532/WETH.json` & `synthetix-0.1.6/synthetix/contracts/deployments/84532/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/core/core.py` & `synthetix-0.1.6/synthetix/core/core.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/perps/perps.py` & `synthetix-0.1.6/synthetix/perps/perps.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/pyth/constants.py` & `synthetix-0.1.6/synthetix/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/pyth/pyth.py` & `synthetix-0.1.6/synthetix/pyth/pyth.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/queries/config.py` & `synthetix-0.1.6/synthetix/queries/config.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/queries/gql.py` & `synthetix-0.1.6/synthetix/queries/gql.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/queries/queries.py` & `synthetix-0.1.6/synthetix/queries/queries.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/spot/spot.py` & `synthetix-0.1.6/synthetix/spot/spot.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/synthetix.py` & `synthetix-0.1.6/synthetix/synthetix.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,27 @@
 from .spot import Spot
 
 from .queries import Queries
 
 warnings.filterwarnings("ignore")
 
 
+def setup_logging():
+    # set up logging
+    logger = logging.getLogger(__name__)
+    logger.setLevel(logging.INFO)
+
+    handler = logging.StreamHandler()
+    handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
+
+    if not logger.handlers:
+        logger.addHandler(handler)
+    return logger
+
+
 class Synthetix:
     """
     The main class for interacting with the Synthetix protocol. The class
     requires a provider RPC endpoint and a wallet address::
 
             snx = Synthetix(
                 provider_rpc='https://base-mainnet.infura.io/v3/...',
@@ -97,29 +110,15 @@
         cannon_config: dict = None,
         gql_endpoint_perps: str = None,
         gql_endpoint_rates: str = None,
         satsuma_api_key: str = None,
         price_service_endpoint: str = None,
         gas_multiplier: float = DEFAULT_GAS_MULTIPLIER,
     ):
-        # set up logging
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(logging.INFO)
-
-        handler = logging.StreamHandler()
-        handler.setFormatter(
-            logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-        )
-        self.logger.addHandler(handler)
-
-        # set default values
-        if network_id is None:
-            network_id = DEFAULT_NETWORK_ID
-        else:
-            network_id = int(network_id)
+        self.logger = setup_logging()
 
         # init account variables
         self.private_key = private_key
         self.use_estimate_gas = use_estimate_gas
         self.cannon_config = cannon_config
         self.provider_rpc = provider_rpc
         self.mainnet_rpc = mainnet_rpc
@@ -140,23 +139,40 @@
             raise Exception("Provider RPC endpoint is invalid")
 
         # check for RPC signers
         self.rpc_signers = web3.eth.accounts
         if address == ADDRESS_ZERO and len(web3.eth.accounts) > 0:
             self.address = web3.eth.accounts[0]
             self.logger.info(f"Using RPC signer: {self.address}")
+        elif address == ADDRESS_ZERO and self.private_key is not None:
+            self.address = web3.eth.account.from_key(self.private_key).address
+            self.logger.info(f"Using private key signer: {self.address}")
+        elif address != ADDRESS_ZERO and self.private_key is not None:
+            # check the address matches the private key
+            if web3.eth.account.from_key(self.private_key).address != address:
+                raise Exception("Private key does not match the provided address")
+            self.address = address
         else:
+            # set address without private key
             self.address = address
+            self.logger.info(f"Using provided address without private key: {self.address}")
 
-        # check if the chain_id matches
-        if web3.eth.chain_id != network_id:
+        # check network id
+        if network_id is None:
+            self.logger.info(
+                f"Setting network_id from RPC chain_id: {web3.eth.chain_id}"
+            )
+            network_id = web3.eth.chain_id
+        elif web3.eth.chain_id != network_id:
             raise Exception("The RPC `chain_id` must match the stored `network_id`")
         else:
-            self.nonce = web3.eth.get_transaction_count(self.address)
+            network_id = int(network_id)
 
+        # set nonce
+        self.nonce = web3.eth.get_transaction_count(self.address)
         self.web3 = web3
         self.network_id = network_id
 
         # init contracts
         self.contracts = load_contracts(self)
         (
             self.v2_markets,
```

### Comparing `synthetix-0.1.5/synthetix/utils/multicall.py` & `synthetix-0.1.6/synthetix/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix/utils/wei.py` & `synthetix-0.1.6/synthetix/utils/wei.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/synthetix.egg-info/PKG-INFO` & `synthetix-0.1.6/synthetix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.5
+Version: 0.1.6
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.5/synthetix.egg-info/SOURCES.txt` & `synthetix-0.1.6/synthetix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/tests/test_perps_v3.py` & `synthetix-0.1.6/tests/test_perps_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/tests/test_spot_v3.py` & `synthetix-0.1.6/tests/test_spot_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.5/tests/test_susd.py` & `synthetix-0.1.6/tests/test_susd.py`

 * *Files identical despite different names*

