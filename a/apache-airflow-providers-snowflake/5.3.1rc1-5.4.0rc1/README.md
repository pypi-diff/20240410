# Comparing `tmp/apache_airflow_providers_snowflake-5.3.1rc1.tar.gz` & `tmp/apache_airflow_providers_snowflake-5.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_snowflake-5.3.1rc1.tar", last modified: Sun Feb 11 07:28:45 2024, max compression
+gzip compressed data, was "apache_airflow_providers_snowflake-5.4.0rc1.tar", last modified: Tue Apr  9 12:41:54 2024, max compression
```

## Comparing `apache_airflow_providers_snowflake-5.3.1rc1.tar` & `apache_airflow_providers_snowflake-5.4.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4480 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/LICENSE
--rw-r--r--   0        0        0     1584 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/__init__.py
--rw-r--r--   0        0        0     4700 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0        0        0    21173 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0        0        0    12701 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0        0        0    26371 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/operators/snowflake.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0        0        0    12632 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0        0        0     4223 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0        0        0     1644 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0        0        0     6762 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
--rw-r--r--   0        0        0     3208 2024-02-11 07:28:45.000000 apache_airflow_providers_snowflake-5.3.1rc1/pyproject.toml
--rw-r--r--   0        0        0     6469 1970-01-01 00:00:00.000000 apache_airflow_providers_snowflake-5.3.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     4485 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/LICENSE
+-rw-r--r--   0        0        0     1584 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0        0        0     4721 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0        0        0    21418 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0        0        0    14773 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0        0        0    26383 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/snowflake.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0        0        0    12631 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0        0        0     4223 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0        0        0     1644 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0        0        0     6762 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+-rw-r--r--   0        0        0     3250 2024-04-09 12:41:54.000000 apache_airflow_providers_snowflake-5.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6521 1970-01-01 00:00:00.000000 apache_airflow_providers_snowflake-5.4.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/README.rst` & `apache_airflow_providers_snowflake-5.4.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``5.3.1.rc1``
+Release: ``5.4.0.rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-snowflake``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -95,8 +95,8 @@
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/LICENSE` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.3.1"
+__version__ = "5.4.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/get_provider_info.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-snowflake",
         "name": "Snowflake",
         "description": "`Snowflake <https://www.snowflake.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1707636525,
+        "source-date-epoch": 1712666514,
         "versions": [
+            "5.4.0",
             "5.3.1",
             "5.3.0",
             "5.2.1",
             "5.2.0",
             "5.1.2",
             "5.1.1",
             "5.1.0",
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/hooks/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/hooks/snowflake.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,23 @@
                 format=serialization.PrivateFormat.PKCS8,
                 encryption_algorithm=serialization.NoEncryption(),
             )
 
             conn_config["private_key"] = pkb
             conn_config.pop("password", None)
 
+        refresh_token = self._get_field(extra_dict, "refresh_token") or ""
+        if refresh_token:
+            conn_config["refresh_token"] = refresh_token
+            conn_config["authenticator"] = "oauth"
+            conn_config["client_id"] = conn.login
+            conn_config["client_secret"] = conn.password
+            conn_config.pop("login", None)
+            conn_config.pop("password", None)
+
         return conn_config
 
     def get_uri(self) -> str:
         """Override DbApiHook get_uri method for get_sqlalchemy_engine()."""
         conn_params = self._get_conn_params()
         return self._conn_params_to_sqlalchemy_uri(conn_params)
 
@@ -308,47 +317,43 @@
         sql: str | Iterable[str],
         autocommit: bool = ...,
         parameters: Iterable | Mapping[str, Any] | None = ...,
         handler: None = ...,
         split_statements: bool = ...,
         return_last: bool = ...,
         return_dictionaries: bool = ...,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @overload
     def run(
         self,
         sql: str | Iterable[str],
         autocommit: bool = ...,
         parameters: Iterable | Mapping[str, Any] | None = ...,
         handler: Callable[[Any], T] = ...,
         split_statements: bool = ...,
         return_last: bool = ...,
         return_dictionaries: bool = ...,
-    ) -> tuple | list[tuple] | list[list[tuple] | tuple] | None:
-        ...
+    ) -> tuple | list[tuple] | list[list[tuple] | tuple] | None: ...
 
     def run(
         self,
         sql: str | Iterable[str],
         autocommit: bool = False,
         parameters: Iterable | Mapping[str, Any] | None = None,
         handler: Callable[[Any], T] | None = None,
         split_statements: bool = True,
         return_last: bool = True,
         return_dictionaries: bool = False,
     ) -> tuple | list[tuple] | list[list[tuple] | tuple] | None:
         """Run a command or list of commands.
 
         Pass a list of SQL statements to the SQL parameter to get them to
-        execute sequentially. The variable ``execution_info`` is returned so
-        that it can be used in the Operators to modify the behavior depending on
-        the result of the query (i.e fail the operator if the copy has processed
-        0 files).
+        execute sequentially. The result of the queries is returned if the
+        ``handler`` callable is set.
 
         :param sql: The SQL string to be executed with possibly multiple
             statements, or a list of sql statements to execute
         :param autocommit: What to set the connection's autocommit setting to
             before executing the query.
         :param parameters: The parameters to render the SQL query with.
         :param handler: The result handler which is called with the result of
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,30 +21,32 @@
 from pathlib import Path
 from typing import Any
 
 import aiohttp
 import requests
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
+from requests.auth import HTTPBasicAuth
 
 from airflow.exceptions import AirflowException
 from airflow.providers.snowflake.hooks.snowflake import SnowflakeHook
 from airflow.providers.snowflake.utils.sql_api_generate_jwt import JWTGenerator
 
 
 class SnowflakeSqlApiHook(SnowflakeHook):
     """
     A client to interact with Snowflake using SQL API and submit multiple SQL statements in a single request.
 
     In combination with aiohttp, make post request to submit SQL statements for execution,
     poll to check the status of the execution of a statement. Fetch query results asynchronously.
 
     This hook requires the snowflake_conn_id connection. This hooks mainly uses account, schema, database,
