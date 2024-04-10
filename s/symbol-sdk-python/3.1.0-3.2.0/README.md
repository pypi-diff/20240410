# Comparing `tmp/symbol_sdk_python-3.1.0.tar.gz` & `tmp/symbol_sdk_python-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol_sdk_python-3.1.0.tar", max compression
+gzip compressed data, was "symbol_sdk_python-3.2.0.tar", max compression
```

## Comparing `symbol_sdk_python-3.1.0.tar` & `symbol_sdk_python-3.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     4585 2023-08-07 15:06:24.834947 symbol_sdk_python-3.1.0/README.md
--rw-r--r--   0        0        0      842 2023-08-07 15:37:11.426322 symbol_sdk_python-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     2508 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/AccountDescriptorRepository.py
--rw-r--r--   0        0        0     3728 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/ArrayHelpers.py
--rw-r--r--   0        0        0     1482 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BaseValue.py
--rw-r--r--   0        0        0     1787 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Bip32.py
--rw-r--r--   0        0        0      723 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BlockchainSettings.py
--rw-r--r--   0        0        0      883 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BufferReader.py
--rw-r--r--   0        0        0      639 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BufferWriter.py
--rw-r--r--   0        0        0     1059 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/ByteArray.py
--rw-r--r--   0        0        0     2158 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Cipher.py
--rw-r--r--   0        0        0     1233 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/CodeWordsEncoder.py
--rw-r--r--   0        0        0     1844 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/CryptoTypes.py
--rw-r--r--   0        0        0     1848 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/DiceMnemonicGenerator.py
--rw-r--r--   0        0        0     3368 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Network.py
--rw-r--r--   0        0        0     1594 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/NetworkTimestamp.py
--rw-r--r--   0        0        0     1019 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/NodeDescriptorRepository.py
--rw-r--r--   0        0        0      397 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Ordered.py
--rw-r--r--   0        0        0     1606 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/PrivateKeyStorage.py
--rw-r--r--   0        0        0     1348 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/QrSignatureStorage.py
--rw-r--r--   0        0        0     1494 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/QrStorage.py
--rw-r--r--   0        0        0     4992 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/RuleBasedTransactionFactory.py
--rw-r--r--   0        0        0      593 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/SharedKey.py
--rw-r--r--   0        0        0     1806 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/TransactionDescriptorProcessor.py
--rw-r--r--   0        0        0      226 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Transforms.py
--rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/external/__init__.py
--rw-r--r--   0        0        0     7833 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/external/ed25519.py
--rw-r--r--   0        0        0     2983 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/BatchOperations.py
--rw-r--r--   0        0        0     2801 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/NemFacade.py
--rw-r--r--   0        0        0     4940 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/SymbolFacade.py
--rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/__init__.py
--rw-r--r--   0        0        0     2152 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/impl/CipherHelpers.py
--rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/impl/__init__.py
--rw-r--r--   0        0        0   178770 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nc/__init__.py
--rw-r--r--   0        0        0     3712 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/KeyPair.py
--rw-r--r--   0        0        0     2583 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/MessageEncoder.py
--rw-r--r--   0        0        0     1746 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/Network.py
--rw-r--r--   0        0        0     1094 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/SharedKey.py
--rw-r--r--   0        0        0     4017 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/TransactionFactory.py
--rw-r--r--   0        0        0        0 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/__init__.py
--rw-r--r--   0        0        0      378 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/ripemd160.py
--rw-r--r--   0        0        0   477679 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/sc/__init__.py
--rw-r--r--   0        0        0     1696 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/IdGenerator.py
--rw-r--r--   0        0        0     1506 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/KeyPair.py
--rw-r--r--   0        0        0     7243 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/Merkle.py
--rw-r--r--   0        0        0     3766 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/MessageEncoder.py
--rw-r--r--   0        0        0      567 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/Metadata.py
--rw-r--r--   0        0        0     2229 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/Network.py
--rw-r--r--   0        0        0      334 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/SharedKey.py
--rw-r--r--   0        0        0     3624 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/TransactionFactory.py
--rw-r--r--   0        0        0     1686 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/VotingKeysGenerator.py
--rw-r--r--   0        0        0        0 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/__init__.py
--rw-r--r--   0        0        0     5584 1970-01-01 00:00:00.000000 symbol_sdk_python-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4585 2024-04-10 01:40:59.424770 symbol_sdk_python-3.2.0/README.md
+-rw-r--r--   0        0        0      842 2024-04-10 01:44:54.079071 symbol_sdk_python-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2508 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/AccountDescriptorRepository.py
+-rw-r--r--   0        0        0     3728 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/ArrayHelpers.py
+-rw-r--r--   0        0        0     1482 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BaseValue.py
+-rw-r--r--   0        0        0     1787 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Bip32.py
+-rw-r--r--   0        0        0      723 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BlockchainSettings.py
+-rw-r--r--   0        0        0      883 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BufferReader.py
+-rw-r--r--   0        0        0      639 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BufferWriter.py
+-rw-r--r--   0        0        0     1059 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/ByteArray.py
+-rw-r--r--   0        0        0     2158 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Cipher.py
+-rw-r--r--   0        0        0     1233 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/CodeWordsEncoder.py
+-rw-r--r--   0        0        0     1844 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/CryptoTypes.py
+-rw-r--r--   0        0        0     1848 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/DiceMnemonicGenerator.py
+-rw-r--r--   0        0        0     3368 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Network.py
+-rw-r--r--   0        0        0     1595 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/NetworkTimestamp.py
+-rw-r--r--   0        0        0     1019 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/NodeDescriptorRepository.py
+-rw-r--r--   0        0        0      397 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Ordered.py
+-rw-r--r--   0        0        0     1606 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/PrivateKeyStorage.py
+-rw-r--r--   0        0        0     1348 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/QrSignatureStorage.py
+-rw-r--r--   0        0        0     1494 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/QrStorage.py
+-rw-r--r--   0        0        0     5101 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/RuleBasedTransactionFactory.py
+-rw-r--r--   0        0        0      593 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/SharedKey.py
+-rw-r--r--   0        0        0     1806 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/TransactionDescriptorProcessor.py
+-rw-r--r--   0        0        0      226 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/Transforms.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/external/__init__.py
+-rw-r--r--   0        0        0     7833 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/external/ed25519.py
+-rw-r--r--   0        0        0     2983 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/BatchOperations.py
+-rw-r--r--   0        0        0     2990 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/NemFacade.py
+-rw-r--r--   0        0        0     5128 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/SymbolFacade.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/__init__.py
+-rw-r--r--   0        0        0     2152 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/impl/CipherHelpers.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/impl/__init__.py
+-rw-r--r--   0        0        0   106403 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nc/__init__.py
+-rw-r--r--   0        0        0     3712 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/KeyPair.py
+-rw-r--r--   0        0        0     2583 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/MessageEncoder.py
+-rw-r--r--   0        0        0     1746 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/Network.py
+-rw-r--r--   0        0        0     1094 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/SharedKey.py
+-rw-r--r--   0        0        0     4017 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/TransactionFactory.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/__init__.py
+-rw-r--r--   0        0        0      378 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/ripemd160.py
+-rw-r--r--   0        0        0   286967 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/sc/__init__.py
+-rw-r--r--   0        0        0     1696 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/IdGenerator.py
+-rw-r--r--   0        0        0     1506 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/KeyPair.py
+-rw-r--r--   0        0        0     7243 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/Merkle.py
+-rw-r--r--   0        0        0     3766 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/MessageEncoder.py
+-rw-r--r--   0        0        0      567 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/Metadata.py
+-rw-r--r--   0        0        0     2229 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/Network.py
+-rw-r--r--   0        0        0      334 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/SharedKey.py
+-rw-r--r--   0        0        0     3624 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/TransactionFactory.py
+-rw-r--r--   0        0        0     1686 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/VotingKeysGenerator.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/__init__.py
+-rw-r--r--   0        0        0     5584 1970-01-01 00:00:00.000000 symbol_sdk_python-3.2.0/PKG-INFO
```

### Comparing `symbol_sdk_python-3.1.0/README.md` & `symbol_sdk_python-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/pyproject.toml` & `symbol_sdk_python-3.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'symbol-sdk-python'
-version = '3.1.0'
+version = '3.2.0'
 description = 'Symbol SDK'
 authors = ['Symbol Contributors <contributors@symbol.dev>']
 maintainers = ['Symbol Contributors <contributors@symbol.dev>']
 license = 'MIT'
 
 readme = 'README.md'
 
