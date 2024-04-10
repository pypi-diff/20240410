# Comparing `tmp/fastembed_haystack-0.0.6.tar.gz` & `tmp/fastembed_haystack-0.1.0.tar.gz`

## Comparing `fastembed_haystack-0.0.6.tar` & `fastembed_haystack-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,21 @@
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/example/example.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/pydoc/config.yml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/__init__.py
--rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/embedding_backend/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/tests/test_fastembed_backend.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/tests/test_fastembed_document_embedder.py
--rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/tests/test_fastembed_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/README.md
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 fastembed_haystack-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/examples/example.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/examples/sparse_example.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/pydoc/config.yml
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/__init__.py
+-rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/__init__.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_backend.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_document_embedder.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_sparse_document_embedder.py
+-rw-r--r--   0        0        0     8779 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_sparse_text_embedder.py
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/README.md
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/PKG-INFO
```

### Comparing `fastembed_haystack-0.0.6/example/example.py` & `fastembed_haystack-0.1.0/examples/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 query_pipeline.add_component("retriever", InMemoryEmbeddingRetriever(document_store=document_store))
 query_pipeline.connect("text_embedder.embedding", "retriever.query_embedding")
 
 query = "Who supports fastembed?"
 
 result = query_pipeline.run({"text_embedder": {"text": query}})
 
-print(result["retriever"]["documents"][0])  # noqa: T201
+print(result["retriever"]["documents"][0])
 
 # Document(id=...,
 #  content: 'fastembed is supported by and maintained by Qdrant.',
 #  score: 0.758..)
```

### Comparing `fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py` & `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py` & `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.0.6/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py` & `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import ClassVar, Dict, List, Optional
 
+from haystack.dataclasses.sparse_embedding import SparseEmbedding
 from tqdm import tqdm
 
 from fastembed import TextEmbedding
+from fastembed.sparse.sparse_text_embedding import SparseTextEmbedding
 
 
 class _FastembedEmbeddingBackendFactory:
     """
     Factory class to create instances of fastembed embedding backends.
     """
 
@@ -46,7 +48,62 @@
         embeddings = []
         embeddings_iterable = self.model.embed(data, **kwargs)
         for np_array in tqdm(
             embeddings_iterable, disable=not progress_bar, desc="Calculating embeddings", total=len(data)
         ):
             embeddings.append(np_array.tolist())
         return embeddings
+
+
+class _FastembedSparseEmbeddingBackendFactory:
+    """
+    Factory class to create instances of fastembed sparse embedding backends.
+    """
+
+    _instances: ClassVar[Dict[str, "_FastembedSparseEmbeddingBackend"]] = {}
+
+    @staticmethod
+    def get_embedding_backend(
+        model_name: str,
+        cache_dir: Optional[str] = None,
+        threads: Optional[int] = None,
+    ):
+        embedding_backend_id = f"{model_name}{cache_dir}{threads}"
+
+        if embedding_backend_id in _FastembedSparseEmbeddingBackendFactory._instances:
+            return _FastembedSparseEmbeddingBackendFactory._instances[embedding_backend_id]
+
+        embedding_backend = _FastembedSparseEmbeddingBackend(
+            model_name=model_name, cache_dir=cache_dir, threads=threads
+        )
+        _FastembedSparseEmbeddingBackendFactory._instances[embedding_backend_id] = embedding_backend
+        return embedding_backend
+
+
+class _FastembedSparseEmbeddingBackend:
+    """
+    Class to manage fastembed sparse embeddings.
+    """
+
+    def __init__(
+        self,
+        model_name: str,
+        cache_dir: Optional[str] = None,
+        threads: Optional[int] = None,
+    ):
+        self.model = SparseTextEmbedding(model_name=model_name, cache_dir=cache_dir, threads=threads)
+
+    def embed(self, data: List[List[str]], progress_bar=True, **kwargs) -> List[SparseEmbedding]:
+        # The embed method returns a Iterable[SparseEmbedding], so we convert to Haystack SparseEmbedding type.
+        # Each SparseEmbedding contains an `indices` key containing a list of int and
+        # an `values` key containing a list of floats.
+
+        sparse_embeddings = []
+        sparse_embeddings_iterable = self.model.embed(data, **kwargs)
+        for sparse_embedding in tqdm(
+            sparse_embeddings_iterable, disable=not progress_bar, desc="Calculating sparse embeddings", total=len(data)
+        ):
+            sparse_embeddings.append(
+                SparseEmbedding(indices=sparse_embedding.indices.tolist(), values=sparse_embedding.values.tolist())
+            )
+
+        return sparse_embeddings
```

### Comparing `fastembed_haystack-0.0.6/tests/test_fastembed_backend.py` & `fastembed_haystack-0.1.0/tests/test_fastembed_backend.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.0.6/tests/test_fastembed_document_embedder.py` & `fastembed_haystack-0.1.0/tests/test_fastembed_document_embedder.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.0.6/tests/test_fastembed_text_embedder.py` & `fastembed_haystack-0.1.0/tests/test_fastembed_text_embedder.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.0.6/.gitignore` & `fastembed_haystack-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.0.6/LICENSE.txt` & `fastembed_haystack-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.0.6/README.md` & `fastembed_haystack-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -39,10 +39,35 @@
     model="BAAI/bge-small-en-v1.5",
 )
 embedder.warm_up()
 doc = Document(content="fastembed is supported by and maintained by Qdrant.", meta={"long_answer": "no",})
 result = embedder.run(documents=[doc])
 ```
 
+You can use `FastembedSparseTextEmbedder` and `FastembedSparseDocumentEmbedder` by importing as:
+
+```python
+from haystack_integrations.components.embedders.fastembed import FastembedSparseTextEmbedder
+
+text = "fastembed is supported by and maintained by Qdrant."
+text_embedder = FastembedSparseTextEmbedder(
+    model="prithvida/Splade_PP_en_v1"
+)
+text_embedder.warm_up()
+embedding = text_embedder.run(text)["embedding"]
+```
+
+```python
+from haystack_integrations.components.embedders.fastembed import FastembedSparseDocumentEmbedder
+from haystack.dataclasses import Document
+
+embedder = FastembedSparseDocumentEmbedder(
+    model="prithvida/Splade_PP_en_v1",
+)
+embedder.warm_up()
+doc = Document(content="fastembed is supported by and maintained by Qdrant.", meta={"long_answer": "no",})
+result = embedder.run(documents=[doc])
+```
+
 ## License
 
 `fastembed-haystack` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
```

