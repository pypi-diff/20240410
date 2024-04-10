# Comparing `tmp/apache_airflow_providers_databricks-6.2.0rc1.tar.gz` & `tmp/apache_airflow_providers_databricks-6.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_databricks-6.2.0rc1.tar", last modified: Sun Feb 11 07:25:45 2024, max compression
+gzip compressed data, was "apache_airflow_providers_databricks-6.3.0rc1.tar", last modified: Tue Apr  9 12:25:57 2024, max compression
```

## Comparing `apache_airflow_providers_databricks-6.2.0rc1.tar` & `apache_airflow_providers_databricks-6.3.0rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4443 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/LICENSE
--rw-r--r--   0        0        0     1585 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/__init__.py
--rw-r--r--   0        0        0     6200 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0        0        0    23076 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0        0        0    30591 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0        0        0    12580 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
--rw-r--r--   0        0        0      787 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0        0        0    41336 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0        0        0    13092 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0        0        0    16809 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/databricks_sql.py
--rw-r--r--   0        0        0      785 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0        0        0    10605 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0        0        0     5771 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
--rw-r--r--   0        0        0      787 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0        0        0     3997 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/triggers/databricks.py
--rw-r--r--   0        0        0      785 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/utils/databricks.py
--rw-r--r--   0        0        0     3226 2024-02-11 07:25:45.000000 apache_airflow_providers_databricks-6.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6448 1970-01-01 00:00:00.000000 apache_airflow_providers_databricks-6.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4448 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/LICENSE
+-rw-r--r--   0        0        0     1585 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/__init__.py
+-rw-r--r--   0        0        0     6221 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0        0        0    23378 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0        0        0    30592 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0        0        0    12564 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0        0        0    42438 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0        0        0    13093 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0        0        0    16800 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0        0        0    10605 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0        0        0     5771 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0        0        0     4125 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/databricks.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/databricks.py
+-rw-r--r--   0        0        0     3268 2024-04-09 12:25:57.000000 apache_airflow_providers_databricks-6.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6500 1970-01-01 00:00:00.000000 apache_airflow_providers_databricks-6.3.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/README.rst` & `apache_airflow_providers_databricks-6.3.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``6.2.0.rc1``
+Release: ``6.3.0.rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-databricks``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==========================
 PIP package                              Version required
 =======================================  ==========================
@@ -95,8 +95,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/LICENSE` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "6.2.0"
+__version__ = "6.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/get_provider_info.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-databricks",
         "name": "Databricks",
         "description": "`Databricks <https://databricks.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1707636345,
