# Comparing `tmp/stac-fastapi.elasticsearch-2.1.0.tar.gz` & `tmp/stac-fastapi.elasticsearch-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.elasticsearch-2.1.0.tar", last modified: Sun Mar  3 15:08:46 2024, max compression
+gzip compressed data, was "stac-fastapi.elasticsearch-2.2.0.tar", last modified: Wed Apr 10 17:05:00 2024, max compression
```

## Comparing `stac-fastapi.elasticsearch-2.1.0.tar` & `stac-fastapi.elasticsearch-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:08:46.092813 stac-fastapi.elasticsearch-2.1.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1516 2024-03-03 15:08:46.092464 stac-fastapi.elasticsearch-2.1.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)       70 2024-01-31 03:57:09.000000 stac-fastapi.elasticsearch-2.1.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-03-03 15:08:46.096058 stac-fastapi.elasticsearch-2.1.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1725 2024-03-03 15:07:57.000000 stac-fastapi.elasticsearch-2.1.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:08:46.062474 stac-fastapi.elasticsearch-2.1.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:08:46.084016 stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2866 2024-02-08 06:37:21.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2432 2024-02-08 06:37:21.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    32590 2024-03-03 14:50:31.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-03-03 14:50:31.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:08:46.085245 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1516 2024-03-03 15:08:46.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-03-03 15:08:46.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-03-03 15:08:46.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-03-03 15:08:46.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      246 2024-03-03 15:08:46.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-03-03 15:08:46.000000 stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.447975 stac-fastapi.elasticsearch-2.2.0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-04-10 17:05:00.447598 stac-fastapi.elasticsearch-2.2.0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      101 2024-03-19 04:19:17.000000 stac-fastapi.elasticsearch-2.2.0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-04-10 17:05:00.449683 stac-fastapi.elasticsearch-2.2.0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1725 2024-04-10 15:59:17.000000 stac-fastapi.elasticsearch-2.2.0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.380576 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.442039 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3212 2024-04-09 14:42:19.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2405 2024-04-09 14:42:19.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    33316 2024-03-19 04:19:17.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-04-10 15:56:09.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.444141 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      246 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/top_level.txt
```

### Comparing `stac-fastapi.elasticsearch-2.1.0/PKG-INFO` & `stac-fastapi.elasticsearch-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.elasticsearch
-Version: 2.1.0
+Version: 2.2.0
 Summary: An implementation of STAC API based on the FastAPI framework with both Elasticsearch and Opensearch.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: stac-fastapi.core==2.1.0
+Requires-Dist: stac-fastapi.core==2.2.0
 Requires-Dist: elasticsearch[async]==8.11.0
 Requires-Dist: elasticsearch-dsl==8.11.0
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -30,10 +30,12 @@
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]==0.19.0; extra == "server"
 
-# Requirements
+# stac-fastapi-elasticsearch
+
+## Requirements
 
 The Elasticsearch backend requires **elasticsearch**.
