# Comparing `tmp/apache_airflow_providers_ftp-3.8.0rc1.tar.gz` & `tmp/apache_airflow_providers_ftp-3.8.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_ftp-3.8.0rc1.tar", last modified: Mon Jan 22 08:28:14 2024, max compression
+gzip compressed data, was "apache_airflow_providers_ftp-3.8.0rc2.tar", last modified: Tue Apr  9 12:29:54 2024, max compression
```

## Comparing `apache_airflow_providers_ftp-3.8.0rc1.tar` & `apache_airflow_providers_ftp-3.8.0rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4074 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/LICENSE
--rw-r--r--   0        0        0     1578 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/__init__.py
--rw-r--r--   0        0        0     2980 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0        0        0     9543 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/hooks/ftp.py
--rw-r--r--   0        0        0      785 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0        0        0     8172 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/operators/ftp.py
--rw-r--r--   0        0        0      787 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0        0        0     3523 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/sensors/ftp.py
--rw-r--r--   0        0        0     2972 2024-01-22 08:28:14.000000 apache_airflow_providers_ftp-3.8.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5775 1970-01-01 00:00:00.000000 apache_airflow_providers_ftp-3.8.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4079 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/LICENSE
+-rw-r--r--   0        0        0     1578 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/__init__.py
+-rw-r--r--   0        0        0     2980 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0        0        0     9720 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/hooks/ftp.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0        0        0     8209 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/operators/ftp.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0        0        0     3523 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/sensors/ftp.py
+-rw-r--r--   0        0        0     3016 2024-04-09 12:29:54.000000 apache_airflow_providers_ftp-3.8.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5829 1970-01-01 00:00:00.000000 apache_airflow_providers_ftp-3.8.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/README.rst` & `apache_airflow_providers_ftp-3.8.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.8.0.rc1``
+Release: ``3.8.0.rc2``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
@@ -60,15 +60,15 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
```

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/LICENSE` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/__init__.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/get_provider_info.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-ftp",
         "name": "File Transfer Protocol (FTP)",
         "description": "`File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912094,
+        "source-date-epoch": 1712665794,
         "versions": [
             "3.8.0",
             "3.7.0",
             "3.6.1",
             "3.6.0",
             "3.5.2",
             "3.5.1",
```

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/hooks/__init__.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/hooks/ftp.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/hooks/ftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     """
 
     conn_name_attr = "ftp_conn_id"
     default_conn_name = "ftp_default"
     conn_type = "ftp"
     hook_name = "FTP"
 
-    def __init__(self, ftp_conn_id: str = default_conn_name, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, ftp_conn_id: str = default_conn_name) -> None:
+        super().__init__()
         self.ftp_conn_id = ftp_conn_id
         self.conn: ftplib.FTP | None = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
@@ -266,18 +266,22 @@
 
 
 class FTPSHook(FTPHook):
     """Interact with FTPS."""
 
     def get_conn(self) -> ftplib.FTP:
         """Return an FTPS connection object."""
+        import ssl
+
         if self.conn is None:
             params = self.get_connection(self.ftp_conn_id)
             pasv = params.extra_dejson.get("passive", True)
 
             if params.port:
                 ftplib.FTP_TLS.port = params.port
 
-            self.conn = ftplib.FTP_TLS(params.host, params.login, params.password)  # nosec: B321
+            # Construct FTP_TLS instance with SSL context to allow certificates to be validated by default
+            context = ssl.create_default_context()
+            self.conn = ftplib.FTP_TLS(params.host, params.login, params.password, context=context)  # nosec: B321
             self.conn.set_pasv(pasv)
 
         return self.conn
```

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/operators/__init__.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/operators/ftp.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/operators/ftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains FTP operator."""
+
 from __future__ import annotations
 
 import os
 import socket
 from ftplib import FTP_PORT  # nosec: B402
 from functools import cached_property
 from pathlib import Path
@@ -152,15 +153,17 @@
         scheme = "file"
 
         local_host = socket.gethostname()
         try:
             local_host = socket.gethostbyname(local_host)
         except Exception as e:
             self.log.warning(
-                f"Failed to resolve local hostname. Using the hostname got by socket.gethostbyname() without resolution. {e}",
+                "Failed to resolve local hostname. "
+                "Using the hostname got by socket.gethostbyname() without resolution. %s",
+                e,
                 exc_info=True,
             )
 
         conn = self.hook.get_conn()
         remote_host = conn.host
         remote_port = conn.port
```

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/sensors/__init__.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/airflow/providers/ftp/sensors/ftp.py` & `apache_airflow_providers_ftp-3.8.0rc2/airflow/providers/ftp/sensors/ftp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/pyproject.toml` & `apache_airflow_providers_ftp-3.8.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-ftp"
-version = "3.8.0.rc1"
+version = "3.8.0.rc2"
 description = "Provider package apache-airflow-providers-ftp for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,19 +47,20 @@
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
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.8.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.8.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_ftp-3.8.0rc1/PKG-INFO` & `apache_airflow_providers_ftp-3.8.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.8.0rc1
+Version: 3.8.0rc2
 Summary: Provider package apache-airflow-providers-ftp for Apache Airflow
 Keywords: airflow-provider,ftp,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,16 +15,17 @@
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
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.8.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.8.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -71,15 +72,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.8.0.rc1``
+Release: ``3.8.0.rc2``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
@@ -93,15 +94,15 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
```

