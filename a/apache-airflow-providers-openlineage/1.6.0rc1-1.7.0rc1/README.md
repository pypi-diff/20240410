# Comparing `tmp/apache_airflow_providers_openlineage-1.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_openlineage-1.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_openlineage-1.6.0rc1.tar", last modified: Mon Mar  4 12:39:20 2024, max compression
+gzip compressed data, was "apache_airflow_providers_openlineage-1.7.0rc1.tar", last modified: Tue Apr  9 12:37:27 2024, max compression
```

## Comparing `apache_airflow_providers_openlineage-1.6.0rc1.tar` & `apache_airflow_providers_openlineage-1.7.0rc1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     4405 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/LICENSE
--rw-r--r--   0        0        0     1586 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/__init__.py
--rw-r--r--   0        0        0     1081 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/__init__.py
--rw-r--r--   0        0        0     6281 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/base.py
--rw-r--r--   0        0        0     2843 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/bash.py
--rw-r--r--   0        0        0    10861 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/manager.py
--rw-r--r--   0        0        0     3423 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/python.py
--rw-r--r--   0        0        0     6127 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/__init__.py
--rw-r--r--   0        0        0    14937 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/adapter.py
--rw-r--r--   0        0        0     2202 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/facets.py
--rw-r--r--   0        0        0    10057 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/listener.py
--rw-r--r--   0        0        0     2532 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/macros.py
--rw-r--r--   0        0        0     1987 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/openlineage.py
--rw-r--r--   0        0        0    13806 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/sqlparser.py
--rw-r--r--   0        0        0      785 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/utils/__init__.py
--rw-r--r--   0        0        0     9366 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/utils/sql.py
--rw-r--r--   0        0        0    14281 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/utils/utils.py
--rw-r--r--   0        0        0     3313 2024-03-04 12:39:20.000000 apache_airflow_providers_openlineage-1.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6329 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4410 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/LICENSE
+-rw-r--r--   0        0        0     1586 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/__init__.py
+-rw-r--r--   0        0        0     3398 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/conf.py
+-rw-r--r--   0        0        0     1081 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/__init__.py
+-rw-r--r--   0        0        0     5070 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/base.py
+-rw-r--r--   0        0        0     2412 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/bash.py
+-rw-r--r--   0        0        0     9996 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/manager.py
+-rw-r--r--   0        0        0     2999 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/python.py
+-rw-r--r--   0        0        0     6605 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/__init__.py
+-rw-r--r--   0        0        0    14634 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/adapter.py
+-rw-r--r--   0        0        0     2644 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/facets.py
+-rw-r--r--   0        0        0    11624 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/listener.py
+-rw-r--r--   0        0        0     3076 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/macros.py
+-rw-r--r--   0        0        0     1625 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/openlineage.py
+-rw-r--r--   0        0        0    13806 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/sqlparser.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/selective_enable.py
+-rw-r--r--   0        0        0     9366 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/sql.py
+-rw-r--r--   0        0        0    13115 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/utils.py
+-rw-r--r--   0        0        0     3355 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6381 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.7.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/README.rst` & `apache_airflow_providers_openlineage-1.7.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.6.0.rc1``
+Release: ``1.7.0.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openlineage``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -95,8 +95,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/LICENSE` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.6.0"
+__version__ = "1.7.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/bash.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/bash.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,23 +15,17 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from __future__ import annotations
 
 from openlineage.client.facet import SourceCodeJobFacet
 
+from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.extractors.base import BaseExtractor, OperatorLineage
-from airflow.providers.openlineage.plugins.facets import (
-    UnknownOperatorAttributeRunFacet,
-    UnknownOperatorInstance,
-)
-from airflow.providers.openlineage.utils.utils import (
-    get_filtered_unknown_operator_keys,
-    is_source_enabled,
-)
+from airflow.providers.openlineage.utils.utils import get_unknown_source_attribute_run_facet
 
 """
 :meta private:
 """
 
 
 class BashExtractor(BaseExtractor):
@@ -47,35 +41,25 @@
 
     @classmethod
     def get_operator_classnames(cls) -> list[str]:
         return ["BashOperator"]
 
     def _execute_extraction(self) -> OperatorLineage | None:
         job_facets: dict = {}
-        if is_source_enabled():
+        if conf.is_source_enabled():
             job_facets = {
                 "sourceCode": SourceCodeJobFacet(
                     language="bash",
                     # We're on worker and should have access to DAG files
                     source=self.operator.bash_command,
                 )
             }
 
         return OperatorLineage(
             job_facets=job_facets,
-            run_facets={
-                # The BashOperator is recorded as an "unknownSource" even though we have an
-                # extractor, as the <i>data lineage</i> cannot be determined from the operator
-                # directly.
-                "unknownSourceAttribute": UnknownOperatorAttributeRunFacet(
-                    unknownItems=[
-                        UnknownOperatorInstance(
-                            name="BashOperator",
-                            properties=get_filtered_unknown_operator_keys(self.operator),
-                        )
-                    ]
-                )
-            },
+            # The BashOperator is recorded as an "unknownSource" even though we have an extractor,
+            # as the <i>data lineage</i> cannot be determined from the operator directly.
+            run_facets=get_unknown_source_attribute_run_facet(task=self.operator, name="BashOperator"),
         )
 
     def extract(self) -> OperatorLineage | None:
         return super().extract()
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/manager.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,23 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import os
 from contextlib import suppress
 from typing import TYPE_CHECKING, Iterator
 
-from airflow.configuration import conf
+from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.extractors import BaseExtractor, OperatorLineage
 from airflow.providers.openlineage.extractors.base import DefaultExtractor
 from airflow.providers.openlineage.extractors.bash import BashExtractor
 from airflow.providers.openlineage.extractors.python import PythonExtractor
-from airflow.providers.openlineage.plugins.facets import (
-    UnknownOperatorAttributeRunFacet,
-    UnknownOperatorInstance,
-)
-from airflow.providers.openlineage.utils.utils import get_filtered_unknown_operator_keys
+from airflow.providers.openlineage.utils.utils import get_unknown_source_attribute_run_facet
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.utils.module_loading import import_string
 
 if TYPE_CHECKING:
     from openlineage.client.run import Dataset
 
     from airflow.lineage.entities import Table
@@ -61,30 +56,25 @@
         self.default_extractor = DefaultExtractor
 
         # Built-in Extractors like Bash and Python
         for extractor in _iter_extractor_types():
             for operator_class in extractor.get_operator_classnames():
                 self.extractors[operator_class] = extractor
 
-        # Semicolon-separated extractors in Airflow configuration or OPENLINEAGE_EXTRACTORS variable.
-        # Extractors should implement BaseExtractor
-        env_extractors = conf.get("openlineage", "extractors", fallback=os.getenv("OPENLINEAGE_EXTRACTORS"))
-        # skip either when it's empty string or None
-        if env_extractors:
-            for extractor in env_extractors.split(";"):
-                extractor: type[BaseExtractor] = try_import_from_string(extractor.strip())
-                for operator_class in extractor.get_operator_classnames():
-                    if operator_class in self.extractors:
-                        self.log.debug(
-                            "Duplicate extractor found for `%s`. `%s` will be used instead of `%s`",
-                            operator_class,
-                            extractor,
-                            self.extractors[operator_class],
-                        )
-                    self.extractors[operator_class] = extractor
+        for extractor_path in conf.custom_extractors():
+            extractor: type[BaseExtractor] = try_import_from_string(extractor_path)
+            for operator_class in extractor.get_operator_classnames():
+                if operator_class in self.extractors:
+                    self.log.debug(
+                        "Duplicate extractor found for `%s`. `%s` will be used instead of `%s`",
+                        operator_class,
+                        extractor_path,
+                        self.extractors[operator_class],
+                    )
+                self.extractors[operator_class] = extractor
 
     def add_extractor(self, operator_class: str, extractor: type[BaseExtractor]):
         self.extractors[operator_class] = extractor
 
     def extract_metadata(self, dagrun, task, complete: bool = False, task_instance=None) -> OperatorLineage:
         extractor = self._get_extractor(task)
         task_info = (
@@ -117,24 +107,15 @@
                     "Failed to extract metadata using found extractor %s - %s %s", extractor, e, task_info
                 )
         else:
             self.log.debug("Unable to find an extractor %s", task_info)
 
             # Only include the unkonwnSourceAttribute facet if there is no extractor
             task_metadata = OperatorLineage(
-                run_facets={
-                    "unknownSourceAttribute": UnknownOperatorAttributeRunFacet(
-                        unknownItems=[
-                            UnknownOperatorInstance(
-                                name=task.task_type,
-                                properties=get_filtered_unknown_operator_keys(task),
-                            )
-                        ]
-                    )
-                },
+                run_facets=get_unknown_source_attribute_run_facet(task=task),
             )
             inlets = task.get_inlet_defs()
             outlets = task.get_outlet_defs()
             self.extract_inlets_and_outlets(task_metadata, inlets, outlets)
             return task_metadata
 
         return OperatorLineage()
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/extractors/python.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/python.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,23 +18,17 @@
 from __future__ import annotations
 
 import inspect
 from typing import Callable
 
 from openlineage.client.facet import SourceCodeJobFacet
 
+from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.extractors.base import BaseExtractor, OperatorLineage
-from airflow.providers.openlineage.plugins.facets import (
-    UnknownOperatorAttributeRunFacet,
-    UnknownOperatorInstance,
-)
-from airflow.providers.openlineage.utils.utils import (
-    get_filtered_unknown_operator_keys,
-    is_source_enabled,
-)
+from airflow.providers.openlineage.utils.utils import get_unknown_source_attribute_run_facet
 
 """
 :meta private:
 """
 
 
 class PythonExtractor(BaseExtractor):
@@ -51,37 +45,27 @@
     @classmethod
     def get_operator_classnames(cls) -> list[str]:
         return ["PythonOperator"]
 
     def _execute_extraction(self) -> OperatorLineage | None:
         source_code = self.get_source_code(self.operator.python_callable)
         job_facet: dict = {}
-        if is_source_enabled() and source_code:
+        if conf.is_source_enabled() and source_code:
             job_facet = {
                 "sourceCode": SourceCodeJobFacet(
                     language="python",
                     # We're on worker and should have access to DAG files
                     source=source_code,
                 )
             }
         return OperatorLineage(
             job_facets=job_facet,
-            run_facets={
-                # The PythonOperator is recorded as an "unknownSource" even though we have an
-                # extractor, as the data lineage cannot be determined from the operator
-                # directly.
-                "unknownSourceAttribute": UnknownOperatorAttributeRunFacet(
-                    unknownItems=[
-                        UnknownOperatorInstance(
-                            name="PythonOperator",
-                            properties=get_filtered_unknown_operator_keys(self.operator),
-                        )
-                    ]
-                )
-            },
+            # The PythonOperator is recorded as an "unknownSource" even though we have an extractor,
+            # as the <i>data lineage</i> cannot be determined from the operator directly.
+            run_facets=get_unknown_source_attribute_run_facet(task=self.operator, name="PythonOperator"),
         )
 
     def get_source_code(self, callable: Callable) -> str | None:
         try:
             return inspect.getsource(callable)
         except TypeError:
             # Trying to extract source code of builtin_function_or_method
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/get_provider_info.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-openlineage",
         "name": "OpenLineage Airflow",
         "description": "`OpenLineage <https://openlineage.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1709555960,
