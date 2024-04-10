# Comparing `tmp/apibara-0.7.5.tar.gz` & `tmp/apibara-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibara-0.7.5.tar", max compression
+gzip compressed data, was "apibara-0.8.0.tar", max compression
```

## Comparing `apibara-0.7.5.tar` & `apibara-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.5/LICENSE.txt
--rw-r--r--   0        0        0     1685 2023-07-24 14:46:53.473584 apibara-0.7.5/README.rst
--rw-r--r--   0        0        0     1268 2023-11-15 13:35:08.982422 apibara-0.7.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 16:15:25.550565 apibara-0.7.5/src/apibara/__init__.py
--rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.5/src/apibara/cursor.py
--rw-r--r--   0        0        0      211 2023-08-28 12:47:19.675051 apibara-0.7.5/src/apibara/indexer/__init__.py
--rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.5/src/apibara/indexer/configuration.py
--rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.5/src/apibara/indexer/indexer.py
--rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.5/src/apibara/indexer/info.py
--rw-r--r--   0        0        0    12882 2023-11-15 13:26:50.516229 apibara-0.7.5/src/apibara/indexer/runner.py
--rw-r--r--   0        0        0    10751 2023-11-15 13:26:50.527229 apibara-0.7.5/src/apibara/indexer/storage.py
--rw-r--r--   0        0        0      687 2023-07-24 14:46:53.473584 apibara-0.7.5/src/apibara/protocol/__init__.py
--rw-r--r--   0        0        0     4424 2023-11-15 11:03:41.558570 apibara-0.7.5/src/apibara/protocol/client.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/protocol/proto/__init__.py
--rw-r--r--   0        0        0     3450 2023-08-01 21:01:03.928913 apibara-0.7.5/src/apibara/protocol/proto/stream_pb2.py
--rw-r--r--   0        0        0     3608 2023-08-01 19:15:20.623565 apibara-0.7.5/src/apibara/protocol/proto/stream_pb2.pyi
--rw-r--r--   0        0        0     4147 2023-08-01 21:00:10.094174 apibara-0.7.5/src/apibara/protocol/proto/stream_pb2_grpc.py
--rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/protocol/proto/stream_pb2_grpc.pyi
--rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/__init__.py
--rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/cursor.py
--rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/felt.py
--rw-r--r--   0        0        0    15182 2023-11-15 11:48:58.048523 apibara-0.7.5/src/apibara/starknet/filter.py
--rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/indexer.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/proto/__init__.py
--rw-r--r--   0        0        0     8213 2023-11-15 12:00:51.597413 apibara-0.7.5/src/apibara/starknet/proto/filter_pb2.py
--rw-r--r--   0        0        0    13536 2023-11-15 11:48:58.049523 apibara-0.7.5/src/apibara/starknet/proto/filter_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/proto/filter_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/proto/filter_pb2_grpc.pyi
--rw-r--r--   0        0        0    12133 2023-11-15 12:00:29.481107 apibara-0.7.5/src/apibara/starknet/proto/starknet_pb2.py
--rw-r--r--   0        0        0    20617 2023-11-15 11:48:58.049523 apibara-0.7.5/src/apibara/starknet/proto/starknet_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/proto/starknet_pb2_grpc.py
--rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1095 2023-11-15 11:59:52.408593 apibara-0.7.5/src/apibara/starknet/proto/types_pb2.py
--rw-r--r--   0        0        0      732 2023-11-15 11:48:58.049523 apibara-0.7.5/src/apibara/starknet/proto/types_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/proto/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.5/src/apibara/starknet/proto/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2751 1970-01-01 00:00:00.000000 apibara-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-14 13:34:33.730740 apibara-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     1685 2024-03-14 13:34:33.730740 apibara-0.8.0/README.rst
+-rw-r--r--   0        0        0     1258 2024-04-10 12:08:20.614189 apibara-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/__init__.py
+-rw-r--r--   0        0        0      514 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/cursor.py
+-rw-r--r--   0        0        0      211 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/indexer/__init__.py
+-rw-r--r--   0        0        0      375 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/indexer/configuration.py
+-rw-r--r--   0        0        0     2393 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/indexer/indexer.py
+-rw-r--r--   0        0        0     1026 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/indexer/info.py
+-rw-r--r--   0        0        0    12882 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/indexer/runner.py
+-rw-r--r--   0        0        0    10751 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/indexer/storage.py
+-rw-r--r--   0        0        0      633 2024-04-10 11:55:50.757928 apibara-0.8.0/src/apibara/protocol/__init__.py
+-rw-r--r--   0        0        0     4424 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/protocol/client.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:34:33.731740 apibara-0.8.0/src/apibara/protocol/proto/__init__.py
+-rw-r--r--   0        0        0     3450 2024-04-10 12:07:53.135825 apibara-0.8.0/src/apibara/protocol/proto/stream_pb2.py
+-rw-r--r--   0        0        0     3560 2024-04-10 12:02:52.674708 apibara-0.8.0/src/apibara/protocol/proto/stream_pb2.pyi
+-rw-r--r--   0        0        0     4147 2024-04-10 12:04:23.749970 apibara-0.8.0/src/apibara/protocol/proto/stream_pb2_grpc.py
+-rw-r--r--   0        0        0      878 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/protocol/proto/stream_pb2_grpc.pyi
+-rw-r--r--   0        0        0      264 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/__init__.py
+-rw-r--r--   0        0        0     1038 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/cursor.py
+-rw-r--r--   0        0        0     1375 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/felt.py
+-rw-r--r--   0        0        0    15182 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/filter.py
+-rw-r--r--   0        0        0      404 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/indexer.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/proto/__init__.py
+-rw-r--r--   0        0        0     8664 2024-04-10 12:07:53.152825 apibara-0.8.0/src/apibara/starknet/proto/filter_pb2.py
+-rw-r--r--   0        0        0    13488 2024-04-10 12:02:52.863710 apibara-0.8.0/src/apibara/starknet/proto/filter_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/proto/filter_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/proto/filter_pb2_grpc.pyi
+-rw-r--r--   0        0        0    19170 2024-04-10 12:07:53.193826 apibara-0.8.0/src/apibara/starknet/proto/starknet_pb2.py
+-rw-r--r--   0        0        0    32899 2024-04-10 12:02:53.237715 apibara-0.8.0/src/apibara/starknet/proto/starknet_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/proto/starknet_pb2_grpc.py
+-rw-r--r--   0        0        0      100 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1138 2024-04-10 12:07:53.092825 apibara-0.8.0/src/apibara/starknet/proto/types_pb2.py
+-rw-r--r--   0        0        0      713 2024-04-10 12:02:52.614707 apibara-0.8.0/src/apibara/starknet/proto/types_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/proto/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-03-14 13:34:33.732740 apibara-0.8.0/src/apibara/starknet/proto/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 apibara-0.8.0/PKG-INFO
```

### Comparing `apibara-0.7.5/LICENSE.txt` & `apibara-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/README.rst` & `apibara-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/pyproject.toml` & `apibara-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 [tool.poetry]
 name = "apibara"
