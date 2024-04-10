# Comparing `tmp/apache_airflow_providers_sftp-4.9.0rc1.tar.gz` & `tmp/apache_airflow_providers_sftp-4.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_sftp-4.9.0rc1.tar", last modified: Sun Feb 11 07:28:31 2024, max compression
+gzip compressed data, was "apache_airflow_providers_sftp-4.9.1rc1.tar", last modified: Tue Apr  9 12:40:52 2024, max compression
```

## Comparing `apache_airflow_providers_sftp-4.9.0rc1.tar` & `apache_airflow_providers_sftp-4.9.1rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4439 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/LICENSE
--rw-r--r--   0        0        0     1579 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/__init__.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/decorators/__init__.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py
--rw-r--r--   0        0        0     2861 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py
--rw-r--r--   0        0        0     3912 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/hooks/__init__.py
--rw-r--r--   0        0        0    21763 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/hooks/sftp.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/operators/__init__.py
--rw-r--r--   0        0        0    11454 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/operators/sftp.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/sensors/__init__.py
--rw-r--r--   0        0        0     7381 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/sensors/sftp.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/triggers/__init__.py
--rw-r--r--   0        0        0     6053 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/triggers/sftp.py
--rw-r--r--   0        0        0     3122 2024-02-11 07:28:31.000000 apache_airflow_providers_sftp-4.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6345 1970-01-01 00:00:00.000000 apache_airflow_providers_sftp-4.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4444 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/LICENSE
+-rw-r--r--   0        0        0     1579 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/__init__.py
+-rw-r--r--   0        0        0     2861 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/sftp.py
+-rw-r--r--   0        0        0     3933 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/__init__.py
+-rw-r--r--   0        0        0    21856 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/sftp.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/__init__.py
+-rw-r--r--   0        0        0    11508 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/sftp.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/__init__.py
+-rw-r--r--   0        0        0     7382 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/sftp.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/__init__.py
+-rw-r--r--   0        0        0     6155 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/sftp.py
+-rw-r--r--   0        0        0     3164 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6397 1970-01-01 00:00:00.000000 apache_airflow_providers_sftp-4.9.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/README.rst` & `apache_airflow_providers_sftp-4.9.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.9.0.rc1``
+Release: ``4.9.1.rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sftp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -95,8 +95,8 @@
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                  ``ssh``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/LICENSE` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.9.0"
+__version__ = "4.9.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/decorators/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/get_provider_info.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-sftp",
         "name": "SFTP",
         "description": "`SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1707636511,