+        "source-date-epoch": 1712665557,
         "versions": [
+            "6.3.0",
             "6.2.0",
             "6.1.0",
             "6.0.0",
             "5.0.1",
             "5.0.0",
             "4.7.0",
             "4.6.0",
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 This hook enable the submitting and running of jobs to the Databricks platform. Internally the
 operators talk to the
 ``api/2.1/jobs/run-now``
 `endpoint <https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunNow>_`
 or the ``api/2.1/jobs/runs/submit``
 `endpoint <https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunsSubmit>`_.
 """
+
 from __future__ import annotations
 
 import json
 from typing import Any
 
 from requests import exceptions as requests_exceptions
 
@@ -46,14 +47,15 @@
 SUBMIT_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/submit")
 GET_RUN_ENDPOINT = ("GET", "api/2.1/jobs/runs/get")
 CANCEL_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/cancel")
 DELETE_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/delete")
 REPAIR_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/repair")
 OUTPUT_RUNS_JOB_ENDPOINT = ("GET", "api/2.1/jobs/runs/get-output")
 CANCEL_ALL_RUNS_ENDPOINT = ("POST", "api/2.1/jobs/runs/cancel-all")
+UPDATE_PERMISSION_ENDPOINT = ("PATCH", "/api/2.0/permissions/jobs")
 
 INSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/install")
 UNINSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/uninstall")
 
 LIST_JOBS_ENDPOINT = ("GET", "api/2.1/jobs/list")
 LIST_PIPELINES_ENDPOINT = ("GET", "api/2.0/pipelines")
 
@@ -192,26 +194,24 @@
         retry_delay: float = 1.0,
         retry_args: dict[Any, Any] | None = None,
         caller: str = "DatabricksHook",
     ) -> None:
         super().__init__(databricks_conn_id, timeout_seconds, retry_limit, retry_delay, retry_args, caller)
 
     def create_job(self, json: dict) -> int:
-        """
-        Utility function to call the ``api/2.1/jobs/create`` endpoint.
+        """Call the ``api/2.1/jobs/create`` endpoint.
 
         :param json: The data used in the body of the request to the ``create`` endpoint.
         :return: the job_id as an int
         """
         response = self._do_api_call(CREATE_ENDPOINT, json)
         return response["job_id"]
 
     def reset_job(self, job_id: str, json: dict) -> None:
-        """
-        Utility function to call the ``api/2.1/jobs/reset`` endpoint.
+        """Call the ``api/2.1/jobs/reset`` endpoint.
 
         :param json: The data used in the new_settings of the request to the ``reset`` endpoint.
         """
         self._do_api_call(RESET_ENDPOINT, {"job_id": job_id, "new_settings": json})
 
     def run_now(self, json: dict) -> int:
         """
@@ -526,15 +526,15 @@
         :param json: repair a job run.
         """
         response = self._do_api_call(REPAIR_RUN_ENDPOINT, json)
         return response["repair_id"]
 
     def get_latest_repair_id(self, run_id: int) -> int | None:
         """Get latest repair id if any exist for run_id else None."""
-        json = {"run_id": run_id, "include_history": True}
+        json = {"run_id": run_id, "include_history": "true"}
         response = self._do_api_call(GET_RUN_ENDPOINT, json)
         repair_history = response["repair_history"]
         if len(repair_history) == 1:
             return None
         else:
             return repair_history[-1]["id"]
 
@@ -652,14 +652,23 @@
                 return str(result["object_id"])
         except requests_exceptions.HTTPError as e:
             if e.response.status_code != 404:
                 raise e
 
         return None
 
+    def update_job_permission(self, json: dict[str, Any]) -> dict:
+        """
+        Update databricks job permission.
+
+        :param json: payload
+        :return: json containing permission specification
+        """
+        return self._do_api_call(UPDATE_PERMISSION_ENDPOINT, json)
+
     def test_connection(self) -> tuple[bool, str]:
         """Test the Databricks connectivity from UI."""
         hook = DatabricksHook(databricks_conn_id=self.databricks_conn_id)
         try:
             hook._do_api_call(endpoint_info=SPARK_VERSIONS_ENDPOINT).get("versions")
             status = True
             message = "Connection successfully tested"
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/databricks_base.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """
 Databricks hook.
 
 This hook enable the submitting and running of jobs to the Databricks platform. Internally the
 operators talk to the ``api/2.0/jobs/runs/submit``
 `endpoint <https://docs.databricks.com/api/latest/jobs.html#runs-submit>`_.
 """
+
 from __future__ import annotations
 
 import copy
 import platform
 import time
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/hooks/databricks_sql.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,28 +179,26 @@
         self,
         sql: str | Iterable[str],
         autocommit: bool = ...,
         parameters: Iterable | Mapping[str, Any] | None = ...,
         handler: None = ...,
         split_statements: bool = ...,
         return_last: bool = ...,
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
-    ) -> tuple | list[tuple] | list[list[tuple] | tuple] | None:
-        ...
+    ) -> tuple | list[tuple] | list[list[tuple] | tuple] | None: ...
 
     def run(
         self,
         sql: str | Iterable[str],
         autocommit: bool = False,
         parameters: Iterable | Mapping[str, Any] | None = None,
         handler: Callable[[Any], T] | None = None,
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Databricks operators."""
+
 from __future__ import annotations
 
 import time
 from functools import cached_property
 from logging import Logger
 from typing import TYPE_CHECKING, Any, Sequence
 
@@ -47,74 +48,75 @@
     Handle the Airflow + Databricks lifecycle logic for a Databricks operator.
 
     :param operator: Databricks operator being handled
     :param context: Airflow context
     """
     if operator.do_xcom_push and context is not None:
         context["ti"].xcom_push(key=XCOM_RUN_ID_KEY, value=operator.run_id)
+
     log.info("Run submitted with run_id: %s", operator.run_id)
     run_page_url = hook.get_run_page_url(operator.run_id)
     if operator.do_xcom_push and context is not None:
         context["ti"].xcom_push(key=XCOM_RUN_PAGE_URL_KEY, value=run_page_url)
 
     if operator.wait_for_termination:
         while True:
             run_info = hook.get_run(operator.run_id)
             run_state = RunState(**run_info["state"])
             if run_state.is_terminal:
                 if run_state.is_successful:
                     log.info("%s completed successfully.", operator.task_id)
                     log.info("View run status, Spark UI, and logs at %s", run_page_url)
                     return
-                else:
-                    if run_state.result_state == "FAILED":
-                        task_run_id = None
-                        if "tasks" in run_info:
-                            for task in run_info["tasks"]:
-                                if task.get("state", {}).get("result_state", "") == "FAILED":
-                                    task_run_id = task["run_id"]
-                        if task_run_id is not None:
-                            run_output = hook.get_run_output(task_run_id)
-                            if "error" in run_output:
-                                notebook_error = run_output["error"]
-                            else:
-                                notebook_error = run_state.state_message
+
+                if run_state.result_state == "FAILED":
+                    task_run_id = None
+                    if "tasks" in run_info:
+                        for task in run_info["tasks"]:
+                            if task.get("state", {}).get("result_state", "") == "FAILED":
+                                task_run_id = task["run_id"]
+                    if task_run_id is not None:
+                        run_output = hook.get_run_output(task_run_id)
+                        if "error" in run_output:
+                            notebook_error = run_output["error"]
                         else:
                             notebook_error = run_state.state_message
-                        error_message = (
-                            f"{operator.task_id} failed with terminal state: {run_state} "
-                            f"and with the error {notebook_error}"
-                        )
                     else:
-                        error_message = (
-                            f"{operator.task_id} failed with terminal state: {run_state} "
-                            f"and with the error {run_state.state_message}"
-                        )
-                    if isinstance(operator, DatabricksRunNowOperator) and operator.repair_run:
-                        operator.repair_run = False
-                        log.warning(
-                            "%s but since repair run is set, repairing the run with all failed tasks",
-                            error_message,
-                        )
-
-                        latest_repair_id = hook.get_latest_repair_id(operator.run_id)
-                        repair_json = {"run_id": operator.run_id, "rerun_all_failed_tasks": True}
-                        if latest_repair_id is not None:
-                            repair_json["latest_repair_id"] = latest_repair_id
-                        operator.json["latest_repair_id"] = hook.repair_run(operator, repair_json)
-                        _handle_databricks_operator_execution(operator, hook, log, context)
-                    raise AirflowException(error_message)
-
-            else:
-                log.info("%s in run state: %s", operator.task_id, run_state)
-                log.info("View run status, Spark UI, and logs at %s", run_page_url)
-                log.info("Sleeping for %s seconds.", operator.polling_period_seconds)
-                time.sleep(operator.polling_period_seconds)
-    else:
-        log.info("View run status, Spark UI, and logs at %s", run_page_url)
+                        notebook_error = run_state.state_message
+                    error_message = (
+                        f"{operator.task_id} failed with terminal state: {run_state} "
+                        f"and with the error {notebook_error}"
+                    )
+                else:
+                    error_message = (
+                        f"{operator.task_id} failed with terminal state: {run_state} "
+                        f"and with the error {run_state.state_message}"
+                    )
+
+                if isinstance(operator, DatabricksRunNowOperator) and operator.repair_run:
+                    operator.repair_run = False
+                    log.warning(
+                        "%s but since repair run is set, repairing the run with all failed tasks",
+                        error_message,
+                    )
+
+                    latest_repair_id = hook.get_latest_repair_id(operator.run_id)
+                    repair_json = {"run_id": operator.run_id, "rerun_all_failed_tasks": True}
+                    if latest_repair_id is not None:
+                        repair_json["latest_repair_id"] = latest_repair_id
+                    operator.json["latest_repair_id"] = hook.repair_run(operator, repair_json)
+                    _handle_databricks_operator_execution(operator, hook, log, context)
+                raise AirflowException(error_message)
+
+            log.info("%s in run state: %s", operator.task_id, run_state)
+            log.info("View run status, Spark UI, and logs at %s", run_page_url)
+            log.info("Sleeping for %s seconds.", operator.polling_period_seconds)
+            time.sleep(operator.polling_period_seconds)
+
+    log.info("View run status, Spark UI, and logs at %s", run_page_url)
 
 
 def _handle_deferrable_databricks_operator_execution(operator, hook, log, context) -> None:
     """
     Handle the Airflow + Databricks lifecycle logic for deferrable Databricks operators.
 
     :param operator: Databricks async operator being handled
@@ -141,14 +143,15 @@
                     run_id=operator.run_id,
                     databricks_conn_id=operator.databricks_conn_id,
                     polling_period_seconds=operator.polling_period_seconds,
                     retry_limit=operator.databricks_retry_limit,
                     retry_delay=operator.databricks_retry_delay,
                     retry_args=operator.databricks_retry_args,
                     run_page_url=run_page_url,
+                    repair_run=getattr(operator, "repair_run", False),
                 ),
                 method_name=DEFER_METHOD_NAME,
             )
         else:
             if run_state.is_successful:
                 log.info("%s completed successfully.", operator.task_id)
 
