# Comparing `tmp/stac-fastapi.opensearch-2.1.0.tar.gz` & `tmp/stac-fastapi.opensearch-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.opensearch-2.1.0.tar", last modified: Sun Mar  3 15:10:18 2024, max compression
+gzip compressed data, was "stac-fastapi.opensearch-2.2.0.tar", last modified: Wed Apr 10 17:06:38 2024, max compression
```

## Comparing `stac-fastapi.opensearch-2.1.0.tar` & `stac-fastapi.opensearch-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:10:18.463238 stac-fastapi.opensearch-2.1.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1396 2024-03-03 15:10:18.462472 stac-fastapi.opensearch-2.1.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)       26 2024-02-08 06:37:21.000000 stac-fastapi.opensearch-2.1.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-03-03 15:10:18.464306 stac-fastapi.opensearch-2.1.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1541 2024-03-03 15:07:57.000000 stac-fastapi.opensearch-2.1.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:10:18.431414 stac-fastapi.opensearch-2.1.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:10:18.455994 stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2851 2024-02-08 06:37:21.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2394 2024-03-03 14:50:31.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    33327 2024-03-03 14:50:31.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-03-03 14:50:31.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-03-03 15:10:18.458181 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1396 2024-03-03 15:10:18.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-03-03 15:10:18.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-03-03 15:10:18.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-03-03 15:10:18.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      240 2024-03-03 15:10:18.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-03-03 15:10:18.000000 stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:38.317047 stac-fastapi.opensearch-2.2.0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-04-10 17:06:38.316791 stac-fastapi.opensearch-2.2.0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)       92 2024-03-19 04:19:17.000000 stac-fastapi.opensearch-2.2.0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-04-10 17:06:38.318054 stac-fastapi.opensearch-2.2.0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1541 2024-04-10 15:59:05.000000 stac-fastapi.opensearch-2.2.0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:37.964237 stac-fastapi.opensearch-2.2.0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:38.233767 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3191 2024-04-09 15:38:36.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2366 2024-04-09 14:42:19.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    34073 2024-03-19 04:19:17.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-04-10 15:56:39.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:38.234910 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      240 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/top_level.txt
```

### Comparing `stac-fastapi.opensearch-2.1.0/PKG-INFO` & `stac-fastapi.opensearch-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.opensearch
-Version: 2.1.0
+Version: 2.2.0
 Summary: Opensearch stac-fastapi backend.
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
 Requires-Dist: opensearch-py==2.4.2
 Requires-Dist: opensearch-py[async]==2.4.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -31,7 +31,11 @@
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]==0.19.0; extra == "server"
 
 # stac-fastapi-opensearch 
+
+## Requirements
+
+The Opensearch backend requires **opensearch**.
```

### Comparing `stac-fastapi.opensearch-2.1.0/setup.py` & `stac-fastapi.opensearch-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.1.0",
+    "stac-fastapi.core==2.2.0",
     "opensearch-py==2.4.2",
     "opensearch-py[async]==2.4.2",
     "uvicorn",
     "starlette",
 ]
 
 extra_reqs = {
```

### Comparing `stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/app.py` & `stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
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
@@ -19,14 +21,15 @@
     TransactionExtension,
 )
 from stac_fastapi.extensions.third_party import BulkTransactionExtension
 from stac_fastapi.opensearch.config import OpensearchSettings
 from stac_fastapi.opensearch.database_logic import (
     DatabaseLogic,
     create_collection_index,
+    create_index_templates,
 )
 
 settings = OpensearchSettings()
 session = Session.create_from_settings(settings)
 
 filter_extension = FilterExtension(client=EsAsyncBaseFiltersClient())
 filter_extension.conformance_classes.append(
@@ -56,27 +59,32 @@
     ContextExtension(),
     filter_extension,
 ]
 
 post_request_model = create_post_request_model(extensions)
 
 api = StacApi(
+    title=os.getenv("STAC_FASTAPI_TITLE", "stac-fastapi-opensearch"),
+    description=os.getenv("STAC_FASTAPI_DESCRIPTION", "stac-fastapi-opensearch"),
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

### Comparing `stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/config.py` & `stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """API configuration."""
 import os
 import ssl
 from typing import Any, Dict, Set
 
+import certifi
 from opensearchpy import AsyncOpenSearch, OpenSearch
 
 from stac_fastapi.types.config import ApiSettings
 
 
 def _es_config() -> Dict[str, Any]:
     # Determine the scheme (http or https)
@@ -28,17 +29,15 @@
 
     # Include SSL settings if using https
     config["ssl_version"] = ssl.PROTOCOL_SSLv23  # type: ignore
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

### Comparing `stac-fastapi.opensearch-2.1.0/stac_fastapi/opensearch/database_logic.py` & `stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/database_logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,26 +169,52 @@
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
+    client = AsyncSearchSettings().create_client
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
     client = AsyncSearchSettings().create_client
 
-    search_body = {
-        "mappings": ES_COLLECTIONS_MAPPINGS,
+    search_body: Dict[str, Any] = {
         "aliases": {COLLECTIONS_INDEX: {}},
     }
 
     index = f"{COLLECTIONS_INDEX}-000001"
 
     try:
         await client.indices.create(index=index, body=search_body)
@@ -199,29 +225,27 @@
             raise e
 
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
     client = AsyncSearchSettings().create_client
     index_name = index_by_collection_id(collection_id)
-    search_body = {
+    search_body: Dict[str, Any] = {
         "aliases": {index_name: {}},
-        "mappings": ES_ITEMS_MAPPINGS,
-        "settings": ES_ITEMS_SETTINGS,
     }
 
     try:
         await client.indices.create(index=f"{index_name}-000001", body=search_body)
     except TransportError as e:
         if e.status_code == 400:
             pass  # Ignore 400 status codes
@@ -331,15 +355,15 @@
 
         # Only add search_after to the query if token is not None and not empty
         if token:
             search_after = [token]
             search_body["search_after"] = search_after
 
         response = await self.client.search(
-            index="collections",
+            index=COLLECTIONS_INDEX,
             body=search_body,
         )
 
         hits = response["hits"]["hits"]
         collections = [
             self.collection_serializer.db_to_stac(
                 collection=hit["_source"], base_url=base_url
```

### Comparing `stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/PKG-INFO` & `stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.opensearch
-Version: 2.1.0
+Version: 2.2.0
 Summary: Opensearch stac-fastapi backend.
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
 Requires-Dist: opensearch-py==2.4.2
 Requires-Dist: opensearch-py[async]==2.4.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -31,7 +31,11 @@
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]==0.19.0; extra == "server"
 
 # stac-fastapi-opensearch 
+
+## Requirements
+
+The Opensearch backend requires **opensearch**.
```

### Comparing `stac-fastapi.opensearch-2.1.0/stac_fastapi.opensearch.egg-info/SOURCES.txt` & `stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

