# Comparing `tmp/apache_airflow_providers_samba-4.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_samba-4.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_samba-4.6.0rc1.tar", last modified: Mon Jan 22 08:30:42 2024, max compression
+gzip compressed data, was "apache_airflow_providers_samba-4.6.0rc2.tar", last modified: Tue Apr  9 12:40:13 2024, max compression
```

## Comparing `apache_airflow_providers_samba-4.6.0rc1.tar` & `apache_airflow_providers_samba-4.6.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4010 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/LICENSE
--rw-r--r--   0        0        0     1580 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/__init__.py
--rw-r--r--   0        0        0     2671 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/hooks/__init__.py
--rw-r--r--   0        0        0     8766 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/hooks/samba.py
--rw-r--r--   0        0        0      785 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/transfers/__init__.py
--rw-r--r--   0        0        0     8488 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/transfers/gcs_to_samba.py
--rw-r--r--   0        0        0     3002 2024-01-22 08:30:42.000000 apache_airflow_providers_samba-4.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 apache_airflow_providers_samba-4.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4015 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/LICENSE
+-rw-r--r--   0        0        0     1580 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/__init__.py
+-rw-r--r--   0        0        0     2671 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/hooks/__init__.py
+-rw-r--r--   0        0        0     9141 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/hooks/samba.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/transfers/__init__.py
+-rw-r--r--   0        0        0     8958 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/transfers/gcs_to_samba.py
+-rw-r--r--   0        0        0     3046 2024-04-09 12:40:13.000000 apache_airflow_providers_samba-4.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5794 1970-01-01 00:00:00.000000 apache_airflow_providers_samba-4.6.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_samba-4.6.0rc1/README.rst` & `apache_airflow_providers_samba-4.6.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-samba``
 
-Release: ``4.6.0.rc1``
+Release: ``4.6.0.rc2``
 
 
 `Samba <https://www.samba.org/>`__
 
 
 Provider package
 ----------------
@@ -60,15 +60,15 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-samba``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
```

### Comparing `apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/LICENSE` & `apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/__init__.py` & `apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/get_provider_info.py` & `apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-samba",
         "name": "Samba",
         "description": "`Samba <https://www.samba.org/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912242,