@@ -158,17 +161,23 @@
     run_state = RunState.from_json(event["run_state"])
     run_page_url = event["run_page_url"]
     log.info("View run status, Spark UI, and logs at %s", run_page_url)
 
     if run_state.is_successful:
         log.info("Job run completed successfully.")
         return
-    else:
-        error_message = f"Job run failed with terminal state: {run_state}"
-        raise AirflowException(error_message)
+
+    error_message = f"Job run failed with terminal state: {run_state}"
+    if event["repair_run"]:
+        log.warning(
+            "%s but since repair run is set, repairing the run with all failed tasks",
+            error_message,
+        )
+        return
+    raise AirflowException(error_message)
 
 
 class DatabricksJobRunLink(BaseOperatorLink):
     """Constructs a link to monitor a Databricks Job Run."""
 
     name = "See Databricks Job Run"
 
@@ -253,15 +262,15 @@
         databricks_conn_id: str = "databricks_default",
         polling_period_seconds: int = 30,
         databricks_retry_limit: int = 3,
         databricks_retry_delay: int = 1,
         databricks_retry_args: dict[Any, Any] | None = None,
         **kwargs,
     ) -> None:
-        """Creates a new ``DatabricksCreateJobsOperator``."""
+        """Create a new ``DatabricksCreateJobsOperator``."""
         super().__init__(**kwargs)
         self.json = json or {}
         self.databricks_conn_id = databricks_conn_id
         self.polling_period_seconds = polling_period_seconds
         self.databricks_retry_limit = databricks_retry_limit
         self.databricks_retry_delay = databricks_retry_delay
         self.databricks_retry_args = databricks_retry_args
