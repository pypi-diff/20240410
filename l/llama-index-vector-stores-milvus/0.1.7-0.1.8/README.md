# Comparing `tmp/llama_index_vector_stores_milvus-0.1.7.tar.gz` & `tmp/llama_index_vector_stores_milvus-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_milvus-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_milvus-0.1.8.tar", max compression
```

## Comparing `llama_index_vector_stores_milvus-0.1.7.tar` & `llama_index_vector_stores_milvus-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       47 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/README.md
--rw-r--r--   0        0        0      101 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/llama_index/vector_stores/milvus/__init__.py
--rw-r--r--   0        0        0    13737 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/llama_index/vector_stores/milvus/base.py
--rw-r--r--   0        0        0     1479 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_milvus-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/README.md
+-rw-r--r--   0        0        0      101 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/llama_index/vector_stores/milvus/__init__.py
+-rw-r--r--   0        0        0    13964 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/llama_index/vector_stores/milvus/base.py
+-rw-r--r--   0        0        0     1479 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_milvus-0.1.8/PKG-INFO
```

### Comparing `llama_index_vector_stores_milvus-0.1.7/llama_index/vector_stores/milvus/base.py` & `llama_index_vector_stores_milvus-0.1.8/llama_index/vector_stores/milvus/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 
 import logging
 from typing import Any, Dict, List, Optional, Union
 
 import pymilvus  # noqa
-from llama_index.core.bridge.pydantic import PrivateAttr
+from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.schema import BaseNode, TextNode
 from llama_index.core.vector_stores.types import (
     BasePydanticVectorStore,
     MetadataFilters,
     VectorStoreQuery,
     VectorStoreQueryMode,
     VectorStoreQueryResult,
@@ -111,14 +111,15 @@
     dim: Optional[int]
     embedding_field: str = DEFAULT_EMBEDDING_KEY
     doc_id_field: str = DEFAULT_DOC_ID_KEY
     similarity_metric: str = "IP"
     consistency_level: str = "Strong"
     overwrite: bool = False
     text_key: Optional[str]
+    output_fields: List[str] = Field(default_factory=list)
     index_config: Optional[dict]
     search_config: Optional[dict]
 
     _milvusclient: MilvusClient = PrivateAttr()
     _collection: Any = PrivateAttr()
 
     def __init__(
@@ -129,27 +130,29 @@
         dim: Optional[int] = None,
         embedding_field: str = DEFAULT_EMBEDDING_KEY,
         doc_id_field: str = DEFAULT_DOC_ID_KEY,
         similarity_metric: str = "IP",
         consistency_level: str = "Strong",
         overwrite: bool = False,
         text_key: Optional[str] = None,
+        output_fields: Optional[List[str]] = None,
         index_config: Optional[dict] = None,
         search_config: Optional[dict] = None,
         **kwargs: Any,
     ) -> None:
         """Init params."""
         super().__init__(
             collection_name=collection_name,
             dim=dim,
             embedding_field=embedding_field,
             doc_id_field=doc_id_field,
             consistency_level=consistency_level,
             overwrite=overwrite,
             text_key=text_key,
+            output_fields=output_fields,
             index_config=index_config if index_config else {},
             search_config=search_config if search_config else {},
         )
 
         # Select the similarity metric
         similarity_metrics_map = {
             "ip": "IP",
@@ -332,17 +335,18 @@
                 try:
                     text = hit["entity"].get(self.text_key)
                 except Exception:
                     raise ValueError(
                         "The passed in text_key value does not exist "
                         "in the retrieved entity."
                     )
-                node = TextNode(
-                    text=text,
-                )
+
+                metadata = {key: hit["entity"].get(key) for key in self.output_fields}
+                node = TextNode(text=text, metadata=metadata)
+
             nodes.append(node)
             similarities.append(hit["distance"])
             ids.append(hit["id"])
 
         return VectorStoreQueryResult(nodes=nodes, similarities=similarities, ids=ids)
 
     def _create_index_if_required(self, force: bool = False) -> None:
```

### Comparing `llama_index_vector_stores_milvus-0.1.7/pyproject.toml` & `llama_index_vector_stores_milvus-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores milvus integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-milvus"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymilvus = "^2.3.6"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_milvus-0.1.7/PKG-INFO` & `llama_index_vector_stores_milvus-0.1.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-milvus
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index vector_stores milvus integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

