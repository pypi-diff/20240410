# Comparing `tmp/dbrepo-1.4.2rc10.tar.gz` & `tmp/dbrepo-1.4.2rc11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrepo-1.4.2rc10.tar", last modified: Tue Apr  9 18:11:50 2024, max compression
+gzip compressed data, was "dbrepo-1.4.2rc11.tar", last modified: Wed Apr 10 10:37:46 2024, max compression
```

## Comparing `dbrepo-1.4.2rc10.tar` & `dbrepo-1.4.2rc11.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-09 18:11:50.244273 dbrepo-1.4.2rc10/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc10/LICENSE
--rw-r--r--   0 mweise    (1000) mweise    (1000)    17676 2024-04-09 18:11:50.244273 dbrepo-1.4.2rc10/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)     3612 2024-04-09 16:17:28.000000 dbrepo-1.4.2rc10/README.md
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-09 18:11:50.240273 dbrepo-1.4.2rc10/dbrepo/
--rw-r--r--   0 mweise    (1000) mweise    (1000)     2835 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc10/dbrepo/AmqpClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    74611 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/dbrepo/RestClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc10/dbrepo/__init__.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-09 18:11:50.240273 dbrepo-1.4.2rc10/dbrepo/api/
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc10/dbrepo/api/__init__.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    21274 2024-04-09 15:48:25.000000 dbrepo-1.4.2rc10/dbrepo/api/dto.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc10/dbrepo/api/exceptions.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-09 18:11:50.244273 dbrepo-1.4.2rc10/dbrepo.egg-info/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    17676 2024-04-09 18:11:50.000000 dbrepo-1.4.2rc10/dbrepo.egg-info/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)      537 2024-04-09 18:11:50.000000 dbrepo-1.4.2rc10/dbrepo.egg-info/SOURCES.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-09 18:11:50.000000 dbrepo-1.4.2rc10/dbrepo.egg-info/dependency_links.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)       35 2024-04-09 18:11:50.000000 dbrepo-1.4.2rc10/dbrepo.egg-info/requires.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-09 18:11:50.000000 dbrepo-1.4.2rc10/dbrepo.egg-info/top_level.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1089 2024-04-09 18:11:47.000000 dbrepo-1.4.2rc10/pyproject.toml
--rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-09 18:11:50.244273 dbrepo-1.4.2rc10/setup.cfg
--rw-r--r--   0 mweise    (1000) mweise    (1000)      411 2024-04-09 18:11:47.000000 dbrepo-1.4.2rc10/setup.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-09 18:11:50.244273 dbrepo-1.4.2rc10/tests/
--rw-r--r--   0 mweise    (1000) mweise    (1000)      734 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc10/tests/test_analyse.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     5570 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_container.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    26201 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_database.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11320 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_identifier.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_license.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    13906 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_query.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc10/tests/test_rest_client.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    28794 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_table.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14747 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_user.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11277 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc10/tests/test_view.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/LICENSE
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-10 10:31:38.000000 dbrepo-1.4.2rc11/README.md
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/dbrepo/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/dbrepo/AmqpClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/dbrepo/RestClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/dbrepo/UploadClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/dbrepo/__init__.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/dbrepo/api/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/dbrepo/api/__init__.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    21274 2024-04-09 15:48:25.000000 dbrepo-1.4.2rc11/dbrepo/api/dto.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/dbrepo/api/exceptions.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/dbrepo.egg-info/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18900 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      560 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/requires.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-04-10 10:37:46.000000 dbrepo-1.4.2rc11/dbrepo.egg-info/top_level.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1103 2024-04-10 10:37:18.000000 dbrepo-1.4.2rc11/pyproject.toml
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/setup.cfg
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      411 2024-04-10 10:37:18.000000 dbrepo-1.4.2rc11/setup.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-04-10 10:37:46.188240 dbrepo-1.4.2rc11/tests/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_analyse.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_container.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_database.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_identifier.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-09 16:08:11.000000 dbrepo-1.4.2rc11/tests/test_license.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_query.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-07 07:50:11.000000 dbrepo-1.4.2rc11/tests/test_rest_client.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_table.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_user.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-10 09:48:18.000000 dbrepo-1.4.2rc11/tests/test_view.py
```

### Comparing `dbrepo-1.4.2rc10/LICENSE` & `dbrepo-1.4.2rc11/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc10/PKG-INFO` & `dbrepo-1.4.2rc11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc10
+Version: 1.4.2rc11
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -220,14 +220,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31
 Requires-Dist: pika
 Requires-Dist: pydantic
 Requires-Dist: tuspy
