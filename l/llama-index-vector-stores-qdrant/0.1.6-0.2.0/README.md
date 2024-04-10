# Comparing `tmp/llama_index_vector_stores_qdrant-0.1.6.tar.gz` & `tmp/llama_index_vector_stores_qdrant-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_qdrant-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_qdrant-0.2.0.tar", max compression
```

## Comparing `llama_index_vector_stores_qdrant-0.1.6.tar` & `llama_index_vector_stores_qdrant-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/README.md
--rw-r--r--   0        0        0      101 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/__init__.py
--rw-r--r--   0        0        0    31682 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/base.py
--rw-r--r--   0        0        0     6897 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/utils.py
--rw-r--r--   0        0        0     1600 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/README.md
+-rw-r--r--   0        0        0      101 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0    33618 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/base.py
+-rw-r--r--   0        0        0     6897 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/utils.py
+-rw-r--r--   0        0        0     1600 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.2.0/PKG-INFO
```

### Comparing `llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/base.py` & `llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     node_to_metadata_dict,
 )
 from llama_index.vector_stores.qdrant.utils import (
     HybridFusionCallable,
     SparseEncoderCallable,
     default_sparse_encoder,
     relative_score_fusion,
+    fastembed_sparse_encoder,
 )
 from qdrant_client.http import models as rest
 from qdrant_client.http.exceptions import UnexpectedResponse
 from qdrant_client.http.models import (
     FieldCondition,
     Filter,
     MatchAny,
@@ -45,14 +46,18 @@
 )
 
 logger = logging.getLogger(__name__)
 import_err_msg = (
     "`qdrant-client` package not found, please run `pip install qdrant-client`"
 )
 