### Comparing `fastembed_haystack-0.0.6/pyproject.toml` & `fastembed_haystack-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-"haystack-ai",
-"fastembed>=0.2",
+"haystack-ai>=2.0.1",
+"fastembed>=0.2.5",
 ]
 
 [project.urls]
 Source = "https://github.com/deepset-ai/haystack-core-integrations"
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/fastembed/README.md"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 
@@ -91,20 +91,20 @@
 ]
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -151,15 +151,15 @@
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "parents"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 # examples can contain "print" commands
-"examples/**/*" = ["T201"]
+"examples/**/*" = ["T201", "E501"]
 
 [tool.coverage.run]
 source = ["haystack_integrations"]
 branch = true
 parallel = false
 
 [tool.coverage.report]
```

### Comparing `fastembed_haystack-0.0.6/PKG-INFO` & `fastembed_haystack-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastembed-haystack
-Version: 0.0.6
+Version: 0.1.0
 Summary: Haystack 2.x component to embed strings and Documents using fastembed embedding model
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/fastembed/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: fastembed>=0.2
-Requires-Dist: haystack-ai
+Requires-Dist: fastembed>=0.2.5
+Requires-Dist: haystack-ai>=2.0.1
 Description-Content-Type: text/markdown
 
 # fastembed-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/fastembed-haystack.svg)](https://pypi.org/project/fastembed-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastembed-haystack.svg)](https://pypi.org/project/fastembed-haystack)
 
@@ -63,10 +63,35 @@
     model="BAAI/bge-small-en-v1.5",
 )
 embedder.warm_up()
 doc = Document(content="fastembed is supported by and maintained by Qdrant.", meta={"long_answer": "no",})
 result = embedder.run(documents=[doc])
 ```
 
+You can use `FastembedSparseTextEmbedder` and `FastembedSparseDocumentEmbedder` by importing as:
+
+```python
+from haystack_integrations.components.embedders.fastembed import FastembedSparseTextEmbedder
+
+text = "fastembed is supported by and maintained by Qdrant."
+text_embedder = FastembedSparseTextEmbedder(
+    model="prithvida/Splade_PP_en_v1"
+)
+text_embedder.warm_up()
+embedding = text_embedder.run(text)["embedding"]
+```
+
+```python
+from haystack_integrations.components.embedders.fastembed import FastembedSparseDocumentEmbedder
+from haystack.dataclasses import Document
+
+embedder = FastembedSparseDocumentEmbedder(
+    model="prithvida/Splade_PP_en_v1",
+)
+embedder.warm_up()
+doc = Document(content="fastembed is supported by and maintained by Qdrant.", meta={"long_answer": "no",})
+result = embedder.run(documents=[doc])
+```
+
 ## License
 
 `fastembed-haystack` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
```