+        "source-date-epoch": 1712666247,
         "versions": [
+            "1.7.0",
             "1.6.0",
             "1.5.0",
             "1.4.0",
             "1.3.1",
             "1.3.0",
             "1.2.1",
             "1.2.0",
@@ -78,14 +79,21 @@
                     "disabled_for_operators": {
                         "description": "Exclude some Operators from emitting OpenLineage events by passing a string of semicolon separated\nfull import paths of Operators to disable.\n",
                         "type": "string",
                         "example": "airflow.operators.bash.BashOperator;airflow.operators.python.PythonOperator",
                         "default": "",
                         "version_added": "1.1.0",
                     },
+                    "selective_enable": {
+                        "description": "If this setting is enabled, OpenLineage integration won't collect and emit metadata,\nunless you explicitly enable it per `DAG` or `Task` using  `enable_lineage` method.\n",
+                        "type": "boolean",
+                        "default": "False",
+                        "example": None,
+                        "version_added": "1.7.0",
+                    },
                     "namespace": {
                         "description": "Set namespace that the lineage data belongs to, so that if you use multiple OpenLineage producers,\nevents coming from them will be logically separated.\n",
                         "version_added": None,
                         "type": "string",
                         "example": "my_airflow_instance_1",
                         "default": None,
                     },
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/adapter.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import os
 import uuid
 from contextlib import ExitStack
 from typing import TYPE_CHECKING
 
 import yaml
 from openlineage.client import OpenLineageClient, set_producer
 from openlineage.client.facet import (
@@ -33,31 +32,24 @@
     OwnershipJobFacetOwners,
     ParentRunFacet,
     ProcessingEngineRunFacet,
     SourceCodeLocationJobFacet,
 )
 from openlineage.client.run import Job, Run, RunEvent, RunState
 
-from airflow.configuration import conf
-from airflow.providers.openlineage import __version__ as OPENLINEAGE_PROVIDER_VERSION
+from airflow.providers.openlineage import __version__ as OPENLINEAGE_PROVIDER_VERSION, conf
 from airflow.providers.openlineage.utils.utils import OpenLineageRedactor
 from airflow.stats import Stats
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 if TYPE_CHECKING:
     from airflow.models.dagrun import DagRun
     from airflow.providers.openlineage.extractors import OperatorLineage
     from airflow.utils.log.secrets_masker import SecretsMasker
 
-_DAG_DEFAULT_NAMESPACE = "default"
-
-_DAG_NAMESPACE = conf.get(
-    "openlineage", "namespace", fallback=os.getenv("OPENLINEAGE_NAMESPACE", _DAG_DEFAULT_NAMESPACE)
-)
-
 _PRODUCER = f"https://github.com/apache/airflow/tree/providers-openlineage/{OPENLINEAGE_PROVIDER_VERSION}"
 
 set_producer(_PRODUCER)
 
 # https://openlineage.io/docs/spec/facets/job-facets/job-type
 # They must be set after the `set_producer(_PRODUCER)`
 # otherwise the `JobTypeJobFacet._producer` will be set with the default value
@@ -84,41 +76,39 @@
                 self._client = OpenLineageClient.from_dict(config=config)
             else:
                 self._client = OpenLineageClient.from_environment()
         return self._client
 
     def get_openlineage_config(self) -> dict | None:
         # First, try to read from YAML file
-        openlineage_config_path = conf.get("openlineage", "config_path")
+        openlineage_config_path = conf.config_path(check_legacy_env_var=False)
         if openlineage_config_path:
             config = self._read_yaml_config(openlineage_config_path)
             if config:
                 return config.get("transport", None)
         # Second, try to get transport config
-        transport = conf.getjson("openlineage", "transport")
-        if not transport:
+        transport_config = conf.transport()
+        if not transport_config:
             return None
-        elif not isinstance(transport, dict):
-            raise ValueError(f"{transport} is not a dict")
-        return transport
+        return transport_config
 
     def _read_yaml_config(self, path: str) -> dict | None:
         with open(path) as config_file:
             return yaml.safe_load(config_file)
 
     @staticmethod
     def build_dag_run_id(dag_id, dag_run_id):
-        return str(uuid.uuid3(uuid.NAMESPACE_URL, f"{_DAG_NAMESPACE}.{dag_id}.{dag_run_id}"))
+        return str(uuid.uuid3(uuid.NAMESPACE_URL, f"{conf.namespace()}.{dag_id}.{dag_run_id}"))
 
     @staticmethod
     def build_task_instance_run_id(dag_id, task_id, execution_date, try_number):
         return str(
             uuid.uuid3(
                 uuid.NAMESPACE_URL,
-                f"{_DAG_NAMESPACE}.{dag_id}.{task_id}.{execution_date}.{try_number}",
+                f"{conf.namespace()}.{dag_id}.{task_id}.{execution_date}.{try_number}",
             )
         )
 
     def emit(self, event: RunEvent):
         """Emit OpenLineage event.
 
         :param event: Event to be emitted.
@@ -349,15 +339,15 @@
     ) -> Run:
         facets: dict[str, BaseFacet] = {}
         if nominal_start_time:
             facets.update({"nominalTime": NominalTimeRunFacet(nominal_start_time, nominal_end_time)})
         if parent_run_id:
             parent_run_facet = ParentRunFacet.create(
                 runId=parent_run_id,
-                namespace=_DAG_NAMESPACE,
+                namespace=conf.namespace(),
                 name=parent_job_name or job_name,
             )
             facets.update(
                 {
                     "parent": parent_run_facet,
                     "parentRun": parent_run_facet,  # Keep sending this for the backward compatibility
                 }
@@ -392,8 +382,8 @@
                 }
             )
         if job_facets:
             facets = {**facets, **job_facets}
 
         facets.update({"jobType": job_type})
 
-        return Job(_DAG_NAMESPACE, job_name, facets)
+        return Job(conf.namespace(), job_name, facets)
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/facets.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/facets.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,18 +13,25 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from attrs import define
+from deprecated import deprecated
 from openlineage.client.facet import BaseFacet
 from openlineage.client.utils import RedactMixin
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 
+
+@deprecated(
+    reason="To be removed in the next release. Make sure to use information from AirflowRunFacet instead.",
+    category=AirflowProviderDeprecationWarning,
+)
 @define(slots=False)
 class AirflowMappedTaskRunFacet(BaseFacet):
     """Run facet containing information about mapped tasks."""
 
     mapIndex: int
     operatorClass: str
 
@@ -62,12 +69,16 @@
     name: str
     properties: dict[str, object]
     type: str = "operator"
 
     _skip_redact = ["name", "type"]
 
 
+@deprecated(
+    reason="To be removed in the next release. Make sure to use information from AirflowRunFacet instead.",
+    category=AirflowProviderDeprecationWarning,
+)
 @define(slots=False)
 class UnknownOperatorAttributeRunFacet(BaseFacet):
     """RunFacet that describes unknown operators in an Airflow DAG."""
 
     unknownItems: list[UnknownOperatorInstance]
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/listener.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from airflow.listeners import hookimpl
 from airflow.providers.openlineage.extractors import ExtractorManager
 from airflow.providers.openlineage.plugins.adapter import OpenLineageAdapter, RunState
 from airflow.providers.openlineage.utils.utils import (
     get_airflow_run_facet,
     get_custom_facets,
     get_job_name,
+    is_operator_disabled,
+    is_selective_lineage_enabled,
     print_warning,
 )
 from airflow.stats import Stats
 from airflow.utils.timeout import timeout
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
@@ -55,25 +57,39 @@
     @hookimpl
     def on_task_instance_running(
         self,
         previous_state,
         task_instance: TaskInstance,
         session: Session,  # This will always be QUEUED
     ):
-        if not hasattr(task_instance, "task"):
+        if not getattr(task_instance, "task", None) is not None:
             self.log.warning(
-                f"No task set for TI object task_id: {task_instance.task_id} - "
-                f"dag_id: {task_instance.dag_id} - run_id {task_instance.run_id}"
+                "No task set for TI object task_id: %s - dag_id: %s - run_id %s",
+                task_instance.task_id,
+                task_instance.dag_id,
+                task_instance.run_id,
             )
             return
 
         self.log.debug("OpenLineage listener got notification about task instance start")
         dagrun = task_instance.dag_run
         task = task_instance.task
+        if TYPE_CHECKING:
+            assert task
         dag = task.dag
+        if is_operator_disabled(task):
+            self.log.debug(
+                "Skipping OpenLineage event emission for operator %s "
+                "due to its presence in [openlineage] disabled_for_operators.",
+                task.task_type,
+            )
+            return None
+
+        if not is_selective_lineage_enabled(task):
+            return
 
         @print_warning(self.log)
         def on_running():
             # that's a workaround to detect task running from deferred state
             # we return here because Airflow 2.3 needs task from deferred state
             if task_instance.next_method is not None:
                 return
@@ -123,15 +139,27 @@
 
     @hookimpl
     def on_task_instance_success(self, previous_state, task_instance: TaskInstance, session):
         self.log.debug("OpenLineage listener got notification about task instance success")
 
         dagrun = task_instance.dag_run
         task = task_instance.task
+        if TYPE_CHECKING:
+            assert task
         dag = task.dag
+        if is_operator_disabled(task):
+            self.log.debug(
+                "Skipping OpenLineage event emission for operator %s "
+                "due to its presence in [openlineage] disabled_for_operators.",
+                task.task_type,
+            )
+            return None
+
+        if not is_selective_lineage_enabled(task):
+            return
 
         @print_warning(self.log)
         def on_success():
             parent_run_id = OpenLineageAdapter.build_dag_run_id(dag.dag_id, dagrun.run_id)
 
             task_uuid = OpenLineageAdapter.build_task_instance_run_id(
                 dag_id=dag.dag_id,
@@ -166,15 +194,27 @@
 
     @hookimpl
     def on_task_instance_failed(self, previous_state, task_instance: TaskInstance, session):
         self.log.debug("OpenLineage listener got notification about task instance failure")
 
         dagrun = task_instance.dag_run
         task = task_instance.task
+        if TYPE_CHECKING:
+            assert task
         dag = task.dag
+        if is_operator_disabled(task):
+            self.log.debug(
+                "Skipping OpenLineage event emission for operator %s "
+                "due to its presence in [openlineage] disabled_for_operators.",
+                task.task_type,
+            )
+            return None
+
+        if not is_selective_lineage_enabled(task):
+            return
 
         @print_warning(self.log)
         def on_failure():
             parent_run_id = OpenLineageAdapter.build_dag_run_id(dag.dag_id, dagrun.run_id)
 
             task_uuid = OpenLineageAdapter.build_task_instance_run_id(
                 dag_id=dag.dag_id,
@@ -216,39 +256,44 @@
     @hookimpl
     def on_starting(self, component):
         self.log.debug("on_starting: %s", component.__class__.__name__)
 
     @hookimpl
     def before_stopping(self, component):
         self.log.debug("before_stopping: %s", component.__class__.__name__)
-        # TODO: configure this with Airflow config
         with timeout(30):
             self.executor.shutdown(wait=True)
 
     @hookimpl
     def on_dag_run_running(self, dag_run: DagRun, msg: str):
+        if dag_run.dag and not is_selective_lineage_enabled(dag_run.dag):
+            return
         data_interval_start = dag_run.data_interval_start.isoformat() if dag_run.data_interval_start else None
         data_interval_end = dag_run.data_interval_end.isoformat() if dag_run.data_interval_end else None
         self.executor.submit(
             self.adapter.dag_started,
             dag_run=dag_run,
             msg=msg,
             nominal_start_time=data_interval_start,
             nominal_end_time=data_interval_end,
         )
 
     @hookimpl
     def on_dag_run_success(self, dag_run: DagRun, msg: str):
+        if dag_run.dag and not is_selective_lineage_enabled(dag_run.dag):
+            return
         if not self.executor:
             self.log.debug("Executor have not started before `on_dag_run_success`")
             return
         self.executor.submit(self.adapter.dag_success, dag_run=dag_run, msg=msg)
 
     @hookimpl
     def on_dag_run_failed(self, dag_run: DagRun, msg: str):
+        if dag_run.dag and not is_selective_lineage_enabled(dag_run.dag):
+            return
         if not self.executor:
             self.log.debug("Executor have not started before `on_dag_run_failed`")
             return
         self.executor.submit(self.adapter.dag_failed, dag_run=dag_run, msg=msg)
 
 
 def get_openlineage_listener() -> OpenLineageListener:
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/plugins/openlineage.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/openlineage.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,40 +12,30 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import os
-
-from airflow.configuration import conf
 from airflow.plugins_manager import AirflowPlugin
+from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.plugins.listener import get_openlineage_listener
-from airflow.providers.openlineage.plugins.macros import lineage_parent_id, lineage_run_id
-
-
-def _is_disabled() -> bool:
-    return (
-        conf.getboolean("openlineage", "disabled", fallback=False)
-        or os.getenv("OPENLINEAGE_DISABLED", "false").lower() == "true"
-        or (
-            conf.get("openlineage", "transport", fallback="") == ""
-            and conf.get("openlineage", "config_path", fallback="") == ""
-            and os.getenv("OPENLINEAGE_URL", "") == ""
-            and os.getenv("OPENLINEAGE_CONFIG", "") == ""
-        )
-    )
+from airflow.providers.openlineage.plugins.macros import (
+    lineage_job_name,
+    lineage_job_namespace,
+    lineage_parent_id,
+    lineage_run_id,
+)
 
 
 class OpenLineageProviderPlugin(AirflowPlugin):
     """
     Listener that emits numerous Events.
 
     OpenLineage Plugin provides listener that emits OL events on DAG start,
     complete and failure and TaskInstances start, complete and failure.
     """
 
     name = "OpenLineageProviderPlugin"
-    if not _is_disabled():
-        macros = [lineage_run_id, lineage_parent_id]
+    if not conf.is_disabled():
+        macros = [lineage_job_namespace, lineage_job_name, lineage_run_id, lineage_parent_id]
         listeners = [get_openlineage_listener()]
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/sqlparser.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/sqlparser.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/utils/__init__.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/utils/sql.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/airflow/providers/openlineage/utils/utils.py` & `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,144 +16,83 @@
 # under the License.
 
 from __future__ import annotations
 
 import datetime
 import json
 import logging
-import os
 from contextlib import suppress
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Iterable
-from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
 import attrs
-from attrs import asdict
+from openlineage.client.utils import RedactMixin  # TODO: move this maybe to Airflow's logic?
 
-# TODO: move this maybe to Airflow's logic?
-from openlineage.client.utils import RedactMixin
-
-from airflow.compat.functools import cache
-from airflow.configuration import conf
+from airflow.models import DAG, BaseOperator, MappedOperator
+from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.plugins.facets import (
     AirflowMappedTaskRunFacet,
     AirflowRunFacet,
+    UnknownOperatorAttributeRunFacet,
+    UnknownOperatorInstance,
+)
+from airflow.providers.openlineage.utils.selective_enable import (
+    is_dag_lineage_enabled,
+    is_task_lineage_enabled,
 )
 from airflow.utils.context import AirflowContextDeprecationWarning
 from airflow.utils.log.secrets_masker import Redactable, Redacted, SecretsMasker, should_hide_value_for_key
 
 if TYPE_CHECKING:
-    from airflow.models import DAG, BaseOperator, Connection, DagRun, TaskInstance
+    from airflow.models import DagRun, TaskInstance
 
 
 log = logging.getLogger(__name__)
 _NOMINAL_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
-def openlineage_job_name(dag_id: str, task_id: str) -> str:
-    return f"{dag_id}.{task_id}"
-
-
 def get_operator_class(task: BaseOperator) -> type:
     if task.__class__.__name__ in ("DecoratedMappedOperator", "MappedOperator"):
         return task.operator_class
     return task.__class__
 
 
-def to_json_encodable(task: BaseOperator) -> dict[str, object]:
-    def _task_encoder(obj):
-        from airflow.models import DAG
-
-        if isinstance(obj, datetime.datetime):
-            return obj.isoformat()
-        elif isinstance(obj, DAG):
-            return {
-                "dag_id": obj.dag_id,
-                "tags": obj.tags,
-                "schedule_interval": obj.schedule_interval,
-                "timetable": obj.timetable.serialize(),
-            }
-        else:
-            return str(obj)
-
-    return json.loads(json.dumps(task.__dict__, default=_task_encoder))
-
-
-def url_to_https(url) -> str | None:
-    # Ensure URL exists
-    if not url:
-        return None
-
-    base_url = None
-    if url.startswith("git@"):
-        part = url.split("git@")[1:2]
-        if part:
-            base_url = f'https://{part[0].replace(":", "/", 1)}'
-    elif url.startswith("https://"):
-        base_url = url
-
-    if not base_url:
-        raise ValueError(f"Unable to extract location from: {url}")
-
-    if base_url.endswith(".git"):
-        base_url = base_url[:-4]
-    return base_url
-
-
-def redacted_connection_uri(conn: Connection, filtered_params=None, filtered_prefixes=None):
-    """
-    Return the connection URI for the given Connection.
-
-    This method additionally filters URI by removing query parameters that are known to carry sensitive data
-    like username, password, access key.
-    """
-    if filtered_prefixes is None:
-        filtered_prefixes = []
-    if filtered_params is None:
-        filtered_params = []
-
-    def filter_key_params(k: str):
-        return k not in filtered_params and any(substr in k for substr in filtered_prefixes)
-
-    conn_uri = conn.get_uri()
-    parsed = urlparse(conn_uri)
-
-    # Remove username and password
-    netloc = f"{parsed.hostname}" + (f":{parsed.port}" if parsed.port else "")
-    parsed = parsed._replace(netloc=netloc)
-    if parsed.query:
-        query_dict = dict(parse_qsl(parsed.query))
-        if conn.EXTRA_KEY in query_dict:
-            query_dict = json.loads(query_dict[conn.EXTRA_KEY])
-        filtered_qs = {k: v for k, v in query_dict.items() if not filter_key_params(k)}
-        parsed = parsed._replace(query=urlencode(filtered_qs))
-    return urlunparse(parsed)
-
-
-def get_connection(conn_id) -> Connection | None:
-    from airflow.hooks.base import BaseHook
-
-    with suppress(Exception):
-        return BaseHook.get_connection(conn_id=conn_id)
-    return None
-
-
-def get_job_name(task):
+def get_job_name(task: TaskInstance) -> str:
     return f"{task.dag_id}.{task.task_id}"
 
 
 def get_custom_facets(task_instance: TaskInstance | None = None) -> dict[str, Any]:
     custom_facets = {}
     # check for -1 comes from SmartSensor compatibility with dynamic task mapping
     # this comes from Airflow code
     if hasattr(task_instance, "map_index") and getattr(task_instance, "map_index") != -1:
         custom_facets["airflow_mappedTask"] = AirflowMappedTaskRunFacet.from_task_instance(task_instance)
     return custom_facets
 
 
+def get_fully_qualified_class_name(operator: BaseOperator | MappedOperator) -> str:
+    return operator.__class__.__module__ + "." + operator.__class__.__name__
+
+
+def is_operator_disabled(operator: BaseOperator | MappedOperator) -> bool:
+    return get_fully_qualified_class_name(operator) in conf.disabled_operators()
+
+
+def is_selective_lineage_enabled(obj: DAG | BaseOperator | MappedOperator) -> bool:
+    """If selective enable is active check if DAG or Task is enabled to emit events."""
+    if not conf.selective_enable():
+        return True
+    if isinstance(obj, DAG):
+        return is_dag_lineage_enabled(obj)
+    elif isinstance(obj, (BaseOperator, MappedOperator)):
+        return is_task_lineage_enabled(obj)
+    else:
+        raise TypeError("is_selective_lineage_enabled can only be used on DAG or Operator objects")
+
+
 class InfoJsonEncodable(dict):
     """
     Airflow objects might not be json-encodable overall.
 
     The class provides additional attributes to control
     what and how is encoded:
 
@@ -201,15 +140,15 @@
     def _cast_fields(self):
         for field, func in self.casts.items():
             setattr(self, field, func(self.obj))
             self._fields.append(field)
 
     def _include_fields(self):
         if self.includes and self.excludes:
-            raise Exception("Don't use both includes and excludes.")
+            raise ValueError("Don't use both includes and excludes.")
         if self.includes:
             for field in self.includes:
                 if field not in self._fields and hasattr(self.obj, field):
                     setattr(self, field, getattr(self.obj, field))
                     self._fields.append(field)
         else:
             for field, val in self.obj.__dict__.items():
@@ -252,31 +191,42 @@
     }
 
 
 class TaskInfo(InfoJsonEncodable):
     """Defines encoding BaseOperator/AbstractOperator object to JSON."""
 
     renames = {
-        "_BaseOperator__init_kwargs": "args",
         "_BaseOperator__from_mapped": "mapped",
         "_downstream_task_ids": "downstream_task_ids",
         "_upstream_task_ids": "upstream_task_ids",
+        "_is_setup": "is_setup",
+        "_is_teardown": "is_teardown",
     }