+Requires-Dist: pandas
 
 # DBRepo Python Library
 
 Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/__APPVERSION__/), a database
 repository to support research based
 on [requests](https://pypi.org/project/requests/), [pydantic](https://pypi.org/project/pydantic/), [tuspy](https://pypi.org/project/tuspy/)
 and [pika](https://pypi.org/project/pika/).
@@ -255,41 +256,41 @@
 analysis = client.analyse_datatypes(file_path="sensor.csv", separator=",")
 print(f"Analysis result: {analysis}")
 # -> columns=(date=date, precipitation=decimal, lat=decimal, lng=decimal), separator=,
 #    line_termination=\n
 
 # create table
 table = client.create_table(database_id=1,
-    name="Sensor Data",
-    constraints=CreateTableConstraints(
-        checks=['precipitation >= 0'],
-        uniques=[['precipitation']]),
-    columns=[CreateTableColumn(name="date",
-                               type=ColumnType.DATE,
-                               dfid=3,  # YYYY-MM-dd
-                               primary_key=True,
-                               null_allowed=False),
-             CreateTableColumn(name="precipitation",
-                               type=ColumnType.DECIMAL,
-                               size=10,
-                               d=4,
-                               primary_key=False,
-                               null_allowed=True),
-             CreateTableColumn(name="lat",
-                               type=ColumnType.DECIMAL,
-                               size=10,
-                               d=4,
-                               primary_key=False,
-                               null_allowed=True),
-             CreateTableColumn(name="lng",
-                               type=ColumnType.DECIMAL,
-                               size=10,
-                               d=4,
-                               primary_key=False,
-                               null_allowed=True)])
+                            name="Sensor Data",
+                            constraints=CreateTableConstraints(
+                                checks=['precipitation >= 0'],
+                                uniques=[['precipitation']]),
+                            columns=[CreateTableColumn(name="date",
+                                                       type=ColumnType.DATE,
+                                                       dfid=3,  # YYYY-MM-dd
+                                                       primary_key=True,
+                                                       null_allowed=False),
+                                     CreateTableColumn(name="precipitation",
+                                                       type=ColumnType.DECIMAL,
+                                                       size=10,
+                                                       d=4,
+                                                       primary_key=False,
+                                                       null_allowed=True),
+                                     CreateTableColumn(name="lat",
+                                                       type=ColumnType.DECIMAL,
+                                                       size=10,
+                                                       d=4,
+                                                       primary_key=False,
+                                                       null_allowed=True),
+                                     CreateTableColumn(name="lng",
+                                                       type=ColumnType.DECIMAL,
+                                                       size=10,
+                                                       d=4,
+                                                       primary_key=False,
+                                                       null_allowed=True)])
 print(f"Create table result {table}")
 # -> (id=1, internal_name=sensor_data, ...)
 
 client.import_table_data(database_id=1, table_id=1, file_path="sensor.csv", separator=",",
                          skip_lines=1, line_encoding="\n")
 print(f"Finished.")
 ```
@@ -306,15 +307,33 @@
   dataset ([docs](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//usage-overview/#private-database-access))
 - Create persistent
   identifiers ([docs](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//usage-overview/#assign-database-pid))
 - Execute
   queries ([docs](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//usage-overview/#export-subset))
 - Get data from tables/views/subsets
 
-## Future
+## Configure
+
+All credentials can optionally be set/overridden with environment variables. This is especially useful when sharing 
+Jupyter Notebooks by creating an invisible `.env` file and loading it:
+
+```
+REST_API_ENDPOINT="https://test.dbrepo.tuwien.ac.at"
+REST_API_USERNAME="foo"
+REST_API_PASSWORD="bar"
+REST_API_SECURE="True"
+AMQP_API_HOST="https://test.dbrepo.tuwien.ac.at"
+AMQP_API_PORT="5672"
+AMQP_API_USERNAME="foo"
+AMQP_API_PASSWORD="bar"
+AMQP_API_VIRTUAL_HOST="/"
+REST_UPLOAD_ENDPOINT="https://test.dbrepo.tuwien.ac.at/api/upload/files"
+```
+
+## Roadmap
 
 - Searching
 
 ## Contact
 
 * Prof. [Andreas Rauber](https://tiss.tuwien.ac.at/person/39608.html)<sup>TU Wien</sup>
 * DI. [Martin Weise](https://tiss.tuwien.ac.at/person/287722.html)<sup>TU Wien</sup>
```

### Comparing `dbrepo-1.4.2rc10/dbrepo/AmqpClient.py` & `dbrepo-1.4.2rc11/dbrepo/AmqpClient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import os
 import pika
 import sys
-import logging
 import json
+import logging
 
 from dbrepo.api.dto import CreateData
 
 
 class AmqpClient:
     """
     The AmqpClient class for communicating with the DBRepo AMQP API to import data. All parameters can be set also \
@@ -28,24 +28,26 @@
 
     def __init__(self,
                  broker_host: str = 'broker-service',
                  broker_port: int = 5672,
                  broker_virtual_host: str = '/',
                  username: str = None,
                  password: str = None) -> None:
+        logging.getLogger('requests').setLevel(logging.INFO)
+        logging.getLogger('urllib3').setLevel(logging.INFO)
         logging.basicConfig(format='%(asctime)s %(name)-12s %(levelname)-6s %(message)s', level=logging.DEBUG,
                             stream=sys.stdout)
-        self.broker_host = os.environ.get('DBREPO_BROKER_HOST', broker_host)
-        self.broker_port = os.environ.get('DBREPO_BROKER_PORT', broker_port)
-        if os.environ.get('DBREPO_BROKER_VIRTUAL_HOST') is not None:
-            self.broker_virtual_host = os.environ.get('DBREPO_BROKER_VIRTUAL_HOST')
+        self.broker_host = os.environ.get('AMQP_API_HOST', broker_host)
+        self.broker_port = os.environ.get('AMQP_API_PORT', broker_port)
+        if os.environ.get('AMQP_API_VIRTUAL_HOST') is not None:
+            self.broker_virtual_host = os.environ.get('AMQP_API_VIRTUAL_HOST')
         else:
             self.broker_virtual_host = broker_virtual_host
-        self.username = os.environ.get('DBREPO_USERNAME', username)
-        self.password = os.environ.get('DBREPO_PASSWORD', password)
+        self.username = os.environ.get('AMQP_API_USERNAME', username)
+        self.password = os.environ.get('AMQP_API_PASSWORD', password)
 
     def publish(self, exchange: str, routing_key: str, data=dict) -> None:
         """
         Publishes data to a given exchange with the given routing key with a blocking connection.
 
         :param exchange: The exchange name.
         :param routing_key: The routing key.
```

### Comparing `dbrepo-1.4.2rc10/dbrepo/RestClient.py` & `dbrepo-1.4.2rc11/dbrepo/RestClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import sys
 import os
 import logging
 
 import requests
 from pydantic import TypeAdapter
 from tusclient.client import TusClient
+from pandas import DataFrame
 
+from dbrepo.UploadClient import UploadClient
 from dbrepo.api.dto import *
 from dbrepo.api.exceptions import ResponseCodeError, UsernameExistsError, EmailExistsError, NotExistsError, \
     ForbiddenError, MalformedError, NameExistsError, QueryStoreError, MetadataConsistencyError, ExternalSystemError, \
     AuthenticationError, UploadError
 
 
 class RestClient:
     """
     The RestClient class for communicating with the DBRepo REST API. All parameters can be set also via environment \
-    variables, e.g. set endpoint with DBREPO_ENDPOINT, username with DBREPO_USERNAME, etc. You can override the \
-    constructor parameters with the environment variables.
+    variables, e.g. set endpoint with REST_API_ENDPOINT, username with REST_API_USERNAME, etc. You can override \
+    the constructor parameters with the environment variables.
 
     :param endpoint: The REST API endpoint. Optional. Default: "http://gateway-service"
     :param username: The REST API username. Optional.
     :param password: The REST API password. Optional.
     :param secure: When set to false, the requests library will not verify the authenticity of your TLS/SSL
         certificates (i.e. when using self-signed certificates). Default: true.
     """
@@ -34,19 +36,19 @@
                  username: str = None,
                  password: str = None,
                  secure: bool = True) -> None:
         logging.getLogger('requests').setLevel(logging.INFO)
         logging.getLogger('urllib3').setLevel(logging.INFO)
         logging.basicConfig(format='%(asctime)s %(name)-12s %(levelname)-6s %(message)s', level=logging.DEBUG,
                             stream=sys.stdout)
-        self.endpoint = os.environ.get('DBREPO_ENDPOINT', endpoint)
-        self.username = os.environ.get('DBREPO_USERNAME', username)
-        self.password = os.environ.get('DBREPO_PASSWORD', password)
-        if os.environ.get('DBREPO_SECURE') is not None:
-            self.secure = os.environ.get('DBREPO_SECURE') == 'True'
+        self.endpoint = os.environ.get('REST_API_ENDPOINT', endpoint)
+        self.username = os.environ.get('REST_API_USERNAME', username)
+        self.password = os.environ.get('REST_API_PASSWORD', password)
+        if os.environ.get('REST_API_SECURE') is not None:
+            self.secure = os.environ.get('REST_API_SECURE') == 'True'
         else:
             self.secure = secure
 
     def _wrapper(self, method: str, url: str, params: [(str,)] = None, payload=None, headers: dict = None,
                  force_auth: bool = False, stream: bool = False) -> requests.Response:
         if force_auth and (self.username is None or self.password is None):
             raise AuthenticationError(f"Failed to perform request: authentication required")
@@ -82,17 +84,19 @@
         uploader = my_client.uploader(file_path=file_path)
         uploader.upload()
         filename = uploader.url[uploader.url.rfind('/') + 1:uploader.url.rfind('+')]
         if filename is None or len(filename) == 0:
             raise UploadError(f'Failed to upload the file to {self.endpoint}')
         return filename
 
-    def whoami(self) -> str:
+    def whoami(self) -> str | None:
         """
         Print the username.
+
+        :returns: The username, if set.
         """
         if self.username is not None:
             logging.info(f"{self.username}")
             return self.username
         logging.info(f"No username set!")
         return None
 
@@ -120,15 +124,15 @@
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises NotExistsError: If theuser does not exist.
         """
         url = f'/api/user/{user_id}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return User.parse_raw(body)
+            return User.model_validate(body)
         if response.status_code == 404:
             raise NotExistsError(f'Failed to find user with id {user_id}')
         raise ResponseCodeError(
             f'Failed to find user with id {user_id}: response code: {response.status_code} is not 200 (OK)')
 
     def create_user(self, username: str, password: str, email: str) -> UserBrief:
         """
@@ -147,15 +151,15 @@
         :raises EmailExistsError: The email exists already.
         """
         url = f'/api/user'
         response = self._wrapper(method="post", url=url,
                                  payload=CreateUser(username=username, password=password, email=email))
         if response.status_code == 201:
             body = response.json()
-            return UserBrief.parse_raw(body)
+            return UserBrief.model_validate(body)
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to update user password: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to create user: default role not found')
         if response.status_code == 409:
             raise UsernameExistsError(f'Failed to create user: user with username exists')
         if response.status_code == 417:
@@ -182,15 +186,15 @@
         """
         url = f'/api/user/{user_id}'
         response = self._wrapper(method="put", url=url, force_auth=True,
                                  payload=UpdateUser(firstname=firstname, lastname=lastname, affiliation=affiliation,
                                                     orcid=orcid))
         if response.status_code == 202:
             body = response.json()
-            return User.parse_raw(body)
+            return User.model_validate(body)
         if response.status_code == 400:
             raise ResponseCodeError(f'Failed to update user: invalid values')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to update user password: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update user: user not found')
         if response.status_code == 405:
@@ -211,15 +215,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If theuser does not exist.
         """
         url = f'/api/user/{user_id}/theme'
         response = self._wrapper(method="put", url=url, force_auth=True, payload=UpdateUserTheme(theme=theme))
         if response.status_code == 202:
             body = response.json()
-            return User.parse_raw(body)
+            return User.model_validate(body)
         if response.status_code == 400:
             raise ResponseCodeError(f'Failed to update user theme: invalid values')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to update user password: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update user theme: user not found')
         if response.status_code == 405:
@@ -240,15 +244,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If theuser does not exist.
         """
         url = f'/api/user/{user_id}/password'
         response = self._wrapper(method="put", url=url, force_auth=True, payload=UpdateUserPassword(password=password))
         if response.status_code == 202:
             body = response.json()
-            return User.parse_raw(body)
+            return User.model_validate(body)
         if response.status_code == 400:
             raise ResponseCodeError(f'Failed to update user password: invalid values')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to update user password: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update user password: not found')
         if response.status_code == 405:
@@ -282,15 +286,15 @@
         :raises NotExistsError: If the container does not exist.
         :raises ResponseCodeError: If something went wrong with the retrieval.
         """
         url = f'/api/container/{container_id}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return Container.parse_raw(body)
+            return Container.model_validate(body)
         if response.status_code == 404:
             raise NotExistsError(f'Failed to get container: not found')
         raise ResponseCodeError(f'Failed to get container: response code: {response.status_code} is not 200 (OK)')
 
     def get_databases(self) -> List[Database]:
         """
         Get all databases.
@@ -329,15 +333,15 @@
 
         :raises ResponseCodeError: If something went wrong with the retrieval.
         """
         url = f'/api/database/{database_id}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return Database.parse_raw(body)
+            return Database.model_validate(body)
         if response.status_code == 404:
             raise NotExistsError(f'Failed to find database with id {database_id}')
         raise ResponseCodeError(
             f'Failed to find database with id {database_id}: response code: {response.status_code} is not 200 (OK)')
 
     def create_database(self, name: str, container_id: int, is_public: bool) -> Database:
         """
@@ -355,15 +359,15 @@
         :raises NotExistsError: If the container does not exist.
         """
         url = f'/api/database'
         response = self._wrapper(method="post", url=url, force_auth=True,
                                  payload=CreateDatabase(name=name, container_id=container_id, is_public=is_public))
         if response.status_code == 201:
             body = response.json()
-            return Database.parse_raw(body)
+            return Database.model_validate(body)
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to create database: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to create database: container not found')
         raise ResponseCodeError(
             f'Failed to create database: response code: {response.status_code} is not 201 (CREATED)')
 
@@ -381,15 +385,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thedatabase does not exist.
         """
         url = f'/api/database/{database_id}'
         response = self._wrapper(method="put", url=url, force_auth=True, payload=ModifyVisibility(is_public=is_public))
         if response.status_code == 202:
             body = response.json()
-            return Database.parse_raw(body)
+            return Database.model_validate(body)
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to update database visibility: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update database visibility: not found')
         raise ResponseCodeError(
             f'Failed to update database visibility: response code: {response.status_code} is not 202 (ACCEPTED)')
 
@@ -405,15 +409,15 @@
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises NotExistsError: If thedatabase does not exist.
         """
         url = f'/api/database/{database_id}/owner'
         response = self._wrapper(method="put", url=url, force_auth=True, payload=ModifyOwner(id=user_id))
         if response.status_code == 202:
             body = response.json()
-            return Database.parse_raw(body)
+            return Database.model_validate(body)
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to update database visibility: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update database visibility: not found')
         raise ResponseCodeError(
             f'Failed to update database visibility: response code: {response.status_code} is not 202 (ACCEPTED)')
 
@@ -438,15 +442,15 @@
         """
         url = f'/api/database/{database_id}/table'
         response = self._wrapper(method="post", url=url, force_auth=True,
                                  payload=CreateTable(name=name, description=description,
                                                      columns=columns, constraints=constraints))
         if response.status_code == 201:
             body = response.json()
-            return Table.parse_raw(body)
+            return Table.model_validate(body)
         if response.status_code == 400:
             raise MalformedError(f'Failed to create table: service rejected malformed payload')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to create table: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to create table: container not found')
         if response.status_code == 409:
@@ -484,15 +488,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thecontainer does not exist.
         """
         url = f'/api/database/{database_id}/table/{table_id}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return Table.parse_raw(body)
+            return Table.model_validate(body)
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to find table: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to find table: not found')
         raise ResponseCodeError(f'Failed to find table: response code: {response.status_code} is not 200 (OK)')
 
     def delete_table(self, database_id: int, table_id: int) -> None:
@@ -552,15 +556,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thecontainer does not exist.
         """
         url = f'/api/database/{database_id}/view/{view_id}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return View.parse_raw(body)
+            return View.model_validate(body)
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to find view: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to find view: not found')
         raise ResponseCodeError(f'Failed to find view: response code: {response.status_code} is not 200 (OK)')
 
     def create_view(self, database_id: int, name: str, query: str, is_public: bool) -> View:
@@ -580,15 +584,15 @@
         :raises NotExistsError: If thecontainer does not exist.
         """
         url = f'/api/database/{database_id}/view'
         response = self._wrapper(method="post", url=url, force_auth=True,
                                  payload=CreateView(name=name, query=query, is_public=is_public))
         if response.status_code == 201:
             body = response.json()
-            return View.parse_raw(body)
+            return View.model_validate(body)
         if response.status_code == 400 or response.status_code == 423:
             raise MalformedError(f'Failed to create view: service rejected malformed payload')
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to create view: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to create view: not found')
         raise ResponseCodeError(f'Failed to create view: response code: {response.status_code} is not 201 (CREATED)')
@@ -612,22 +616,24 @@
             raise MalformedError(f'Failed to delete view: service rejected malformed payload')
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to delete view: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to delete view: not found')
         raise ResponseCodeError(f'Failed to delete view: response code: {response.status_code} is not 202 (ACCEPTED)')
 
-    def get_view_data(self, database_id: int, view_id: int, page: int = 0, size: int = 10) -> Result:
+    def get_view_data(self, database_id: int, view_id: int, page: int = 0, size: int = 10,
+                      df: bool = False) -> Result | DataFrame:
         """
         Get data of a view in a database with given database id and view id.
 
         :param database_id: The database id.
         :param view_id: The view id.
         :param page: The result pagination number. Optional. Default: 0.
         :param size: The result pagination size. Optional. Default: 10.
+        :param df: If true, the result is returned as Pandas DataFrame. Optional. Default: False.
 
         :returns: The result of the view query, if successful.
 
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If the view does not exist.
         """
@@ -635,33 +641,37 @@
         params = []
         if page is not None and size is not None:
             params.append(('page', page))
             params.append(('size', size))
         response = self._wrapper(method="get", url=url, params=params)
         if response.status_code == 200:
             body = response.json()
-            return Result.parse_raw(body)
+            res = Result.model_validate(body)
+            if df:
+                return DataFrame.from_records(res.result)
+            return res
         if response.status_code == 400:
             raise MalformedError(f'Failed to get view data: service rejected malformed payload')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to get view data: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to get view data: not found')
         raise ResponseCodeError(f'Failed to get view data: response code: {response.status_code} is not 200 (OK)')
 
     def get_table_data(self, database_id: int, table_id: int, page: int = 0, size: int = 10,
-                       timestamp: datetime.datetime = None) -> Result:
+                       timestamp: datetime.datetime = None, df: bool = False) -> Result | DataFrame:
         """
         Get data of a table in a database with given database id and table id.
 
         :param database_id: The database id.
         :param table_id: The table id.
         :param page: The result pagination number. Optional. Default: 0.
         :param size: The result pagination size. Optional. Default: 10.
         :param timestamp: The query execution time. Optional.
+        :param df: If true, the result is returned as Pandas DataFrame. Optional. Default: False.
 
         :returns: The result of the view query, if successful.
 
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If the table does not exist.
         :raises QueryStoreError: If the result set could not be counted.
@@ -672,15 +682,18 @@
             params.append(('page', page))
             params.append(('size', size))
         if timestamp is not None:
             params.append(('timestamp', timestamp))
         response = self._wrapper(method="get", url=url, params=params)
         if response.status_code == 200:
             body = response.json()