-     warehouse, private_key_file or private_key_content field must be setup in the connection. Other inputs
-      can be defined in the connection or hook instantiation.
+    warehouse, and an authentication mechanism from one of below:
+    1. JWT Token generated from private_key_file or private_key_content. Other inputs can be defined in the connection or hook instantiation.
+    2. OAuth Token generated from the refresh_token, client_id and client_secret specified in the connection
 
     :param snowflake_conn_id: Reference to
         :ref:`Snowflake connection id<howto/connection:snowflake>`
     :param account: snowflake account name
     :param authenticator: authenticator for Snowflake.
         'snowflake' (default) to use the internal Snowflake authenticator
         'externalbrowser' to authenticate using your web browser and
@@ -77,14 +79,25 @@
     ):
         self.snowflake_conn_id = snowflake_conn_id
         self.token_life_time = token_life_time
         self.token_renewal_delta = token_renewal_delta
         super().__init__(snowflake_conn_id, *args, **kwargs)
         self.private_key: Any = None
 
+    @property
+    def account_identifier(self) -> str:
+        """Returns snowflake account identifier."""
+        conn_config = self._get_conn_params()
+        account_identifier = f"https://{conn_config['account']}"
+
+        if conn_config["region"]:
+            account_identifier += f".{conn_config['region']}"
+
+        return account_identifier
+
     def get_private_key(self) -> None:
         """Get the private key from snowflake connection."""
         conn = self.get_connection(self.snowflake_conn_id)
 
         # If private_key_file is specified in the extra json, load the contents of the file as a private key.
         # If private_key_content is specified in the extra json, use it as a private key.
         # As a next step, specify this private key in the connection configuration.
@@ -133,18 +146,15 @@
         :param bindings: (Optional) Values of bind variables in the SQL statement.
             When executing the statement, Snowflake replaces placeholders (? and :name) in
             the statement with these specified values.
         """
         conn_config = self._get_conn_params()
 
         req_id = uuid.uuid4()
-        url = (
-            f"https://{conn_config['account']}.{conn_config['region']}"
-            f".snowflakecomputing.com/api/v2/statements"
-        )
+        url = f"{self.account_identifier}.snowflakecomputing.com/api/v2/statements"
         params: dict[str, Any] | None = {"requestId": str(req_id), "async": True, "pageSize": 10}
         headers = self.get_headers()
         if bindings is None:
             bindings = {}
         data = {
             "statement": sql,
             "resultSetMetaData": {"format": "json"},
@@ -171,20 +181,35 @@
         elif "statementHandle" in json_response:
             self.query_ids.append(json_response["statementHandle"])
         else:
             raise AirflowException("No statementHandle/statementHandles present in response")
         return self.query_ids
 
     def get_headers(self) -> dict[str, Any]:
-        """Form JWT Token and header based on the private key, and connection details."""
+        """Form auth headers based on either OAuth token or JWT token from private key."""
+        conn_config = self._get_conn_params()
+
+        # Use OAuth if refresh_token and client_id and client_secret are provided
+        if all(
+            [conn_config.get("refresh_token"), conn_config.get("client_id"), conn_config.get("client_secret")]
+        ):
+            oauth_token = self.get_oauth_token()
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {oauth_token}",
+                "Accept": "application/json",
+                "User-Agent": "snowflakeSQLAPI/1.0",
+                "X-Snowflake-Authorization-Token-Type": "OAUTH",
+            }
+            return headers
+
+        # Alternatively, get the JWT token from the connection details and the private key
         if not self.private_key:
             self.get_private_key()
-        conn_config = self._get_conn_params()
 
-        # Get the JWT token from the connection details and the private key
         token = JWTGenerator(
             conn_config["account"],  # type: ignore[arg-type]
             conn_config["user"],  # type: ignore[arg-type]
             private_key=self.private_key,
             lifetime=self.token_life_time,
             renewal_delay=self.token_renewal_delta,
         ).get_token()
@@ -194,28 +219,49 @@
             "Authorization": f"Bearer {token}",
             "Accept": "application/json",
             "User-Agent": "snowflakeSQLAPI/1.0",
             "X-Snowflake-Authorization-Token-Type": "KEYPAIR_JWT",
         }
         return headers
 
+    def get_oauth_token(self) -> str:
+        """Generate temporary OAuth access token using refresh token in connection details."""
+        conn_config = self._get_conn_params()
+        url = f"{self.account_identifier}.snowflakecomputing.com/oauth/token-request"
+        data = {
+            "grant_type": "refresh_token",
+            "refresh_token": conn_config["refresh_token"],
+            "redirect_uri": conn_config.get("redirect_uri", "https://localhost.com"),
+        }
+        response = requests.post(
+            url,
+            data=data,
+            headers={
+                "Content-Type": "application/x-www-form-urlencoded",
+            },
+            auth=HTTPBasicAuth(conn_config["client_id"], conn_config["client_secret"]),  # type: ignore[arg-type]
+        )
+
+        try:
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as e:  # pragma: no cover
+            msg = f"Response: {e.response.content.decode()} Status Code: {e.response.status_code}"
+            raise AirflowException(msg)
+        return response.json()["access_token"]
+
     def get_request_url_header_params(self, query_id: str) -> tuple[dict[str, Any], dict[str, Any], str]:
         """
         Build the request header Url with account name identifier and query id from the connection params.
 
         :param query_id: statement handles query ids for the individual statements.
         """
-        conn_config = self._get_conn_params()
         req_id = uuid.uuid4()
         header = self.get_headers()
         params = {"requestId": str(req_id)}
-        url = (
-            f"https://{conn_config['account']}.{conn_config['region']}"
-            f".snowflakecomputing.com/api/v2/statements/{query_id}"
-        )
+        url = f"{self.account_identifier}.snowflakecomputing.com/api/v2/statements/{query_id}"
         return header, params, url
 
     def check_query_output(self, query_ids: list[str]) -> None:
         """
         Make HTTP request to snowflake SQL API based on the provided query ids and log the response.
 
         :param query_ids: statement handles query id for the individual statements.
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/operators/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/operators/snowflake.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
     :param statement_count: Number of SQL statement to be executed
     :param token_life_time: lifetime of the JWT Token
     :param token_renewal_delta: Renewal time of the JWT Token
     :param bindings: (Optional) Values of bind variables in the SQL statement.
             When executing the statement, Snowflake replaces placeholders (? and :name) in
             the statement with these specified values.
     :param deferrable: Run operator in the deferrable mode.