@@ -283,16 +292,16 @@
             self.json["schedule"] = schedule
         if max_concurrent_runs is not None:
             self.json["max_concurrent_runs"] = max_concurrent_runs
         if git_source is not None:
             self.json["git_source"] = git_source
         if access_control_list is not None:
             self.json["access_control_list"] = access_control_list
-
-        self.json = normalise_json_content(self.json)
+        if self.json:
+            self.json = normalise_json_content(self.json)
 
     @cached_property
     def _hook(self):
         return DatabricksHook(
             self.databricks_conn_id,
             retry_limit=self.databricks_retry_limit,
             retry_delay=self.databricks_retry_delay,
@@ -303,14 +312,18 @@
     def execute(self, context: Context) -> int:
         if "name" not in self.json:
             raise AirflowException("Missing required parameter: name")
         job_id = self._hook.find_job_id_by_name(self.json["name"])
         if job_id is None:
             return self._hook.create_job(self.json)
         self._hook.reset_job(str(job_id), self.json)
+        if (access_control_list := self.json.get("access_control_list")) is not None:
+            acl_json = {"access_control_list": access_control_list}
+            self._hook.update_job_permission(normalise_json_content(acl_json))
+
         return job_id
 
 
 class DatabricksSubmitRunOperator(BaseOperator):
     """
     Submits a Spark job run to Databricks using the api/2.1/jobs/runs/submit API endpoint.
 
@@ -579,17 +592,14 @@
 
     def execute(self, context):
         hook = self._get_hook(caller="DatabricksSubmitRunDeferrableOperator")
         json_normalised = normalise_json_content(self.json)
         self.run_id = hook.submit_run(json_normalised)
         _handle_deferrable_databricks_operator_execution(self, hook, self.log, context)
 
-    def execute_complete(self, context: dict | None, event: dict):
-        _handle_deferrable_databricks_operator_completion(event, self.log)
-
 
 class DatabricksRunNowOperator(BaseOperator):
     """
     Runs an existing Spark job run to Databricks using the api/2.1/jobs/run-now API endpoint.
 
     See: https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunNow
 
@@ -641,14 +651,15 @@
         - ``notebook_params``
         - ``python_params``
         - ``python_named_parameters``
         - ``jar_params``
         - ``spark_submit_params``
         - ``idempotency_token``
         - ``repair_run``
+        - ``cancel_previous_runs``
 
     :param job_id: the job_id of the existing Databricks job.
         This field will be templated.
 
         .. seealso::
             https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunNow
     :param job_name: the name of the existing Databricks job.
@@ -729,15 +740,16 @@
         unreachable. Its value must be greater than or equal to 1.
     :param databricks_retry_delay: Number of seconds to wait between retries (it
             might be a floating point number).
     :param databricks_retry_args: An optional dictionary with arguments passed to ``tenacity.Retrying`` class.
     :param do_xcom_push: Whether we should push run_id and run_page_url to xcom.
     :param wait_for_termination: if we should wait for termination of the job run. ``True`` by default.
     :param deferrable: Run operator in the deferrable mode.
-    :param repair_run: Repair the databricks run in case of failure, doesn't work in deferrable mode
+    :param repair_run: Repair the databricks run in case of failure.
+    :param cancel_previous_runs: Cancel all existing running jobs before submitting new one.
     """
 
     # Used in airflow.models.BaseOperator
     template_fields: Sequence[str] = ("json", "databricks_conn_id")
     template_ext: Sequence[str] = (".json-tpl",)
     # Databricks brand color (blue) under white text
     ui_color = "#1CB1C2"
@@ -761,27 +773,29 @@
         databricks_retry_limit: int = 3,
         databricks_retry_delay: int = 1,
         databricks_retry_args: dict[Any, Any] | None = None,
         do_xcom_push: bool = True,
         wait_for_termination: bool = True,
         deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         repair_run: bool = False,
+        cancel_previous_runs: bool = False,
         **kwargs,
     ) -> None:
         """Create a new ``DatabricksRunNowOperator``."""
         super().__init__(**kwargs)
         self.json = json or {}
         self.databricks_conn_id = databricks_conn_id
         self.polling_period_seconds = polling_period_seconds
         self.databricks_retry_limit = databricks_retry_limit
         self.databricks_retry_delay = databricks_retry_delay
         self.databricks_retry_args = databricks_retry_args
         self.wait_for_termination = wait_for_termination
         self.deferrable = deferrable
         self.repair_run = repair_run
+        self.cancel_previous_runs = cancel_previous_runs
 
         if job_id is not None:
             self.json["job_id"] = job_id
         if job_name is not None:
             self.json["job_name"] = job_name
         if "job_id" in self.json and "job_name" in self.json:
             raise AirflowException("Argument 'job_name' is not allowed with argument 'job_id'")
@@ -793,16 +807,16 @@
             self.json["python_named_params"] = python_named_params
         if jar_params is not None:
             self.json["jar_params"] = jar_params
         if spark_submit_params is not None:
             self.json["spark_submit_params"] = spark_submit_params
         if idempotency_token is not None:
             self.json["idempotency_token"] = idempotency_token
-
-        self.json = normalise_json_content(self.json)
+        if self.json:
+            self.json = normalise_json_content(self.json)
         # This variable will be used in case our task gets killed.
         self.run_id: int | None = None
         self.do_xcom_push = do_xcom_push
 
     @cached_property
     def _hook(self):
         return self._get_hook(caller="DatabricksRunNowOperator")
@@ -820,25 +834,38 @@
         hook = self._hook
         if "job_name" in self.json:
             job_id = hook.find_job_id_by_name(self.json["job_name"])
             if job_id is None:
                 raise AirflowException(f"Job ID for job name {self.json['job_name']} can not be found")
             self.json["job_id"] = job_id
             del self.json["job_name"]
+
+        if self.cancel_previous_runs and self.json["job_id"] is not None:
+            hook.cancel_all_runs(self.json["job_id"])
+
         self.run_id = hook.run_now(self.json)
         if self.deferrable:
             _handle_deferrable_databricks_operator_execution(self, hook, self.log, context)
         else:
             _handle_databricks_operator_execution(self, hook, self.log, context)
 
     def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
         if event:
             _handle_deferrable_databricks_operator_completion(event, self.log)
+            if event["repair_run"]:
+                self.repair_run = False
+                self.run_id = event["run_id"]
+                latest_repair_id = self._hook.get_latest_repair_id(self.run_id)
+                repair_json = {"run_id": self.run_id, "rerun_all_failed_tasks": True}
+                if latest_repair_id is not None:
+                    repair_json["latest_repair_id"] = latest_repair_id
+                self.json["latest_srepair_id"] = self._hook.repair_run(repair_json)
+                _handle_deferrable_databricks_operator_execution(self, self._hook, self.log, context)
 
-    def on_kill(self):
+    def on_kill(self) -> None:
         if self.run_id:
             self._hook.cancel_run(self.run_id)
             self.log.info(
                 "Task: %s with run_id: %s was requested to be cancelled.", self.task_id, self.run_id
             )
         else:
             self.log.error("Error: Task: %s with invalid run_id was requested to be cancelled.", self.task_id)
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/databricks_repos.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Databricks operators."""
+
 from __future__ import annotations
 
 import re
 from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 from urllib.parse import urlsplit
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/operators/databricks_sql.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Databricks operators."""
+
 from __future__ import annotations
 
 import csv
 import json
 from typing import TYPE_CHECKING, Any, Sequence
 
 from databricks.sql.utils import ParamEscaper
@@ -203,17 +204,17 @@
         (could be also specified in ``copy_options``).
     :param validate: optional configuration for schema & data validation. ``True`` forces validation
         of all rows, integer number - validate only N first rows
     :param copy_options: optional dictionary of copy options. Right now only ``force`` option is supported.
     """
 
     template_fields: Sequence[str] = (
-        "_file_location",
-        "_files",
-        "_table_name",
+        "file_location",
+        "files",
+        "table_name",
         "databricks_conn_id",
     )
 
     def __init__(
         self,
         *,
         table_name: str,
@@ -245,25 +246,25 @@
             raise AirflowException("Only one of 'pattern' or 'files' should be specified")
         if table_name == "":
             raise AirflowException("table_name shouldn't be empty")
         if file_location == "":
             raise AirflowException("file_location shouldn't be empty")
         if file_format not in COPY_INTO_APPROVED_FORMATS:
             raise AirflowException(f"file_format '{file_format}' isn't supported")
-        self._files = files
+        self.files = files
         self._pattern = pattern
         self._file_format = file_format
         self.databricks_conn_id = databricks_conn_id
         self._http_path = http_path
         self._sql_endpoint_name = sql_endpoint_name
         self.session_config = session_configuration
-        self._table_name = table_name
+        self.table_name = table_name
         self._catalog = catalog
         self._schema = schema
-        self._file_location = file_location
+        self.file_location = file_location
         self._expression_list = expression_list
         self._credential = credential
         self._storage_credential = storage_credential
         self._encryption = encryption
         self._format_options = format_options
         self._copy_options = copy_options or {}
         self._validate = validate
@@ -309,22 +310,22 @@
             maybe_encryption = ""
             if self._encryption is not None:
                 maybe_encryption = self._generate_options("ENCRYPTION", escaper, self._encryption, False)
             maybe_credential = ""
             if self._credential is not None:
                 maybe_credential = self._generate_options("CREDENTIAL", escaper, self._credential, False)
             maybe_with = f" WITH ({maybe_credential} {maybe_encryption})"
-        location = escaper.escape_item(self._file_location) + maybe_with
+        location = escaper.escape_item(self.file_location) + maybe_with
         if self._expression_list is not None:
             location = f"(SELECT {self._expression_list} FROM {location})"
         files_or_pattern = ""
         if self._pattern is not None:
             files_or_pattern = f"PATTERN = {escaper.escape_item(self._pattern)}\n"
-        elif self._files is not None:
-            files_or_pattern = f"FILES = {escaper.escape_item(self._files)}\n"
+        elif self.files is not None:
+            files_or_pattern = f"FILES = {escaper.escape_item(self.files)}\n"
         format_options = self._generate_options("FORMAT_OPTIONS", escaper, self._format_options) + "\n"
         copy_options = self._generate_options("COPY_OPTIONS", escaper, self._copy_options) + "\n"
         storage_cred = ""
         if self._storage_credential:
             storage_cred = f" WITH (CREDENTIAL {self._storage_credential})"
         validation = ""
         if self._validate is not None:
@@ -336,15 +337,15 @@
                     raise AirflowException(
                         f"Number of rows for validation should be positive, got: {self._validate}"
                     )
                 validation = f"VALIDATE {self._validate} ROWS\n"
             else:
                 raise AirflowException(f"Incorrect data type for validate parameter: {type(self._validate)}")
         # TODO: think on how to make sure that table_name and expression_list aren't used for SQL injection
-        sql = f"""COPY INTO {self._table_name}{storage_cred}
+        sql = f"""COPY INTO {self.table_name}{storage_cred}
 FROM {location}
 FILEFORMAT = {self._file_format}
 {validation}{files_or_pattern}{format_options}{copy_options}
 """
         return sql.strip()
 
     def execute(self, context: Context) -> Any:
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/sensors/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/sensors/databricks_partition.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/sensors/databricks_sql.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/triggers/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/triggers/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/triggers/databricks.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,23 +43,25 @@
         run_id: int,
         databricks_conn_id: str,
         polling_period_seconds: int = 30,
         retry_limit: int = 3,
         retry_delay: int = 10,
         retry_args: dict[Any, Any] | None = None,
         run_page_url: str | None = None,
+        repair_run: bool = False,
     ) -> None:
         super().__init__()
         self.run_id = run_id
         self.databricks_conn_id = databricks_conn_id
         self.polling_period_seconds = polling_period_seconds
         self.retry_limit = retry_limit
         self.retry_delay = retry_delay
         self.retry_args = retry_args
         self.run_page_url = run_page_url
+        self.repair_run = repair_run
         self.hook = DatabricksHook(
             databricks_conn_id,
             retry_limit=self.retry_limit,
             retry_delay=self.retry_delay,
             retry_args=retry_args,
         )
 
@@ -70,31 +72,33 @@
                 "run_id": self.run_id,
                 "databricks_conn_id": self.databricks_conn_id,
                 "polling_period_seconds": self.polling_period_seconds,
                 "retry_limit": self.retry_limit,
                 "retry_delay": self.retry_delay,
                 "retry_args": self.retry_args,
                 "run_page_url": self.run_page_url,
+                "repair_run": self.repair_run,
             },
         )
 
     async def run(self):
         async with self.hook:
             while True:
                 run_state = await self.hook.a_get_run_state(self.run_id)
                 if run_state.is_terminal:
                     yield TriggerEvent(
                         {
                             "run_id": self.run_id,
                             "run_page_url": self.run_page_url,
                             "run_state": run_state.to_json(),
+                            "repair_run": self.repair_run,
                         }
                     )
                     return
-                else:
-                    self.log.info(
-                        "run-id %s in run state %s. sleeping for %s seconds",
-                        self.run_id,
-                        run_state,
-                        self.polling_period_seconds,
-                    )
-                    await asyncio.sleep(self.polling_period_seconds)
+
+                self.log.info(
+                    "run-id %s in run state %s. sleeping for %s seconds",
+                    self.run_id,
+                    run_state,
+                    self.polling_period_seconds,
+                )
+                await asyncio.sleep(self.polling_period_seconds)
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/utils/__init__.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/airflow/providers/databricks/utils/databricks.py` & `apache_airflow_providers_databricks-6.3.0rc1/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/pyproject.toml` & `apache_airflow_providers_databricks-6.3.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-databricks"
-version = "6.2.0.rc1"
+version = "6.3.0.rc1"
 description = "Provider package apache-airflow-providers-databricks for Apache Airflow"
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
     "aiohttp>=3.9.2, <4",
-    "apache-airflow-providers-common-sql>=1.10.0.dev0",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow-providers-common-sql>=1.10.0rc0",
+    "apache-airflow>=2.6.0rc0",
     "databricks-sql-connector>=2.0.0, <3.0.0, !=2.9.0",
     "requests>=2.27.0,<3",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_databricks-6.2.0rc1/PKG-INFO` & `apache_airflow_providers_databricks-6.3.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 6.2.0rc1
+Version: 6.3.0rc1
 Summary: Provider package apache-airflow-providers-databricks for Apache Airflow
 Keywords: airflow-provider,databricks,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,25 +15,26 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: aiohttp>=3.9.2, <4
-Requires-Dist: apache-airflow-providers-common-sql>=1.10.0.dev0
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow-providers-common-sql>=1.10.0rc0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: databricks-sql-connector>=2.0.0, <3.0.0, !=2.9.0
 Requires-Dist: requests>=2.27.0,<3
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: databricks-sdk==0.10.0 ; extra == "sdk"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 Provides-Extra: sdk
 
@@ -77,37 +78,37 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``6.2.0.rc1``
+Release: ``6.3.0.rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-databricks``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==========================
 PIP package                              Version required
 =======================================  ==========================
@@ -134,8 +135,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/6.3.0/changelog.html>`_.
```

