# Comparing `tmp/shipyard_dbt-0.2.0a1.tar.gz` & `tmp/shipyard_dbt-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_dbt-0.2.0a1.tar", max compression
+gzip compressed data, was "shipyard_dbt-0.2.0a2.tar", max compression
```

## Comparing `shipyard_dbt-0.2.0a1.tar` & `shipyard_dbt-0.2.0a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-26 19:00:30.084274 shipyard_dbt-0.2.0a1/README.md
--rw-r--r--   0        0        0      573 2024-04-08 14:57:56.376837 shipyard_dbt-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-26 19:00:30.085016 shipyard_dbt-0.2.0a1/shipyard_dbt/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.434381 shipyard_dbt-0.2.0a1/shipyard_dbt/cli/__init__.py
--rw-r--r--   0        0        0      273 2024-04-04 19:39:49.110800 shipyard_dbt-0.2.0a1/shipyard_dbt/cli/authtest.py
--rw-r--r--   0        0        0     3702 2024-04-08 14:57:35.198305 shipyard_dbt-0.2.0a1/shipyard_dbt/cli/download_logs_artifacts.py
--rw-r--r--   0        0        0     4698 2024-04-08 14:56:19.585350 shipyard_dbt-0.2.0a1/shipyard_dbt/cli/trigger_and_download.py
--rw-r--r--   0        0        0     2363 2024-04-08 14:56:19.592068 shipyard_dbt-0.2.0a1/shipyard_dbt/cli/trigger_job.py
--rw-r--r--   0        0        0     7238 2024-04-08 14:56:19.611580 shipyard_dbt-0.2.0a1/shipyard_dbt/dbt.py
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 shipyard_dbt-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 19:00:30.084274 shipyard_dbt-0.2.0a2/README.md
+-rw-r--r--   0        0        0      573 2024-04-10 17:47:24.602020 shipyard_dbt-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-26 19:00:30.085016 shipyard_dbt-0.2.0a2/shipyard_dbt/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.434381 shipyard_dbt-0.2.0a2/shipyard_dbt/cli/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-04 19:39:49.110800 shipyard_dbt-0.2.0a2/shipyard_dbt/cli/authtest.py
+-rw-r--r--   0        0        0     3702 2024-04-08 14:57:35.198305 shipyard_dbt-0.2.0a2/shipyard_dbt/cli/download_logs_artifacts.py
+-rw-r--r--   0        0        0     4998 2024-04-10 17:47:24.593621 shipyard_dbt-0.2.0a2/shipyard_dbt/cli/trigger_and_download.py
+-rw-r--r--   0        0        0     2363 2024-04-08 14:56:19.592068 shipyard_dbt-0.2.0a2/shipyard_dbt/cli/trigger_job.py
+-rw-r--r--   0        0        0     7238 2024-04-08 14:56:19.611580 shipyard_dbt-0.2.0a2/shipyard_dbt/dbt.py
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 shipyard_dbt-0.2.0a2/PKG-INFO
```

### Comparing `shipyard_dbt-0.2.0a1/pyproject.toml` & `shipyard_dbt-0.2.0a2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-dbt"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = ""
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_dbt"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `shipyard_dbt-0.2.0a1/shipyard_dbt/cli/download_logs_artifacts.py` & `shipyard_dbt-0.2.0a2/shipyard_dbt/cli/download_logs_artifacts.py`

 * *Files identical despite different names*

### Comparing `shipyard_dbt-0.2.0a1/shipyard_dbt/cli/trigger_and_download.py` & `shipyard_dbt-0.2.0a2/shipyard_dbt/cli/trigger_and_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,24 @@
                     run_details_response["data"]["run_steps"], start=1
                 ):
                     step_id = step["id"]
                     logger.info(
                         f"Grabbing step details for step {step_id} ({index} of {number_of_steps})"
                     )
                     artifact.responses.write_json(f"step_{step_id}_response", step)
-
-                    with open(debug_log_name, "a") as debug_file:
-                        debug_file.write(step["debug_logs"])
-
-                    with open(output_log_name, "a") as log_file:
-                        log_file.write(step["logs"])
+                    if step.get("debug_logs"):
+                        with open(debug_log_name, "a") as debug_file:
+                            debug_file.write(step["debug_logs"])
+                    else:
+                        logger.warning(f"No debug logs for step {step_id}")
+                    if step.get("logs"):
+                        with open(output_log_name, "a") as log_file:
+                            log_file.write(step["logs"])
+                    else:
+                        logger.warning(f"No logs for step {step_id}")
 
                 logger.info(f"Successfully wrote logs to {output_log_name}")
                 logger.info(f"Successfully wrote debug_logs to {debug_log_name}")
             elif number_of_steps == 0:
                 logger.info(f"No logs to download for run {run_id}")
 
         if download_artifacts:
```

### Comparing `shipyard_dbt-0.2.0a1/shipyard_dbt/cli/trigger_job.py` & `shipyard_dbt-0.2.0a2/shipyard_dbt/cli/trigger_job.py`

 * *Files identical despite different names*

### Comparing `shipyard_dbt-0.2.0a1/shipyard_dbt/dbt.py` & `shipyard_dbt-0.2.0a2/shipyard_dbt/dbt.py`

 * *Files identical despite different names*

### Comparing `shipyard_dbt-0.2.0a1/PKG-INFO` & `shipyard_dbt-0.2.0a2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-dbt
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