@@ -14,16 +14,16 @@
 
 keywords = ['symbol', 'sdk', 'Symbol SDK']
 
 classifiers = ['Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11']
 
 [tool.poetry.dependencies]
 python = "^3.9"
-cryptography = ">=41.0.3,<41.1.0"
+cryptography = ">=42.0.2,<42.1.0"
 mnemonic = ">=0.20,<1.0"
-pillow = ">=10.0.0,<10.1.0"
+pillow = ">=10.3.0,<10.4.0"
 pynacl = ">=1.5.0,<1.6.0"
 pyyaml = ">=6.0.1,<6.1.0"
 pyzbar = ">=0.1.9,<0.2.0"
 qrcode = ">=7.4.2,<7.5.0"
 ripemd-hash = ">=1.0.1,<1.1.0"
 safe-pysha3 = ">=1.0.4,<1.1.0"
```

### Comparing `symbol_sdk_python-3.1.0/symbolchain/AccountDescriptorRepository.py` & `symbol_sdk_python-3.2.0/symbolchain/AccountDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/ArrayHelpers.py` & `symbol_sdk_python-3.2.0/symbolchain/ArrayHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/BaseValue.py` & `symbol_sdk_python-3.2.0/symbolchain/BaseValue.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/Bip32.py` & `symbol_sdk_python-3.2.0/symbolchain/Bip32.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/BlockchainSettings.py` & `symbol_sdk_python-3.2.0/symbolchain/BlockchainSettings.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/BufferReader.py` & `symbol_sdk_python-3.2.0/symbolchain/BufferReader.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/BufferWriter.py` & `symbol_sdk_python-3.2.0/symbolchain/BufferWriter.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/ByteArray.py` & `symbol_sdk_python-3.2.0/symbolchain/ByteArray.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/Cipher.py` & `symbol_sdk_python-3.2.0/symbolchain/Cipher.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/CodeWordsEncoder.py` & `symbol_sdk_python-3.2.0/symbolchain/CodeWordsEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/CryptoTypes.py` & `symbol_sdk_python-3.2.0/symbolchain/CryptoTypes.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/DiceMnemonicGenerator.py` & `symbol_sdk_python-3.2.0/symbolchain/DiceMnemonicGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/Network.py` & `symbol_sdk_python-3.2.0/symbolchain/Network.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/NetworkTimestamp.py` & `symbol_sdk_python-3.2.0/symbolchain/NetworkTimestamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,8 +46,8 @@
 		return self.epoch + datetime.timedelta(**{self.time_units: raw_timestamp})
 
 	def to_difference(self, reference_datetime):
 		"""Subtracts the network epoch from the reference date."""
 		if reference_datetime < self.epoch:
 			raise ValueError('timestamp cannot be before epoch')
 
