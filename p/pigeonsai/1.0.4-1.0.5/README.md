# Comparing `tmp/pigeonsai-1.0.4.tar.gz` & `tmp/pigeonsai-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-1.0.4.tar", last modified: Tue Apr  2 15:06:50 2024, max compression
+gzip compressed data, was "pigeonsai-1.0.5.tar", last modified: Wed Apr 10 17:15:02 2024, max compression
```

## Comparing `pigeonsai-1.0.4.tar` & `pigeonsai-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/
--rw-r--r--   0 bs        (1000) bs        (1000)     2046 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      560 2024-03-25 05:17:42.000000 pigeonsai-1.0.4/README.md
--rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/setup.cfg
--rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-03-28 04:38:26.000000 pigeonsai-1.0.4/setup.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.138120 pigeonsai-1.0.4/src/
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.138120 pigeonsai-1.0.4/src/pigeonsai/
--rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.4/src/pigeonsai/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.4/src/pigeonsai/_client.py
--rw-r--r--   0 bs        (1000) bs        (1000)       48 2024-04-02 15:06:23.000000 pigeonsai-1.0.4/src/pigeonsai/_constants.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.4/src/pigeonsai/_exceptions.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.138120 pigeonsai-1.0.4/src/pigeonsai/_utils/
--rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.4/src/pigeonsai/_utils/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.4/src/pigeonsai/_utils/_utils.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/src/pigeonsai/resources/
--rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.4/src/pigeonsai/resources/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.4/src/pigeonsai/resources/anomaly_detector.py
--rw-r--r--   0 bs        (1000) bs        (1000)     9645 2024-03-28 04:03:04.000000 pigeonsai-1.0.4/src/pigeonsai/resources/data_connector.py
--rw-r--r--   0 bs        (1000) bs        (1000)     8314 2024-03-30 06:05:17.000000 pigeonsai-1.0.4/src/pigeonsai/resources/recommender.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/src/pigeonsai.egg-info/
--rw-r--r--   0 bs        (1000) bs        (1000)     2046 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       31 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/
+-rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      374 2024-04-10 17:12:16.000000 pigeonsai-1.0.5/README.md
+-rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/setup.cfg
+-rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-04-10 17:14:41.000000 pigeonsai-1.0.5/setup.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai/
+-rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.5/src/pigeonsai/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.5/src/pigeonsai/_client.py
+-rw-r--r--   0 bs        (1000) bs        (1000)       48 2024-04-02 15:06:23.000000 pigeonsai-1.0.5/src/pigeonsai/_constants.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.5/src/pigeonsai/_exceptions.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai/_utils/
+-rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.5/src/pigeonsai/_utils/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.5/src/pigeonsai/_utils/_utils.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai/resources/
+-rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.5/src/pigeonsai/resources/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.5/src/pigeonsai/resources/anomaly_detector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)    10791 2024-04-10 16:56:58.000000 pigeonsai-1.0.5/src/pigeonsai/resources/data_connector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)    10436 2024-04-06 23:41:09.000000 pigeonsai-1.0.5/src/pigeonsai/resources/recommender.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai.egg-info/
+-rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/top_level.txt
```

### Comparing `pigeonsai-1.0.4/PKG-INFO` & `pigeonsai-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.4
+Version: 1.0.5
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
@@ -28,18 +28,19 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.28.2
 Requires-Dist: httpx>=0.26.0
+Requires-Dist: pandas
 
 # PigeonsAI SDK
 
-The PigeonsAI SDK is a Python package that provides an interface to interact with the PigeonsDB database. This SDK allows you to search, initialize, get database information, and add documents to the database.
+PigeonsAI python client
 
 ## Installation
 
 To install the PigeonsAI SDK, use pip:
 
 ```
 pip install pigeonsai
```

### Comparing `pigeonsai-1.0.4/setup.py` & `pigeonsai-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="1.0.4",
+    version="1.0.5",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-1.0.4/src/pigeonsai/_client.py` & `pigeonsai-1.0.5/src/pigeonsai/_client.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.4/src/pigeonsai/_exceptions.py` & `pigeonsai-1.0.5/src/pigeonsai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.4/src/pigeonsai/resources/data_connector.py` & `pigeonsai-1.0.5/src/pigeonsai/resources/data_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # resources/data_connector.py
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 from typing import Literal
 from .._constants import (BASE_URL_V2)
 
 import httpx
 import os
 import json
+import pandas as pd
 
 if TYPE_CHECKING:
     from .._client import PigeonsAI
 
 
 class DataConnector:
     data_connection_uri_global = None
