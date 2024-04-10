# Comparing `tmp/pyckb-0.1.7.tar.gz` & `tmp/pyckb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyckb-0.1.7.tar", last modified: Mon Jan 22 11:33:12 2024, max compression
+gzip compressed data, was "pyckb-0.1.8.tar", last modified: Wed Apr 10 07:01:22 2024, max compression
```

## Comparing `pyckb-0.1.7.tar` & `pyckb-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 11:33:12.235537 pyckb-0.1.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.1.7/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2024-01-22 11:33:12.235537 pyckb-0.1.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1582 2024-01-10 08:40:52.000000 pyckb-0.1.7/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 11:33:12.231537 pyckb-0.1.7/ckb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2024-01-19 12:10:21.000000 pyckb-0.1.7/ckb/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4369 2023-12-30 06:34:14.000000 pyckb-0.1.7/ckb/bech32.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-01-19 12:16:39.000000 pyckb-0.1.7/ckb/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17356 2024-01-22 11:27:36.000000 pyckb-0.1.7/ckb/core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2024-01-22 07:26:45.000000 pyckb-0.1.7/ckb/ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3833 2024-01-22 11:27:41.000000 pyckb-0.1.7/ckb/molecule.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4413 2024-01-19 03:18:32.000000 pyckb-0.1.7/ckb/rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4268 2024-01-12 02:06:10.000000 pyckb-0.1.7/ckb/secp256k1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23642 2024-01-04 08:04:46.000000 pyckb-0.1.7/ckb/wallet.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 11:33:12.235537 pyckb-0.1.7/pyckb.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2024-01-22 11:33:12.000000 pyckb-0.1.7/pyckb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      377 2024-01-22 11:33:12.000000 pyckb-0.1.7/pyckb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-22 11:33:12.000000 pyckb-0.1.7/pyckb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-01-22 11:33:12.000000 pyckb-0.1.7/pyckb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-01-22 11:33:12.000000 pyckb-0.1.7/pyckb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-01-22 11:32:33.000000 pyckb-0.1.7/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-22 11:33:12.235537 pyckb-0.1.7/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 11:33:12.235537 pyckb-0.1.7/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2279 2024-01-22 07:24:50.000000 pyckb-0.1.7/test/test_core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.1.7/test/test_ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-12-28 09:23:55.000000 pyckb-0.1.7/test/test_rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-12-30 05:46:36.000000 pyckb-0.1.7/test/test_wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.492136 pyckb-0.1.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.1.8/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-10 07:01:22.492136 pyckb-0.1.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2024-04-10 03:25:41.000000 pyckb-0.1.8/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.488136 pyckb-0.1.8/ckb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2024-02-26 07:22:12.000000 pyckb-0.1.8/ckb/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4369 2023-12-30 06:34:14.000000 pyckb-0.1.8/ckb/bech32.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-04-09 03:33:20.000000 pyckb-0.1.8/ckb/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17356 2024-01-22 11:27:36.000000 pyckb-0.1.8/ckb/core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2024-01-22 07:26:45.000000 pyckb-0.1.8/ckb/ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3833 2024-01-22 11:27:41.000000 pyckb-0.1.8/ckb/molecule.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4413 2024-01-19 03:18:32.000000 pyckb-0.1.8/ckb/rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4268 2024-01-12 02:06:10.000000 pyckb-0.1.8/ckb/secp256k1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23788 2024-01-31 03:11:03.000000 pyckb-0.1.8/ckb/wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.492136 pyckb-0.1.8/pyckb.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      377 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-04-10 06:59:09.000000 pyckb-0.1.8/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-10 07:01:22.492136 pyckb-0.1.8/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.492136 pyckb-0.1.8/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2254 2024-03-21 07:26:46.000000 pyckb-0.1.8/test/test_core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.1.8/test/test_ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-12-28 09:23:55.000000 pyckb-0.1.8/test/test_rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1791 2024-04-09 03:55:53.000000 pyckb-0.1.8/test/test_wallet.py
```

### Comparing `pyckb-0.1.7/LICENSE` & `pyckb-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/README.md` & `pyckb-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,53 +7,91 @@
 - No third-party dependencies. All code is visible.
 - Incredibly simple.
 
 ## Installation
 
 ```sh
 $ python -m pip install pyckb
+# or
+$ git clone https://github.com/mohanson/pyckb
+$ cd pyckb
+$ python -m pip install --editable . --config-settings editable_mode=strict
 ```
 
 ## Usage
 
