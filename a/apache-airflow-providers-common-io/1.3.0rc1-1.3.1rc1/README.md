# Comparing `tmp/apache_airflow_providers_common_io-1.3.0rc1.tar.gz` & `tmp/apache_airflow_providers_common_io-1.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_common_io-1.3.0rc1.tar", last modified: Sun Feb 11 07:25:26 2024, max compression
+gzip compressed data, was "apache_airflow_providers_common_io-1.3.1rc1.tar", last modified: Tue Apr  9 12:23:20 2024, max compression
```

## Comparing `apache_airflow_providers_common_io-1.3.0rc1.tar` & `apache_airflow_providers_common_io-1.3.1rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4069 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/LICENSE
--rw-r--r--   0        0        0     1584 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/__init__.py
--rw-r--r--   0        0        0     3790 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/operators/__init__.py
--rw-r--r--   0        0        0     3479 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/operators/file_transfer.py
--rw-r--r--   0        0        0     1263 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/xcom/__init__.py
--rw-r--r--   0        0        0     5907 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/xcom/backend.py
--rw-r--r--   0        0        0     3014 2024-02-11 07:25:26.000000 apache_airflow_providers_common_io-1.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 apache_airflow_providers_common_io-1.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4074 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/LICENSE
+-rw-r--r--   0        0        0     1584 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/__init__.py
+-rw-r--r--   0        0        0     3799 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/__init__.py
+-rw-r--r--   0        0        0     3479 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/file_transfer.py
+-rw-r--r--   0        0        0     1362 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/__init__.py
+-rw-r--r--   0        0        0     5979 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/backend.py
+-rw-r--r--   0        0        0     3058 2024-04-09 12:23:20.000000 apache_airflow_providers_common_io-1.3.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 apache_airflow_providers_common_io-1.3.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/README.rst` & `apache_airflow_providers_common_io-1.3.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-common-io``
 
-Release: ``1.3.0.rc1``
+Release: ``1.3.1.rc1``
 
 
 ``Common IO Provider``
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.io`` provider. All classes for this provider package
 are in ``airflow.providers.common.io`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-common-io``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -91,8 +91,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/LICENSE` & `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/__init__.py` & `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/get_provider_info.py` & `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-common-io",
         "name": "Common IO",
         "description": "``Common IO Provider``\n",
         "state": "ready",
-        "source-date-epoch": 1707636326,
-        "versions": ["1.3.0", "1.2.0", "1.1.0", "1.0.1", "1.0.0"],
+        "source-date-epoch": 1712665400,
+        "versions": ["1.3.1", "1.3.0", "1.2.0", "1.1.0", "1.0.1", "1.0.0"],
         "dependencies": ["apache-airflow>=2.8.0"],
         "integrations": [
             {
                 "integration-name": "Common IO",
                 "external-doc-url": "https://filesystem-spec.readthedocs.io/en/latest/index.html",
                 "how-to-guide": ["/docs/apache-airflow-providers-common-io/operators.rst"],
                 "tags": ["software"],
```

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/operators/__init__.py` & `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/operators/file_transfer.py` & `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/operators/file_transfer.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/xcom/__init__.py` & `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import packaging.version
 
+from airflow.exceptions import AirflowOptionalProviderFeatureException
+
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.9.0"
 ):