@@ -19,34 +20,49 @@
 
     def __init__(self, client: PigeonsAI):
         self.client = client
 
     def create_connector(
         self,
         connection_name: str,
-        connection_type: Literal['postgres', 'mysql'],
-        db_host: str,
-        db_name: str,
-        db_username: str,
-        db_password: str,
-        db_port: int
+        connection_type: Literal['postgres', 'mysql', 'mongodb'],
+        db_host: Optional[str] = None,
+        db_name: Optional[str] = None,
+        db_username: Optional[str] = None,
+        db_password: Optional[str] = None,
+        db_port: Optional[int] = None,
+        mongodb_uri: Optional[str] = None
     ):
-        if connection_type not in ['postgres', 'mysql']:
-            raise ValueError("Invalid connection type. Please choose 'postgres' or 'mysql'.")
-    
+        if connection_type not in ['postgres', 'mysql', 'mongodb']:
+            raise ValueError("Invalid connection type. Please choose 'postgres', 'mysql', or 'mongodb'.")
+        
+        if connection_type in ['postgres', 'mysql']:
+            if not all([db_host, db_name, db_username, db_password, db_port]):
+                missing = [name for name, value in locals().items() if not value and name.startswith('db_')]
+                raise ValueError(f"Missing required parameters for {connection_type} connection: {', '.join(missing)}")
+        elif connection_type == 'mongodb':
+            if not mongodb_uri or not db_name:
+                missing = []
+                if not mongodb_uri:
+                    missing.append('mongodb_uri')
+                if not db_name:
+                    missing.append('db_name')
+                raise ValueError("Missing required parameters for MongoDB connection: " + ', '.join(missing))
+        
         url = f"{BASE_URL_V2}/create-data-connector"
         headers = self.client.auth_headers
         data = {
             "data_connection_custom_name": connection_name,
             "data_connection_type": connection_type,
             "data_connection_host": db_host,
             "data_connection_port": db_port,
             "data_connection_database_name": db_name,
             "data_connection_username": db_username,
-            "data_connection_password": db_password
+            "data_connection_password": db_password,
+            "data_connection_mongodb_uri": mongodb_uri
         }
 
         response = self.client._request("POST", url, headers=headers, data=data)
         response_json = response.json()
 
         _data = response_json['data']
 
@@ -203,25 +219,29 @@
 def _prepare_data_with_file(
     headers,
     train_set_name: str,
     file_path: str,
     columns_map: dict
 ):
     url = f"{BASE_URL_V2}/create-train-dataset-with-file"
+    
+    df = pd.read_csv(file_path, nrows=0)
+    csv_headers = df.columns.tolist()
 
     file_name = os.path.basename(file_path)
     file_size = os.path.getsize(file_path)
 
     if 'Content-Type' in headers:
         headers.pop('Content-Type')
 
     data = {
         'train_dataset_name': train_set_name,
         'file_name': file_name,
         'file_size': str(file_size),
+        'csv_header': json.dumps(csv_headers),
         'columns_map': json.dumps(columns_map)
     }
     try:
         with open(file_path, 'rb') as f:
             files = {'file': (file_path, f)}
             response = httpx.post(url, headers=headers, files=files, data=data, timeout=300.0)
             response.raise_for_status()
```

### Comparing `pigeonsai-1.0.4/src/pigeonsai/resources/recommender.py` & `pigeonsai-1.0.5/src/pigeonsai/resources/recommender.py`

 * *Files 16% similar despite different names*

```diff
@@ -131,25 +131,75 @@
 class Transformer(BaseModelTrainer):
     def __init__(self, client: PigeonsAI):
         super().__init__(client, model_architecture='transformer')
 
     def train(
         self,
         custom_model_name: str,
-        train_set_uri: Optional[str] = None,
-        n_epochs: Optional[str] = None,
-        batch_size: Optional[str] = None,
-        learn_rate: Optional[str] = None,
+        train_set_uri: str,
+        n_epochs: Optional[int] = None,
+        batch_size: Optional[int] = None,
+        learning_rate: Optional[float] = None,
+        sequence_len: Optional[int] = None,
+        train_num_negatives: Optional[int] = None,
+        valid_num_negatives: Optional[int] = None,
+        random_cut_prob: Optional[float] = None,
+        replace_user_prob: Optional[float] = None,
+        replace_item_prob: Optional[float] = None,
+        random_seed: Optional[int] = None,
+        hidden_dim: Optional[int] = None,
+        temporal_dim: Optional[int] = None,
+        num_proxy_item: Optional[int] = None,
+        num_known_item: Optional[int] = None,
+        num_layers: Optional[int] = None,
+        num_heads: Optional[int] = None,
+        dropout_prob: Optional[float] = None,
+        temperature: Optional[float] = None,
+        every: Optional[int] = None,
+        patience: Optional[int] = None,
+        optimizer_algorithm: Optional[str] = None,
+        beta1: Optional[float] = None,
+        beta2: Optional[float] = None,
+        weight_decay: Optional[float] = None,
+        subset: Optional[float] = None,
+        threshold: Optional[float] = None
     ):
         kwargs = {
             'n_epochs': n_epochs,
             'batch_size': batch_size,
-            'learn_rate': learn_rate,
+            'learning_rate': learning_rate,
+            'sequence_len': sequence_len,
+            'train_num_negatives': train_num_negatives,
+            'valid_num_negatives': valid_num_negatives,
+            'random_cut_prob': random_cut_prob,
+            'replace_user_prob': replace_user_prob,
+            'replace_item_prob': replace_item_prob,
+            'random_seed': random_seed,
+            'hidden_dim': hidden_dim,
+            'temporal_dim': temporal_dim,
+            'num_proxy_item': num_proxy_item,
+            'num_known_item': num_known_item,
+            'num_layers': num_layers,
+            'num_heads': num_heads,
+            'dropout_prob': dropout_prob,
+            'temperature': temperature,
+            'every': every,
+            'patience': patience,
+            'optimizer_algorithm': optimizer_algorithm,
+            'beta1': beta1,
+            'beta2': beta2,
+            'weight_decay': weight_decay,
+            'subset': subset,
+            'threshold': threshold,
         }
