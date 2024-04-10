# Comparing `tmp/apache_airflow_providers_microsoft_psrp-2.6.0rc2.tar.gz` & `tmp/apache_airflow_providers_microsoft_psrp-2.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_microsoft_psrp-2.6.0rc2.tar", last modified: Mon Mar  4 12:38:13 2024, max compression
+gzip compressed data, was "apache_airflow_providers_microsoft_psrp-2.6.1rc1.tar", last modified: Tue Apr  9 12:36:19 2024, max compression
```

## Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2.tar` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3225 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/LICENSE
--rw-r--r--   0        0        0     1589 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/__init__.py
--rw-r--r--   0        0        0     2852 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/hooks/__init__.py
--rw-r--r--   0        0        0    11108 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/hooks/psrp.py
--rw-r--r--   0        0        0      787 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/operators/__init__.py
--rw-r--r--   0        0        0     7180 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/operators/psrp.py
--rw-r--r--   0        0        0     2974 2024-03-04 12:38:13.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4905 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_psrp-2.6.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     3230 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/LICENSE
+-rw-r--r--   0        0        0     1589 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/__init__.py
+-rw-r--r--   0        0        0     2873 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/__init__.py
+-rw-r--r--   0        0        0    11157 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/psrp.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/__init__.py
+-rw-r--r--   0        0        0     7180 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/psrp.py
+-rw-r--r--   0        0        0     3018 2024-04-09 12:36:19.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4959 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_psrp-2.6.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/README.rst` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,45 +38,45 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.6.0.rc2``
+Release: ``2.6.1.rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/openspecs/windows_protocols/ms-psrp/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.psrp`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.psrp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-psrp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.6.0``
 ``pypsrp``          ``>=0.8.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/LICENSE` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/__init__.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/get_provider_info.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-psrp",
         "name": "PowerShell Remoting Protocol (PSRP)",
         "description": "This package provides remote execution capabilities via the\n`PowerShell Remoting Protocol (PSRP)\n<https://docs.microsoft.com/openspecs/windows_protocols/ms-psrp/>`__.\n",
         "state": "ready",
-        "source-date-epoch": 1709555893,
+        "source-date-epoch": 1712666179,
         "versions": [
+            "2.6.1",
             "2.6.0",
             "2.5.0",
             "2.4.0",
             "2.3.2",
             "2.3.1",
             "2.3.0",
             "2.2.0",
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/hooks/__init__.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/hooks/psrp.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/hooks/psrp.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from contextlib import contextmanager
 from copy import copy
 from logging import DEBUG, ERROR, INFO, WARNING
-from typing import Any, Callable, Generator
+from typing import TYPE_CHECKING, Any, Callable, Generator
 from warnings import warn
 from weakref import WeakKeyDictionary
 
 from pypsrp.host import PSHost
 from pypsrp.messages import MessageType
 from pypsrp.powershell import PowerShell, PSInvocationState, RunspacePool
 from pypsrp.wsman import WSMan
@@ -169,15 +169,16 @@
         """
         logger = copy(self.log)
         logger.setLevel(self._logging_level)
         local_context = self._conn is None
         if local_context:
             self.__enter__()
         try:
-            assert self._conn is not None
+            if TYPE_CHECKING:
+                assert self._conn is not None
             ps = PowerShell(self._conn)
             yield ps
             ps.begin_invoke()
 
             streams = [
                 ps.output,
                 ps.streams.debug,
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/operators/__init__.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/airflow/providers/microsoft/psrp/operators/psrp.py` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/airflow/providers/microsoft/psrp/operators/psrp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/pyproject.toml` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-microsoft-psrp"
-version = "2.6.0.rc2"
+version = "2.6.1.rc1"
 description = "Provider package apache-airflow-providers-microsoft-psrp for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,25 +47,26 @@
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
     "pypsrp>=0.8.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_microsoft_psrp-2.6.0rc2/PKG-INFO` & `apache_airflow_providers_microsoft_psrp-2.6.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.6.0rc2
+Version: 2.6.1rc1
 Summary: Provider package apache-airflow-providers-microsoft-psrp for Apache Airflow
 Keywords: airflow-provider,microsoft.psrp,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,20 +15,21 @@
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
 Requires-Dist: pypsrp>=0.8.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -70,45 +71,45 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.6.0.rc2``
+Release: ``2.6.1.rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/openspecs/windows_protocols/ms-psrp/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.psrp`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.psrp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-psrp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.6.0``
 ``pypsrp``          ``>=0.8.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.6.1/changelog.html>`_.
```