-            return Result.parse_raw(body)
+            res = Result.model_validate(body)
+            if df:
+                return DataFrame.from_records(res.result)
+            return res
         if response.status_code == 400:
             raise MalformedError(f'Failed to get table data: service rejected malformed payload')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to get table data: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to get table data: not found')
         if response.status_code == 409:
@@ -732,16 +745,16 @@
         :param line_encoding: The encoding of the line termination. Optional. Default: CR (Windows).
 
         :raises ResponseCodeError: If something went wrong with the insert.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If the table does not exist.
         :raises MalformedError: If the payload is rejected by the service (e.g. LOB data could not be imported).
         """
-        upload = UploadClient(endpoint=self.endpoint)
-        filename = upload.upload(file_path=file_path)
+        client = UploadClient(endpoint=self.endpoint)
+        filename = client.upload(file_path=file_path)
         url = f'/api/database/{database_id}/table/{table_id}/data/import'
         response = self._wrapper(method="post", url=url, force_auth=True,
                                  payload=Import(location=filename, separator=separator, quote=quote,
                                                 skip_lines=skip_lines, false_element=false_encoding,
                                                 true_element=true_encoding, null_element=null_encoding,
                                                 line_termination=line_encoding))
         if response.status_code == 202:
@@ -786,15 +799,15 @@
             ('enum', enum),
             ('enum_tol', enum_tol)
         ]
         url = f'/api/analyse/datatypes'
         response = self._wrapper(method="get", url=url, params=params)
         if response.status_code == 202:
             body = response.json()
-            return DatatypeAnalysis.parse_raw(body)
+            return DatatypeAnalysis.model_validate(body)
         if response.status_code == 400 or response.status_code == 500:
             raise MalformedError(f'Failed to analyse data types: service rejected malformed payload')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to analyse data types: failed to find file in Storage Service')
         raise ResponseCodeError(
             f'Failed to analyse data types: response code: {response.status_code} is not 202 (ACCEPTED)')
 
@@ -822,15 +835,15 @@
             ('filename', filename),
             ('separator', separator),
         ]
         url = f'/api/analyse/keys'
         response = self._wrapper(method="get", url=url, params=params)
         if response.status_code == 202:
             body = response.json()
-            return KeyAnalysis.parse_raw(body)
+            return KeyAnalysis.model_validate(body)
         if response.status_code == 400 or response.status_code == 500:
             raise MalformedError(f'Failed to analyse data types: service rejected malformed payload')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to analyse data types: failed to find file in Storage Service')
         raise ResponseCodeError(
             f'Failed to analyse data types: response code: {response.status_code} is not 202 (ACCEPTED)')
 
@@ -847,15 +860,15 @@
         :raises MalformedError: If the payload is rejected by the service.
         :raises NotExistsError: If the file was not found by the Analyse Service.
         """
         url = f'/api/analyse/database/{database_id}/table/{table_id}/statistics'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 202:
             body = response.json()
-            return TableStatistics.parse_raw(body)
+            return TableStatistics.model_validate(body)
         if response.status_code == 400:
             raise MalformedError(f'Failed to analyse table statistics: service rejected malformed payload')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to analyse table statistics: separator error')
         raise ResponseCodeError(
             f'Failed to analyse table statistics: response code: {response.status_code} is not 202 (ACCEPTED)')
 
@@ -990,15 +1003,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thecontainer does not exist.
         """
         url = f'/api/database/{database_id}/access'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return DatabaseAccess.parse_raw(body).type
+            return DatabaseAccess.model_validate(body).type
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to get database access: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to get database access: not found')
         raise ResponseCodeError(f'Failed to get database access: response code: {response.status_code} is not 200 (OK)')
 
     def create_database_access(self, database_id: int, user_id: str, type: AccessType) -> AccessType:
@@ -1016,15 +1029,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thedatabase or user does not exist.
         """
         url = f'/api/database/{database_id}/access/{user_id}'
         response = self._wrapper(method="post", url=url, force_auth=True, payload=CreateAccess(type=type))
         if response.status_code == 202:
             body = response.json()