+DENSE_VECTOR_NAME = "text-dense"
+SPARSE_VECTOR_NAME_OLD = "text-sparse"
+SPARSE_VECTOR_NAME = "text-sparse-new"
+
 
 class QdrantVectorStore(BasePydanticVectorStore):
     """
     Qdrant Vector Store.
 
     In this vector store, embeddings and docs are stored within a
     Qdrant collection.
@@ -159,19 +164,20 @@
             self._collection_initialized = self._collection_exists(collection_name)
         else:
             #  need to do lazy init for async clients
             self._collection_initialized = False
 
         # setup hybrid search if enabled
         if enable_hybrid:
-            self._sparse_doc_fn = sparse_doc_fn or default_sparse_encoder(
-                "naver/efficient-splade-VI-BT-large-doc"
+            self._sparse_doc_fn = sparse_doc_fn or self.get_default_sparse_doc_encoder(
+                collection_name
             )
-            self._sparse_query_fn = sparse_query_fn or default_sparse_encoder(
-                "naver/efficient-splade-VI-BT-large-query"
+            self._sparse_query_fn = (
+                sparse_query_fn
+                or self.get_default_sparse_query_encoder(collection_name)
             )
             self._hybrid_fusion_fn = hybrid_fusion_fn or cast(
                 HybridFusionCallable, relative_score_fusion
             )
 
         super().__init__(
             collection_name=collection_name,
@@ -224,25 +230,26 @@
                     if (
                         len(sparse_vectors) > 0
                         and len(sparse_indices) > 0
                         and len(sparse_vectors) == len(sparse_indices)
                     ):
                         vectors.append(
                             {
-                                "text-sparse": rest.SparseVector(
+                                # Dynamically switch between the old and new sparse vector name
+                                self.sparse_vector_name: rest.SparseVector(
                                     indices=sparse_indices[i],
                                     values=sparse_vectors[i],
                                 ),
-                                "text-dense": node.get_embedding(),
+                                DENSE_VECTOR_NAME: node.get_embedding(),
                             }
                         )
                     else:
                         vectors.append(
                             {
-                                "text-dense": node.get_embedding(),
+                                DENSE_VECTOR_NAME: node.get_embedding(),
                             }
                         )
                 else:
                     vectors.append(node.get_embedding())
 
                 metadata = node_to_metadata_dict(
                     node, remove_text=False, flat_metadata=self.flat_metadata
@@ -371,21 +378,22 @@
         from qdrant_client.http.exceptions import UnexpectedResponse
 
         try:
             if self.enable_hybrid:
                 self._client.create_collection(
                     collection_name=collection_name,
                     vectors_config={
-                        "text-dense": rest.VectorParams(
+                        DENSE_VECTOR_NAME: rest.VectorParams(
                             size=vector_size,
                             distance=rest.Distance.COSINE,
                         )
                     },
+                    # Newly created collection will have the new sparse vector name
                     sparse_vectors_config={
-                        "text-sparse": rest.SparseVectorParams(
+                        SPARSE_VECTOR_NAME: rest.SparseVectorParams(
                             index=rest.SparseIndexParams()
                         )
                     },
                 )
             else:
                 self._client.create_collection(
                     collection_name=collection_name,
@@ -409,21 +417,21 @@
         from qdrant_client.http.exceptions import UnexpectedResponse
 
         try:
             if self.enable_hybrid:
                 await self._aclient.create_collection(
                     collection_name=collection_name,
                     vectors_config={
-                        "text-dense": rest.VectorParams(
+                        DENSE_VECTOR_NAME: rest.VectorParams(
                             size=vector_size,
                             distance=rest.Distance.COSINE,
                         )
                     },
                     sparse_vectors_config={
-                        "text-sparse": rest.SparseVectorParams(
+                        SPARSE_VECTOR_NAME: rest.SparseVectorParams(
                             index=rest.SparseIndexParams()
                         )
                     },
                 )
             else:
                 await self._aclient.create_collection(
                     collection_name=collection_name,
@@ -493,24 +501,25 @@
             sparse_top_k = query.sparse_top_k or query.similarity_top_k
 
             sparse_response = self._client.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedVector(
-                            name="text-dense",
+                            name=DENSE_VECTOR_NAME,
                             vector=query_embedding,
                         ),
                         limit=query.similarity_top_k,
                         filter=query_filter,
                         with_payload=True,
                     ),
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
-                            name="text-sparse",
+                            # Dynamically switch between the old and new sparse vector name
+                            name=self.sparse_vector_name,
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -544,15 +553,16 @@
             sparse_top_k = query.sparse_top_k or query.similarity_top_k
 
             sparse_response = self._client.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
-                            name="text-sparse",
+                            # Dynamically switch between the old and new sparse vector name
+                            name=self.sparse_vector_name,
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -565,15 +575,15 @@
         elif self.enable_hybrid:
             # search for dense vectors only
             response = self._client.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedVector(
-                            name="text-dense",
+                            name=DENSE_VECTOR_NAME,
                             vector=query_embedding,
                         ),
                         limit=query.similarity_top_k,
                         filter=query_filter,
                         with_payload=True,
                     ),
                 ],
@@ -625,24 +635,25 @@
             sparse_top_k = query.sparse_top_k or query.similarity_top_k
 
             sparse_response = await self._aclient.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedVector(
-                            name="text-dense",
+                            name=DENSE_VECTOR_NAME,
                             vector=query_embedding,
                         ),
                         limit=query.similarity_top_k,
                         filter=query_filter,
                         with_payload=True,
                     ),
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
-                            name="text-sparse",
+                            # Dynamically switch between the old and new sparse vector name
+                            name=self.sparse_vector_name,
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -675,15 +686,16 @@
             sparse_top_k = query.sparse_top_k or query.similarity_top_k
 
             sparse_response = await self._aclient.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
-                            name="text-sparse",
+                            # Dynamically switch between the old and new sparse vector name
+                            name=self.sparse_vector_name,
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -695,15 +707,15 @@
         elif self.enable_hybrid:
             # search for dense vectors only
             response = await self._aclient.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedVector(
-                            name="text-dense",
+                            name=DENSE_VECTOR_NAME,
                             vector=query_embedding,
                         ),
                         limit=query.similarity_top_k,
                         filter=query_filter,
                         with_payload=True,
                     ),
                 ],
@@ -853,7 +865,38 @@
                     FieldCondition(
                         key=subfilter.key,
                         match=MatchAny(any=str(subfilter.value).split(",")),
                     )
                 )
 
         return Filter(must=must_conditions)
+
+    def use_old_sparse_encoder(self, collection_name: str) -> bool:
+        return (
+            self._collection_exists(collection_name)
+            and SPARSE_VECTOR_NAME_OLD
+            in self.client.get_collection(collection_name).config.params.vectors
+        )
+
+    @property
+    def sparse_vector_name(self) -> str:
+        return (
+            SPARSE_VECTOR_NAME_OLD
+            if self.use_old_sparse_encoder(self.collection_name)
+            else SPARSE_VECTOR_NAME
+        )
+
+    def get_default_sparse_doc_encoder(
+        self, collection_name: str
+    ) -> SparseEncoderCallable:
+        if self.use_old_sparse_encoder(collection_name):
+            return default_sparse_encoder("naver/efficient-splade-VI-BT-large-doc")
+
+        return fastembed_sparse_encoder(model_name="prithvida/Splade_PP_en_v1")
+
+    def get_default_sparse_query_encoder(
+        self, collection_name: str
+    ) -> SparseEncoderCallable:
+        if self.use_old_sparse_encoder(collection_name):
+            return default_sparse_encoder("naver/efficient-splade-VI-BT-large-query")
+
+        return fastembed_sparse_encoder(model_name="prithvida/Splade_PP_en_v1")
```

### Comparing `llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/utils.py` & `llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_qdrant-0.1.6/pyproject.toml` & `llama_index_vector_stores_qdrant-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores qdrant integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-qdrant"
 readme = "README.md"
-version = "0.1.6"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 llama-index-core = "^0.10.1"
 qdrant-client = "^1.7.1"
 grpcio = "^1.60.0"
```

### Comparing `llama_index_vector_stores_qdrant-0.1.6/PKG-INFO` & `llama_index_vector_stores_qdrant-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-qdrant
-Version: 0.1.6
+Version: 0.2.0
 Summary: llama-index vector_stores qdrant integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

