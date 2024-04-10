# Comparing `tmp/dedust-1.1.2.tar.gz` & `tmp/dedust-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedust-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dedust-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dedust-1.1.2.tar` & `dedust-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       17 2023-09-19 13:32:36.953436 dedust-1.1.2/.gitignore
--rw-r--r--   0        0        0     1077 2023-09-19 12:59:05.189083 dedust-1.1.2/LICENSE.md
--rw-r--r--   0        0        0     2518 2024-01-18 19:56:39.064971 dedust-1.1.2/README.md
--rw-r--r--   0        0        0      164 2023-09-19 13:30:44.402665 dedust-1.1.2/dedust/__init__.py
--rw-r--r--   0        0        0       73 2023-09-19 12:59:05.189372 dedust-1.1.2/dedust/constants.py
--rw-r--r--   0        0        0      178 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/__init__.py
--rw-r--r--   0        0        0      120 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/dex/__init__.py
--rw-r--r--   0        0        0      141 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/dex/common/__init__.py
--rw-r--r--   0        0        0     2311 2023-12-11 14:12:15.397622 dedust-1.1.2/dedust/contracts/dex/common/asset.py
--rw-r--r--   0        0        0       95 2023-09-19 12:59:05.000000 dedust-1.1.2/dedust/contracts/dex/common/asset_error.py
--rw-r--r--   0        0        0       75 2023-09-19 12:59:05.000000 dedust-1.1.2/dedust/contracts/dex/common/asset_type.py
--rw-r--r--   0        0        0      133 2023-09-19 12:59:05.000000 dedust-1.1.2/dedust/contracts/dex/common/readiness_status.py
--rw-r--r--   0        0        0       29 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/dex/factory/__init__.py
--rw-r--r--   0        0        0     4168 2023-12-11 14:12:15.398301 dedust-1.1.2/dedust/contracts/dex/factory/factory.py
--rw-r--r--   0        0        0       48 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/dex/liquidity_deposit/__init__.py
--rw-r--r--   0        0        0     3516 2023-12-11 14:12:15.398483 dedust-1.1.2/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py
--rw-r--r--   0        0        0       55 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/dex/pool/__init__.py
--rw-r--r--   0        0        0     3883 2023-12-11 14:12:15.398660 dedust-1.1.2/dedust/contracts/dex/pool/pool.py
--rw-r--r--   0        0        0       76 2023-09-19 12:59:05.000000 dedust-1.1.2/dedust/contracts/dex/pool/pool_type.py
--rw-r--r--   0        0        0      123 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/dex/vault/__init__.py
--rw-r--r--   0        0        0     2564 2023-12-11 14:12:15.398801 dedust-1.1.2/dedust/contracts/dex/vault/vault.py
--rw-r--r--   0        0        0     2443 2023-12-11 14:12:15.398943 dedust-1.1.2/dedust/contracts/dex/vault/vault_jetton.py
--rw-r--r--   0        0        0     2530 2023-12-11 14:12:15.399101 dedust-1.1.2/dedust/contracts/dex/vault/vault_native.py
--rw-r--r--   0        0        0       76 2023-09-19 13:30:44.000000 dedust-1.1.2/dedust/contracts/jettons/__init__.py
--rw-r--r--   0        0        0     1591 2023-12-11 14:12:15.399375 dedust-1.1.2/dedust/contracts/jettons/jetton_root.py
--rw-r--r--   0        0        0     2156 2023-12-11 14:12:15.399510 dedust-1.1.2/dedust/contracts/jettons/jetton_wallet.py
--rw-r--r--   0        0        0     2370 2023-12-11 14:12:15.399665 dedust-1.1.2/examples/deposit_liquidity.py
--rw-r--r--   0        0        0      814 2023-12-11 14:12:15.399803 dedust-1.1.2/examples/get_jetton_price.py
--rw-r--r--   0        0        0     1620 2023-12-11 14:12:15.399938 dedust-1.1.2/examples/multihop.py
--rw-r--r--   0        0        0     1310 2023-12-11 14:12:15.400071 dedust-1.1.2/examples/swap_jetton_to_ton.py
--rw-r--r--   0        0        0     1386 2023-12-11 14:12:15.400208 dedust-1.1.2/examples/swap_ton_to_jetton.py
--rw-r--r--   0        0        0      961 2023-12-11 14:12:15.400349 dedust-1.1.2/examples/withdraw_liquidity.py
--rw-r--r--   0        0        0      323 2024-01-18 19:56:28.011388 dedust-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       32 2023-12-11 14:12:15.400647 dedust-1.1.2/requirements.txt
--rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 dedust-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-09-19 13:32:36.953436 dedust-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1077 2023-09-19 12:59:05.189083 dedust-1.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2540 2024-04-10 18:26:28.499939 dedust-1.1.3/README.md
+-rw-r--r--   0        0        0      164 2023-09-19 13:30:44.402665 dedust-1.1.3/dedust/__init__.py
+-rw-r--r--   0        0        0       73 2023-09-19 12:59:05.189372 dedust-1.1.3/dedust/constants.py
+-rw-r--r--   0        0        0      178 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/__init__.py
+-rw-r--r--   0        0        0      120 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/__init__.py
+-rw-r--r--   0        0        0      141 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/common/__init__.py
+-rw-r--r--   0        0        0     2311 2023-12-11 14:12:15.397622 dedust-1.1.3/dedust/contracts/dex/common/asset.py
+-rw-r--r--   0        0        0       95 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/common/asset_error.py
+-rw-r--r--   0        0        0       75 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/common/asset_type.py
+-rw-r--r--   0        0        0      133 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/common/readiness_status.py
+-rw-r--r--   0        0        0       29 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/factory/__init__.py
+-rw-r--r--   0        0        0     4168 2023-12-11 14:12:15.398301 dedust-1.1.3/dedust/contracts/dex/factory/factory.py
+-rw-r--r--   0        0        0       48 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/liquidity_deposit/__init__.py
+-rw-r--r--   0        0        0     3516 2023-12-11 14:12:15.398483 dedust-1.1.3/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py
+-rw-r--r--   0        0        0       55 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/pool/__init__.py
+-rw-r--r--   0        0        0     3883 2023-12-11 14:12:15.398660 dedust-1.1.3/dedust/contracts/dex/pool/pool.py
+-rw-r--r--   0        0        0       76 2023-09-19 12:59:05.000000 dedust-1.1.3/dedust/contracts/dex/pool/pool_type.py
+-rw-r--r--   0        0        0      123 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/dex/vault/__init__.py
+-rw-r--r--   0        0        0     2564 2023-12-11 14:12:15.398801 dedust-1.1.3/dedust/contracts/dex/vault/vault.py
+-rw-r--r--   0        0        0     2443 2023-12-11 14:12:15.398943 dedust-1.1.3/dedust/contracts/dex/vault/vault_jetton.py
+-rw-r--r--   0        0        0     2530 2023-12-11 14:12:15.399101 dedust-1.1.3/dedust/contracts/dex/vault/vault_native.py
+-rw-r--r--   0        0        0       76 2023-09-19 13:30:44.000000 dedust-1.1.3/dedust/contracts/jettons/__init__.py
+-rw-r--r--   0        0        0     1591 2023-12-11 14:12:15.399375 dedust-1.1.3/dedust/contracts/jettons/jetton_root.py
+-rw-r--r--   0        0        0     2156 2023-12-11 14:12:15.399510 dedust-1.1.3/dedust/contracts/jettons/jetton_wallet.py
+-rw-r--r--   0        0        0     2370 2023-12-11 14:12:15.399665 dedust-1.1.3/examples/deposit_liquidity.py
+-rw-r--r--   0        0        0      814 2023-12-11 14:12:15.399803 dedust-1.1.3/examples/get_jetton_price.py
+-rw-r--r--   0        0        0     1620 2023-12-11 14:12:15.399938 dedust-1.1.3/examples/multihop.py
+-rw-r--r--   0        0        0     1310 2023-12-11 14:12:15.400071 dedust-1.1.3/examples/swap_jetton_to_ton.py
+-rw-r--r--   0        0        0     1386 2023-12-11 14:12:15.400208 dedust-1.1.3/examples/swap_ton_to_jetton.py
+-rw-r--r--   0        0        0      961 2023-12-11 14:12:15.400349 dedust-1.1.3/examples/withdraw_liquidity.py
+-rw-r--r--   0        0        0      323 2024-04-10 18:26:12.514335 dedust-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-12-11 14:12:15.400647 dedust-1.1.3/requirements.txt
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 dedust-1.1.3/PKG-INFO
```

### Comparing `dedust-1.1.2/LICENSE.md` & `dedust-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/README.md` & `dedust-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 ## Authors
 
 [@shibdev](https://t.me/dogpy)
 [@VladPavly](https://t.me/dalvpv)
 
 ## Version History
 
+* 1.1.3
+    * Bug fix
 * 1.1.2
     * Bug fix
 * 1.1.1
     * Bug fix
 * 1.1.0
     * Change tonsdk to pytoniq
 * 1.0.5
```

### Comparing `dedust-1.1.2/dedust/contracts/dex/common/asset.py` & `dedust-1.1.3/dedust/contracts/dex/common/asset.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/dex/factory/factory.py` & `dedust-1.1.3/dedust/contracts/dex/factory/factory.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py` & `dedust-1.1.3/dedust/contracts/dex/liquidity_deposit/liquidity_deposit.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/dex/pool/pool.py` & `dedust-1.1.3/dedust/contracts/dex/pool/pool.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/dex/vault/vault.py` & `dedust-1.1.3/dedust/contracts/dex/vault/vault.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/dex/vault/vault_jetton.py` & `dedust-1.1.3/dedust/contracts/dex/vault/vault_jetton.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/dex/vault/vault_native.py` & `dedust-1.1.3/dedust/contracts/dex/vault/vault_native.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/jettons/jetton_root.py` & `dedust-1.1.3/dedust/contracts/jettons/jetton_root.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/dedust/contracts/jettons/jetton_wallet.py` & `dedust-1.1.3/dedust/contracts/jettons/jetton_wallet.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/examples/deposit_liquidity.py` & `dedust-1.1.3/examples/deposit_liquidity.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/examples/get_jetton_price.py` & `dedust-1.1.3/examples/get_jetton_price.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/examples/multihop.py` & `dedust-1.1.3/examples/multihop.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/examples/swap_jetton_to_ton.py` & `dedust-1.1.3/examples/swap_jetton_to_ton.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/examples/swap_ton_to_jetton.py` & `dedust-1.1.3/examples/swap_ton_to_jetton.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/examples/withdraw_liquidity.py` & `dedust-1.1.3/examples/withdraw_liquidity.py`

 * *Files identical despite different names*

### Comparing `dedust-1.1.2/PKG-INFO` & `dedust-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedust
-Version: 1.1.2
+Version: 1.1.3
 Summary: DeDust - DeDust SDK for Python.
 Author: Shibdev, Dalvpv
 Description-Content-Type: text/markdown
 Requires-Dist: httpx==0.19.0
 Requires-Dist: pytoniq>=0.1.19
 
 # DeDust SDK for Python
@@ -75,14 +75,16 @@
 ## Authors
 
 [@shibdev](https://t.me/dogpy)
 [@VladPavly](https://t.me/dalvpv)
 
 ## Version History
 
+* 1.1.3
+    * Bug fix
 * 1.1.2
     * Bug fix
 * 1.1.1
     * Bug fix
 * 1.1.0
     * Change tonsdk to pytoniq
 * 1.0.5
```