-            return DatabaseAccess.parse_raw(body).type
+            return DatabaseAccess.model_validate(body).type
         if response.status_code == 400:
             raise MalformedError(f'Failed to create database access: service rejected malformed payload')
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to create database access: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to create database access: not found')
         raise ResponseCodeError(
@@ -1045,15 +1058,15 @@
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thedatabase or user does not exist.
         """
         url = f'/api/database/{database_id}/access/{user_id}'
         response = self._wrapper(method="put", url=url, force_auth=True, payload=UpdateAccess(type=type))
         if response.status_code == 202:
             body = response.json()
-            return DatabaseAccess.parse_raw(body).type
+            return DatabaseAccess.model_validate(body).type
         if response.status_code == 400:
             raise MalformedError(f'Failed to update database access: service rejected malformed payload')
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to update database access: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update database access: not found')
         raise ResponseCodeError(
@@ -1109,65 +1122,60 @@
         url = f'/api/database/{database_id}/query'
         if page is not None and size is not None:
             url += f'?page={page}&size={size}'
         response = self._wrapper(method="post", url=url, force_auth=True,
                                  payload=ExecuteQuery(statement=query, timestamp=timestamp))
         if response.status_code == 202:
             body = response.json()
-            return Result.parse_raw(body)
+            return Result.model_validate(body)
         if response.status_code == 400:
             raise MalformedError(f'Failed to execute query: service rejected malformed payload')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to execute query: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to execute query: not found')
         if response.status_code == 409:
             raise QueryStoreError(f'Failed to execute query: query store rejected query')
         if response.status_code == 417:
             raise MetadataConsistencyError(f'Failed to execute query: service expected other metadata')
         raise ResponseCodeError(
             f'Failed to execute query: response code: {response.status_code} is not 202 (ACCEPTED)')
 
     def get_query_data(self, database_id: int, query_id: int, page: int = 0, size: int = 10,
-                       file_path: str = None) -> Result:
+                       df: bool = False) -> Result | DataFrame:
         """
         Re-executes a query in a database with given database id and query id.
 
         :param database_id: The database id.
         :param query_id: The query id.
         :param page: The result pagination number. Optional. Default: 0.
         :param size: The result pagination size. Optional. Default: 10.
         :param size: The result pagination size. Optional. Default: 10.
-        :param file_path: The file path where the result should be saved. Optional.
+        :param df: If true, the result is returned as Pandas DataFrame. Optional. Default: False.
 
         :returns: The result set, if successful.
 
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises MalformedError: If the payload is rejected by the service.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If the database, query or user does not exist.
         :raises QueryStoreError: The query store rejected the query.
         :raises MetadataConsistencyError: The service failed to parse columns from the metadata database.
         """
-        stream = False
         headers = {}
         url = f'/api/database/{database_id}/query/{query_id}/data'
         if page is not None and size is not None:
             url += f'?page={page}&size={size}'
-        if file_path is not None:
-            stream = True
-            headers = {'Accept': 'text/csv'}
-        response = self._wrapper(method="get", url=url, headers=headers, stream=stream)
+        response = self._wrapper(method="get", url=url, headers=headers)
         if response.status_code == 200:
-            if file_path is None:
-                body = response.json()
-                return Result.parse_raw(body)
-            else:
-                with open(file_path, "w") as f:
-                    f.write(response.content.decode("utf-8"))
+            body = response.json()
+            res = Result.model_validate(body)
+            if df:
+                return DataFrame.from_records(res.result)
+            return res
         if response.status_code == 400:
             raise MalformedError(f'Failed to re-execute query: service rejected malformed payload')
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to re-execute query: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to re-execute query: not found')
         if response.status_code == 409:
@@ -1229,15 +1237,15 @@
         :raises QueryStoreError: The query store rejected the query.
         :raises MetadataConsistencyError: The service failed to parse columns from the metadata database.
         """
         url = f'/api/database/{database_id}/query/{query_id}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return Query.parse_raw(body)
+            return Query.model_validate(body)
         if response.status_code == 404:
             raise NotExistsError(f'Failed to find query: not found')
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to find query: not allowed')
         if response.status_code == 417:
             raise MetadataConsistencyError(f'Failed to find query: service expected other metadata')
         if response.status_code == 501 or response.status_code == 503 or response.status_code == 504:
@@ -1291,15 +1299,15 @@
         :raises NotExistsError: If thedatabase or user does not exist.
         :raises QueryStoreError: The query store rejected the update.
         """
         url = f'/api/database/{database_id}/query/{query_id}'
         response = self._wrapper(method="put", url=url, force_auth=True, payload=UpdateQuery(persist=persist))
         if response.status_code == 202:
             body = response.json()
-            return Query.parse_raw(body)
+            return Query.model_validate(body)
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to update query: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update query: not found')
         if response.status_code == 412:
             raise QueryStoreError(f'Failed to update query: query store rejected update')
         raise ResponseCodeError(
@@ -1345,15 +1353,15 @@
                                    creators=creators, publication_year=publication_year, descriptions=descriptions,
                                    funders=funders, licenses=licenses, language=language, query_id=query_id,
                                    view_id=view_id, table_id=table_id, publication_day=publication_day,
                                    publication_month=publication_month, related_identifiers=related_identifiers)
         response = self._wrapper(method="post", url=url, force_auth=True, payload=payload)
         if response.status_code == 201:
             body = response.json()
-            return Identifier.parse_raw(body)
+            return Identifier.model_validate(body)
         if response.status_code == 400:
             raise MalformedError(f'Failed to create identifier: service rejected malformed payload')
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to create identifier: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to create identifier: not found')
         if response.status_code == 503:
@@ -1372,15 +1380,15 @@
         :raises ResponseCodeError: If something went wrong with the suggestion of the identifier.
         :raises NotExistsError: If no metadata can be found or the identifier type is not supported.
         """
         url = f'/api/identifier?url={uri}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
-            return Identifier.parse_raw(body)
+            return Identifier.model_validate(body)
         if response.status_code == 404:
             raise NotExistsError(f'Failed to suggest identifier: not found or not supported')
         raise ResponseCodeError(f'Failed to suggest identifier: response code: {response.status_code} is not 200 (OK)')
 
     def get_licenses(self) -> List[License]:
         """
         Get list of licenses allowed.
@@ -1438,15 +1446,15 @@
         :raises NotExistsError: If the accept header is neither application/json nor application/ld+json.
         """
         url = f'/api/database/{database_id}/table/{table_id}/column/{column_id}'
         response = self._wrapper(method="put", url=url, force_auth=True,
                                  payload=UpdateColumn(concept_uri=concept_uri, unit_uri=unit_uri))
         if response.status_code == 202:
             body = response.json()
-            return Column.parse_raw(body)
+            return Column.model_validate(body)
         if response.status_code == 400:
             raise MalformedError(f'Failed to update column: service rejected malformed payload')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to update colum: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to update colum: not found')
         raise ResponseCodeError(f'Failed to update colum: response code: {response.status_code} is not 202 (ACCEPTED)')
```

### Comparing `dbrepo-1.4.2rc10/dbrepo/api/dto.py` & `dbrepo-1.4.2rc11/dbrepo/api/dto.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc10/dbrepo/api/exceptions.py` & `dbrepo-1.4.2rc11/dbrepo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc10/dbrepo.egg-info/PKG-INFO` & `dbrepo-1.4.2rc11/dbrepo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.2rc10
+Version: 1.4.2rc11
 Summary: DBRepo Python Library
 Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -220,14 +220,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31
 Requires-Dist: pika
 Requires-Dist: pydantic
 Requires-Dist: tuspy
+Requires-Dist: pandas
 
 # DBRepo Python Library
 
 Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/__APPVERSION__/), a database
 repository to support research based
 on [requests](https://pypi.org/project/requests/), [pydantic](https://pypi.org/project/pydantic/), [tuspy](https://pypi.org/project/tuspy/)
 and [pika](https://pypi.org/project/pika/).
@@ -255,41 +256,41 @@
 analysis = client.analyse_datatypes(file_path="sensor.csv", separator=",")
 print(f"Analysis result: {analysis}")
 # -> columns=(date=date, precipitation=decimal, lat=decimal, lng=decimal), separator=,
 #    line_termination=\n
 
 # create table
 table = client.create_table(database_id=1,
-    name="Sensor Data",
-    constraints=CreateTableConstraints(
-        checks=['precipitation >= 0'],
-        uniques=[['precipitation']]),
-    columns=[CreateTableColumn(name="date",
-                               type=ColumnType.DATE,
-                               dfid=3,  # YYYY-MM-dd
-                               primary_key=True,
-                               null_allowed=False),
-             CreateTableColumn(name="precipitation",
-                               type=ColumnType.DECIMAL,
-                               size=10,
-                               d=4,
-                               primary_key=False,
-                               null_allowed=True),
-             CreateTableColumn(name="lat",
-                               type=ColumnType.DECIMAL,
-                               size=10,
-                               d=4,
-                               primary_key=False,
-                               null_allowed=True),
-             CreateTableColumn(name="lng",
-                               type=ColumnType.DECIMAL,
-                               size=10,
-                               d=4,
-                               primary_key=False,
-                               null_allowed=True)])
+                            name="Sensor Data",
+                            constraints=CreateTableConstraints(
+                                checks=['precipitation >= 0'],
+                                uniques=[['precipitation']]),
+                            columns=[CreateTableColumn(name="date",
+                                                       type=ColumnType.DATE,
+                                                       dfid=3,  # YYYY-MM-dd
+                                                       primary_key=True,
+                                                       null_allowed=False),
+                                     CreateTableColumn(name="precipitation",
+                                                       type=ColumnType.DECIMAL,
+                                                       size=10,
+                                                       d=4,
+                                                       primary_key=False,
+                                                       null_allowed=True),
+                                     CreateTableColumn(name="lat",
+                                                       type=ColumnType.DECIMAL,
+                                                       size=10,
+                                                       d=4,
+                                                       primary_key=False,
+                                                       null_allowed=True),
+                                     CreateTableColumn(name="lng",
+                                                       type=ColumnType.DECIMAL,
+                                                       size=10,
+                                                       d=4,
+                                                       primary_key=False,
+                                                       null_allowed=True)])
 print(f"Create table result {table}")
 # -> (id=1, internal_name=sensor_data, ...)
 
 client.import_table_data(database_id=1, table_id=1, file_path="sensor.csv", separator=",",
                          skip_lines=1, line_encoding="\n")
 print(f"Finished.")
 ```
@@ -306,15 +307,33 @@
   dataset ([docs](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//usage-overview/#private-database-access))
 - Create persistent
   identifiers ([docs](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//usage-overview/#assign-database-pid))
 - Execute
   queries ([docs](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//usage-overview/#export-subset))
 - Get data from tables/views/subsets
 
-## Future
+## Configure
+
+All credentials can optionally be set/overridden with environment variables. This is especially useful when sharing 
+Jupyter Notebooks by creating an invisible `.env` file and loading it:
+
+```
+REST_API_ENDPOINT="https://test.dbrepo.tuwien.ac.at"
+REST_API_USERNAME="foo"
+REST_API_PASSWORD="bar"
+REST_API_SECURE="True"
+AMQP_API_HOST="https://test.dbrepo.tuwien.ac.at"
+AMQP_API_PORT="5672"
+AMQP_API_USERNAME="foo"
+AMQP_API_PASSWORD="bar"
+AMQP_API_VIRTUAL_HOST="/"
+REST_UPLOAD_ENDPOINT="https://test.dbrepo.tuwien.ac.at/api/upload/files"
+```
+
+## Roadmap
 
 - Searching
 
 ## Contact
 
 * Prof. [Andreas Rauber](https://tiss.tuwien.ac.at/person/39608.html)<sup>TU Wien</sup>
 * DI. [Martin Weise](https://tiss.tuwien.ac.at/person/287722.html)<sup>TU Wien</sup>
```

### Comparing `dbrepo-1.4.2rc10/dbrepo.egg-info/SOURCES.txt` & `dbrepo-1.4.2rc11/dbrepo.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 dbrepo/AmqpClient.py
 dbrepo/RestClient.py
+dbrepo/UploadClient.py
 dbrepo/__init__.py
 dbrepo.egg-info/PKG-INFO
 dbrepo.egg-info/SOURCES.txt
 dbrepo.egg-info/dependency_links.txt
 dbrepo.egg-info/requires.txt
 dbrepo.egg-info/top_level.txt
 dbrepo/api/__init__.py
```

### Comparing `dbrepo-1.4.2rc10/pyproject.toml` & `dbrepo-1.4.2rc11/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbrepo"
-version = "1.4.2rc10"
+version = "1.4.2rc11"
 description = "DBRepo Python Library"
 keywords = [
     "DBRepo",
     "Database Repository"
 ]
 authors = [
     { name = "Martin Weise, TU Wien", email = "martin.weise@tuwien.ac.at" }
@@ -19,15 +19,16 @@
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.11"
 dependencies = [
     "requests >= 2.31",
     "pika",
     "pydantic",
-    "tuspy"
+    "tuspy",
+    "pandas"
 ]
 
 [build-system]
 requires = [
     "setuptools >= 61.0"
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `dbrepo-1.4.2rc10/tests/test_analyse.py` & `dbrepo-1.4.2rc11/tests/test_analyse.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class AnalyseTest(unittest.TestCase):
 
     def test_analyse_keys_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = KeyAnalysis(keys={'id': 0, 'firstname': 1, 'lastname': 2})
             # mock
-            mock.get('/api/analyse/keys', json=exp.model_dump_json(), status_code=202)
+            mock.get('/api/analyse/keys', json=exp.model_dump(), status_code=202)
             # test
             response = RestClient().analyse_keys(file_path='f705a7bd0cb2d5e37ab2b425036810a2', separator=',',
                                                  upload=False)
             self.assertEqual(exp, response)
 
 
 if __name__ == "__main__":
```

### Comparing `dbrepo-1.4.2rc10/tests/test_container.py` & `dbrepo-1.4.2rc11/tests/test_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                                                       unix_format="yyyy-MM-dd",
                                                       has_time=False,
                                                       created_at=datetime.datetime(2024, 3, 26, 0, 0, 0, 0,
                                                                                    datetime.timezone.utc)),
                                         ]),
                             hash="f829dd8a884182d0da846f365dee1221fd16610a14c81b8f9f295ff162749e50")
             # mock
