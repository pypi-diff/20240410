# Comparing `tmp/offchain-0.3.1.tar.gz` & `tmp/offchain-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offchain-0.3.1.tar", max compression
+gzip compressed data, was "offchain-0.3.2.tar", max compression
```

## Comparing `offchain-0.3.1.tar` & `offchain-0.3.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1066 2024-03-20 22:26:26.138195 offchain-0.3.1/LICENSE
--rw-r--r--   0        0        0     2805 2024-03-20 22:26:26.138195 offchain-0.3.1/README.md
--rw-r--r--   0        0        0      193 2024-03-20 22:26:26.138195 offchain-0.3.1/offchain/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.138195 offchain-0.3.1/offchain/base/__init__.py
--rw-r--r--   0        0        0       45 2024-03-20 22:26:26.138195 offchain-0.3.1/offchain/base/base_model.py
--rw-r--r--   0        0        0      486 2024-03-20 22:26:26.138195 offchain-0.3.1/offchain/base/types.py
--rw-r--r--   0        0        0     1891 2024-03-20 22:26:26.138195 offchain-0.3.1/offchain/concurrency.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/constants/__init__.py
--rw-r--r--   0        0        0     1061 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/constants/addresses.py
--rw-r--r--   0        0        0      183 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/constants/providers.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/logger/__init__.py
--rw-r--r--   0        0        0      417 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/logger/logging.py
--rw-r--r--   0        0        0      217 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/__init__.py
--rw-r--r--   0        0        0      264 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/adapters/__init__.py
--rw-r--r--   0        0        0     3627 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/adapters/arweave.py
--rw-r--r--   0        0        0     3084 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/adapters/base_adapter.py
--rw-r--r--   0        0        0     3105 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/adapters/data_uri.py
--rw-r--r--   0        0        0     1190 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/adapters/default_adapter_configs.py
--rw-r--r--   0        0        0      317 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/adapters/http_adapter.py
--rw-r--r--   0        0        0     5046 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/adapters/ipfs.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/constants/__init__.py
--rw-r--r--   0        0        0      359 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/constants/autoglyphs.py
--rw-r--r--   0        0        0     7181 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/constants/nouns.py
--rw-r--r--   0        0        0       84 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/fetchers/__init__.py
--rw-r--r--   0        0        0     2796 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/fetchers/base_fetcher.py
--rw-r--r--   0        0        0     7430 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/fetchers/metadata_fetcher.py
--rw-r--r--   0        0        0      642 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/get_token_metadata.py
--rw-r--r--   0        0        0      225 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/models/__init__.py
--rw-r--r--   0        0        0     3572 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/models/metadata.py
--rw-r--r--   0        0        0      844 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/models/metadata_processing_error.py
--rw-r--r--   0        0        0     1139 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/models/token.py
--rw-r--r--   0        0        0      867 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/__init__.py
--rw-r--r--   0        0        0     3168 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/catchall/__init__.py
--rw-r--r--   0        0        0      628 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/catchall/catchall_parser.py
--rw-r--r--   0        0        0     9961 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/catchall/default_catchall.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/__init__.py
--rw-r--r--   0        0        0    12276 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/artblocks.py
--rw-r--r--   0        0        0     8386 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/autoglyphs.py
--rw-r--r--   0        0        0     2786 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/chainrunners.py
--rw-r--r--   0        0        0     2112 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/collection_parser.py
--rw-r--r--   0        0        0     3875 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/decentraland.py
--rw-r--r--   0        0        0     7629 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/ens.py
--rw-r--r--   0        0        0     2769 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/foundation.py
--rw-r--r--   0        0        0     5651 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/hashmasks.py
--rw-r--r--   0        0        0     6284 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/loot.py
--rw-r--r--   0        0        0     5314 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/makersplace.py
--rw-r--r--   0        0        0     7188 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/nouns.py
--rw-r--r--   0        0        0     6495 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/punks.py
--rw-r--r--   0        0        0     6921 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/superrare.py
--rw-r--r--   0        0        0     6143 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/collection/zora.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/schema/__init__.py
--rw-r--r--   0        0        0     7747 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/schema/opensea.py
--rw-r--r--   0        0        0      713 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/parsers/schema/schema_parser.py
--rw-r--r--   0        0        0       88 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/pipelines/__init__.py
--rw-r--r--   0        0        0      248 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/pipelines/base_pipeline.py
--rw-r--r--   0        0        0    15052 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/pipelines/metadata_pipeline.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/registries/__init__.py
--rw-r--r--   0        0        0     1043 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/registries/adapter_registry.py
--rw-r--r--   0        0        0     1577 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/registries/base_registry.py
--rw-r--r--   0        0        0      907 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/registries/fetcher_registry.py
--rw-r--r--   0        0        0     2661 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/metadata/registries/parser_registry.py
--rw-r--r--   0        0        0     1350 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/utils/utils.py
--rw-r--r--   0        0        0        0 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/web3/__init__.py
--rw-r--r--   0        0        0     7277 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/web3/contract_caller.py
--rw-r--r--   0        0        0      531 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/web3/contract_utils.py
--rw-r--r--   0        0        0     3671 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/web3/jsonrpc.py
--rw-r--r--   0        0        0     9440 2024-03-20 22:26:26.142195 offchain-0.3.1/offchain/web3/read_async.py
--rw-r--r--   0        0        0      920 2024-03-20 22:26:26.142195 offchain-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 offchain-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-10 19:48:24.993478 offchain-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2805 2024-04-10 19:48:24.993478 offchain-0.3.2/README.md
+-rw-r--r--   0        0        0      193 2024-04-10 19:48:24.993478 offchain-0.3.2/offchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.993478 offchain-0.3.2/offchain/base/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-10 19:48:24.993478 offchain-0.3.2/offchain/base/base_model.py
+-rw-r--r--   0        0        0      486 2024-04-10 19:48:24.993478 offchain-0.3.2/offchain/base/types.py
+-rw-r--r--   0        0        0     1891 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/concurrency.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/constants/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/constants/addresses.py
+-rw-r--r--   0        0        0      183 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/constants/providers.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/logger/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/logger/logging.py
+-rw-r--r--   0        0        0      217 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/__init__.py
+-rw-r--r--   0        0        0      264 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/adapters/__init__.py
+-rw-r--r--   0        0        0     3627 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/adapters/arweave.py
+-rw-r--r--   0        0        0     3084 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/adapters/base_adapter.py
+-rw-r--r--   0        0        0     3292 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/adapters/data_uri.py
+-rw-r--r--   0        0        0     1190 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/adapters/default_adapter_configs.py
+-rw-r--r--   0        0        0      317 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/adapters/http_adapter.py
+-rw-r--r--   0        0        0     5046 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/adapters/ipfs.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/constants/__init__.py
+-rw-r--r--   0        0        0      359 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/constants/autoglyphs.py
+-rw-r--r--   0        0        0     7181 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/constants/nouns.py
+-rw-r--r--   0        0        0       84 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/fetchers/__init__.py
+-rw-r--r--   0        0        0     2796 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/fetchers/base_fetcher.py
+-rw-r--r--   0        0        0     7430 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/fetchers/metadata_fetcher.py
+-rw-r--r--   0        0        0      642 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/get_token_metadata.py
+-rw-r--r--   0        0        0      225 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/models/__init__.py
+-rw-r--r--   0        0        0     3572 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/models/metadata.py
+-rw-r--r--   0        0        0      844 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/models/metadata_processing_error.py
+-rw-r--r--   0        0        0     1139 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/models/token.py
+-rw-r--r--   0        0        0      867 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/__init__.py
+-rw-r--r--   0        0        0     3168 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/catchall/__init__.py
+-rw-r--r--   0        0        0      628 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/catchall/catchall_parser.py
+-rw-r--r--   0        0        0     9961 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/catchall/default_catchall.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/__init__.py
+-rw-r--r--   0        0        0    12276 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/artblocks.py
+-rw-r--r--   0        0        0     8386 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/autoglyphs.py
+-rw-r--r--   0        0        0     2786 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/chainrunners.py
+-rw-r--r--   0        0        0     2112 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/collection_parser.py
+-rw-r--r--   0        0        0     3875 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/decentraland.py
+-rw-r--r--   0        0        0     7629 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/ens.py
+-rw-r--r--   0        0        0     2769 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/foundation.py
+-rw-r--r--   0        0        0     5651 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/hashmasks.py
+-rw-r--r--   0        0        0     6284 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/loot.py
+-rw-r--r--   0        0        0     5314 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/makersplace.py
+-rw-r--r--   0        0        0     7188 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/nouns.py
+-rw-r--r--   0        0        0     6495 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/punks.py
+-rw-r--r--   0        0        0     6921 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/superrare.py
+-rw-r--r--   0        0        0     6143 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/collection/zora.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/schema/__init__.py
+-rw-r--r--   0        0        0     7747 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/schema/opensea.py
+-rw-r--r--   0        0        0      713 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/parsers/schema/schema_parser.py
+-rw-r--r--   0        0        0       88 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/pipelines/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/pipelines/base_pipeline.py
+-rw-r--r--   0        0        0    15052 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/pipelines/metadata_pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/registries/__init__.py
+-rw-r--r--   0        0        0     1043 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/registries/adapter_registry.py
+-rw-r--r--   0        0        0     1577 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/registries/base_registry.py
+-rw-r--r--   0        0        0      907 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/registries/fetcher_registry.py
+-rw-r--r--   0        0        0     2661 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/metadata/registries/parser_registry.py
+-rw-r--r--   0        0        0     1350 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/web3/__init__.py
+-rw-r--r--   0        0        0     7277 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/web3/contract_caller.py
+-rw-r--r--   0        0        0      531 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/web3/contract_utils.py
+-rw-r--r--   0        0        0     3671 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/web3/jsonrpc.py
+-rw-r--r--   0        0        0     9440 2024-04-10 19:48:24.997478 offchain-0.3.2/offchain/web3/read_async.py
+-rw-r--r--   0        0        0      920 2024-04-10 19:48:24.997478 offchain-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 offchain-0.3.2/PKG-INFO
```

### Comparing `offchain-0.3.1/LICENSE` & `offchain-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/README.md` & `offchain-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/concurrency.py` & `offchain-0.3.2/offchain/concurrency.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/constants/addresses.py` & `offchain-0.3.2/offchain/constants/addresses.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/adapters/arweave.py` & `offchain-0.3.2/offchain/metadata/adapters/arweave.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/adapters/base_adapter.py` & `offchain-0.3.2/offchain/metadata/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/adapters/data_uri.py` & `offchain-0.3.2/offchain/metadata/adapters/data_uri.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import base64
 from email.message import Message
 from urllib.request import urlopen
 
 import httpx
