# Comparing `tmp/jobbergate_agent-5.0.0a1.tar.gz` & `tmp/jobbergate_agent-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_agent-5.0.0a1.tar", max compression
+gzip compressed data, was "jobbergate_agent-5.0.0a2.tar", max compression
```

## Comparing `jobbergate_agent-5.0.0a1.tar` & `jobbergate_agent-5.0.0a2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1077 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/LICENSE
--rw-r--r--   0        0        0     1346 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/README.md
--rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/clients/__init__.py
--rw-r--r--   0        0        0     3597 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/clients/cluster_api.py
--rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/internals/__init__.py
--rw-r--r--   0        0        0     2737 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/internals/update.py
--rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/__init__.py
--rw-r--r--   0        0        0      150 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/constants.py
--rw-r--r--   0        0        0     2805 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/schemas.py
--rw-r--r--   0        0        0    10780 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/submit.py
--rw-r--r--   0        0        0     3676 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/update.py
--rw-r--r--   0        0        0      491 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/main.py
--rw-r--r--   0        0        0     2759 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/settings.py
--rw-r--r--   0        0        0     2627 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/tasks.py
--rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/__init__.py
--rw-r--r--   0        0        0     4663 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/exception.py
--rw-r--r--   0        0        0     1440 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/logging.py
--rw-r--r--   0        0        0     1414 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/plugin.py
--rw-r--r--   0        0        0     2153 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/scheduler.py
--rw-r--r--   0        0        0      730 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/sentry.py
--rw-r--r--   0        0        0     2500 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/user_mapper.py
--rw-r--r--   0        0        0     3235 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/LICENSE
+-rw-r--r--   0        0        0     1346 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/clients/__init__.py
+-rw-r--r--   0        0        0     3597 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/clients/cluster_api.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/internals/__init__.py
+-rw-r--r--   0        0        0     4305 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/internals/update.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/constants.py
+-rw-r--r--   0        0        0     2805 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/schemas.py
+-rw-r--r--   0        0        0    11259 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/submit.py
+-rw-r--r--   0        0        0     3676 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/update.py
+-rw-r--r--   0        0        0      491 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/main.py
+-rw-r--r--   0        0        0     2759 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/settings.py
+-rw-r--r--   0        0        0     2627 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/__init__.py
+-rw-r--r--   0        0        0     4663 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/exception.py
+-rw-r--r--   0        0        0     1440 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/logging.py
+-rw-r--r--   0        0        0     1414 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/plugin.py
+-rw-r--r--   0        0        0     2153 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/scheduler.py
+-rw-r--r--   0        0        0      730 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/sentry.py
+-rw-r--r--   0        0        0     2500 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/user_mapper.py
+-rw-r--r--   0        0        0     3235 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.0.0a2/PKG-INFO
```

### Comparing `jobbergate_agent-5.0.0a1/LICENSE` & `jobbergate_agent-5.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/README.md` & `jobbergate_agent-5.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/clients/cluster_api.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/clients/cluster_api.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/schemas.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/submit.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/submit.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import functools
 import os
 import pwd
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from buzz import DoExceptParams
-from jobbergate_core.tools.sbatch import SubmissionHandler, inject_sbatch_params
+from jobbergate_core.tools.sbatch import InfoHandler, SubmissionHandler, inject_sbatch_params
 from loguru import logger
 
 from jobbergate_agent.clients.cluster_api import backend_client as jobbergate_api_client
 from jobbergate_agent.jobbergate.constants import FileType
-from jobbergate_agent.jobbergate.schemas import JobScriptFile, PendingJobSubmission
+from jobbergate_agent.jobbergate.schemas import JobScriptFile, PendingJobSubmission, SlurmJobData
+from jobbergate_agent.jobbergate.update import fetch_job_data
 from jobbergate_agent.settings import SETTINGS
 from jobbergate_agent.utils.exception import JobbergateApiError, JobSubmissionError, handle_errors_async
 from jobbergate_agent.utils.logging import log_error
 from jobbergate_agent.utils.user_mapper import SlurmUserMapper, manufacture
 
 
 async def retrieve_submission_file(file: JobScriptFile) -> str:
@@ -114,29 +115,32 @@
         response.raise_for_status()
         pending_job_submissions = [PendingJobSubmission(**pjs) for pjs in response.json().get("items", [])]
 
     logger.debug(f"Retrieved {len(pending_job_submissions)} pending job submissions")
     return pending_job_submissions
 
 
-async def mark_as_submitted(job_submission_id: int, slurm_job_id: int):
+async def mark_as_submitted(job_submission_id: int, slurm_job_id: int, slurm_job_data: SlurmJobData):
     """
     Mark job_submission as submitted in the Jobbergate API.
     """
     logger.debug(f"Marking job submission {job_submission_id=} as submitted ({slurm_job_id=})")
 
     with JobbergateApiError.handle_errors(
         f"Could not mark job submission {job_submission_id} as submitted via the Jobbergate API",
         do_except=log_error,
     ):
         response = await jobbergate_api_client.post(
             "jobbergate/job-submissions/agent/submitted",
             json=dict(
                 id=job_submission_id,
                 slurm_job_id=slurm_job_id,
+                slurm_job_state=slurm_job_data.job_state,
+                slurm_job_info=slurm_job_data.job_info,
+                slurm_job_state_reason=slurm_job_data.state_reason,
             ),
         )
         response.raise_for_status()
 
 
 async def mark_as_rejected(job_submission_id: int, report_message: str):
     """
@@ -252,14 +256,16 @@
     """
     Submit all pending jobs and update them with ``SUBMITTED`` status and slurm_job_id.
 
     :returns: The ``slurm_job_id`` for the submitted job
     """
     logger.debug("Started submitting pending jobs...")
 
+    info_handler = InfoHandler(scontrol_path=SETTINGS.SCONTROL_PATH)
+
     logger.debug("Building user-mapper")
     user_mapper = manufacture()
 
     logger.debug("Fetching pending jobs...")
     pending_job_submissions = await fetch_pending_submissions()
 
     for pending_job_submission in pending_job_submissions:
@@ -267,11 +273,12 @@
         with JobSubmissionError.handle_errors(
             (f"Failed to submit pending job_submission {pending_job_submission.id}" "...skipping to next pending job"),
             do_except=log_error,
             do_else=lambda: logger.debug(f"Finished submitting pending job_submission {pending_job_submission.id}"),
             re_raise=False,
         ):
             slurm_job_id = await submit_job_script(pending_job_submission, user_mapper)
+            slurm_job_data: SlurmJobData = await fetch_job_data(slurm_job_id, info_handler)
 
-            await mark_as_submitted(pending_job_submission.id, slurm_job_id)
+            await mark_as_submitted(pending_job_submission.id, slurm_job_id, slurm_job_data)
 
     logger.debug("...Finished submitting pending jobs")
```

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/update.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/settings.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/settings.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/tasks.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/tasks.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/exception.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/exception.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/logging.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/plugin.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/scheduler.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/sentry.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/user_mapper.py` & `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/user_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a1/pyproject.toml` & `jobbergate_agent-5.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-agent"
-version = "5.0.0a1"
+version = "5.0.0a2"
 description = "Jobbergate Agent"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_agent-5.0.0a1/PKG-INFO` & `jobbergate_agent-5.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-agent
-Version: 5.0.0a1
+Version: 5.0.0a2
 Summary: Jobbergate Agent
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: apscheduler (==3.10.3)
 Requires-Dist: auto-name-enum (>=2.0.0,<3.0.0)
 Requires-Dist: httpx (==0.24.1)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0) ; python_version < "3.10"
-Requires-Dist: jobbergate-core (==5.0.0a1)
+Requires-Dist: jobbergate-core (==5.0.0a2)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: py-buzz (>=4.0.0,<5.0.0)
 Requires-Dist: pydantic (==1.10.12)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-jose (==3.3.0)
 Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0)
```