-    excludes = [
-        "_BaseOperator__instantiated",
-        "_dag",
-        "_hook",
-        "_log",
-        "_outlets",
-        "_inlets",
-        "_lock_for_execution",
-        "handler",
-        "params",
-        "python_callable",
-        "retry_delay",
+    includes = [
+        "depends_on_past",
+        "downstream_task_ids",
+        "execution_timeout",
+        "executor_config",
+        "ignore_first_depends_on_past",
+        "max_active_tis_per_dag",
+        "max_active_tis_per_dagrun",
+        "max_retry_delay",
+        "multiple_outputs",
+        "owner",
+        "priority_weight",
+        "queue",
+        "retries",
+        "retry_exponential_backoff",
+        "run_as_user",
+        "task_id",
+        "trigger_rule",
+        "upstream_task_ids",
+        "wait_for_downstream",
+        "wait_for_past_depends_before_skipping",
+        "weight_rule",
     ]
     casts = {
         "operator_class": lambda task: task.task_type,
         "task_group": lambda task: TaskGroupInfo(task.task_group)
         if hasattr(task, "task_group") and getattr(task.task_group, "_group_id", None)
         else None,
     }
@@ -302,26 +252,38 @@
     dag_run: DagRun,
     dag: DAG,
     task_instance: TaskInstance,
     task: BaseOperator,
     task_uuid: str,
 ):
     return {
-        "airflow": json.loads(
-            json.dumps(
-                asdict(
-                    AirflowRunFacet(
-                        dag=DagInfo(dag),
-                        dagRun=DagRunInfo(dag_run),
-                        taskInstance=TaskInstanceInfo(task_instance),
-                        task=TaskInfo(task),
-                        taskUuid=task_uuid,
+        "airflow": attrs.asdict(
+            AirflowRunFacet(
+                dag=DagInfo(dag),
+                dagRun=DagRunInfo(dag_run),
+                taskInstance=TaskInstanceInfo(task_instance),
+                task=TaskInfo(task),
+                taskUuid=task_uuid,
+            )
+        )
+    }
+
+
+def get_unknown_source_attribute_run_facet(task: BaseOperator, name: str | None = None):
+    if not name:
+        name = get_operator_class(task).__name__
+    return {
+        "unknownSourceAttribute": attrs.asdict(
+            UnknownOperatorAttributeRunFacet(
+                unknownItems=[
+                    UnknownOperatorInstance(
+                        name=name,
+                        properties=TaskInfo(task),
                     )
-                ),
-                default=str,
+                ]
             )
         )
     }
 
 
 class OpenLineageRedactor(SecretsMasker):
     """
@@ -408,22 +370,14 @@
                 log.warning(e)
 
         return wrapper
 
     return decorator
 
 
-@cache
-def is_source_enabled() -> bool:
-    source_var = conf.get(
-        "openlineage", "disable_source_code", fallback=os.getenv("OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE")
-    )
-    return isinstance(source_var, str) and source_var.lower() not in ("true", "1", "t")
-
-
 def get_filtered_unknown_operator_keys(operator: BaseOperator) -> dict:
     not_required_keys = {"dag", "task_group"}
     return {attr: value for attr, value in operator.__dict__.items() if attr not in not_required_keys}
 
 
 def normalize_sql(sql: str | Iterable[str]):
     if isinstance(sql, str):
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/pyproject.toml` & `apache_airflow_providers_openlineage-1.7.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-openlineage"
-version = "1.6.0.rc1"
+version = "1.7.0.rc1"
 description = "Provider package apache-airflow-providers-openlineage for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,28 +47,29 @@
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
-    "apache-airflow-providers-common-sql>=1.6.0.dev0",
-    "apache-airflow>=2.7.0.dev0",
+    "apache-airflow-providers-common-sql>=1.6.0rc0",
+    "apache-airflow>=2.7.0rc0",
     "attrs>=22.2",
     "openlineage-integration-common>=0.28.0",
     "openlineage-python>=0.28.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_openlineage-1.6.0rc1/PKG-INFO` & `apache_airflow_providers_openlineage-1.7.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.6.0rc1
+Version: 1.7.0rc1
 Summary: Provider package apache-airflow-providers-openlineage for Apache Airflow
 Keywords: airflow-provider,openlineage,airflow,integration
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
-Requires-Dist: apache-airflow-providers-common-sql>=1.6.0.dev0
-Requires-Dist: apache-airflow>=2.7.0.dev0
+Requires-Dist: apache-airflow-providers-common-sql>=1.6.0rc0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: attrs>=22.2
 Requires-Dist: openlineage-integration-common>=0.28.0
 Requires-Dist: openlineage-python>=0.28.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 
 
@@ -75,37 +76,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.6.0.rc1``
+Release: ``1.7.0.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openlineage``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -132,8 +133,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html>`_.
```