-    """  # noqa
+    """  # noqa: D205, D400
 
     LIFETIME = timedelta(minutes=59)  # The tokens will have a 59 minutes lifetime
     RENEWAL_DELTA = timedelta(minutes=54)  # Tokens will be renewed after 54 minutes
 
     def __init__(
         self,
         *,
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/transfers/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Abstract operator that child classes implement ``COPY INTO <TABLE> SQL in Snowflake``."""
+
 from __future__ import annotations
 
 from typing import Any, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.snowflake.hooks.snowflake import SnowflakeHook
 from airflow.providers.snowflake.utils.common import enclose_param
@@ -250,16 +251,16 @@
             query_results
         )
         input_datasets = [Dataset(namespace=namespace, name=name) for namespace, name in unique_dataset_paths]
 
         run_facets = {}
         if extraction_error_files:
             self.log.debug(
-                f"Unable to extract Dataset namespace and name "
-                f"for the following files: `{extraction_error_files}`."
+                "Unable to extract Dataset namespace and name for the following files: `%s`.",
+                extraction_error_files,
             )
             run_facets["extractionError"] = ExtractionErrorRunFacet(
                 totalTasks=len(query_results),
                 failedTasks=len(extraction_error_files),
                 errors=[
                     ExtractionError(
                         errorMessage="Unable to extract Dataset namespace and name.",
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/triggers/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/utils/__init__.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/utils/common.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache_airflow_providers_snowflake-5.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/pyproject.toml` & `apache_airflow_providers_snowflake-5.4.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-snowflake"
-version = "5.3.1.rc1"
+version = "5.4.0.rc1"
 description = "Provider package apache-airflow-providers-snowflake for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,27 +47,28 @@
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
-    "apache-airflow-providers-common-sql>=1.10.0.dev0",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow-providers-common-sql>=1.10.0rc0",
+    "apache-airflow>=2.6.0rc0",
     "snowflake-connector-python>=2.7.8",
     "snowflake-sqlalchemy>=1.1.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_snowflake-5.3.1rc1/PKG-INFO` & `apache_airflow_providers_snowflake-5.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 5.3.1rc1
+Version: 5.4.0rc1
 Summary: Provider package apache-airflow-providers-snowflake for Apache Airflow
 Keywords: airflow-provider,snowflake,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,24 +15,25 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.10.0.dev0
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow-providers-common-sql>=1.10.0rc0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: snowflake-connector-python>=2.7.8
 Requires-Dist: snowflake-sqlalchemy>=1.1.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 Provides-Extra: openlineage
 
@@ -76,37 +77,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``5.3.1.rc1``
+Release: ``5.4.0.rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-snowflake``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -133,8 +134,8 @@
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/5.4.0/changelog.html>`_.
```