+        "source-date-epoch": 1712666413,
         "versions": [
             "4.6.0",
             "4.5.0",
             "4.4.0",
             "4.3.0",
             "4.2.2",
             "4.2.1",
```

### Comparing `apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/hooks/__init__.py` & `apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/hooks/samba.py` & `apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/hooks/samba.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     """
 
     conn_name_attr = "samba_conn_id"
     default_conn_name = "samba_default"
     conn_type = "samba"
     hook_name = "Samba"
 
-    def __init__(self, samba_conn_id: str = default_conn_name, share: str | None = None, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, samba_conn_id: str = default_conn_name, share: str | None = None) -> None:
+        super().__init__()
         conn = self.get_connection(samba_conn_id)
 
         if not conn.login:
             self.log.info("Login not provided")
 
         if not conn.password:
             self.log.info("Password not provided")
@@ -241,19 +241,28 @@
             attribute,
             value,
             flags=flags,
             follow_symlinks=follow_symlinks,
             **self._conn_kwargs,
         )
 
-    def push_from_local(self, destination_filepath: str, local_filepath: str):
-        """Push local file to samba server."""
+    def push_from_local(self, destination_filepath: str, local_filepath: str, buffer_size: int | None = None):
+        """
+        Push local file to samba server.
+
+        :param destination_filepath: the samba location to push to
+        :param local_filepath: the file to push
+        :param buffer_size:
+            size in bytes of the individual chunks of file to send. Larger values may
+            speed up large file transfers
+        """
+        extra_args = (buffer_size,) if buffer_size else ()
         with open(local_filepath, "rb") as f, self.open_file(destination_filepath, mode="wb") as g:
-            copyfileobj(f, g)
+            copyfileobj(f, g, *extra_args)
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["extra"],
             "relabeling": {"schema": "Share"},
         }
```

### Comparing `apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/transfers/__init__.py` & `apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.6.0rc1/airflow/providers/samba/transfers/gcs_to_samba.py` & `apache_airflow_providers_samba-4.6.0rc2/airflow/providers/samba/transfers/gcs_to_samba.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Google Cloud Storage to Samba operator."""
+
 from __future__ import annotations
 
 import os
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.exceptions import AirflowException
@@ -88,14 +89,17 @@
         credentials, or chained list of accounts required to get the access_token
         of the last account in the list, which will be impersonated in the request.
         If set as a string, the account must grant the originating account
         the Service Account Token Creator IAM role.
         If set as a sequence, the identities from the list must grant
         Service Account Token Creator IAM role to the directly preceding identity, with first
         account from the list granting this role to the originating account (templated).
+    :param buffer_size: Optional specification of the size in bytes of the chunks sent to
+        Samba. Larger buffer lengths may decrease the time to upload large files. The default
+        length is determined by shutil, which is 64 KB.
     """
 
     template_fields: Sequence[str] = (
         "source_bucket",
         "source_object",
         "destination_path",
         "impersonation_chain",
@@ -109,27 +113,29 @@
         source_object: str,
         destination_path: str,
         keep_directory_structure: bool = True,
         move_object: bool = False,
         gcp_conn_id: str = "google_cloud_default",
         samba_conn_id: str = "samba_default",
         impersonation_chain: str | Sequence[str] | None = None,
+        buffer_size: int | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
 
         self.source_bucket = source_bucket
         self.source_object = source_object
         self.destination_path = destination_path
         self.keep_directory_structure = keep_directory_structure
         self.move_object = move_object
         self.gcp_conn_id = gcp_conn_id
         self.samba_conn_id = samba_conn_id
         self.impersonation_chain = impersonation_chain
         self.sftp_dirs = None
+        self.buffer_size = buffer_size
 
     def execute(self, context: Context):
         gcs_hook = GCSHook(
             gcp_conn_id=self.gcp_conn_id,
             impersonation_chain=self.impersonation_chain,
         )
 
@@ -149,20 +155,24 @@
             # TODO: After deprecating delimiter and wildcards in source objects,
             #       remove the previous line and uncomment the following:
             # match_glob = f"**/*{delimiter}" if delimiter else None
             # objects = gcs_hook.list(self.source_bucket, prefix=prefix, match_glob=match_glob)
 
             for source_object in objects:
                 destination_path = self._resolve_destination_path(source_object, prefix=prefix_dirname)
-                self._copy_single_object(gcs_hook, samba_hook, source_object, destination_path)
+                self._copy_single_object(
+                    gcs_hook, samba_hook, source_object, destination_path, self.buffer_size
+                )
 
             self.log.info("Done. Uploaded '%d' files to %s", len(objects), self.destination_path)
         else:
             destination_path = self._resolve_destination_path(self.source_object)
-            self._copy_single_object(gcs_hook, samba_hook, self.source_object, destination_path)
+            self._copy_single_object(
+                gcs_hook, samba_hook, self.source_object, destination_path, self.buffer_size
+            )
             self.log.info("Done. Uploaded '%s' file to %s", self.source_object, destination_path)
 
     def _resolve_destination_path(self, source_object: str, prefix: str | None = None) -> str:
         if not self.keep_directory_structure:
             if prefix:
                 source_object = os.path.relpath(source_object, start=prefix)
             else:
@@ -171,16 +181,17 @@
 
     def _copy_single_object(
         self,
         gcs_hook: GCSHook,
         samba_hook: SambaHook,
         source_object: str,
         destination_path: str,
+        buffer_size: int | None = None,
     ) -> None:
-        """Helper function to copy single object."""
+        """Copy single object."""
         self.log.info(
             "Executing copy of gs://%s/%s to %s",
             self.source_bucket,
             source_object,
             destination_path,
         )
 
@@ -189,12 +200,12 @@
 
         with NamedTemporaryFile("w") as tmp:
             gcs_hook.download(
                 bucket_name=self.source_bucket,
                 object_name=source_object,
                 filename=tmp.name,
             )
-            samba_hook.push_from_local(destination_path, tmp.name)
+            samba_hook.push_from_local(destination_path, tmp.name, buffer_size=buffer_size)
 
         if self.move_object:
             self.log.info("Executing delete of gs://%s/%s", self.source_bucket, source_object)
             gcs_hook.delete(self.source_bucket, source_object)
```

### Comparing `apache_airflow_providers_samba-4.6.0rc1/pyproject.toml` & `apache_airflow_providers_samba-4.6.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-samba"
-version = "4.6.0.rc1"
+version = "4.6.0.rc2"
 description = "Provider package apache-airflow-providers-samba for Apache Airflow"
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
     "smbprotocol>=1.5.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-samba/4.6.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-samba/4.6.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_samba-4.6.0rc1/PKG-INFO` & `apache_airflow_providers_samba-4.6.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-samba
-Version: 4.6.0rc1
+Version: 4.6.0rc2
 Summary: Provider package apache-airflow-providers-samba for Apache Airflow
 Keywords: airflow-provider,samba,airflow,integration
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
 Requires-Dist: smbprotocol>=1.5.0
 Requires-Dist: apache-airflow-providers-google ; extra == "google"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.6.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.6.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -72,15 +73,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-samba``
 
-Release: ``4.6.0.rc1``
+Release: ``4.6.0.rc2``
 
 
 `Samba <https://www.samba.org/>`__
 
 
 Provider package
 ----------------
@@ -94,15 +95,15 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-samba``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
```