-            mock.get('/api/container/1', json=exp.model_dump_json())
+            mock.get('/api/container/1', json=exp.model_dump())
             # test
             response = RestClient().get_container(container_id=1)
             self.assertEqual(exp, response)
 
     def test_get_container_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
```

### Comparing `dbrepo-1.4.2rc10/tests/test_database.py` & `dbrepo-1.4.2rc11/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                     jdbc_method='mariadb',
                     default_port=3306
                 )
             )
         )
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1', json=exp.model_dump_json())
+            mock.get('/api/database/1', json=exp.model_dump())
             # test
             response = RestClient().get_database(1)
             self.assertEqual(exp, response)
 
     def test_get_database_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
@@ -174,15 +174,15 @@
                     jdbc_method='mariadb',
                     default_port=3306
                 )
             )
         )
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database', json=exp.model_dump_json(), status_code=201)
+            mock.post('/api/database', json=exp.model_dump(), status_code=201)
             # test
             client = RestClient(username="a", password="b")
             response = client.create_database(name='test', container_id=1, is_public=True)
             self.assertEqual(response.name, 'test')
 
     def test_create_database_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
@@ -249,15 +249,15 @@
                     jdbc_method='mariadb',
                     default_port=3306
                 )
             )
         )
         with requests_mock.Mocker() as mock:
             # mock
-            mock.put('/api/database/1', json=exp.model_dump_json(), status_code=202)
+            mock.put('/api/database/1', json=exp.model_dump(), status_code=202)
             # test
             client = RestClient(username="a", password="b")
             response = client.update_database_visibility(database_id=1, is_public=True)
             self.assertEqual(response.is_public, True)
 
     def test_update_database_visibility_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
@@ -324,15 +324,15 @@
                     jdbc_method='mariadb',
                     default_port=3306
                 )
             )
         )
         with requests_mock.Mocker() as mock:
             # mock
-            mock.put('/api/database/1/owner', json=exp.model_dump_json(), status_code=202)
+            mock.put('/api/database/1/owner', json=exp.model_dump(), status_code=202)
             # test
             client = RestClient(username="a", password="b")
             response = client.update_database_owner(database_id=1, user_id='abdbf897-e599-4e5a-a3f0-7529884ea011')
             self.assertEqual(response.owner.id, 'abdbf897-e599-4e5a-a3f0-7529884ea011')
 
     def test_update_database_owner_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
@@ -372,15 +372,15 @@
     def test_get_database_access_succeeds(self):
         exp = DatabaseAccess(type=AccessType.READ,
                              created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                              user=User(id='abdbf897-e599-4e5a-a3f0-7529884ea011', username='other',
                                        attributes=UserAttributes(theme='light')))
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/access', json=exp.model_dump_json())
+            mock.get('/api/database/1/access', json=exp.model_dump())
             # test
             response = RestClient().get_database_access(database_id=1)
             self.assertEqual(response, AccessType.READ)
 
     def test_get_database_access_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
@@ -404,15 +404,15 @@
     def test_create_database_access_succeeds(self):
         exp = DatabaseAccess(type=AccessType.READ,
                              created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                              user=User(id='abdbf897-e599-4e5a-a3f0-7529884ea011', username='other',
                                        attributes=UserAttributes(theme='light')))
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/access/abdbf897-e599-4e5a-a3f0-7529884ea011', json=exp.model_dump_json(),
+            mock.post('/api/database/1/access/abdbf897-e599-4e5a-a3f0-7529884ea011', json=exp.model_dump(),
                       status_code=202)
             # test
             client = RestClient(username="a", password="b")
             response = client.create_database_access(database_id=1, type=AccessType.READ,
                                                      user_id='abdbf897-e599-4e5a-a3f0-7529884ea011')
             self.assertEqual(response, exp.type)
 
@@ -466,15 +466,15 @@
     def test_update_database_access_succeeds(self):
         exp = DatabaseAccess(type=AccessType.READ,
                              created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                              user=User(id='abdbf897-e599-4e5a-a3f0-7529884ea011', username='other',
                                        attributes=UserAttributes(theme='light')))
         with requests_mock.Mocker() as mock:
             # mock
-            mock.put('/api/database/1/access/abdbf897-e599-4e5a-a3f0-7529884ea011', json=exp.model_dump_json(),
+            mock.put('/api/database/1/access/abdbf897-e599-4e5a-a3f0-7529884ea011', json=exp.model_dump(),
                      status_code=202)
             # test
             client = RestClient(username="a", password="b")
             response = client.update_database_access(database_id=1, type=AccessType.READ,
                                                      user_id='abdbf897-e599-4e5a-a3f0-7529884ea011')
             self.assertEqual(response, exp.type)
```

### Comparing `dbrepo-1.4.2rc10/tests/test_identifier.py` & `dbrepo-1.4.2rc11/tests/test_identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                              titles=[IdentifierTitle(id=3, title='Test Title')],
                              funders=[IdentifierFunder(id=4, funder_name='FWF')],
                              related_identifiers=[
                                  RelatedIdentifier(id=7, value='10.12345/abc', relation=RelatedIdentifierRelation.CITES,
                                                    type=RelatedIdentifierType.DOI)],
                              creators=[IdentifierCreator(id=5, creator_name='Carberry, Josiah')])
             # mock
-            mock.post('/api/identifier', json=exp.model_dump_json(), status_code=201)
+            mock.post('/api/identifier', json=exp.model_dump(), status_code=201)
             # test
             client = RestClient(username="a", password="b")
             response = client.create_identifier(database_id=1, type=IdentifierType.VIEW,
                                                 titles=[CreateIdentifierTitle(title='Test Title')],
                                                 publisher='TU Wien', publication_year=2024,
                                                 language=Language.EN,
                                                 funders=[CreateIdentifierFunder(funder_name='FWF')],
@@ -133,15 +133,15 @@
                              publisher='TU Wien',
                              created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                              last_modified=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                              type=IdentifierType.VIEW,
                              creators=[IdentifierCreator(id=5, creator_name='Carberry, Josiah',
                                                          name_identifier='https://orcid.org/0000-0002-1825-0097')])
             # mock