-By default, pyckb is configured on the testnet. To switch networks, see `ckb.config`.
+By default, pyckb is configured on the develop. To switch networks, see `ckb.config`.
+
+**example/addr.py**
+
+Calculate address from private key in secp256k1 lock.
+
+```sh
+$ python example/addr.py --prikey 0x0000000000000000000000000000000000000000000000000000000000000001
+
+# ckt1qzda0cr08m85hc8jlnfp3zer7xulejywt49kt2rr0vthywaa50xwsqt4z78ng4yutl5u6xsv27ht6q08mhujf8s2r0n40
+```
+
+**example/capacity.py**
+
+Get the capacity by an address.
+
+```sh
+$ python example/capacity.py --addr ckt1qzda0cr08m85hc8jlnfp3zer7xulejywt49kt2rr0vthywaa50xwsqt4z78ng4yutl5u6xsv27ht6q08mhujf8s2r0n40
+
+# 3523312.39054609
+```
 
 **example/deploy.py**
 
 Deploy a script to the chain.
 
 ```sh
-$ python example/deploy.py LICENSE
+$ python example/deploy.py --prikey 0x0000000000000000000000000000000000000000000000000000000000000001 --file LICENSE
 
-script.code_hash = 0x1a124d54d4f37713b8f17fc12142ede488906d4290fbb178d7aad214977814ee
-script.hash_type = 2(data1)
-out_point.hash   = 0x418f60d67ff3e9841a3091c55cb4eb50837602582495931c372fff99f3107f38
-out_point.index  = 0
+# script.code_hash = 0x1a124d54d4f37713b8f17fc12142ede488906d4290fbb178d7aad214977814ee
+# script.hash_type = 2(data1)
+# out_point.hash   = 0x418f60d67ff3e9841a3091c55cb4eb50837602582495931c372fff99f3107f38
+# out_point.index  = 0
 ```
 
 **example/faucet.py**
 
-One faucet to send 300000 CKB to any ckb addresses. The script execution takes 2 blocks, which is about 20 seconds.
+One faucet to send 300000 CKB to any ckb addresses. Note this only takes effect on the testnet.
 
 ```sh
-$ python example/faucet.py ckt1qzda0cr08m85hc8jlnfp3zer7xulejywt49kt2rr0vthywaa50xwsqt4z78ng4yutl5u6xsv27ht6q08mhujf8s2r0n40
+$ python example/faucet.py --addr ckt1qzda0cr08m85hc8jlnfp3zer7xulejywt49kt2rr0vthywaa50xwsqt4z78ng4yutl5u6xsv27ht6q08mhujf8s2r0n40
 ```
 
 **example/redeem.py**
 
 Attempt to withdraw all funds from Dao. When running the test case of pyckb by `pytest -v`, a part of ckb will be locked in Dao. Use this script to recover this part of the funds.
 
 ```sh
-$ python example/redeem.py
+$ python example/redeem.py --prikey 0x0000000000000000000000000000000000000000000000000000000000000001
 ```
 
 **example/txdump.py**
 
