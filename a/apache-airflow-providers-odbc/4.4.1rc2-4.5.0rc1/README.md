# Comparing `tmp/apache_airflow_providers_odbc-4.4.1rc2.tar.gz` & `tmp/apache_airflow_providers_odbc-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_odbc-4.4.1rc2.tar", last modified: Mon Jan 22 08:29:43 2024, max compression
+gzip compressed data, was "apache_airflow_providers_odbc-4.5.0rc1.tar", last modified: Tue Apr  9 12:36:44 2024, max compression
```

## Comparing `apache_airflow_providers_odbc-4.4.1rc2.tar` & `apache_airflow_providers_odbc-4.5.0rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4220 2024-01-22 08:29:43.000000 apache_airflow_providers_odbc-4.4.1rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:29:43.000000 apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/LICENSE
--rw-r--r--   0        0        0     1579 2024-01-22 08:29:43.000000 apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/__init__.py
--rw-r--r--   0        0        0     2428 2024-01-22 08:29:43.000000 apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-01-22 08:29:43.000000 apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/hooks/__init__.py
--rw-r--r--   0        0        0    10574 2024-01-22 08:29:43.000000 apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/hooks/odbc.py
--rw-r--r--   0        0        0     3047 2024-01-22 08:29:43.000000 apache_airflow_providers_odbc-4.4.1rc2/pyproject.toml
--rw-r--r--   0        0        0     6009 1970-01-01 00:00:00.000000 apache_airflow_providers_odbc-4.4.1rc2/PKG-INFO
+-rw-r--r--   0        0        0     4225 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/LICENSE
+-rw-r--r--   0        0        0     1579 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/__init__.py
+-rw-r--r--   0        0        0     2449 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/__init__.py
+-rw-r--r--   0        0        0     9984 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/odbc.py
+-rw-r--r--   0        0        0     3089 2024-04-09 12:36:44.000000 apache_airflow_providers_odbc-4.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 apache_airflow_providers_odbc-4.5.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/README.rst` & `apache_airflow_providers_odbc-4.5.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.4.1.rc2``
+Release: ``4.5.0.rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``odbc`` provider. All classes for this provider package
 are in ``airflow.providers.odbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-odbc``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -93,8 +93,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/LICENSE` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/__init__.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.4.1"
+__version__ = "4.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/get_provider_info.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-odbc",
         "name": "ODBC",
         "description": "`ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912183,
+        "source-date-epoch": 1712666204,
         "versions": [
+            "4.5.0",
             "4.4.1",
             "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.0",
             "3.3.0",
```

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/hooks/__init__.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/airflow/providers/odbc/hooks/odbc.py` & `apache_airflow_providers_odbc-4.5.0rc1/airflow/providers/odbc/hooks/odbc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains ODBC hook."""
+
 from __future__ import annotations
 
 from collections import namedtuple
 from typing import Any, List, Sequence, cast
 from urllib.parse import quote_plus
 
 from pyodbc import Connection, Row, connect
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.utils.helpers import merge_dicts
 
-DEFAULT_ODBC_PLACEHOLDERS = frozenset({"%s", "?"})
-
 
 class OdbcHook(DbApiHook):
     """
     Interact with odbc data sources using pyodbc.
 
     To configure driver, in addition to supplying as constructor arg, the following are also supported:
         * set ``driver`` parameter in ``hook_params`` dictionary when instantiating hook by SQL operators.
@@ -193,32 +192,18 @@
             merged_connect_kwargs["attrs_before"] = {
                 int(k): int(v) for k, v in merged_connect_kwargs["attrs_before"].items()
             }
 
         return merged_connect_kwargs
 
     def get_conn(self) -> Connection:
-        """Returns a pyodbc connection object."""
+        """Return ``pyodbc`` connection object."""
         conn = connect(self.odbc_connection_string, **self.connect_kwargs)
         return conn
 
-    @property
-    def placeholder(self):
-        placeholder = self.connection.extra_dejson.get("placeholder")
-        if placeholder in DEFAULT_ODBC_PLACEHOLDERS:
-            return placeholder
-        else:
-            self.log.warning(
-                "Placeholder defined in Connection '%s' is not listed in 'DEFAULT_ODBC_PLACEHOLDERS' "
-                "and got ignored. Falling back to the default placeholder '%s'.",
-                placeholder,
-                self._placeholder,
-            )
-            return self._placeholder
-
     def get_uri(self) -> str:
         """URI invoked in :meth:`~airflow.providers.common.sql.hooks.sql.DbApiHook.get_sqlalchemy_engine`."""
         quoted_conn_str = quote_plus(self.odbc_connection_string)
         uri = f"{self.sqlalchemy_scheme}:///?odbc_connect={quoted_conn_str}"
         return uri
 
     def get_sqlalchemy_connection(
```

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/pyproject.toml` & `apache_airflow_providers_odbc-4.5.0rc1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-odbc"
-version = "4.4.1.rc2"
+version = "4.5.0.rc1"
 description = "Provider package apache-airflow-providers-odbc for Apache Airflow"
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
-    "apache-airflow-providers-common-sql>=1.10.0.dev0",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow-providers-common-sql>=1.10.0rc0",
+    "apache-airflow>=2.6.0rc0",
     "pyodbc",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_odbc-4.4.1rc2/PKG-INFO` & `apache_airflow_providers_odbc-4.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-odbc
-Version: 4.4.1rc2
+Version: 4.5.0rc1
 Summary: Provider package apache-airflow-providers-odbc for Apache Airflow
 Keywords: airflow-provider,odbc,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,22 +15,23 @@
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
 Requires-Dist: pyodbc
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 
 
@@ -73,37 +74,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.4.1.rc2``
+Release: ``4.5.0.rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``odbc`` provider. All classes for this provider package
 are in ``airflow.providers.odbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-odbc``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -128,8 +129,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.4.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.5.0/changelog.html>`_.
```