+        "source-date-epoch": 1712666452,
         "versions": [
+            "4.9.1",
             "4.9.0",
             "4.8.1",
             "4.8.0",
             "4.7.0",
             "4.6.1",
             "4.6.0",
             "4.5.0",
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/hooks/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/hooks/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/sftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains SFTP hook."""
+
 from __future__ import annotations
 
 import datetime
 import os
 import stat
 import warnings
 from fnmatch import fnmatch
@@ -511,33 +512,32 @@
             _private_key = asyncssh.import_private_key(self.private_key, self.passphrase)
             conn_config.update(client_keys=[_private_key])
         if self.passphrase:
             conn_config.update(passphrase=self.passphrase)
         ssh_client_conn = await asyncssh.connect(**conn_config)
         return ssh_client_conn
 
-    async def list_directory(self, path: str = "") -> list[str] | None:
+    async def list_directory(self, path: str = "") -> list[str] | None:  # type: ignore[return]
         """Return a list of files on the SFTP server at the provided path."""
-        ssh_conn = await self._get_conn()
-        sftp_client = await ssh_conn.start_sftp_client()
-        try:
-            files = await sftp_client.listdir(path)
-            return sorted(files)
-        except asyncssh.SFTPNoSuchFile:
-            return None
+        async with await self._get_conn() as ssh_conn:
+            sftp_client = await ssh_conn.start_sftp_client()
+            try:
+                files = await sftp_client.listdir(path)
+                return sorted(files)
+            except asyncssh.SFTPNoSuchFile:
+                return None
 
-    async def read_directory(self, path: str = "") -> Sequence[asyncssh.sftp.SFTPName] | None:
+    async def read_directory(self, path: str = "") -> Sequence[asyncssh.sftp.SFTPName] | None:  # type: ignore[return]
         """Return a list of files along with their attributes on the SFTP server at the provided path."""
-        ssh_conn = await self._get_conn()
-        sftp_client = await ssh_conn.start_sftp_client()
-        try:
-            files = await sftp_client.readdir(path)
-            return files
-        except asyncssh.SFTPNoSuchFile:
-            return None
+        async with await self._get_conn() as ssh_conn:
+            sftp_client = await ssh_conn.start_sftp_client()
+            try:
+                return await sftp_client.readdir(path)
+            except asyncssh.SFTPNoSuchFile:
+                return None
 
     async def get_files_and_attrs_by_pattern(
         self, path: str = "", fnmatch_pattern: str = ""
     ) -> Sequence[asyncssh.sftp.SFTPName]:
         """
         Get the files along with their attributes matching the pattern (e.g. ``*.pdf``) at the provided path.
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/operators/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/operators/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/sftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains SFTP operator."""
+
 from __future__ import annotations
 
 import os
 import socket
 import warnings
 from pathlib import Path
 from typing import Any, Sequence
@@ -206,30 +207,33 @@
 
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
 
         hook = self.sftp_hook or self.ssh_hook or SFTPHook(ssh_conn_id=self.ssh_conn_id)
 
         if self.remote_host is not None:
             remote_host = self.remote_host
         else:
             remote_host = hook.get_connection(hook.ssh_conn_id).host
 
         try:
             remote_host = socket.gethostbyname(remote_host)
         except OSError as e:
             self.log.warning(
-                f"Failed to resolve remote hostname. Using the provided hostname without resolution. {e}",
+                "Failed to resolve remote hostname. Using the provided hostname without resolution. %s",
+                e,
                 exc_info=True,
             )
 
         if hasattr(hook, "port"):
             remote_port = hook.port
         elif hasattr(hook, "ssh_hook"):
             remote_port = hook.ssh_hook.port
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/sensors/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/sensors/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains SFTP sensor."""
+
 from __future__ import annotations
 
 import os
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from paramiko.sftp import SFTP_NO_SUCH_FILE
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/triggers/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/airflow/providers/sftp/triggers/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,29 +109,32 @@
                     if files_sensed:
                         yield TriggerEvent(
                             {
                                 "status": "success",
                                 "message": f"Sensed {len(files_sensed)} files: {files_sensed}",
                             }
                         )
+                        return
                 else:
                     mod_time = await hook.get_mod_time(self.path)
                     if _newer_than:
                         mod_time_utc = convert_to_utc(datetime.strptime(mod_time, "%Y%m%d%H%M%S"))
                         if _newer_than <= mod_time_utc:
                             yield TriggerEvent({"status": "success", "message": f"Sensed file: {self.path}"})
+                            return
                     else:
                         yield TriggerEvent({"status": "success", "message": f"Sensed file: {self.path}"})
+                        return
                 await asyncio.sleep(self.poke_interval)
             except AirflowException:
                 await asyncio.sleep(self.poke_interval)
             except FileNotFoundError:
                 await asyncio.sleep(self.poke_interval)
             except Exception as e:
                 exc = e
                 # Break loop to avoid infinite retries on terminal failure
                 break
 
-        yield TriggerEvent({"status": "error", "message": exc})
+        yield TriggerEvent({"status": "error", "message": str(exc)})
 
     def _get_async_hook(self) -> SFTPHookAsync:
         return SFTPHookAsync(sftp_conn_id=self.sftp_conn_id)
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/pyproject.toml` & `apache_airflow_providers_sftp-4.9.1rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-sftp"
-version = "4.9.0.rc1"
+version = "4.9.1.rc1"
 description = "Provider package apache-airflow-providers-sftp for Apache Airflow"
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
-    "apache-airflow-providers-ssh>=2.1.0.dev0",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow-providers-ssh>=2.1.0rc0",
+    "apache-airflow>=2.6.0rc0",
     "asyncssh>=2.12.0",
     "paramiko>=2.8.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_sftp-4.9.0rc1/PKG-INFO` & `apache_airflow_providers_sftp-4.9.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.9.0rc1
+Version: 4.9.1rc1
 Summary: Provider package apache-airflow-providers-sftp for Apache Airflow
 Keywords: airflow-provider,sftp,airflow,integration
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
-Requires-Dist: apache-airflow-providers-ssh>=2.1.0.dev0
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow-providers-ssh>=2.1.0rc0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: asyncssh>=2.12.0
 Requires-Dist: paramiko>=2.8.0
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Requires-Dist: apache-airflow-providers-ssh ; extra == "ssh"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: openlineage
 Provides-Extra: ssh
 
@@ -76,37 +77,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.9.0.rc1``
+Release: ``4.9.1.rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sftp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -133,8 +134,8 @@
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                  ``ssh``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/changelog.html>`_.
```