-version = "0.7.5"
+version = "0.8.0"
 description = "Apibara cliend SDK. Stream and transform on-chain data with Python."
 authors = ["Francesco Ceccon <francesco@apibara.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://www.apibara.com"
-repository= "https://github.com/apibara/python-sdk"
-keywords = [
-    "ethereum",
-    "web3",
-    "starknet"
-]
+repository = "https://github.com/apibara/python-sdk"
+keywords = ["ethereum", "web3", "starknet"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.13"
 grpcio = ">=1.50,<2.0"
 protobuf = ">=4.20,<5"
 pymongo = "^4.3.3"
 
 [tool.poetry.extras]
 indexer = ["pymongo"]
 
@@ -34,15 +30,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 black = "^22.12.0"
 isort = "^5.11.4"
 pytest-asyncio = "^0.20.3"
 grpcio-tools = ">=1.50,<2.0"
-testcontainers = {extras = ["mongodb"], version = "^3.7.1"}
+testcontainers = { extras = ["mongodb"], version = "^3.7.1" }
 
 [tool.black]
 line-length = 88
 target-version = ['py38', 'py39', 'py310']
 
 [tool.isort]
 profile = "black"
```

### Comparing `apibara-0.7.5/src/apibara/cursor.py` & `apibara-0.8.0/src/apibara/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/indexer/indexer.py` & `apibara-0.8.0/src/apibara/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/indexer/info.py` & `apibara-0.8.0/src/apibara/indexer/info.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/indexer/runner.py` & `apibara-0.8.0/src/apibara/indexer/runner.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/indexer/storage.py` & `apibara-0.8.0/src/apibara/indexer/storage.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/protocol/__init__.py` & `apibara-0.8.0/src/apibara/protocol/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     StreamDataResponse,
 )
 
 
 @dataclass
 class StarkNetStreamAddress:
     Mainnet: ClassVar[str] = "mainnet.starknet.a5a.ch"
-    Goerli: ClassVar[str] = "goerli.starknet.a5a.ch"
-    Goerli2: ClassVar[str] = "goerli-2.starknet.a5a.ch"
+    Sepolia: ClassVar[str] = "sepolia.starknet.a5a.ch"
 
 
 @dataclass
 class StreamAddress:
     """Defines well-known addresses for the Apibara Stream service."""
 
     StarkNet: ClassVar[StarkNetStreamAddress] = StarkNetStreamAddress
```

### Comparing `apibara-0.7.5/src/apibara/protocol/client.py` & `apibara-0.8.0/src/apibara/protocol/client.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/protocol/proto/stream_pb2.py` & `apibara-0.8.0/src/apibara/protocol/proto/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/protocol/proto/stream_pb2.pyi` & `apibara-0.8.0/src/apibara/protocol/proto/stream_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import ClassVar as _ClassVar
-from typing import Iterable as _Iterable
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import (
+    ClassVar as _ClassVar,
+    Iterable as _Iterable,
+    Mapping as _Mapping,
+    Optional as _Optional,
+    Union as _Union,
+)
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DataFinality(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
     DATA_STATUS_UNKNOWN: _ClassVar[DataFinality]
     DATA_STATUS_PENDING: _ClassVar[DataFinality]
```

### Comparing `apibara-0.7.5/src/apibara/protocol/proto/stream_pb2_grpc.py` & `apibara-0.8.0/src/apibara/protocol/proto/stream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/protocol/proto/stream_pb2_grpc.pyi` & `apibara-0.8.0/src/apibara/protocol/proto/stream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/starknet/cursor.py` & `apibara-0.8.0/src/apibara/starknet/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/starknet/felt.py` & `apibara-0.8.0/src/apibara/starknet/felt.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/starknet/filter.py` & `apibara-0.8.0/src/apibara/starknet/filter.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.5/src/apibara/starknet/proto/filter_pb2.py` & `apibara-0.8.0/src/apibara/starknet/proto/filter_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,48 +11,49 @@
 
 _sym_db = _symbol_database.Default()
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b"\n\x0c\x66ilter.proto\x12\x19\x61pibara.starknet.v1alpha2\x1a\x0btypes.proto\"\xc3\x02\n\x06\x46ilter\x12\x37\n\x06header\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.HeaderFilter\x12\x42\n\x0ctransactions\x18\x02 \x03(\x0b\x32,.apibara.starknet.v1alpha2.TransactionFilter\x12\x42\n\x0cstate_update\x18\x03 \x01(\x0b\x32,.apibara.starknet.v1alpha2.StateUpdateFilter\x12\x36\n\x06\x65vents\x18\x04 \x03(\x0b\x32&.apibara.starknet.v1alpha2.EventFilter\x12@\n\x08messages\x18\x05 \x03(\x0b\x32..apibara.starknet.v1alpha2.L2ToL1MessageFilter\"\x1c\n\x0cHeaderFilter\x12\x0c\n\x04weak\x18\x01 \x01(\x08\"\xfd\x03\n\x11TransactionFilter\x12I\n\tinvoke_v0\x18\x01 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV0FilterH\x00\x12I\n\tinvoke_v1\x18\x02 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV1FilterH\x00\x12\x44\n\x06\x64\x65ploy\x18\x03 \x01(\x0b\x32\x32.apibara.starknet.v1alpha2.DeployTransactionFilterH\x00\x12\x46\n\x07\x64\x65\x63lare\x18\x04 \x01(\x0b\x32\x33.apibara.starknet.v1alpha2.DeclareTransactionFilterH\x00\x12K\n\nl1_handler\x18\x05 \x01(\x0b\x32\x35.apibara.starknet.v1alpha2.L1HandlerTransactionFilterH\x00\x12S\n\x0e\x64\x65ploy_account\x18\x06 \x01(\x0b\x32\x39.apibara.starknet.v1alpha2.DeployAccountTransactionFilterH\x00\x12\x18\n\x10include_reverted\x18\x07 \x01(\x08\x42\x08\n\x06\x66ilter\"\xe0\x01\n\x19InvokeTransactionV0Filter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x97\x01\n\x19InvokeTransactionV1Filter\x12?\n\x0esender_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe5\x01\n\x17\x44\x65ployTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x18\x44\x65\x63lareTransactionFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12?\n\x0esender_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe1\x01\n\x1aL1HandlerTransactionFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xec\x01\n\x1e\x44\x65ployAccountTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xa6\x01\n\x13L2ToL1MessageFilter\x12;\n\nto_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07payload\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x18\n\x10include_reverted\x18\x03 \x01(\x08\"\xda\x02\n\x0b\x45ventFilter\x12=\n\x0c\x66rom_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04keys\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x1d\n\x10include_reverted\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12 \n\x13include_transaction\x18\x05 \x01(\x08H\x01\x88\x01\x01\x12\x1c\n\x0finclude_receipt\x18\x06 \x01(\x08H\x02\x88\x01\x01\x42\x13\n\x11_include_revertedB\x16\n\x14_include_transactionB\x12\n\x10_include_receipt\"\xc8\x03\n\x11StateUpdateFilter\x12\x43\n\rstorage_diffs\x18\x01 \x03(\x0b\x32,.apibara.starknet.v1alpha2.StorageDiffFilter\x12M\n\x12\x64\x65\x63lared_contracts\x18\x02 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeclaredContractFilter\x12M\n\x12\x64\x65ployed_contracts\x18\x03 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeployedContractFilter\x12<\n\x06nonces\x18\x04 \x03(\x0b\x32,.apibara.starknet.v1alpha2.NonceUpdateFilter\x12H\n\x10\x64\x65\x63lared_classes\x18\x05 \x03(\x0b\x32..apibara.starknet.v1alpha2.DeclaredClassFilter\x12H\n\x10replaced_classes\x18\x06 \x03(\x0b\x32..apibara.starknet.v1alpha2.ReplacedClassFilter\"V\n\x11StorageDiffFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"U\n\x16\x44\x65\x63laredContractFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x13\x44\x65\x63laredClassFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x44\n\x13\x63ompiled_class_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x95\x01\n\x13ReplacedClassFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x16\x44\x65ployedContractFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8e\x01\n\x11NonceUpdateFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElementb\x06proto3"
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "filter_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "filter_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _FILTER._serialized_start = 57
-    _FILTER._serialized_end = 380
-    _HEADERFILTER._serialized_start = 382
-    _HEADERFILTER._serialized_end = 410
-    _TRANSACTIONFILTER._serialized_start = 413
-    _TRANSACTIONFILTER._serialized_end = 922
-    _INVOKETRANSACTIONV0FILTER._serialized_start = 925
-    _INVOKETRANSACTIONV0FILTER._serialized_end = 1149
-    _INVOKETRANSACTIONV1FILTER._serialized_start = 1152
-    _INVOKETRANSACTIONV1FILTER._serialized_end = 1303
-    _DEPLOYTRANSACTIONFILTER._serialized_start = 1306
-    _DEPLOYTRANSACTIONFILTER._serialized_end = 1535
-    _DECLARETRANSACTIONFILTER._serialized_start = 1538
-    _DECLARETRANSACTIONFILTER._serialized_end = 1690
-    _L1HANDLERTRANSACTIONFILTER._serialized_start = 1693
-    _L1HANDLERTRANSACTIONFILTER._serialized_end = 1918
-    _DEPLOYACCOUNTTRANSACTIONFILTER._serialized_start = 1921
-    _DEPLOYACCOUNTTRANSACTIONFILTER._serialized_end = 2157
-    _L2TOL1MESSAGEFILTER._serialized_start = 2160
-    _L2TOL1MESSAGEFILTER._serialized_end = 2326
-    _EVENTFILTER._serialized_start = 2329
-    _EVENTFILTER._serialized_end = 2675
-    _STATEUPDATEFILTER._serialized_start = 2678
-    _STATEUPDATEFILTER._serialized_end = 3134
-    _STORAGEDIFFFILTER._serialized_start = 3136
-    _STORAGEDIFFFILTER._serialized_end = 3222
-    _DECLAREDCONTRACTFILTER._serialized_start = 3224
-    _DECLAREDCONTRACTFILTER._serialized_end = 3309
-    _DECLAREDCLASSFILTER._serialized_start = 3312
-    _DECLAREDCLASSFILTER._serialized_end = 3464
-    _REPLACEDCLASSFILTER._serialized_start = 3467
-    _REPLACEDCLASSFILTER._serialized_end = 3616
-    _DEPLOYEDCONTRACTFILTER._serialized_start = 3619
-    _DEPLOYEDCONTRACTFILTER._serialized_end = 3771
-    _NONCEUPDATEFILTER._serialized_start = 3774
-    _NONCEUPDATEFILTER._serialized_end = 3916
+    _globals["_FILTER"]._serialized_start = 57
+    _globals["_FILTER"]._serialized_end = 380
+    _globals["_HEADERFILTER"]._serialized_start = 382
+    _globals["_HEADERFILTER"]._serialized_end = 410
+    _globals["_TRANSACTIONFILTER"]._serialized_start = 413
+    _globals["_TRANSACTIONFILTER"]._serialized_end = 922
+    _globals["_INVOKETRANSACTIONV0FILTER"]._serialized_start = 925
+    _globals["_INVOKETRANSACTIONV0FILTER"]._serialized_end = 1149
+    _globals["_INVOKETRANSACTIONV1FILTER"]._serialized_start = 1152
+    _globals["_INVOKETRANSACTIONV1FILTER"]._serialized_end = 1303
+    _globals["_DEPLOYTRANSACTIONFILTER"]._serialized_start = 1306
+    _globals["_DEPLOYTRANSACTIONFILTER"]._serialized_end = 1535
+    _globals["_DECLARETRANSACTIONFILTER"]._serialized_start = 1538
+    _globals["_DECLARETRANSACTIONFILTER"]._serialized_end = 1690
+    _globals["_L1HANDLERTRANSACTIONFILTER"]._serialized_start = 1693
+    _globals["_L1HANDLERTRANSACTIONFILTER"]._serialized_end = 1918
+    _globals["_DEPLOYACCOUNTTRANSACTIONFILTER"]._serialized_start = 1921
+    _globals["_DEPLOYACCOUNTTRANSACTIONFILTER"]._serialized_end = 2157
+    _globals["_L2TOL1MESSAGEFILTER"]._serialized_start = 2160
+    _globals["_L2TOL1MESSAGEFILTER"]._serialized_end = 2326
+    _globals["_EVENTFILTER"]._serialized_start = 2329
+    _globals["_EVENTFILTER"]._serialized_end = 2675
+    _globals["_STATEUPDATEFILTER"]._serialized_start = 2678
+    _globals["_STATEUPDATEFILTER"]._serialized_end = 3134
+    _globals["_STORAGEDIFFFILTER"]._serialized_start = 3136
+    _globals["_STORAGEDIFFFILTER"]._serialized_end = 3222
+    _globals["_DECLAREDCONTRACTFILTER"]._serialized_start = 3224
+    _globals["_DECLAREDCONTRACTFILTER"]._serialized_end = 3309
+    _globals["_DECLAREDCLASSFILTER"]._serialized_start = 3312
+    _globals["_DECLAREDCLASSFILTER"]._serialized_end = 3464
+    _globals["_REPLACEDCLASSFILTER"]._serialized_start = 3467
+    _globals["_REPLACEDCLASSFILTER"]._serialized_end = 3616
+    _globals["_DEPLOYEDCONTRACTFILTER"]._serialized_start = 3619
+    _globals["_DEPLOYEDCONTRACTFILTER"]._serialized_end = 3771
+    _globals["_NONCEUPDATEFILTER"]._serialized_start = 3774
+    _globals["_NONCEUPDATEFILTER"]._serialized_end = 3916
 # @@protoc_insertion_point(module_scope)
```

### Comparing `apibara-0.7.5/src/apibara/starknet/proto/filter_pb2.pyi` & `apibara-0.8.0/src/apibara/starknet/proto/filter_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,274 +1,256 @@
-from typing import ClassVar as _ClassVar
-from typing import Iterable as _Iterable
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
 import types_pb2 as _types_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf.internal import containers as _containers
+from typing import (
+    ClassVar as _ClassVar,
+    Iterable as _Iterable,
+    Mapping as _Mapping,
+    Optional as _Optional,
+    Union as _Union,
+)
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeclareTransactionFilter(_message.Message):
-    __slots__ = ["class_hash", "sender_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    sender_address: _types_pb2.FieldElement
+class Filter(_message.Message):
+    __slots__ = ["header", "transactions", "state_update", "events", "messages"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
+    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
+    MESSAGES_FIELD_NUMBER: _ClassVar[int]
+    header: HeaderFilter
+    transactions: _containers.RepeatedCompositeFieldContainer[TransactionFilter]
+    state_update: StateUpdateFilter
+    events: _containers.RepeatedCompositeFieldContainer[EventFilter]
+    messages: _containers.RepeatedCompositeFieldContainer[L2ToL1MessageFilter]
     def __init__(
         self,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        header: _Optional[_Union[HeaderFilter, _Mapping]] = ...,
+        transactions: _Optional[_Iterable[_Union[TransactionFilter, _Mapping]]] = ...,
+        state_update: _Optional[_Union[StateUpdateFilter, _Mapping]] = ...,
+        events: _Optional[_Iterable[_Union[EventFilter, _Mapping]]] = ...,
+        messages: _Optional[_Iterable[_Union[L2ToL1MessageFilter, _Mapping]]] = ...,
     ) -> None: ...
 
-class DeclaredClassFilter(_message.Message):
-    __slots__ = ["class_hash", "compiled_class_hash"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    compiled_class_hash: _types_pb2.FieldElement
+class HeaderFilter(_message.Message):
+    __slots__ = ["weak"]
+    WEAK_FIELD_NUMBER: _ClassVar[int]
+    weak: bool
+    def __init__(self, weak: bool = ...) -> None: ...
+
+class TransactionFilter(_message.Message):
+    __slots__ = [
+        "invoke_v0",
+        "invoke_v1",
+        "deploy",
+        "declare",
+        "l1_handler",
+        "deploy_account",
+        "include_reverted",
+    ]
+    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
+    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_FIELD_NUMBER: _ClassVar[int]
+    DECLARE_FIELD_NUMBER: _ClassVar[int]
+    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
+    INCLUDE_REVERTED_FIELD_NUMBER: _ClassVar[int]
+    invoke_v0: InvokeTransactionV0Filter
+    invoke_v1: InvokeTransactionV1Filter
+    deploy: DeployTransactionFilter
+    declare: DeclareTransactionFilter
+    l1_handler: L1HandlerTransactionFilter
+    deploy_account: DeployAccountTransactionFilter
+    include_reverted: bool
     def __init__(
         self,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        invoke_v0: _Optional[_Union[InvokeTransactionV0Filter, _Mapping]] = ...,
+        invoke_v1: _Optional[_Union[InvokeTransactionV1Filter, _Mapping]] = ...,
+        deploy: _Optional[_Union[DeployTransactionFilter, _Mapping]] = ...,
+        declare: _Optional[_Union[DeclareTransactionFilter, _Mapping]] = ...,
+        l1_handler: _Optional[_Union[L1HandlerTransactionFilter, _Mapping]] = ...,
+        deploy_account: _Optional[
+            _Union[DeployAccountTransactionFilter, _Mapping]
+        ] = ...,
+        include_reverted: bool = ...,
     ) -> None: ...
 
-class DeclaredContractFilter(_message.Message):
-    __slots__ = ["class_hash"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+class InvokeTransactionV0Filter(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
-        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        entry_point_selector: _Optional[
+            _Union[_types_pb2.FieldElement, _Mapping]
+        ] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
-class DeployAccountTransactionFilter(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    constructor_calldata: _containers.RepeatedCompositeFieldContainer[
-        _types_pb2.FieldElement
-    ]
-    contract_address_salt: _types_pb2.FieldElement
+class InvokeTransactionV1Filter(_message.Message):
+    __slots__ = ["sender_address", "calldata"]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    sender_address: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
-        contract_address_salt: _Optional[
-            _Union[_types_pb2.FieldElement, _Mapping]
-        ] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        constructor_calldata: _Optional[
-            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
-        ] = ...,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
 class DeployTransactionFilter(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
+    __slots__ = ["contract_address_salt", "class_hash", "constructor_calldata"]
+    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
+    contract_address_salt: _types_pb2.FieldElement
     class_hash: _types_pb2.FieldElement
     constructor_calldata: _containers.RepeatedCompositeFieldContainer[
         _types_pb2.FieldElement
     ]
-    contract_address_salt: _types_pb2.FieldElement
     def __init__(
         self,
         contract_address_salt: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         constructor_calldata: _Optional[
             _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
         ] = ...,
     ) -> None: ...
 
-class DeployedContractFilter(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
+class DeclareTransactionFilter(_message.Message):
+    __slots__ = ["class_hash", "sender_address"]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
-    contract_address: _types_pb2.FieldElement
+    sender_address: _types_pb2.FieldElement
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class EventFilter(_message.Message):
-    __slots__ = [
-        "data",
-        "from_address",
-        "include_receipt",
-        "include_reverted",
-        "include_transaction",
-        "keys",
-    ]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    INCLUDE_RECEIPT_FIELD_NUMBER: _ClassVar[int]
-    INCLUDE_REVERTED_FIELD_NUMBER: _ClassVar[int]
-    INCLUDE_TRANSACTION_FIELD_NUMBER: _ClassVar[int]
-    KEYS_FIELD_NUMBER: _ClassVar[int]
-    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    from_address: _types_pb2.FieldElement
-    include_receipt: bool
-    include_reverted: bool
-    include_transaction: bool
-    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    def __init__(
-        self,
-        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-        include_reverted: bool = ...,
-        include_transaction: bool = ...,
-        include_receipt: bool = ...,
-    ) -> None: ...
-
-class Filter(_message.Message):
-    __slots__ = ["events", "header", "messages", "state_update", "transactions"]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    MESSAGES_FIELD_NUMBER: _ClassVar[int]
-    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
-    events: _containers.RepeatedCompositeFieldContainer[EventFilter]
-    header: HeaderFilter
-    messages: _containers.RepeatedCompositeFieldContainer[L2ToL1MessageFilter]
-    state_update: StateUpdateFilter
-    transactions: _containers.RepeatedCompositeFieldContainer[TransactionFilter]
-    def __init__(
-        self,
-        header: _Optional[_Union[HeaderFilter, _Mapping]] = ...,
-        transactions: _Optional[_Iterable[_Union[TransactionFilter, _Mapping]]] = ...,
-        state_update: _Optional[_Union[StateUpdateFilter, _Mapping]] = ...,
-        events: _Optional[_Iterable[_Union[EventFilter, _Mapping]]] = ...,
-        messages: _Optional[_Iterable[_Union[L2ToL1MessageFilter, _Mapping]]] = ...,
-    ) -> None: ...
-
-class HeaderFilter(_message.Message):
-    __slots__ = ["weak"]
-    WEAK_FIELD_NUMBER: _ClassVar[int]
-    weak: bool
-    def __init__(self, weak: bool = ...) -> None: ...
-
-class InvokeTransactionV0Filter(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+class L1HandlerTransactionFilter(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         entry_point_selector: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
-class InvokeTransactionV1Filter(_message.Message):
-    __slots__ = ["calldata", "sender_address"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    sender_address: _types_pb2.FieldElement
-    def __init__(
-        self,
-        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-    ) -> None: ...
-
-class L1HandlerTransactionFilter(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    contract_address: _types_pb2.FieldElement
-    entry_point_selector: _types_pb2.FieldElement
+class DeployAccountTransactionFilter(_message.Message):
+    __slots__ = ["contract_address_salt", "class_hash", "constructor_calldata"]
+    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    contract_address_salt: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
+    constructor_calldata: _containers.RepeatedCompositeFieldContainer[
+        _types_pb2.FieldElement
+    ]
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        entry_point_selector: _Optional[
+        contract_address_salt: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        constructor_calldata: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
     ) -> None: ...
 
 class L2ToL1MessageFilter(_message.Message):
-    __slots__ = ["include_reverted", "payload", "to_address"]
-    INCLUDE_REVERTED_FIELD_NUMBER: _ClassVar[int]
-    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["to_address", "payload", "include_reverted"]
     TO_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    include_reverted: bool
-    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    INCLUDE_REVERTED_FIELD_NUMBER: _ClassVar[int]
     to_address: _types_pb2.FieldElement
+    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    include_reverted: bool
     def __init__(
         self,
         to_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         payload: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
         include_reverted: bool = ...,
     ) -> None: ...
 
-class NonceUpdateFilter(_message.Message):
-    __slots__ = ["contract_address", "nonce"]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    NONCE_FIELD_NUMBER: _ClassVar[int]
-    contract_address: _types_pb2.FieldElement
-    nonce: _types_pb2.FieldElement
-    def __init__(
-        self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-    ) -> None: ...
-
-class ReplacedClassFilter(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    contract_address: _types_pb2.FieldElement
+class EventFilter(_message.Message):
+    __slots__ = [
+        "from_address",
+        "keys",
+        "data",
+        "include_reverted",
+        "include_transaction",
+        "include_receipt",
+    ]
+    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    KEYS_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    INCLUDE_REVERTED_FIELD_NUMBER: _ClassVar[int]
+    INCLUDE_TRANSACTION_FIELD_NUMBER: _ClassVar[int]
+    INCLUDE_RECEIPT_FIELD_NUMBER: _ClassVar[int]
+    from_address: _types_pb2.FieldElement
+    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    include_reverted: bool
+    include_transaction: bool
+    include_receipt: bool
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        include_reverted: bool = ...,
+        include_transaction: bool = ...,
+        include_receipt: bool = ...,
     ) -> None: ...
 
 class StateUpdateFilter(_message.Message):
     __slots__ = [
-        "declared_classes",
+        "storage_diffs",
         "declared_contracts",
         "deployed_contracts",
         "nonces",
+        "declared_classes",
         "replaced_classes",
-        "storage_diffs",
     ]
-    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
+    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
     DECLARED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     DEPLOYED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     NONCES_FIELD_NUMBER: _ClassVar[int]
+    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     REPLACED_CLASSES_FIELD_NUMBER: _ClassVar[int]
-    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
-    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClassFilter]
+    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiffFilter]
     declared_contracts: _containers.RepeatedCompositeFieldContainer[
         DeclaredContractFilter
     ]
     deployed_contracts: _containers.RepeatedCompositeFieldContainer[
         DeployedContractFilter
     ]
     nonces: _containers.RepeatedCompositeFieldContainer[NonceUpdateFilter]
+    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClassFilter]
     replaced_classes: _containers.RepeatedCompositeFieldContainer[ReplacedClassFilter]
-    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiffFilter]
     def __init__(
         self,
         storage_diffs: _Optional[_Iterable[_Union[StorageDiffFilter, _Mapping]]] = ...,
         declared_contracts: _Optional[
             _Iterable[_Union[DeclaredContractFilter, _Mapping]]
         ] = ...,
         deployed_contracts: _Optional[
@@ -288,43 +270,62 @@
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class TransactionFilter(_message.Message):
-    __slots__ = [
-        "declare",
-        "deploy",
-        "deploy_account",
-        "include_reverted",
-        "invoke_v0",
-        "invoke_v1",
-        "l1_handler",
-    ]
-    DECLARE_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_FIELD_NUMBER: _ClassVar[int]
-    INCLUDE_REVERTED_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
-    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
-    declare: DeclareTransactionFilter
-    deploy: DeployTransactionFilter
-    deploy_account: DeployAccountTransactionFilter
-    include_reverted: bool
-    invoke_v0: InvokeTransactionV0Filter
-    invoke_v1: InvokeTransactionV1Filter
-    l1_handler: L1HandlerTransactionFilter
+class DeclaredContractFilter(_message.Message):
+    __slots__ = ["class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
+    ) -> None: ...
+
+class DeclaredClassFilter(_message.Message):
+    __slots__ = ["class_hash", "compiled_class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        invoke_v0: _Optional[_Union[InvokeTransactionV0Filter, _Mapping]] = ...,
-        invoke_v1: _Optional[_Union[InvokeTransactionV1Filter, _Mapping]] = ...,
-        deploy: _Optional[_Union[DeployTransactionFilter, _Mapping]] = ...,
-        declare: _Optional[_Union[DeclareTransactionFilter, _Mapping]] = ...,
-        l1_handler: _Optional[_Union[L1HandlerTransactionFilter, _Mapping]] = ...,
-        deploy_account: _Optional[
-            _Union[DeployAccountTransactionFilter, _Mapping]
-        ] = ...,
-        include_reverted: bool = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
+class ReplacedClassFilter(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
+class DeployedContractFilter(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
+class NonceUpdateFilter(_message.Message):
+    __slots__ = ["contract_address", "nonce"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    NONCE_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    nonce: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
```

### Comparing `apibara-0.7.5/src/apibara/starknet/proto/starknet_pb2.pyi` & `apibara-0.8.0/src/apibara/starknet/proto/starknet_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,373 +1,612 @@
-from typing import ClassVar as _ClassVar
-from typing import Iterable as _Iterable
-from typing import Mapping as _Mapping
-from typing import Optional as _Optional
-from typing import Union as _Union
-
-import types_pb2 as _types_pb2
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+import types_pb2 as _types_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import (
+    ClassVar as _ClassVar,
+    Iterable as _Iterable,
+    Mapping as _Mapping,
+    Optional as _Optional,
+    Union as _Union,
+)
 
-BLOCK_STATUS_ACCEPTED_ON_L1: BlockStatus
-BLOCK_STATUS_ACCEPTED_ON_L2: BlockStatus
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class L1DataAvailabilityMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    L1_DATA_AVAILABILITY_MODE_UNSPECIFIED: _ClassVar[L1DataAvailabilityMode]
+    L1_DATA_AVAILABILITY_MODE_BLOB: _ClassVar[L1DataAvailabilityMode]
+    L1_DATA_AVAILABILITY_MODE_CALLDATA: _ClassVar[L1DataAvailabilityMode]
+
+class BlockStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    BLOCK_STATUS_UNSPECIFIED: _ClassVar[BlockStatus]
+    BLOCK_STATUS_PENDING: _ClassVar[BlockStatus]
+    BLOCK_STATUS_ACCEPTED_ON_L2: _ClassVar[BlockStatus]
+    BLOCK_STATUS_ACCEPTED_ON_L1: _ClassVar[BlockStatus]
+    BLOCK_STATUS_REJECTED: _ClassVar[BlockStatus]
+
+class ExecutionStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    EXECUTION_STATUS_UNSPECIFIED: _ClassVar[ExecutionStatus]
+    EXECUTION_STATUS_SUCCEEDED: _ClassVar[ExecutionStatus]
+    EXECUTION_STATUS_REVERTED: _ClassVar[ExecutionStatus]
+
+class PriceUnit(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    PRICE_UNIT_UNSPECIFIED: _ClassVar[PriceUnit]
+    PRICE_UNIT_WEI: _ClassVar[PriceUnit]
+    PRICE_UNIT_FRI: _ClassVar[PriceUnit]
+
+class DataAvailabilityMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    DATA_AVAILABILITY_MODE_UNSPECIFIED: _ClassVar[DataAvailabilityMode]
+    DATA_AVAILABILITY_MODE_L1: _ClassVar[DataAvailabilityMode]
+    DATA_AVAILABILITY_MODE_L2: _ClassVar[DataAvailabilityMode]
+
+L1_DATA_AVAILABILITY_MODE_UNSPECIFIED: L1DataAvailabilityMode
+L1_DATA_AVAILABILITY_MODE_BLOB: L1DataAvailabilityMode
+L1_DATA_AVAILABILITY_MODE_CALLDATA: L1DataAvailabilityMode
+BLOCK_STATUS_UNSPECIFIED: BlockStatus
 BLOCK_STATUS_PENDING: BlockStatus
+BLOCK_STATUS_ACCEPTED_ON_L2: BlockStatus
+BLOCK_STATUS_ACCEPTED_ON_L1: BlockStatus
 BLOCK_STATUS_REJECTED: BlockStatus
-BLOCK_STATUS_UNSPECIFIED: BlockStatus
-DESCRIPTOR: _descriptor.FileDescriptor
-EXECUTION_STATUS_REVERTED: ExecutionStatus
-EXECUTION_STATUS_SUCCEEDED: ExecutionStatus
 EXECUTION_STATUS_UNSPECIFIED: ExecutionStatus
+EXECUTION_STATUS_SUCCEEDED: ExecutionStatus
+EXECUTION_STATUS_REVERTED: ExecutionStatus
+PRICE_UNIT_UNSPECIFIED: PriceUnit
+PRICE_UNIT_WEI: PriceUnit
+PRICE_UNIT_FRI: PriceUnit
+DATA_AVAILABILITY_MODE_UNSPECIFIED: DataAvailabilityMode
+DATA_AVAILABILITY_MODE_L1: DataAvailabilityMode
+DATA_AVAILABILITY_MODE_L2: DataAvailabilityMode
 
 class Block(_message.Message):
     __slots__ = [
-        "events",
-        "header",
-        "l2_to_l1_messages",
-        "state_update",
         "status",
+        "header",
         "transactions",
+        "state_update",
+        "events",
+        "l2_to_l1_messages",
+        "empty",
     ]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
-    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
     TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
-    events: _containers.RepeatedCompositeFieldContainer[EventWithTransaction]
+    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
+    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
+    EMPTY_FIELD_NUMBER: _ClassVar[int]
+    status: BlockStatus
     header: BlockHeader
+    transactions: _containers.RepeatedCompositeFieldContainer[TransactionWithReceipt]
+    state_update: StateUpdate
+    events: _containers.RepeatedCompositeFieldContainer[EventWithTransaction]
     l2_to_l1_messages: _containers.RepeatedCompositeFieldContainer[
         L2ToL1MessageWithTransaction
     ]
-    state_update: StateUpdate
-    status: BlockStatus
-    transactions: _containers.RepeatedCompositeFieldContainer[TransactionWithReceipt]
+    empty: bool
     def __init__(
         self,
         status: _Optional[_Union[BlockStatus, str]] = ...,
         header: _Optional[_Union[BlockHeader, _Mapping]] = ...,
         transactions: _Optional[
             _Iterable[_Union[TransactionWithReceipt, _Mapping]]
         ] = ...,
         state_update: _Optional[_Union[StateUpdate, _Mapping]] = ...,
         events: _Optional[_Iterable[_Union[EventWithTransaction, _Mapping]]] = ...,
         l2_to_l1_messages: _Optional[
             _Iterable[_Union[L2ToL1MessageWithTransaction, _Mapping]]
         ] = ...,
+        empty: bool = ...,
     ) -> None: ...
 
 class BlockHeader(_message.Message):
     __slots__ = [
         "block_hash",
-        "block_number",
-        "new_root",
         "parent_block_hash",
+        "block_number",
         "sequencer_address",
+        "new_root",
         "timestamp",
+        "starknet_version",
+        "l1_gas_price",
+        "l1_data_gas_price",
+        "l1_data_availability_mode",
     ]
     BLOCK_HASH_FIELD_NUMBER: _ClassVar[int]
-    BLOCK_NUMBER_FIELD_NUMBER: _ClassVar[int]
-    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
     PARENT_BLOCK_HASH_FIELD_NUMBER: _ClassVar[int]
+    BLOCK_NUMBER_FIELD_NUMBER: _ClassVar[int]
     SEQUENCER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    STARKNET_VERSION_FIELD_NUMBER: _ClassVar[int]
+    L1_GAS_PRICE_FIELD_NUMBER: _ClassVar[int]
+    L1_DATA_GAS_PRICE_FIELD_NUMBER: _ClassVar[int]
+    L1_DATA_AVAILABILITY_MODE_FIELD_NUMBER: _ClassVar[int]
     block_hash: _types_pb2.FieldElement
-    block_number: int
-    new_root: _types_pb2.FieldElement
     parent_block_hash: _types_pb2.FieldElement
+    block_number: int
     sequencer_address: _types_pb2.FieldElement
+    new_root: _types_pb2.FieldElement
     timestamp: _timestamp_pb2.Timestamp
+    starknet_version: str
+    l1_gas_price: ResourcePrice
+    l1_data_gas_price: ResourcePrice
+    l1_data_availability_mode: L1DataAvailabilityMode
     def __init__(
         self,
         block_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         parent_block_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         block_number: _Optional[int] = ...,
         sequencer_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         new_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
+        starknet_version: _Optional[str] = ...,
+        l1_gas_price: _Optional[_Union[ResourcePrice, _Mapping]] = ...,
+        l1_data_gas_price: _Optional[_Union[ResourcePrice, _Mapping]] = ...,
+        l1_data_availability_mode: _Optional[_Union[L1DataAvailabilityMode, str]] = ...,
+    ) -> None: ...
+
+class TransactionWithReceipt(_message.Message):
+    __slots__ = ["transaction", "receipt"]
+    TRANSACTION_FIELD_NUMBER: _ClassVar[int]
+    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+    transaction: Transaction
+    receipt: TransactionReceipt
+    def __init__(
+        self,
+        transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
+        receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
+    ) -> None: ...
+
+class Transaction(_message.Message):
+    __slots__ = [
+        "meta",
+        "invoke_v0",
+        "invoke_v1",
+        "deploy",
+        "declare",
+        "l1_handler",
+        "deploy_account",
+        "deploy_account_v3",
+        "invoke_v3",
+        "declare_v3",
+    ]
+    META_FIELD_NUMBER: _ClassVar[int]
+    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
+    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_FIELD_NUMBER: _ClassVar[int]
+    DECLARE_FIELD_NUMBER: _ClassVar[int]
+    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_ACCOUNT_V3_FIELD_NUMBER: _ClassVar[int]
+    INVOKE_V3_FIELD_NUMBER: _ClassVar[int]
+    DECLARE_V3_FIELD_NUMBER: _ClassVar[int]
+    meta: TransactionMeta
+    invoke_v0: InvokeTransactionV0
+    invoke_v1: InvokeTransactionV1
+    deploy: DeployTransaction
+    declare: DeclareTransaction
+    l1_handler: L1HandlerTransaction
+    deploy_account: DeployAccountTransaction
+    deploy_account_v3: DeployAccountTransactionV3
+    invoke_v3: InvokeTransactionV3
+    declare_v3: DeclareTransactionV3
+    def __init__(
+        self,
+        meta: _Optional[_Union[TransactionMeta, _Mapping]] = ...,
+        invoke_v0: _Optional[_Union[InvokeTransactionV0, _Mapping]] = ...,
+        invoke_v1: _Optional[_Union[InvokeTransactionV1, _Mapping]] = ...,
+        deploy: _Optional[_Union[DeployTransaction, _Mapping]] = ...,
+        declare: _Optional[_Union[DeclareTransaction, _Mapping]] = ...,
+        l1_handler: _Optional[_Union[L1HandlerTransaction, _Mapping]] = ...,
+        deploy_account: _Optional[_Union[DeployAccountTransaction, _Mapping]] = ...,
+        deploy_account_v3: _Optional[
+            _Union[DeployAccountTransactionV3, _Mapping]
+        ] = ...,
+        invoke_v3: _Optional[_Union[InvokeTransactionV3, _Mapping]] = ...,
+        declare_v3: _Optional[_Union[DeclareTransactionV3, _Mapping]] = ...,
+    ) -> None: ...
+
+class TransactionMeta(_message.Message):
+    __slots__ = [
+        "hash",
+        "max_fee",
+        "signature",
+        "nonce",
+        "version",
+        "resource_bounds",
+        "tip",
+        "paymaster_data",
+        "nonce_data_availability_mode",
+        "fee_data_availability_mode",
+        "transaction_index",
+    ]
+    HASH_FIELD_NUMBER: _ClassVar[int]
+    MAX_FEE_FIELD_NUMBER: _ClassVar[int]
+    SIGNATURE_FIELD_NUMBER: _ClassVar[int]
+    NONCE_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    RESOURCE_BOUNDS_FIELD_NUMBER: _ClassVar[int]
+    TIP_FIELD_NUMBER: _ClassVar[int]
+    PAYMASTER_DATA_FIELD_NUMBER: _ClassVar[int]
+    NONCE_DATA_AVAILABILITY_MODE_FIELD_NUMBER: _ClassVar[int]
+    FEE_DATA_AVAILABILITY_MODE_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTION_INDEX_FIELD_NUMBER: _ClassVar[int]
+    hash: _types_pb2.FieldElement
+    max_fee: _types_pb2.FieldElement
+    signature: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    nonce: _types_pb2.FieldElement
+    version: int
+    resource_bounds: ResourceBoundsMapping
+    tip: int
+    paymaster_data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    nonce_data_availability_mode: DataAvailabilityMode
+    fee_data_availability_mode: DataAvailabilityMode
+    transaction_index: int
+    def __init__(
+        self,
+        hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        max_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        signature: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
+        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        version: _Optional[int] = ...,
+        resource_bounds: _Optional[_Union[ResourceBoundsMapping, _Mapping]] = ...,
+        tip: _Optional[int] = ...,
+        paymaster_data: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
+        nonce_data_availability_mode: _Optional[
+            _Union[DataAvailabilityMode, str]
+        ] = ...,
+        fee_data_availability_mode: _Optional[_Union[DataAvailabilityMode, str]] = ...,
+        transaction_index: _Optional[int] = ...,
+    ) -> None: ...
+
+class InvokeTransactionV0(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        entry_point_selector: _Optional[
+            _Union[_types_pb2.FieldElement, _Mapping]
+        ] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+    ) -> None: ...
+
+class InvokeTransactionV1(_message.Message):
+    __slots__ = ["sender_address", "calldata"]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    sender_address: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    def __init__(
+        self,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+    ) -> None: ...
+
+class InvokeTransactionV3(_message.Message):
+    __slots__ = ["sender_address", "calldata", "account_deployment_data"]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    ACCOUNT_DEPLOYMENT_DATA_FIELD_NUMBER: _ClassVar[int]
+    sender_address: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    account_deployment_data: _containers.RepeatedCompositeFieldContainer[
+        _types_pb2.FieldElement
+    ]
+    def __init__(
+        self,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        account_deployment_data: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
+    ) -> None: ...
+
+class DeployTransaction(_message.Message):
+    __slots__ = ["constructor_calldata", "contract_address_salt", "class_hash"]
+    CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    constructor_calldata: _containers.RepeatedCompositeFieldContainer[
+        _types_pb2.FieldElement
+    ]
+    contract_address_salt: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self,
+        constructor_calldata: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
+        contract_address_salt: _Optional[
+            _Union[_types_pb2.FieldElement, _Mapping]
+        ] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
 class DeclareTransaction(_message.Message):
-    __slots__ = ["class_hash", "compiled_class_hash", "sender_address"]
+    __slots__ = ["class_hash", "sender_address", "compiled_class_hash"]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
-    compiled_class_hash: _types_pb2.FieldElement
     sender_address: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
     def __init__(
         self,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class DeclaredClass(_message.Message):
-    __slots__ = ["class_hash", "compiled_class_hash"]
+class DeclareTransactionV3(_message.Message):
+    __slots__ = [
+        "class_hash",
+        "sender_address",
+        "compiled_class_hash",
+        "account_deployment_data",
+    ]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    ACCOUNT_DEPLOYMENT_DATA_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
+    sender_address: _types_pb2.FieldElement
     compiled_class_hash: _types_pb2.FieldElement
+    account_deployment_data: _containers.RepeatedCompositeFieldContainer[
+        _types_pb2.FieldElement
+    ]
     def __init__(
         self,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        account_deployment_data: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
     ) -> None: ...
 
-class DeclaredContract(_message.Message):
-    __slots__ = ["class_hash"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+class L1HandlerTransaction(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
-        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        entry_point_selector: _Optional[
+            _Union[_types_pb2.FieldElement, _Mapping]
+        ] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
 class DeployAccountTransaction(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["constructor_calldata", "contract_address_salt", "class_hash"]
     CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
     CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     constructor_calldata: _containers.RepeatedCompositeFieldContainer[
         _types_pb2.FieldElement
     ]
     contract_address_salt: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
         constructor_calldata: _Optional[
             _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
         ] = ...,
         contract_address_salt: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class DeployTransaction(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+class DeployAccountTransactionV3(_message.Message):
+    __slots__ = ["constructor_calldata", "contract_address_salt", "class_hash"]
     CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
     CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     constructor_calldata: _containers.RepeatedCompositeFieldContainer[
         _types_pb2.FieldElement
     ]
     contract_address_salt: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
         constructor_calldata: _Optional[
             _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
         ] = ...,
         contract_address_salt: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class DeployedContract(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+class TransactionReceipt(_message.Message):
+    __slots__ = [
+        "transaction_hash",
+        "transaction_index",
+        "actual_fee",
+        "l2_to_l1_messages",
+        "events",
+        "contract_address",
+        "execution_status",
+        "revert_reason",
+        "actual_fee_paid",
+        "execution_resources",
+    ]
+    TRANSACTION_HASH_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTION_INDEX_FIELD_NUMBER: _ClassVar[int]
+    ACTUAL_FEE_FIELD_NUMBER: _ClassVar[int]
+    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+    EXECUTION_STATUS_FIELD_NUMBER: _ClassVar[int]
+    REVERT_REASON_FIELD_NUMBER: _ClassVar[int]
+    ACTUAL_FEE_PAID_FIELD_NUMBER: _ClassVar[int]
+    EXECUTION_RESOURCES_FIELD_NUMBER: _ClassVar[int]
+    transaction_hash: _types_pb2.FieldElement
+    transaction_index: int
+    actual_fee: _types_pb2.FieldElement
+    l2_to_l1_messages: _containers.RepeatedCompositeFieldContainer[L2ToL1Message]
+    events: _containers.RepeatedCompositeFieldContainer[Event]
     contract_address: _types_pb2.FieldElement
+    execution_status: ExecutionStatus
+    revert_reason: str
+    actual_fee_paid: FeePayment
+    execution_resources: ExecutionResources
     def __init__(
         self,
+        transaction_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        transaction_index: _Optional[int] = ...,
+        actual_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        l2_to_l1_messages: _Optional[_Iterable[_Union[L2ToL1Message, _Mapping]]] = ...,
+        events: _Optional[_Iterable[_Union[Event, _Mapping]]] = ...,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-    ) -> None: ...
-
-class Event(_message.Message):
-    __slots__ = ["data", "from_address", "index", "keys"]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    INDEX_FIELD_NUMBER: _ClassVar[int]
-    KEYS_FIELD_NUMBER: _ClassVar[int]
-    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    from_address: _types_pb2.FieldElement
-    index: int
-    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    def __init__(
-        self,
-        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-        index: _Optional[int] = ...,
+        execution_status: _Optional[_Union[ExecutionStatus, str]] = ...,
+        revert_reason: _Optional[str] = ...,
+        actual_fee_paid: _Optional[_Union[FeePayment, _Mapping]] = ...,
+        execution_resources: _Optional[_Union[ExecutionResources, _Mapping]] = ...,
     ) -> None: ...
 
-class EventWithTransaction(_message.Message):
-    __slots__ = ["event", "receipt", "transaction"]
-    EVENT_FIELD_NUMBER: _ClassVar[int]
-    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+class L2ToL1MessageWithTransaction(_message.Message):
+    __slots__ = ["transaction", "receipt", "message"]
     TRANSACTION_FIELD_NUMBER: _ClassVar[int]
-    event: Event
-    receipt: TransactionReceipt
+    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
     transaction: Transaction
+    receipt: TransactionReceipt
+    message: L2ToL1Message
     def __init__(
         self,
         transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
         receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
-        event: _Optional[_Union[Event, _Mapping]] = ...,
-    ) -> None: ...
-
-class InvokeTransactionV0(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    contract_address: _types_pb2.FieldElement
-    entry_point_selector: _types_pb2.FieldElement
-    def __init__(
-        self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        entry_point_selector: _Optional[
-            _Union[_types_pb2.FieldElement, _Mapping]
-        ] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-    ) -> None: ...
-
-class InvokeTransactionV1(_message.Message):
-    __slots__ = ["calldata", "sender_address"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    sender_address: _types_pb2.FieldElement
-    def __init__(
-        self,
-        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-    ) -> None: ...
-
-class L1HandlerTransaction(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    contract_address: _types_pb2.FieldElement
-    entry_point_selector: _types_pb2.FieldElement
-    def __init__(
-        self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        entry_point_selector: _Optional[
-            _Union[_types_pb2.FieldElement, _Mapping]
-        ] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        message: _Optional[_Union[L2ToL1Message, _Mapping]] = ...,
     ) -> None: ...
 
 class L2ToL1Message(_message.Message):
-    __slots__ = ["from_address", "index", "payload", "to_address"]
-    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    INDEX_FIELD_NUMBER: _ClassVar[int]
-    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["to_address", "payload", "index", "from_address"]
     TO_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    from_address: _types_pb2.FieldElement
-    index: int
-    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     to_address: _types_pb2.FieldElement
+    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    index: int
+    from_address: _types_pb2.FieldElement
     def __init__(
         self,
         to_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         payload: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
         index: _Optional[int] = ...,
         from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class L2ToL1MessageWithTransaction(_message.Message):
-    __slots__ = ["message", "receipt", "transaction"]
-    MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+class EventWithTransaction(_message.Message):
+    __slots__ = ["transaction", "receipt", "event"]
     TRANSACTION_FIELD_NUMBER: _ClassVar[int]
-    message: L2ToL1Message
-    receipt: TransactionReceipt
+    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+    EVENT_FIELD_NUMBER: _ClassVar[int]
     transaction: Transaction
+    receipt: TransactionReceipt
+    event: Event
     def __init__(
         self,
         transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
         receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
-        message: _Optional[_Union[L2ToL1Message, _Mapping]] = ...,
+        event: _Optional[_Union[Event, _Mapping]] = ...,
     ) -> None: ...
 
-class NonceUpdate(_message.Message):
-    __slots__ = ["contract_address", "nonce"]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    NONCE_FIELD_NUMBER: _ClassVar[int]
-    contract_address: _types_pb2.FieldElement
-    nonce: _types_pb2.FieldElement
+class Event(_message.Message):
+    __slots__ = ["from_address", "keys", "data", "index"]
+    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    KEYS_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    from_address: _types_pb2.FieldElement
+    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    index: int
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        index: _Optional[int] = ...,
     ) -> None: ...
 
-class ReplacedClass(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    contract_address: _types_pb2.FieldElement
+class StateUpdate(_message.Message):
+    __slots__ = ["new_root", "old_root", "state_diff"]
+    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
+    OLD_ROOT_FIELD_NUMBER: _ClassVar[int]
+    STATE_DIFF_FIELD_NUMBER: _ClassVar[int]
+    new_root: _types_pb2.FieldElement
+    old_root: _types_pb2.FieldElement
+    state_diff: StateDiff
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        new_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        old_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        state_diff: _Optional[_Union[StateDiff, _Mapping]] = ...,
     ) -> None: ...
 
 class StateDiff(_message.Message):
     __slots__ = [
-        "declared_classes",
+        "storage_diffs",
         "declared_contracts",
         "deployed_contracts",
         "nonces",
+        "declared_classes",
         "replaced_classes",
-        "storage_diffs",
     ]
-    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
+    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
     DECLARED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     DEPLOYED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     NONCES_FIELD_NUMBER: _ClassVar[int]
+    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     REPLACED_CLASSES_FIELD_NUMBER: _ClassVar[int]
-    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
-    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClass]
+    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiff]
     declared_contracts: _containers.RepeatedCompositeFieldContainer[DeclaredContract]
     deployed_contracts: _containers.RepeatedCompositeFieldContainer[DeployedContract]
     nonces: _containers.RepeatedCompositeFieldContainer[NonceUpdate]
+    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClass]
     replaced_classes: _containers.RepeatedCompositeFieldContainer[ReplacedClass]
-    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiff]
     def __init__(
         self,
         storage_diffs: _Optional[_Iterable[_Union[StorageDiff, _Mapping]]] = ...,
         declared_contracts: _Optional[
             _Iterable[_Union[DeclaredContract, _Mapping]]
         ] = ...,
         deployed_contracts: _Optional[
             _Iterable[_Union[DeployedContract, _Mapping]]
         ] = ...,
         nonces: _Optional[_Iterable[_Union[NonceUpdate, _Mapping]]] = ...,
         declared_classes: _Optional[_Iterable[_Union[DeclaredClass, _Mapping]]] = ...,
         replaced_classes: _Optional[_Iterable[_Union[ReplacedClass, _Mapping]]] = ...,
     ) -> None: ...
 
-class StateUpdate(_message.Message):
-    __slots__ = ["new_root", "old_root", "state_diff"]
-    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
-    OLD_ROOT_FIELD_NUMBER: _ClassVar[int]
-    STATE_DIFF_FIELD_NUMBER: _ClassVar[int]
-    new_root: _types_pb2.FieldElement
-    old_root: _types_pb2.FieldElement
-    state_diff: StateDiff
-    def __init__(
-        self,
-        new_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        old_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        state_diff: _Optional[_Union[StateDiff, _Mapping]] = ...,
-    ) -> None: ...
-
 class StorageDiff(_message.Message):
     __slots__ = ["contract_address", "storage_entries"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     STORAGE_ENTRIES_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     storage_entries: _containers.RepeatedCompositeFieldContainer[StorageEntry]
     def __init__(
@@ -384,121 +623,189 @@
     value: _types_pb2.FieldElement
     def __init__(
         self,
         key: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         value: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class Transaction(_message.Message):
-    __slots__ = [
-        "declare",
-        "deploy",
-        "deploy_account",
-        "invoke_v0",
-        "invoke_v1",
-        "l1_handler",
-        "meta",
-    ]
-    DECLARE_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
-    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
-    META_FIELD_NUMBER: _ClassVar[int]
-    declare: DeclareTransaction
-    deploy: DeployTransaction
-    deploy_account: DeployAccountTransaction
-    invoke_v0: InvokeTransactionV0
-    invoke_v1: InvokeTransactionV1
-    l1_handler: L1HandlerTransaction
-    meta: TransactionMeta
+class DeclaredContract(_message.Message):
+    __slots__ = ["class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
+    ) -> None: ...
+
+class DeclaredClass(_message.Message):
+    __slots__ = ["class_hash", "compiled_class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        meta: _Optional[_Union[TransactionMeta, _Mapping]] = ...,
-        invoke_v0: _Optional[_Union[InvokeTransactionV0, _Mapping]] = ...,
-        invoke_v1: _Optional[_Union[InvokeTransactionV1, _Mapping]] = ...,
-        deploy: _Optional[_Union[DeployTransaction, _Mapping]] = ...,
-        declare: _Optional[_Union[DeclareTransaction, _Mapping]] = ...,
-        l1_handler: _Optional[_Union[L1HandlerTransaction, _Mapping]] = ...,
-        deploy_account: _Optional[_Union[DeployAccountTransaction, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class TransactionMeta(_message.Message):
-    __slots__ = ["hash", "max_fee", "nonce", "signature", "version"]
-    HASH_FIELD_NUMBER: _ClassVar[int]
-    MAX_FEE_FIELD_NUMBER: _ClassVar[int]
-    NONCE_FIELD_NUMBER: _ClassVar[int]
-    SIGNATURE_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    hash: _types_pb2.FieldElement
-    max_fee: _types_pb2.FieldElement
-    nonce: _types_pb2.FieldElement
-    signature: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    version: int
+class ReplacedClass(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        max_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        signature: _Optional[
-            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
-        ] = ...,
-        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        version: _Optional[int] = ...,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class TransactionReceipt(_message.Message):
-    __slots__ = [
-        "actual_fee",
-        "contract_address",
-        "events",
-        "execution_status",
-        "l2_to_l1_messages",
-        "revert_reason",
-        "transaction_hash",
-        "transaction_index",
-    ]
-    ACTUAL_FEE_FIELD_NUMBER: _ClassVar[int]
+class DeployedContract(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
-    EXECUTION_STATUS_FIELD_NUMBER: _ClassVar[int]
-    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
-    REVERT_REASON_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTION_HASH_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTION_INDEX_FIELD_NUMBER: _ClassVar[int]
-    actual_fee: _types_pb2.FieldElement
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
-    events: _containers.RepeatedCompositeFieldContainer[Event]
-    execution_status: ExecutionStatus
-    l2_to_l1_messages: _containers.RepeatedCompositeFieldContainer[L2ToL1Message]
-    revert_reason: str
-    transaction_hash: _types_pb2.FieldElement
-    transaction_index: int
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        transaction_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        transaction_index: _Optional[int] = ...,
-        actual_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        l2_to_l1_messages: _Optional[_Iterable[_Union[L2ToL1Message, _Mapping]]] = ...,
-        events: _Optional[_Iterable[_Union[Event, _Mapping]]] = ...,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        execution_status: _Optional[_Union[ExecutionStatus, str]] = ...,
-        revert_reason: _Optional[str] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class TransactionWithReceipt(_message.Message):
-    __slots__ = ["receipt", "transaction"]
-    RECEIPT_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTION_FIELD_NUMBER: _ClassVar[int]
-    receipt: TransactionReceipt
-    transaction: Transaction
+class NonceUpdate(_message.Message):
+    __slots__ = ["contract_address", "nonce"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    NONCE_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    nonce: _types_pb2.FieldElement
     def __init__(
         self,
-        transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
-        receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class BlockStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class ResourcePrice(_message.Message):
+    __slots__ = ["price_in_fri", "price_in_wei"]
+    PRICE_IN_FRI_FIELD_NUMBER: _ClassVar[int]
+    PRICE_IN_WEI_FIELD_NUMBER: _ClassVar[int]
+    price_in_fri: _types_pb2.FieldElement
+    price_in_wei: _types_pb2.FieldElement
+    def __init__(
+        self,
+        price_in_fri: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        price_in_wei: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
 
-class ExecutionStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class FeePayment(_message.Message):
+    __slots__ = ["amount", "unit"]
+    AMOUNT_FIELD_NUMBER: _ClassVar[int]
+    UNIT_FIELD_NUMBER: _ClassVar[int]
+    amount: _types_pb2.FieldElement
+    unit: PriceUnit
+    def __init__(
+        self,
+        amount: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        unit: _Optional[_Union[PriceUnit, str]] = ...,
+    ) -> None: ...
+
+class ExecutionResources(_message.Message):
+    __slots__ = ["computation", "data_availability"]
+    COMPUTATION_FIELD_NUMBER: _ClassVar[int]
+    DATA_AVAILABILITY_FIELD_NUMBER: _ClassVar[int]
+    computation: ComputationResources
+    data_availability: DataAvailabilityResources
+    def __init__(
+        self,
+        computation: _Optional[_Union[ComputationResources, _Mapping]] = ...,
+        data_availability: _Optional[_Union[DataAvailabilityResources, _Mapping]] = ...,
+    ) -> None: ...
+
+class ComputationResources(_message.Message):
+    __slots__ = [
+        "steps",
+        "memory_holes",
+        "range_check_builtin_applications",
+        "pedersen_builtin_applications",
+        "poseidon_builtin_applications",
+        "ec_op_builtin_applications",
+        "ecdsa_builtin_applications",
+        "bitwise_builtin_applications",
+        "keccak_builtin_applications",
+        "segment_arena_builtin",
+    ]
+    STEPS_FIELD_NUMBER: _ClassVar[int]
+    MEMORY_HOLES_FIELD_NUMBER: _ClassVar[int]
+    RANGE_CHECK_BUILTIN_APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
+    PEDERSEN_BUILTIN_APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
+    POSEIDON_BUILTIN_APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
+    EC_OP_BUILTIN_APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
+    ECDSA_BUILTIN_APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
+    BITWISE_BUILTIN_APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
+    KECCAK_BUILTIN_APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
+    SEGMENT_ARENA_BUILTIN_FIELD_NUMBER: _ClassVar[int]
+    steps: int
+    memory_holes: int
+    range_check_builtin_applications: int
+    pedersen_builtin_applications: int
+    poseidon_builtin_applications: int
+    ec_op_builtin_applications: int
+    ecdsa_builtin_applications: int
+    bitwise_builtin_applications: int
+    keccak_builtin_applications: int
+    segment_arena_builtin: int
+    def __init__(
+        self,
+        steps: _Optional[int] = ...,
+        memory_holes: _Optional[int] = ...,
+        range_check_builtin_applications: _Optional[int] = ...,
+        pedersen_builtin_applications: _Optional[int] = ...,
+        poseidon_builtin_applications: _Optional[int] = ...,
+        ec_op_builtin_applications: _Optional[int] = ...,
+        ecdsa_builtin_applications: _Optional[int] = ...,
+        bitwise_builtin_applications: _Optional[int] = ...,
+        keccak_builtin_applications: _Optional[int] = ...,
+        segment_arena_builtin: _Optional[int] = ...,
+    ) -> None: ...
+
+class DataAvailabilityResources(_message.Message):
+    __slots__ = ["l1_gas", "l1_data_gas"]
+    L1_GAS_FIELD_NUMBER: _ClassVar[int]
+    L1_DATA_GAS_FIELD_NUMBER: _ClassVar[int]
+    l1_gas: int
+    l1_data_gas: int
+    def __init__(
+        self, l1_gas: _Optional[int] = ..., l1_data_gas: _Optional[int] = ...
+    ) -> None: ...
+
+class ResourceBoundsMapping(_message.Message):
+    __slots__ = ["l1_gas", "l2_gas"]
+    L1_GAS_FIELD_NUMBER: _ClassVar[int]
+    L2_GAS_FIELD_NUMBER: _ClassVar[int]
+    l1_gas: ResourceBounds
+    l2_gas: ResourceBounds
+    def __init__(
+        self,
+        l1_gas: _Optional[_Union[ResourceBounds, _Mapping]] = ...,
+        l2_gas: _Optional[_Union[ResourceBounds, _Mapping]] = ...,
+    ) -> None: ...
+
+class ResourceBounds(_message.Message):
+    __slots__ = ["max_amount", "max_price_per_unit"]
+    MAX_AMOUNT_FIELD_NUMBER: _ClassVar[int]
+    MAX_PRICE_PER_UNIT_FIELD_NUMBER: _ClassVar[int]
+    max_amount: int
+    max_price_per_unit: Uint128
+    def __init__(
+        self,
+        max_amount: _Optional[int] = ...,
+        max_price_per_unit: _Optional[_Union[Uint128, _Mapping]] = ...,
+    ) -> None: ...
+
+class Uint128(_message.Message):
+    __slots__ = ["low", "high"]
+    LOW_FIELD_NUMBER: _ClassVar[int]
+    HIGH_FIELD_NUMBER: _ClassVar[int]
+    low: int
+    high: int
+    def __init__(
+        self, low: _Optional[int] = ..., high: _Optional[int] = ...
+    ) -> None: ...
```

### Comparing `apibara-0.7.5/src/apibara/starknet/proto/types_pb2.pyi` & `apibara-0.8.0/src/apibara/starknet/proto/types_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import ClassVar as _ClassVar
-from typing import Optional as _Optional
-
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class FieldElement(_message.Message):
-    __slots__ = ["hi_hi", "hi_lo", "lo_hi", "lo_lo"]
-    HI_HI_FIELD_NUMBER: _ClassVar[int]
-    HI_LO_FIELD_NUMBER: _ClassVar[int]
-    LO_HI_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["lo_lo", "lo_hi", "hi_lo", "hi_hi"]
     LO_LO_FIELD_NUMBER: _ClassVar[int]
-    hi_hi: int
-    hi_lo: int
-    lo_hi: int
+    LO_HI_FIELD_NUMBER: _ClassVar[int]
+    HI_LO_FIELD_NUMBER: _ClassVar[int]
+    HI_HI_FIELD_NUMBER: _ClassVar[int]
     lo_lo: int
+    lo_hi: int
+    hi_lo: int
+    hi_hi: int
     def __init__(
         self,
         lo_lo: _Optional[int] = ...,
         lo_hi: _Optional[int] = ...,
         hi_lo: _Optional[int] = ...,
         hi_hi: _Optional[int] = ...,
     ) -> None: ...
```

### Comparing `apibara-0.7.5/PKG-INFO` & `apibara-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: apibara
-Version: 0.7.5
+Version: 0.8.0
 Summary: Apibara cliend SDK. Stream and transform on-chain data with Python.
 Home-page: https://www.apibara.com
 License: Apache-2.0
 Keywords: ethereum,web3,starknet
 Author: Francesco Ceccon
 Author-email: francesco@apibara.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: indexer
 Requires-Dist: grpcio (>=1.50,<2.0)
 Requires-Dist: protobuf (>=4.20,<5)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0) ; extra == "indexer"
 Project-URL: Repository, https://github.com/apibara/python-sdk
 Description-Content-Type: text/x-rst
```