```

### Comparing `stac-fastapi.elasticsearch-2.1.0/setup.py` & `stac-fastapi.elasticsearch-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.1.0",
+    "stac-fastapi.core==2.2.0",
     "elasticsearch[async]==8.11.0",
     "elasticsearch-dsl==8.11.0",
     "uvicorn",
     "starlette",
 ]
 
 extra_reqs = {
```

### Comparing `stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/app.py` & `stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """FastAPI application."""
 
+import os
+
 from stac_fastapi.api.app import StacApi
 from stac_fastapi.api.models import create_get_request_model, create_post_request_model
 from stac_fastapi.core.core import (
     BulkTransactionsClient,
     CoreClient,
     EsAsyncBaseFiltersClient,
     TransactionsClient,
 )
 from stac_fastapi.core.extensions import QueryExtension
 from stac_fastapi.core.session import Session
 from stac_fastapi.elasticsearch.config import ElasticsearchSettings
 from stac_fastapi.elasticsearch.database_logic import (
     DatabaseLogic,
     create_collection_index,
+    create_index_templates,
 )
 from stac_fastapi.extensions.core import (
     ContextExtension,
     FieldsExtension,
     FilterExtension,
     SortExtension,
     TokenPaginationExtension,
@@ -56,27 +59,32 @@
     ContextExtension(),
     filter_extension,
 ]
 
 post_request_model = create_post_request_model(extensions)
 
 api = StacApi(
+    title=os.getenv("STAC_FASTAPI_TITLE", "stac-fastapi-elasticsearch"),
+    description=os.getenv("STAC_FASTAPI_DESCRIPTION", "stac-fastapi-elasticsearch"),
+    api_version=os.getenv("STAC_FASTAPI_VERSION", "2.1"),
     settings=settings,
     extensions=extensions,
     client=CoreClient(
         database=database_logic, session=session, post_request_model=post_request_model
     ),
     search_get_request_model=create_get_request_model(extensions),
     search_post_request_model=post_request_model,
 )
 app = api.app
+app.root_path = os.getenv("STAC_FASTAPI_ROOT_PATH", "")
 
 
 @app.on_event("startup")
 async def _startup_event() -> None:
+    await create_index_templates()
     await create_collection_index()
 
 
 def run() -> None:
     """Run app from command line using uvicorn if available."""
     try:
         import uvicorn
```

### Comparing `stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/config.py` & `stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """API configuration."""
 import os
 import ssl
 from typing import Any, Dict, Set
 
+import certifi
+
 from elasticsearch import AsyncElasticsearch, Elasticsearch  # type: ignore
 from stac_fastapi.types.config import ApiSettings
 
 
 def _es_config() -> Dict[str, Any]:
     # Determine the scheme (http or https)
     use_ssl = os.getenv("ES_USE_SSL", "true").lower() == "true"
@@ -27,17 +29,15 @@
 
     # Include SSL settings if using https
     config["ssl_version"] = ssl.TLSVersion.TLSv1_3  # type: ignore
     config["verify_certs"] = os.getenv("ES_VERIFY_CERTS", "true").lower() != "false"  # type: ignore
 
     # Include CA Certificates if verifying certs
     if config["verify_certs"]:
-        config["ca_certs"] = os.getenv(
-            "CURL_CA_BUNDLE", "/etc/ssl/certs/ca-certificates.crt"
-        )
+        config["ca_certs"] = os.getenv("CURL_CA_BUNDLE", certifi.where())
 
     # Handle authentication
     if (u := os.getenv("ES_USER")) and (p := os.getenv("ES_PASS")):
         config["http_auth"] = (u, p)
 
     if api_key := os.getenv("ES_API_KEY"):
         if isinstance(config["headers"], dict):
```

### Comparing `stac-fastapi.elasticsearch-2.1.0/stac_fastapi/elasticsearch/database_logic.py` & `stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/database_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,51 +167,75 @@
     """
     if collection_ids is None:
         return ITEM_INDICES
     else:
         return ",".join([index_by_collection_id(c) for c in collection_ids])
 
 
+async def create_index_templates() -> None:
+    """
+    Create index templates for the Collection and Item indices.
+
+    Returns:
+        None
+
+    """
+    client = AsyncElasticsearchSettings().create_client
+    await client.indices.put_template(
+        name=f"template_{COLLECTIONS_INDEX}",
+        body={
+            "index_patterns": [f"{COLLECTIONS_INDEX}*"],
+            "mappings": ES_COLLECTIONS_MAPPINGS,
+        },
+    )
+    await client.indices.put_template(
+        name=f"template_{ITEMS_INDEX_PREFIX}",
+        body={
+            "index_patterns": [f"{ITEMS_INDEX_PREFIX}*"],
+            "settings": ES_ITEMS_SETTINGS,
+            "mappings": ES_ITEMS_MAPPINGS,
+        },
+    )
+    await client.close()
+
+
 async def create_collection_index() -> None:
     """
-    Create the index for a Collection.
+    Create the index for a Collection. The settings of the index template will be used implicitly.
 
     Returns:
         None
 
     """
     client = AsyncElasticsearchSettings().create_client
 
     await client.options(ignore_status=400).indices.create(
         index=f"{COLLECTIONS_INDEX}-000001",
         aliases={COLLECTIONS_INDEX: {}},
-        mappings=ES_COLLECTIONS_MAPPINGS,
     )
     await client.close()
 
 
 async def create_item_index(collection_id: str):
     """
-    Create the index for Items.
+    Create the index for Items. The settings of the index template will be used implicitly.
 
     Args:
         collection_id (str): Collection identifier.
 
     Returns:
         None
 
     """
     client = AsyncElasticsearchSettings().create_client
     index_name = index_by_collection_id(collection_id)
 
     await client.options(ignore_status=400).indices.create(
         index=f"{index_by_collection_id(collection_id)}-000001",
         aliases={index_name: {}},
-        mappings=ES_ITEMS_MAPPINGS,
-        settings=ES_ITEMS_SETTINGS,
     )
     await client.close()
 
 
 async def delete_item_index(collection_id: str):
     """Delete the index for items in a collection.
```

### Comparing `stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO` & `stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.elasticsearch
-Version: 2.1.0
+Version: 2.2.0
 Summary: An implementation of STAC API based on the FastAPI framework with both Elasticsearch and Opensearch.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: stac-fastapi.core==2.1.0
+Requires-Dist: stac-fastapi.core==2.2.0
 Requires-Dist: elasticsearch[async]==8.11.0
 Requires-Dist: elasticsearch-dsl==8.11.0
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -30,10 +30,12 @@
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]==0.19.0; extra == "server"
 
-# Requirements
+# stac-fastapi-elasticsearch
+
+## Requirements
 
 The Elasticsearch backend requires **elasticsearch**.
```

### Comparing `stac-fastapi.elasticsearch-2.1.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt` & `stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