-        return self._train(custom_model_name, train_set_uri, **{k: v for k, v in kwargs.items() if v is not None})
+        
+        # get rid of None    
+        filtered_kwargs = {k: v for k, v in kwargs.items() if v is not None}
+
+        return self._train(custom_model_name, train_set_uri, **filtered_kwargs)
 
     def inference(
         self,
         user_history_ids: Optional[str] = None,
         user_id: Optional[int] = None,
         k: int = 10,
         model_endpoint: str = None,
@@ -177,15 +227,15 @@
 class VAE(BaseModelTrainer):
     def __init__(self, client: PigeonsAI):
         super().__init__(client, model_architecture='autoencoder')
 
     def train(
         self,
         custom_model_name: str,
-        train_set_uri: Optional[str] = None,
+        train_set_uri: str,
         n_epochs: Optional[str] = None,
         batch_size: Optional[str] = None,
         learn_rate: Optional[str] = None,
         beta: Optional[str] = None,
         verbose: Optional[str] = None,
         train_prop: Optional[str] = None,
         random_seed: Optional[str] = None,
@@ -209,15 +259,19 @@
             'hidden_dims': hidden_dims,
             'recall_at_k': recall_at_k,
             'eval_iterations': eval_iterations,
             'act_fn': act_fn,
             'likelihood': likelihood,
             'data_subset_percent': data_subset_percent,
         }
-        return self._train(custom_model_name, train_set_uri, **{k: v for k, v in kwargs.items() if v is not None})
+        
+        # get rid of None
+        filtered_kwargs = {k: v for k, v in kwargs.items() if v is not None}
+        
+        return self._train(custom_model_name, train_set_uri, **filtered_kwargs)
         
     def inference(
         self,
         user_history_ids: Optional[str] = None,
         user_id: Optional[int] = None,
         exclude_seen: Optional[bool] = None,
         k: int = 10,
@@ -242,12 +296,12 @@
             unique_identifier=unique_identifier,
             pull_latest_data=pull_latest_data,
         )
 
 
 def _construct_model_url(model_name: Optional[str] = None, model_endpoint: Optional[str] = None) -> str:
     if model_name:
-        return f"https://{model_name}.apps.api1.pigeonsai.cloud/recommend"
+        return f"https://{model_name}.apps.pigeonsai.cloud/recommend"
     elif model_endpoint:
         return f"{model_endpoint.rstrip('/')}/recommend"
     else:
         raise ValueError("Either model_name or model_endpoint must be provided")
```

### Comparing `pigeonsai-1.0.4/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-1.0.5/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.4
+Version: 1.0.5
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
@@ -28,18 +28,19 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.28.2
 Requires-Dist: httpx>=0.26.0
+Requires-Dist: pandas
 
 # PigeonsAI SDK
 
-The PigeonsAI SDK is a Python package that provides an interface to interact with the PigeonsDB database. This SDK allows you to search, initialize, get database information, and add documents to the database.
+PigeonsAI python client
 
 ## Installation
 
 To install the PigeonsAI SDK, use pip:
 
 ```
 pip install pigeonsai
```

### Comparing `pigeonsai-1.0.4/src/pigeonsai.egg-info/SOURCES.txt` & `pigeonsai-1.0.5/src/pigeonsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

