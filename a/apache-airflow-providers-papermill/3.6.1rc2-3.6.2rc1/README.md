# Comparing `tmp/apache_airflow_providers_papermill-3.6.1rc2.tar.gz` & `tmp/apache_airflow_providers_papermill-3.6.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_papermill-3.6.1rc2.tar", last modified: Mon Jan 22 08:30:16 2024, max compression
+gzip compressed data, was "apache_airflow_providers_papermill-3.6.2rc1.tar", last modified: Tue Apr  9 12:38:44 2024, max compression
```

## Comparing `apache_airflow_providers_papermill-3.6.1rc2.tar` & `apache_airflow_providers_papermill-3.6.2rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3114 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/LICENSE
--rw-r--r--   0        0        0     1584 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/__init__.py
--rw-r--r--   0        0        0     2814 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/hooks/__init__.py
--rw-r--r--   0        0        0     6009 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/hooks/kernel.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/operators/__init__.py
--rw-r--r--   0        0        0     4689 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/operators/papermill.py
--rw-r--r--   0        0        0     2986 2024-01-22 08:30:16.000000 apache_airflow_providers_papermill-3.6.1rc2/pyproject.toml
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 apache_airflow_providers_papermill-3.6.1rc2/PKG-INFO
+-rw-r--r--   0        0        0     3114 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/LICENSE
+-rw-r--r--   0        0        0     1584 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/__init__.py
+-rw-r--r--   0        0        0     2881 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/__init__.py
+-rw-r--r--   0        0        0     5937 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/kernel.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/__init__.py
+-rw-r--r--   0        0        0     4689 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/papermill.py
+-rw-r--r--   0        0        0     2984 2024-04-09 12:38:44.000000 apache_airflow_providers_papermill-3.6.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 apache_airflow_providers_papermill-3.6.2rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/README.rst` & `apache_airflow_providers_papermill-3.6.2rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.6.1.rc2``
+Release: ``3.6.2.rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``papermill`` provider. All classes for this provider package
 are in ``airflow.providers.papermill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-papermill``
@@ -75,8 +75,8 @@
 ``apache-airflow``  ``>=2.6.0``
 ``papermill[all]``  ``>=2.4.0``
 ``scrapbook[all]``
 ``ipykernel``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2/changelog.html>`_.
```

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/LICENSE` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/__init__.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.6.1"
+__version__ = "3.6.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/get_provider_info.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-papermill",
         "name": "Papermill",
         "description": "`Papermill <https://github.com/nteract/papermill>`__\n",
+        "excluded-python-versions": ["3.12"],
         "state": "ready",
-        "source-date-epoch": 1705912216,
+        "source-date-epoch": 1712666324,
         "versions": [
+            "3.6.2",
             "3.6.1",
             "3.6.0",
             "3.5.0",
             "3.4.0",
             "3.2.1",
             "3.2.0",
             "3.1.1",
```

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/hooks/__init__.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/hooks/kernel.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/hooks/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,22 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+import typing
 
 from jupyter_client import AsyncKernelManager
 from papermill.clientwrap import PapermillNotebookClient
 from papermill.engines import NBClientEngine
 from papermill.utils import merge_kwargs, remove_args
 from traitlets import Unicode
 
-if TYPE_CHECKING:
-    from pydantic import typing
-
 from airflow.hooks.base import BaseHook
 
 JUPYTER_KERNEL_SHELL_PORT = 60316
 JUPYTER_KERNEL_IOPUB_PORT = 60317
 JUPYTER_KERNEL_STDIN_PORT = 60318
 JUPYTER_KERNEL_CONTROL_PORT = 60319
 JUPYTER_KERNEL_HB_PORT = 60320
@@ -86,15 +83,15 @@
         )
         kernel_connection.hb_port = self.kernel_conn.extra_dejson.get("hb_port", JUPYTER_KERNEL_HB_PORT)
         kernel_connection.session_key = self.kernel_conn.extra_dejson.get("session_key", "")
         return kernel_connection
 
 
 def register_remote_kernel_engine():
-    """Registers ``RemoteKernelEngine`` papermill engine."""
+    """Register ``RemoteKernelEngine`` papermill engine."""
     from papermill.engines import papermill_engines
 
     papermill_engines.register(REMOTE_KERNEL_ENGINE, RemoteKernelEngine)
 
 
 class RemoteKernelManager(AsyncKernelManager):
     """Jupyter kernel manager that connects to a remote kernel."""
@@ -141,15 +138,15 @@
         log_output=False,
         stdout_file=None,
         stderr_file=None,
         start_timeout=60,
         execution_timeout=None,
         **kwargs,
     ):
-        """Performs the actual execution of the parameterized notebook locally."""
+        """Perform the actual execution of the parameterized notebook locally."""
         km = RemoteKernelManager()
         km.ip = kwargs["kernel_ip"]
         km.shell_port = kwargs["kernel_shell_port"]
         km.iopub_port = kwargs["kernel_iopub_port"]
         km.stdin_port = kwargs["kernel_stdin_port"]
         km.control_port = kwargs["kernel_control_port"]
         km.hb_port = kwargs["kernel_hb_port"]
```

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/operators/__init__.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/airflow/providers/papermill/operators/papermill.py` & `apache_airflow_providers_papermill-3.6.2rc1/airflow/providers/papermill/operators/papermill.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/pyproject.toml` & `apache_airflow_providers_papermill-3.6.2rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-papermill"
-version = "3.6.1.rc2"
+version = "3.6.2.rc1"
 description = "Provider package apache-airflow-providers-papermill for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -51,23 +51,23 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow>=2.6.0rc0",
     "ipykernel",
     "papermill[all]>=2.4.0",
     "scrapbook[all]",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_papermill-3.6.1rc2/PKG-INFO` & `apache_airflow_providers_papermill-3.6.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-papermill
-Version: 3.6.1rc2
+Version: 3.6.2rc1
 Summary: Provider package apache-airflow-providers-papermill for Apache Airflow
 Keywords: airflow-provider,papermill,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,21 +16,21 @@
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: ipykernel
 Requires-Dist: papermill[all]>=2.4.0
 Requires-Dist: scrapbook[all]
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -72,28 +72,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.6.1.rc2``
+Release: ``3.6.2.rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``papermill`` provider. All classes for this provider package
 are in ``airflow.providers.papermill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-papermill``
@@ -109,8 +109,8 @@
 ``apache-airflow``  ``>=2.6.0``
 ``papermill[all]``  ``>=2.4.0``
 ``scrapbook[all]``
 ``ipykernel``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.6.2/changelog.html>`_.
```