-		return (reference_datetime - self.epoch) / datetime.timedelta(**{self.time_units: 1})
+		return (reference_datetime - self.epoch) // datetime.timedelta(**{self.time_units: 1})
```

### Comparing `symbol_sdk_python-3.1.0/symbolchain/NodeDescriptorRepository.py` & `symbol_sdk_python-3.2.0/symbolchain/NodeDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/PrivateKeyStorage.py` & `symbol_sdk_python-3.2.0/symbolchain/PrivateKeyStorage.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/QrSignatureStorage.py` & `symbol_sdk_python-3.2.0/symbolchain/QrSignatureStorage.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/QrStorage.py` & `symbol_sdk_python-3.2.0/symbolchain/QrStorage.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/RuleBasedTransactionFactory.py` & `symbol_sdk_python-3.2.0/symbolchain/RuleBasedTransactionFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
 		self.rules[name] = lambda value: pod_class(value) if not isinstance(value, pod_class) else value
 
 	def add_flags_parser(self, name):
 		"""Creates flag type parser."""
 		flags_class = self._get_module_class(name)
 		string_to_enum = dict(map(lambda key: (key.name.lower(), key), flags_class))
+		string_to_enum['none'] = flags_class(0)  # automatically add none => 0 mapping (required for python 3.11+)
 
 		def parser(flags):
 			if isinstance(flags, str):
 				enum_array = list(map(lambda flag_name: _name_to_enum_value(string_to_enum, name, flag_name), flags.split(' ')))
 				return functools.reduce(operator.or_, enum_array)
 
 			if isinstance(flags, int):
```

### Comparing `symbol_sdk_python-3.1.0/symbolchain/SharedKey.py` & `symbol_sdk_python-3.2.0/symbolchain/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/TransactionDescriptorProcessor.py` & `symbol_sdk_python-3.2.0/symbolchain/TransactionDescriptorProcessor.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/external/ed25519.py` & `symbol_sdk_python-3.2.0/symbolchain/external/ed25519.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/facade/BatchOperations.py` & `symbol_sdk_python-3.2.0/symbolchain/facade/BatchOperations.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/facade/NemFacade.py` & `symbol_sdk_python-3.2.0/symbolchain/facade/NemFacade.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from datetime import datetime, timezone
+
 import sha3
 
 from ..CryptoTypes import Hash256, PrivateKey, PublicKey
 from ..nem.KeyPair import KeyPair, Verifier
 from ..nem.Network import Address, Network
 from ..nem.SharedKey import SharedKey
 from ..nem.TransactionFactory import TransactionFactory
