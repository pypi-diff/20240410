# Comparing `tmp/apache_airflow_providers_weaviate-1.3.3rc1.tar.gz` & `tmp/apache_airflow_providers_weaviate-1.3.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_weaviate-1.3.3rc1.tar", last modified: Mon Mar  4 12:46:23 2024, max compression
+gzip compressed data, was "apache_airflow_providers_weaviate-1.3.4rc1.tar", last modified: Tue Apr  9 12:42:44 2024, max compression
```

## Comparing `apache_airflow_providers_weaviate-1.3.3rc1.tar` & `apache_airflow_providers_weaviate-1.3.4rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3122 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/LICENSE
--rw-r--r--   0        0        0     1583 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/__init__.py
--rw-r--r--   0        0        0     2394 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/get_provider_info.py
--rw-r--r--   0        0        0     1053 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/hooks/__init__.py
--rw-r--r--   0        0        0    47559 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/hooks/weaviate.py
--rw-r--r--   0        0        0     1053 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/operators/__init__.py
--rw-r--r--   0        0        0     7962 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/operators/weaviate.py
--rw-r--r--   0        0        0     2968 2024-03-04 12:46:23.000000 apache_airflow_providers_weaviate-1.3.3rc1/pyproject.toml
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 apache_airflow_providers_weaviate-1.3.3rc1/PKG-INFO
+-rw-r--r--   0        0        0     3127 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/LICENSE
+-rw-r--r--   0        0        0     1583 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/__init__.py
+-rw-r--r--   0        0        0     2403 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/get_provider_info.py
+-rw-r--r--   0        0        0     1053 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/__init__.py
+-rw-r--r--   0        0        0    47541 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/weaviate.py
+-rw-r--r--   0        0        0     1053 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/__init__.py
+-rw-r--r--   0        0        0     8500 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/weaviate.py
+-rw-r--r--   0        0        0     3012 2024-04-09 12:42:44.000000 apache_airflow_providers_weaviate-1.3.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 apache_airflow_providers_weaviate-1.3.4rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/README.rst` & `apache_airflow_providers_weaviate-1.3.4rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,44 +38,44 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-weaviate``
 
-Release: ``1.3.3.rc1``
+Release: ``1.3.4.rc1``
 
 
 `Weaviate <https://weaviate.io/developers/weaviate>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``weaviate`` provider. All classes for this provider package
 are in ``airflow.providers.weaviate`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-weaviate``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
 ``apache-airflow``   ``>=2.6.0``
 ``weaviate-client``  ``>=3.24.2``
 ``pandas``           ``>=1.2.5,<2.2``
 ===================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/changelog.html>`_.
```

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/LICENSE` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/__init__.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/get_provider_info.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-weaviate",
         "name": "Weaviate",
         "description": "`Weaviate <https://weaviate.io/developers/weaviate>`__\n",
         "state": "ready",