-            mock.get('/api/identifier?url=https://orcid.org/0000-0002-1825-0097', json=exp.model_dump_json())
+            mock.get('/api/identifier?url=https://orcid.org/0000-0002-1825-0097', json=exp.model_dump())
             # test
             response = RestClient().suggest_identifier("https://orcid.org/0000-0002-1825-0097")
             self.assertEqual(exp, response)
 
     def test_suggest_identifier_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
```

### Comparing `dbrepo-1.4.2rc10/tests/test_license.py` & `dbrepo-1.4.2rc11/tests/test_license.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc10/tests/test_query.py` & `dbrepo-1.4.2rc11/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import unittest
+from json import dumps
+from typing import Any
 
 import requests_mock
 import datetime
 
 from dbrepo.RestClient import RestClient
+from pandas import DataFrame
 
 from dbrepo.api.dto import Result, Query, User, UserAttributes, QueryType
 from dbrepo.api.exceptions import MalformedError, NotExistsError, ForbiddenError, QueryStoreError, \
     MetadataConsistencyError, AuthenticationError
 
 
 class QueryTest(unittest.TestCase):
 
     def test_execute_query_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
                          headers=[{'id': 0, 'username': 1}],
                          id=None)
             # mock
-            mock.post('/api/database/1/query', json=exp.model_dump_json(), status_code=202)
+            mock.post('/api/database/1/query', json=exp.model_dump(), status_code=202)
             # test
             client = RestClient(username="a", password="b")
             response = client.execute_query(database_id=1, page=0, size=10,
                                             query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             self.assertEqual(exp, response)
 
     def test_execute_query_malformed_fails(self):
@@ -110,15 +113,15 @@
                         database_id=1,
                         query_hash='da5ff66c4a57683171e2ffcec25298ee684680d1e03633cd286f9067d6924ad8',
                         result_hash='464740ba612225913bb15b26f13377707949b55e65288e89c3f8b4c6469aecb4',
                         is_persisted=False,
                         result_number=None,
                         identifiers=[])
             # mock
-            mock.get('/api/database/1/query/6', json=exp.model_dump_json())
+            mock.get('/api/database/1/query/6', json=exp.model_dump())
             # test
             response = RestClient().get_query(database_id=1, query_id=6)
             self.assertEqual(exp, response)
 
     def test_find_query_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
@@ -233,19 +236,32 @@
 
     def test_get_query_data_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
                          headers=[{'id': 0, 'username': 1}],
                          id=6)
             # mock
-            mock.get('/api/database/1/query/6/data', json=exp.model_dump_json())
+            mock.get('/api/database/1/query/6/data', json=exp.model_dump())
             # test
             response = RestClient().get_query_data(database_id=1, query_id=6)
             self.assertEqual(exp, response)
 
+    def test_get_query_data_dataframe_succeeds(self):
+        with requests_mock.Mocker() as mock:
+            res = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
+                         headers=[{'id': 0, 'username': 1}],
+                         id=6)
+            exp = DataFrame.from_records(res.model_dump()['result'])
+            # mock
+            mock.get('/api/database/1/query/6/data', json=res.model_dump())
+            # test
+            response = RestClient().get_query_data(database_id=1, query_id=6, df=True)
+            self.assertEqual(exp.shape, response.shape)
+            self.assertTrue(DataFrame.equals(exp, response))
+
     def test_get_query_data_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.get('/api/database/1/query/6/data', status_code=403)
             # test
             try:
                 response = RestClient().get_query_data(database_id=1, query_id=6)
```

### Comparing `dbrepo-1.4.2rc10/tests/test_rest_client.py` & `dbrepo-1.4.2rc11/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.2rc10/tests/test_table.py` & `dbrepo-1.4.2rc11/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import unittest
+from json import dumps
 
 import requests_mock
 import datetime
 
 from dbrepo.RestClient import RestClient
+from pandas import DataFrame
 
 from dbrepo.api.dto import Table, CreateTableConstraints, UserAttributes, User, Column, Constraints, ColumnType, Result, \
     Concept, Unit, TableStatistics, ColumnStatistic
 from dbrepo.api.exceptions import MalformedError, ForbiddenError, NotExistsError, NameExistsError, QueryStoreError, \
     AuthenticationError
 
 
@@ -38,15 +40,15 @@
                                     auto_generated=True,
                                     is_primary_key=True,
                                     column_type=ColumnType.BIGINT,
                                     is_public=True,
                                     is_null_allowed=False)])
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/table', json=exp.model_dump_json(), status_code=201)
+            mock.post('/api/database/1/table', json=exp.model_dump(), status_code=201)
             # test
             client = RestClient(username="a", password="b")
             response = client.create_table(database_id=1, name="Test", description="Test Table", columns=[],
                                            constraints=CreateTableConstraints())
             self.assertEqual(exp, response)
 
     def test_create_table_malformed_fails(self):
@@ -175,15 +177,15 @@
                                         internal_name="id",
                                         auto_generated=True,
                                         is_primary_key=True,
                                         column_type=ColumnType.BIGINT,
                                         is_public=True,
                                         is_null_allowed=False)])
             # mock
-            mock.get('/api/database/1/table/2', json=exp.model_dump_json())
+            mock.get('/api/database/1/table/2', json=exp.model_dump())
             # test
             response = RestClient().get_table(database_id=1, table_id=2)
             self.assertEqual(exp, response)
 
     def test_get_table_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
@@ -246,19 +248,32 @@
 
     def test_get_table_data_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
                          headers=[{'id': 0, 'username': 1}],
                          id=None)
             # mock
-            mock.get('/api/database/1/table/9/data', json=exp.model_dump_json())
+            mock.get('/api/database/1/table/9/data', json=exp.model_dump())
             # test
             response = RestClient().get_table_data(database_id=1, table_id=9)
             self.assertEqual(exp, response)
 
+    def test_get_table_data_dataframe_succeeds(self):
+        with requests_mock.Mocker() as mock:
+            res = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
+                         headers=[{'id': 0, 'username': 1}],
+                         id=None)
+            exp = DataFrame.from_records(res.model_dump()['result'])
+            # mock
+            mock.get('/api/database/1/table/9/data', json=res.model_dump())
+            # test
+            response = RestClient().get_table_data(database_id=1, table_id=9, df=True)
+            self.assertEqual(exp.shape, response.shape)
+            self.assertTrue(DataFrame.equals(exp, response))
+
     def test_get_table_data_malformed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.get('/api/database/1/table/9/data', status_code=400)
             # test
             try:
                 response = RestClient().get_table_data(database_id=1, table_id=9)
@@ -554,15 +569,15 @@
                                          name="Precipitation"),
                          unit=Unit(id=2,
                                    uri="http://www.wikidata.org/entity/Q119856947",
                                    created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                                    name="liters per square meter"),
                          is_null_allowed=False)
             # mock
-            mock.put('/api/database/1/table/2/column/1', json=exp.model_dump_json(), status_code=202)
+            mock.put('/api/database/1/table/2/column/1', json=exp.model_dump(), status_code=202)
             # test
             client = RestClient(username="a", password="b")
             response = client.update_table_column(database_id=1, table_id=2, column_id=1,
                                                   unit_uri="http://www.wikidata.org/entity/Q119856947",
                                                   concept_uri="http://dbpedia.org/page/Category:Precipitation")
             self.assertEqual(exp, response)
 
@@ -618,15 +633,15 @@
                 pass
 
     def test_analyse_table_statistics_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = TableStatistics(
                 columns={"id": ColumnStatistic(val_min=1.0, val_max=9.0, mean=5.0, median=5.0, std_dev=2.73)})
             # mock
-            mock.get('/api/analyse/database/1/table/2/statistics', json=exp.model_dump_json(), status_code=202)
+            mock.get('/api/analyse/database/1/table/2/statistics', json=exp.model_dump(), status_code=202)
             # test
             response = RestClient().analyse_table_statistics(database_id=1, table_id=2)
             self.assertEqual(exp, response)
 
     def test_analyse_table_statistics_malformed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