-    raise RuntimeError(
+    raise AirflowOptionalProviderFeatureException(
         "The package xcom backend feature of `apache-airflow-providers-common-io` needs "
         "Apache Airflow 2.9.0+"
     )
```

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/airflow/providers/common/io/xcom/backend.py` & `apache_airflow_providers_common_io-1.3.1rc1/airflow/providers/common/io/xcom/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import contextlib
 import json
 import uuid
 from typing import TYPE_CHECKING, Any, TypeVar
 from urllib.parse import urlsplit
 
 import fsspec.utils
 
+from airflow.compat.functools import cache
 from airflow.configuration import conf
 from airflow.io.path import ObjectStoragePath
 from airflow.models.xcom import BaseXCom
 from airflow.utils.json import XComDecoder, XComEncoder
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
@@ -35,68 +37,83 @@
 
 T = TypeVar("T")
 
 SECTION = "common.io"
 
 
 def _is_relative_to(o: ObjectStoragePath, other: ObjectStoragePath) -> bool:
-    """This is a port of the pathlib.Path.is_relative_to method. It is not available in python 3.8."""
+    """Return whether or not this path is relative to the other path.
+
+    This is a port of the pathlib.Path.is_relative_to method. It is not available in python 3.8.
+    """
     if hasattr(o, "is_relative_to"):
         return o.is_relative_to(other)
 
     try:
         o.relative_to(other)
         return True
     except ValueError:
         return False
 
 
 def _get_compression_suffix(compression: str) -> str:
-    """This returns the compression suffix for the given compression.
+    """Return the compression suffix for the given compression.
 
     :raises ValueError: if the compression is not supported
     """
     for suffix, c in fsspec.utils.compressions.items():
         if c == compression:
             return suffix
 
     raise ValueError(f"Compression {compression} is not supported. Make sure it is installed.")
 
 
-class XComObjectStoreBackend(BaseXCom):
+@cache
+def _get_base_path() -> ObjectStoragePath:
+    return ObjectStoragePath(conf.get_mandatory_value(SECTION, "xcom_objectstorage_path"))
+
+
+@cache
+def _get_compression() -> str | None:
+    return conf.get(SECTION, "xcom_objectstorage_compression", fallback=None) or None
+
+
+@cache
+def _get_threshold() -> int:
+    return conf.getint(SECTION, "xcom_objectstorage_threshold", fallback=-1)
+
+
+class XComObjectStorageBackend(BaseXCom):
     """XCom backend that stores data in an object store or database depending on the size of the data.
 
     If the value is larger than the configured threshold, it will be stored in an object store.
     Otherwise, it will be stored in the database. If it is stored in an object store, the path
     to the object in the store will be returned and saved in the database (by BaseXCom). Otherwise, the value
     itself will be returned and thus saved in the database.
     """
 
     @staticmethod
-    def _get_key(data: str) -> str:
-        """This gets the key from the url and normalizes it to be relative to the configured path.
+    def _get_full_path(data: str) -> ObjectStoragePath:
+        """Get the path from stored value.
 
         :raises ValueError: if the key is not relative to the configured path
         :raises TypeError: if the url is not a valid url or cannot be split
         """
-        path = conf.get(SECTION, "xcom_objectstore_path", fallback="")
-        p = ObjectStoragePath(path)
+        p = _get_base_path()
 
+        # normalize the path
         try:
             url = urlsplit(data)
         except AttributeError:
-            raise TypeError(f"Not a valid url: {data}")
+            raise TypeError(f"Not a valid url: {data}") from None
 
         if url.scheme:
-            k = ObjectStoragePath(data)
-
-            if _is_relative_to(k, p) is False:
+            if not _is_relative_to(ObjectStoragePath(data), p):
                 raise ValueError(f"Invalid key: {data}")
-            else:
-                return data.replace(path, "", 1).lstrip("/")
+            return p / data.replace(str(p), "", 1).lstrip("/")
 
         raise ValueError(f"Not a valid url: {data}")
 
     @staticmethod
     def serialize_value(
         value: T,
         *,
@@ -105,64 +122,51 @@
         dag_id: str | None = None,
         run_id: str | None = None,
         map_index: int | None = None,
     ) -> bytes | str:
         # we will always serialize ourselves and not by BaseXCom as the deserialize method
         # from BaseXCom accepts only XCom objects and not the value directly
         s_val = json.dumps(value, cls=XComEncoder).encode("utf-8")
-        path = conf.get(SECTION, "xcom_objectstore_path", fallback="")
-        compression = conf.get(SECTION, "xcom_objectstore_compression", fallback=None)
 
-        if compression:
-            suffix = "." + _get_compression_suffix(compression)
+        if compression := _get_compression():
+            suffix = f".{_get_compression_suffix(compression)}"
         else:
             suffix = ""
 
-        threshold = conf.getint(SECTION, "xcom_objectstore_threshold", fallback=-1)
-
-        if path and -1 < threshold < len(s_val):
-            # safeguard against collisions
-            while True:
-                p = ObjectStoragePath(path) / f"{dag_id}/{run_id}/{task_id}/{str(uuid.uuid4())}{suffix}"
-                if not p.exists():
-                    break
-
-            if not p.parent.exists():
-                p.parent.mkdir(parents=True, exist_ok=True)
-
-            with p.open("wb", compression=compression) as f:
-                f.write(s_val)
-
-            return BaseXCom.serialize_value(str(p))
-        else:
+        threshold = _get_threshold()
+        if threshold < 0 or len(s_val) < threshold:  # Either no threshold or value is small enough.
             return s_val
 
+        base_path = _get_base_path()
+        while True:  # Safeguard against collisions.
+            p = base_path.joinpath(dag_id, run_id, task_id, f"{uuid.uuid4()}{suffix}")
+            if not p.exists():
+                break
+        p.parent.mkdir(parents=True, exist_ok=True)
+
+        with p.open(mode="wb", compression=compression) as f:
+            f.write(s_val)
+        return BaseXCom.serialize_value(str(p))
+
     @staticmethod
-    def deserialize_value(
-        result: XCom,
-    ) -> Any:
+    def deserialize_value(result: XCom) -> Any:
         """Deserializes the value from the database or object storage.
 
         Compression is inferred from the file extension.
         """
         data = BaseXCom.deserialize_value(result)
-        path = conf.get(SECTION, "xcom_objectstore_path", fallback="")
-
         try:
-            p = ObjectStoragePath(path) / XComObjectStoreBackend._get_key(data)
-            return json.load(p.open("rb", compression="infer"), cls=XComDecoder)
-        except TypeError:
+            path = XComObjectStorageBackend._get_full_path(data)
+        except (TypeError, ValueError):  # Likely value stored directly in the database.
             return data
-        except ValueError:
+        try:
+            with path.open(mode="rb", compression="infer") as f:
+                return json.load(f, cls=XComDecoder)
+        except (TypeError, ValueError):
             return data
 
     @staticmethod
     def purge(xcom: XCom, session: Session) -> None:
-        path = conf.get(SECTION, "xcom_objectstore_path", fallback="")
-        if isinstance(xcom.value, str):
-            try:
-                p = ObjectStoragePath(path) / XComObjectStoreBackend._get_key(xcom.value)
-                p.unlink(missing_ok=True)
-            except TypeError:
-                pass
-            except ValueError:
-                pass
+        if not isinstance(xcom.value, str):
+            return
+        with contextlib.suppress(TypeError, ValueError):
+            XComObjectStorageBackend._get_full_path(xcom.value).unlink(missing_ok=True)
```

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/pyproject.toml` & `apache_airflow_providers_common_io-1.3.1rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-common-io"
-version = "1.3.0.rc1"
+version = "1.3.1.rc1"
 description = "Provider package apache-airflow-providers-common-io for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,24 +47,25 @@
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
-    "apache-airflow>=2.8.0.dev0",
+    "apache-airflow>=2.8.0rc0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_common_io-1.3.0rc1/PKG-INFO` & `apache_airflow_providers_common_io-1.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-io
-Version: 1.3.0rc1
+Version: 1.3.1rc1
 Summary: Provider package apache-airflow-providers-common-io for Apache Airflow
 Keywords: airflow-provider,common.io,airflow,integration
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
-Requires-Dist: apache-airflow>=2.8.0.dev0
+Requires-Dist: apache-airflow>=2.8.0rc0
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: openlineage
 
 
@@ -71,37 +72,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-common-io``
 
-Release: ``1.3.0.rc1``
+Release: ``1.3.1.rc1``
 
 
 ``Common IO Provider``
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.io`` provider. All classes for this provider package
 are in ``airflow.providers.common.io`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-common-io``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -124,8 +125,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-io/1.3.1/changelog.html>`_.
```