-        "source-date-epoch": 1709556383,
-        "versions": ["1.3.3", "1.3.2", "1.3.1", "1.3.0", "1.2.0", "1.1.0", "1.0.0"],
+        "source-date-epoch": 1712666564,
+        "versions": ["1.3.4", "1.3.3", "1.3.2", "1.3.1", "1.3.0", "1.2.0", "1.1.0", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Weaviate",
                 "external-doc-url": "https://weaviate.io/developers/weaviate",
                 "how-to-guide": ["/docs/apache-airflow-providers-weaviate/operators/weaviate.rst"],
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/hooks/__init__.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/hooks/weaviate.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/hooks/weaviate.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
 
         if not batch_config_params.get("connection_error_retries"):
             batch_config_params["connection_error_retries"] = 5
 
         client.batch.configure(**batch_config_params)
         with client.batch as batch:
             # Batch import all data
-            for index, data_obj in enumerate(converted_data):
+            for data_obj in converted_data:
                 for attempt in Retrying(
                     stop=stop_after_attempt(retry_attempts_per_object),
                     retry=(
                         retry_if_exception(lambda exc: check_http_error_is_retryable(exc))
                         | retry_if_exception_type(REQUESTS_EXCEPTIONS_TYPES)
                     ),
                 ):
```

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/operators/__init__.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/airflow/providers/weaviate/operators/weaviate.py` & `apache_airflow_providers_weaviate-1.3.4rc1/airflow/providers/weaviate/operators/weaviate.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,43 +42,48 @@
     Operator that accepts input json or pandas dataframe to generate embeddings on or accepting provided
     custom vectors and store them in the Weaviate class.
 
     :param conn_id: The Weaviate connection.
     :param class_name: The Weaviate class to be used for storing the data objects into.
     :param input_data: The list of dicts or pandas dataframe representing Weaviate data objects to generate
         embeddings on (or provides custom vectors) and store them in the Weaviate class.
-    :param input_json: (Deprecated) The JSON representing Weaviate data objects to generate embeddings on (or provides
-        custom vectors) and store them in the Weaviate class.
     :param vector_col: key/column name in which the vectors are stored.
+    :param batch_params: Additional parameters for Weaviate batch configuration.
+    :param hook_params: Optional config params to be passed to the underlying hook.
+        Should match the desired hook constructor params.
+    :param input_json: (Deprecated) The JSON representing Weaviate data objects to generate embeddings on
+        (or provides custom vectors) and store them in the Weaviate class.
     """
 
     template_fields: Sequence[str] = ("input_json", "input_data")
 
     def __init__(
         self,
         conn_id: str,
         class_name: str,
-        input_json: list[dict[str, Any]] | pd.DataFrame | None = None,
         input_data: list[dict[str, Any]] | pd.DataFrame | None = None,
         vector_col: str = "Vector",
         uuid_column: str = "id",
         tenant: str | None = None,
+        batch_params: dict | None = None,
+        hook_params: dict | None = None,
+        input_json: list[dict[str, Any]] | pd.DataFrame | None = None,
         **kwargs: Any,
     ) -> None:
-        self.batch_params = kwargs.pop("batch_params", {})
-        self.hook_params = kwargs.pop("hook_params", {})
-
         super().__init__(**kwargs)
         self.class_name = class_name
         self.conn_id = conn_id
         self.vector_col = vector_col
         self.input_json = input_json
         self.uuid_column = uuid_column
         self.tenant = tenant
         self.input_data = input_data
+        self.batch_params = batch_params or {}
+        self.hook_params = hook_params or {}
+
         if (self.input_data is None) and (input_json is not None):
             warnings.warn(
                 "Passing 'input_json' to WeaviateIngestOperator is deprecated and"
                 " you should use 'input_data' instead",
                 AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
@@ -131,15 +136,16 @@
     :param existing: Strategy for handling existing data: 'skip', or 'replace'. Default is 'skip'.
     :param document_column: Column in DataFrame that identifying source document.
     :param uuid_column: Column with pre-generated UUIDs. If not provided, UUIDs will be generated.
     :param vector_column: Column with embedding vectors for pre-embedded data.
     :param batch_config_params: Additional parameters for Weaviate batch configuration.
     :param tenant: The tenant to which the object will be added.
     :param verbose: Flag to enable verbose output during the ingestion process.
-    :return: list of UUID which failed to create
+    :param hook_params: Optional config params to be passed to the underlying hook.
+        Should match the desired hook constructor params.
     """
 
     template_fields: Sequence[str] = ("input_data",)
 
     def __init__(
         self,
         conn_id: str,
@@ -148,37 +154,41 @@
         document_column: str,
         existing: str = "skip",
         uuid_column: str = "id",
         vector_col: str = "Vector",
         batch_config_params: dict | None = None,
         tenant: str | None = None,
         verbose: bool = False,
+        hook_params: dict | None = None,
         **kwargs: Any,
     ) -> None:
-        self.hook_params = kwargs.pop("hook_params", {})
-
         super().__init__(**kwargs)
-
         self.conn_id = conn_id
         self.input_data = input_data
         self.class_name = class_name
         self.document_column = document_column
         self.existing = existing
         self.uuid_column = uuid_column
         self.vector_col = vector_col
         self.batch_config_params = batch_config_params
         self.tenant = tenant
         self.verbose = verbose
+        self.hook_params = hook_params or {}
 
     @cached_property
     def hook(self) -> WeaviateHook:
         """Return an instance of the WeaviateHook."""
         return WeaviateHook(conn_id=self.conn_id, **self.hook_params)
 
     def execute(self, context: Context) -> list:
+        """
+        Create or replace objects belonging to documents.
+
+        :return: List of UUID which failed to create
+        """
         self.log.debug("Total input objects : %s", len(self.input_data))
         insertion_errors = self.hook.create_or_replace_document_objects(
             data=self.input_data,
             class_name=self.class_name,
             document_column=self.document_column,
             existing=self.existing,
             uuid_column=self.uuid_column,
```

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/pyproject.toml` & `apache_airflow_providers_weaviate-1.3.4rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-weaviate"
-version = "1.3.3.rc1"
+version = "1.3.4.rc1"
 description = "Provider package apache-airflow-providers-weaviate for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,26 +47,27 @@
     "Framework :: Apache Airflow",
     "Framework :: Apache Airflow :: Provider",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow>=2.6.0rc0",
     "pandas>=1.2.5,<2.2",
     "weaviate-client>=3.24.2",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_weaviate-1.3.3rc1/PKG-INFO` & `apache_airflow_providers_weaviate-1.3.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-weaviate
-Version: 1.3.3rc1
+Version: 1.3.4rc1
 Summary: Provider package apache-airflow-providers-weaviate for Apache Airflow
 Keywords: airflow-provider,weaviate,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,21 +15,22 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: pandas>=1.2.5,<2.2
 Requires-Dist: weaviate-client>=3.24.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -71,44 +72,44 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-weaviate``
 
-Release: ``1.3.3.rc1``
+Release: ``1.3.4.rc1``
 
 
 `Weaviate <https://weaviate.io/developers/weaviate>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``weaviate`` provider. All classes for this provider package
 are in ``airflow.providers.weaviate`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-weaviate``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
 ``apache-airflow``   ``>=2.6.0``
 ``weaviate-client``  ``>=3.24.2``
 ``pandas``           ``>=1.2.5,<2.2``
 ===================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.3/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-weaviate/1.3.4/changelog.html>`_.
```