```

### Comparing `dbrepo-1.4.2rc10/tests/test_user.py` & `dbrepo-1.4.2rc11/tests/test_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,81 +49,81 @@
             except ResponseCodeError as e:
                 pass
 
     def test_create_user_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise')
             # mock
-            mock.post('http://gateway-service/api/user', json=exp.model_dump_json(), status_code=201)
+            mock.post('http://gateway-service/api/user', json=exp.model_dump(), status_code=201)
             # test
             response = RestClient().create_user(username='mweise', password='s3cr3t', email='mweise@example.com')
             self.assertEqual(exp, response)
 
     def test_create_user_bad_request_fails(self):
         with requests_mock.Mocker() as mock:
             exp = UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise')
             # mock
-            mock.post('http://gateway-service/api/user', json=exp.model_dump_json(), status_code=400)
+            mock.post('http://gateway-service/api/user', json=exp.model_dump(), status_code=400)
             # test
             try:
                 response = RestClient().create_user(username='mweise', password='s3cr3t', email='mweise@example.com')
             except ResponseCodeError as e:
                 pass
 
     def test_create_user_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             exp = UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise')
             # mock
-            mock.post('http://gateway-service/api/user', json=exp.model_dump_json(), status_code=403)
+            mock.post('http://gateway-service/api/user', json=exp.model_dump(), status_code=403)
             # test
             try:
                 response = RestClient().create_user(username='mweise', password='s3cr3t', email='mweise@example.com')
             except ForbiddenError as e:
                 pass
 
     def test_create_user_username_exists_fails(self):
         with requests_mock.Mocker() as mock:
             exp = UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise')
             # mock
-            mock.post('http://gateway-service/api/user', json=exp.model_dump_json(), status_code=409)
+            mock.post('http://gateway-service/api/user', json=exp.model_dump(), status_code=409)
             # test
             try:
                 response = RestClient().create_user(username='mweise', password='s3cr3t', email='mweise@example.com')
             except UsernameExistsError as e:
                 pass
 
     def test_create_user_default_role_not_exists_fails(self):
         with requests_mock.Mocker() as mock:
             exp = UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise')
             # mock
-            mock.post('http://gateway-service/api/user', json=exp.model_dump_json(), status_code=404)
+            mock.post('http://gateway-service/api/user', json=exp.model_dump(), status_code=404)
             # test
             try:
                 response = RestClient().create_user(username='mweise', password='s3cr3t', email='mweise@example.com')
             except NotExistsError as e:
                 pass
 
     def test_create_user_emails_exists_fails(self):
         with requests_mock.Mocker() as mock:
             exp = UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise')
             # mock
-            mock.post('http://gateway-service/api/user', json=exp.model_dump_json(), status_code=417)
+            mock.post('http://gateway-service/api/user', json=exp.model_dump(), status_code=417)
             # test
             try:
                 response = RestClient().create_user(username='mweise', password='s3cr3t', email='mweise@example.com')
             except EmailExistsError as e:
                 pass
 
     def test_get_user_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = User(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise',
                        attributes=UserAttributes(theme='dark'))
             # mock
             mock.get('http://gateway-service/api/user/8638c043-5145-4be8-a3e4-4b79991b0a16',
-                     json=exp.model_dump_json())
+                     json=exp.model_dump())
             # test
             response = RestClient().get_user(user_id='8638c043-5145-4be8-a3e4-4b79991b0a16')
             self.assertEqual(exp, response)
 
     def test_get_user_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
@@ -136,15 +136,15 @@
 
     def test_update_user_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = User(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise', given_name='Martin',
                        attributes=UserAttributes(theme='dark'))
             # mock
             mock.put('http://gateway-service/api/user/8638c043-5145-4be8-a3e4-4b79991b0a16', status_code=202,
-                     json=exp.model_dump_json())
+                     json=exp.model_dump())
             # test
             client = RestClient(username="a", password="b")
             response = client.update_user(user_id='8638c043-5145-4be8-a3e4-4b79991b0a16', firstname='Martin')
             self.assertEqual(exp, response)
 
     def test_update_user_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
@@ -191,15 +191,15 @@
 
     def test_update_user_theme_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = User(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise', given_name='Martin',
                        attributes=UserAttributes(theme='dark'))
             # mock
             mock.put('http://gateway-service/api/user/8638c043-5145-4be8-a3e4-4b79991b0a16/theme', status_code=202,
-                     json=exp.model_dump_json())
+                     json=exp.model_dump())
             # test
             client = RestClient(username="a", password="b")
             response = client.update_user_theme(user_id='8638c043-5145-4be8-a3e4-4b79991b0a16', theme='dark')
             self.assertEqual(exp, response)
 
     def test_update_user_theme_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
@@ -246,15 +246,15 @@
 
     def test_update_user_password_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = User(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise', given_name='Martin',
                        attributes=UserAttributes(theme='dark'))
             # mock
             mock.put('http://gateway-service/api/user/8638c043-5145-4be8-a3e4-4b79991b0a16/password', status_code=202,
-                     json=exp.model_dump_json())
+                     json=exp.model_dump())
             # test
             client = RestClient(username="a", password="b")
             response = client.update_user_password(user_id='8638c043-5145-4be8-a3e4-4b79991b0a16',
                                                    password='s3cr3t1n0rm4t10n')
             self.assertEqual(exp, response)
 
     def test_update_user_password_not_allowed_fails(self):
```

### Comparing `dbrepo-1.4.2rc10/tests/test_view.py` & `dbrepo-1.4.2rc11/tests/test_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import unittest
+from json import dumps
 
 import requests_mock
 import datetime
 
 from dbrepo.RestClient import RestClient
+from pandas import DataFrame
 
 from dbrepo.api.dto import UserAttributes, User, View, Result
 from dbrepo.api.exceptions import ForbiddenError, NotExistsError, MalformedError, AuthenticationError
 
 
 class ViewTest(unittest.TestCase):
 
@@ -72,15 +74,15 @@
                        creator=User(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise',
                                     attributes=UserAttributes(theme='light')),
                        is_public=True,
                        created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                        last_modified=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                        identifiers=[])
             # mock
-            mock.get('/api/database/1/view/3', json=exp.model_dump_json())
+            mock.get('/api/database/1/view/3', json=exp.model_dump())
             # test
             response = RestClient().get_view(database_id=1, view_id=3)
             self.assertEqual(exp, response)
 
     def test_get_view_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
@@ -113,15 +115,15 @@
                        creator=User(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise',
                                     attributes=UserAttributes(theme='light')),
                        is_public=True,
                        created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                        last_modified=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                        identifiers=[])
             # mock
-            mock.post('/api/database/1/view', json=exp.model_dump_json(), status_code=201)
+            mock.post('/api/database/1/view', json=exp.model_dump(), status_code=201)
             # test
             client = RestClient(username="a", password="b")
             response = client.create_view(database_id=1, name="Data", is_public=True,
                                           query="SELECT id FROM mytable WHERE deg > 0")
             self.assertEqual(exp, response)
 
     def test_create_view_malformed_fails(self):
@@ -213,19 +215,32 @@
 
     def test_get_view_data_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
                          headers=[{'id': 0, 'username': 1}],
                          id=None)
             # mock
-            mock.get('/api/database/1/view/3/data', json=exp.model_dump_json())
+            mock.get('/api/database/1/view/3/data', json=exp.model_dump())
             # test
             response = RestClient().get_view_data(database_id=1, view_id=3)
             self.assertEqual(exp, response)
 
+    def test_get_view_data_dataframe_succeeds(self):
+        with requests_mock.Mocker() as mock:
+            res = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
+                         headers=[{'id': 0, 'username': 1}],
+                         id=None)
+            exp = DataFrame.from_records(res.model_dump()['result'])
+            # mock
+            mock.get('/api/database/1/view/3/data', json=res.model_dump())
+            # test
+            response: DataFrame = RestClient().get_view_data(database_id=1, view_id=3, df=True)
+            self.assertEqual(exp.shape, response.shape)
+            self.assertTrue(DataFrame.equals(exp, response))
+
     def test_get_view_data_malformed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.get('/api/database/1/view/3/data', status_code=400)
             # test
             try:
                 response = RestClient().get_view_data(database_id=1, view_id=3)
```