-Dump full transaction data for [ckb-debugger](https://github.com/nervosnetwork/ckb-standalone-debugger) to use.
+Dump full transaction data for ckb-debugger to use.
+
+```sh
+$ python example/txdump.py --net testnet --hash 0x123b09a89e65cc9c375dab739c9c921f7067d0b205e563135bb5a1221f8948d9
+```
+
+## Test
 
 ```sh
-$ python example/txdump.py -x 0x123b09a89e65cc9c375dab739c9c921f7067d0b205e563135bb5a1221f8948d9
+$ wget https://github.com/nervosnetwork/ckb/releases/download/v0.115.0/ckb_v0.115.0_x86_64-unknown-linux-gnu.tar.gz
+$ tar -zxvf ckb_v0.115.0_x86_64-unknown-linux-gnu.tar.gz
+$ cd ckb_v0.115.0_x86_64-unknown-linux-gnu/
+
+$ ckb init --chain dev --ba-arg 0x75178f34549c5fe9cd1a0c57aebd01e7ddf9249e --ba-message 0xabcd
+$ ckb run --indexer
+$ ckb miner
+
+$ pytest -v
 ```
 
 ## License
 
 MIT
```

### Comparing `pyckb-0.1.7/ckb/bech32.py` & `pyckb-0.1.8/ckb/bech32.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/ckb/config.py` & `pyckb-0.1.8/ckb/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,8 +112,8 @@
     })
     t = r.json()['result']['transactions']
     develop.url = url
     develop.script.dao.cell_dep.out_point.tx_hash = bytearray.fromhex(t[0]['hash'][2:])
     develop.script.secp256k1_blake160.cell_dep.out_point.tx_hash = bytearray.fromhex(t[1]['hash'][2:])
 
 
-current = testnet
+current = develop
```

### Comparing `pyckb-0.1.7/ckb/core.py` & `pyckb-0.1.8/ckb/core.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/ckb/ecdsa.py` & `pyckb-0.1.8/ckb/ecdsa.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/ckb/molecule.py` & `pyckb-0.1.8/ckb/molecule.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/ckb/rpc.py` & `pyckb-0.1.8/ckb/rpc.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/ckb/secp256k1.py` & `pyckb-0.1.8/ckb/secp256k1.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/ckb/wallet.py` & `pyckb-0.1.8/ckb/wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,17 @@
             result = ckb.rpc.get_transaction('0x' + out_point.tx_hash.hex())
             origin = ckb.core.CellOutput.json_read(result['transaction']['outputs'][out_point.index])
             sender_capacity += origin.capacity
         for e in self.tx.raw.outputs:
             output_capacity += e.capacity
         assert sender_capacity - output_capacity <= 1 * ckb.core.shannon
 
+    def analyze_outputs_data(self):
+        assert len(self.tx.raw.outputs) == len(self.tx.raw.outputs_data)
+
     def analyze_since(self):
         # Transaction since precondition
         # See https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0017-tx-valid-since/0017-tx-valid-since.md
         for e in self.tx.raw.inputs:
             if e.since == 0:
                 continue
             if e.since >> 56 == 0x00:
@@ -45,14 +48,15 @@
             if e.since >> 56 == 0xa0:
                 pass
             if e.since >> 56 == 0xe0:
                 pass
 
     def analyze(self):
         self.analyze_mining_fee()
+        self.analyze_outputs_data()
         self.analyze_since()
 
 
 class Wallet:
     def __init__(self, prikey: int):
         self.prikey = ckb.core.PriKey(prikey)
         self.pubkey = self.prikey.pubkey()
```

### Comparing `pyckb-0.1.7/test/test_core.py` & `pyckb-0.1.8/test/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import ckb
 
 
 def test_addr():
     prikey = ckb.core.PriKey(1)
     pubkey = prikey.pubkey()
-    args = ckb.core.hash(pubkey.molecule())[:20].hex()
+    args = ckb.core.hash(pubkey.molecule())[:20]
     script = ckb.core.Script(
         ckb.config.current.script.secp256k1_blake160.code_hash,
         ckb.config.current.script.secp256k1_blake160.hash_type,
-        bytearray.fromhex(args)
+        args
     )
     addr = ckb.core.address_encode(script)
     assert addr == 'ckt1qzda0cr08m85hc8jlnfp3zer7xulejywt49kt2rr0vthywaa50xwsqt4z78ng4yutl5u6xsv27ht6q08mhujf8s2r0n40'
     assert ckb.core.address_decode(addr) == script
     assert script.hash().hex() == '0b1bae4beaf456349c63c3ce67491fc75a1276d7f9eedd7ea84d6a77f9f3f5f7'
     assert ckb.core.Script.molecule_read(script.molecule()) == script
```

### Comparing `pyckb-0.1.7/test/test_ecdsa.py` & `pyckb-0.1.8/test/test_ecdsa.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.7/test/test_rpc.py` & `pyckb-0.1.8/test/test_rpc.py`

 * *Files identical despite different names*