+import json
 from requests import PreparedRequest, Response
 
 from offchain.metadata.adapters.base_adapter import BaseAdapter
 from offchain.metadata.registries.adapter_registry import AdapterRegistry
 
 
 def decode_data_url(data_url):  # type: ignore[no-untyped-def]
     data_parts = data_url.split(",")
     data = data_parts[1]
 
     if ";base64" in data_parts[0]:
         decoded_data = base64.b64decode(data)
         decoded_text = decoded_data.decode("utf-8")
         return decoded_text
+    elif "json;utf8" in data_parts[0]:
+        decoded_data = urlopen(data_url).read()
+        decoded_text = json.dumps(json.loads(decoded_data))
+        return decoded_text
 
     return None
 
 
 @AdapterRegistry.register
 class DataURIAdapter(BaseAdapter):
     """Provides an interface for Requests sessions to handle data uris."""
```

### Comparing `offchain-0.3.1/offchain/metadata/adapters/default_adapter_configs.py` & `offchain-0.3.2/offchain/metadata/adapters/default_adapter_configs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/adapters/ipfs.py` & `offchain-0.3.2/offchain/metadata/adapters/ipfs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/constants/nouns.py` & `offchain-0.3.2/offchain/metadata/constants/nouns.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/fetchers/base_fetcher.py` & `offchain-0.3.2/offchain/metadata/fetchers/base_fetcher.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/fetchers/metadata_fetcher.py` & `offchain-0.3.2/offchain/metadata/fetchers/metadata_fetcher.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/get_token_metadata.py` & `offchain-0.3.2/offchain/metadata/get_token_metadata.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/models/metadata.py` & `offchain-0.3.2/offchain/metadata/models/metadata.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/models/metadata_processing_error.py` & `offchain-0.3.2/offchain/metadata/models/metadata_processing_error.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/models/token.py` & `offchain-0.3.2/offchain/metadata/models/token.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/__init__.py` & `offchain-0.3.2/offchain/metadata/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/base_parser.py` & `offchain-0.3.2/offchain/metadata/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/catchall/catchall_parser.py` & `offchain-0.3.2/offchain/metadata/parsers/catchall/catchall_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/catchall/default_catchall.py` & `offchain-0.3.2/offchain/metadata/parsers/catchall/default_catchall.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/artblocks.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/artblocks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/autoglyphs.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/autoglyphs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/chainrunners.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/chainrunners.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/collection_parser.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/collection_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/decentraland.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/decentraland.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/ens.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/ens.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/foundation.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/foundation.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/hashmasks.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/hashmasks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/loot.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/loot.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/makersplace.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/makersplace.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/nouns.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/nouns.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/punks.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/punks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/superrare.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/superrare.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/collection/zora.py` & `offchain-0.3.2/offchain/metadata/parsers/collection/zora.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/schema/opensea.py` & `offchain-0.3.2/offchain/metadata/parsers/schema/opensea.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/parsers/schema/schema_parser.py` & `offchain-0.3.2/offchain/metadata/parsers/schema/schema_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/pipelines/metadata_pipeline.py` & `offchain-0.3.2/offchain/metadata/pipelines/metadata_pipeline.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/registries/adapter_registry.py` & `offchain-0.3.2/offchain/metadata/registries/adapter_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/registries/base_registry.py` & `offchain-0.3.2/offchain/metadata/registries/base_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/registries/fetcher_registry.py` & `offchain-0.3.2/offchain/metadata/registries/fetcher_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/metadata/registries/parser_registry.py` & `offchain-0.3.2/offchain/metadata/registries/parser_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/utils/utils.py` & `offchain-0.3.2/offchain/utils/utils.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/web3/contract_caller.py` & `offchain-0.3.2/offchain/web3/contract_caller.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/web3/contract_utils.py` & `offchain-0.3.2/offchain/web3/contract_utils.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/web3/jsonrpc.py` & `offchain-0.3.2/offchain/web3/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/offchain/web3/read_async.py` & `offchain-0.3.2/offchain/web3/read_async.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.1/pyproject.toml` & `offchain-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "offchain"
-version = "0.3.1"
+version = "0.3.2"
 description = "Open source metadata processing framework"
 authors = ["Zora eng <eng@zora.co>"]
 readme = "README.md"
 documentation = "https://ourzora.github.io/offchain"
 
 [tool.poetry.dependencies]
 python = ">=3.9 <4"
```

### Comparing `offchain-0.3.1/PKG-INFO` & `offchain-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offchain
-Version: 0.3.1
+Version: 0.3.2
 Summary: Open source metadata processing framework
 Author: Zora eng
 Author-email: eng@zora.co
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