@@ -36,14 +38,18 @@
 	@staticmethod
 	def _create_nem_type_to_property_mapping():
 		return {
 			Address: 'address',
 			PublicKey: 'public_key'
 		}
 
+	def now(self):
+		"""Creates a network timestamp representing the current time."""
+		return self.network.from_datetime(datetime.now(timezone.utc))
+
 	@staticmethod
 	def hash_transaction(transaction):
 		"""Hashes a NEM transaction."""
 		non_verifiable_transaction = TransactionFactory.to_non_verifiable_transaction(transaction)
 		return Hash256(sha3.keccak_256(non_verifiable_transaction.serialize()).digest())
 
 	@staticmethod
```

### Comparing `symbol_sdk_python-3.1.0/symbolchain/facade/SymbolFacade.py` & `symbol_sdk_python-3.2.0/symbolchain/facade/SymbolFacade.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import hashlib
+from datetime import datetime, timezone
 
 from .. import sc
 from ..CryptoTypes import Hash256, PublicKey, Signature
 from ..Network import NetworkLocator
 from ..symbol.KeyPair import KeyPair, Verifier
 from ..symbol.Merkle import MerkleHashBuilder
 from ..symbol.Network import Address, Network
@@ -54,14 +55,18 @@
 	@staticmethod
 	def _create_symbol_type_to_property_mapping():
 		return {
 			Address: 'address',
 			PublicKey: 'public_key',
 		}
 
+	def now(self):
+		"""Creates a network timestamp representing the current time."""
+		return self.network.from_datetime(datetime.now(timezone.utc))
+
 	def hash_transaction(self, transaction):
 		"""Hashes a Symbol transaction."""
 		hasher = hashlib.sha3_256()
 		hasher.update(transaction.signature.bytes)
 		hasher.update(transaction.signer_public_key.bytes)
 		hasher.update(self.network.generation_hash_seed.bytes)
 		hasher.update(self._transaction_data_buffer(transaction.serialize()))
```

### Comparing `symbol_sdk_python-3.1.0/symbolchain/impl/CipherHelpers.py` & `symbol_sdk_python-3.2.0/symbolchain/impl/CipherHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/nem/KeyPair.py` & `symbol_sdk_python-3.2.0/symbolchain/nem/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/nem/MessageEncoder.py` & `symbol_sdk_python-3.2.0/symbolchain/nem/MessageEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/nem/Network.py` & `symbol_sdk_python-3.2.0/symbolchain/nem/Network.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/nem/SharedKey.py` & `symbol_sdk_python-3.2.0/symbolchain/nem/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/nem/TransactionFactory.py` & `symbol_sdk_python-3.2.0/symbolchain/nem/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/IdGenerator.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/IdGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/KeyPair.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/Merkle.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/Merkle.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/MessageEncoder.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/MessageEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/Metadata.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/Metadata.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/Network.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/Network.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/TransactionFactory.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/symbolchain/symbol/VotingKeysGenerator.py` & `symbol_sdk_python-3.2.0/symbolchain/symbol/VotingKeysGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.1.0/PKG-INFO` & `symbol_sdk_python-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: symbol-sdk-python
-Version: 3.1.0
+Version: 3.2.0
 Summary: Symbol SDK
 Home-page: https://github.com/symbol/symbol/tree/main/sdk/python
 License: MIT
 Keywords: symbol,sdk,Symbol SDK
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
 Maintainer-email: contributors@symbol.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=41.0.3,<41.1.0)
+Requires-Dist: cryptography (>=42.0.2,<42.1.0)
 Requires-Dist: mnemonic (>=0.20,<1.0)
-Requires-Dist: pillow (>=10.0.0,<10.1.0)
+Requires-Dist: pillow (>=10.3.0,<10.4.0)
 Requires-Dist: pynacl (>=1.5.0,<1.6.0)
 Requires-Dist: pyyaml (>=6.0.1,<6.1.0)
 Requires-Dist: pyzbar (>=0.1.9,<0.2.0)
 Requires-Dist: qrcode (>=7.4.2,<7.5.0)
 Requires-Dist: ripemd-hash (>=1.0.1,<1.1.0)
 Requires-Dist: safe-pysha3 (>=1.0.4,<1.1.0)
 Project-URL: Repository, https://github.com/symbol/symbol/tree/main/sdk/python
```

