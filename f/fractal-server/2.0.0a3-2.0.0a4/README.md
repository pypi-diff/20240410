# Comparing `tmp/fractal_server-2.0.0a3.tar.gz` & `tmp/fractal_server-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-2.0.0a3.tar", max compression
+gzip compressed data, was "fractal_server-2.0.0a4.tar", max compression
```

## Comparing `fractal_server-2.0.0a3.tar` & `fractal_server-2.0.0a4.tar`

### file list

```diff
@@ -1,159 +1,163 @@
--rw-r--r--   0        0        0     1576 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/LICENSE
--rw-r--r--   0        0        0     2466 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/README.md
--rw-r--r--   0        0        0       24 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      183 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0      567 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     3378 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1090 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/state.py
--rw-r--r--   0        0        0      413 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/dataset.py
--rw-r--r--   0        0        0     3304 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/job.py
--rw-r--r--   0        0        0      859 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/project.py
--rw-r--r--   0        0        0     2782 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/task.py
--rw-r--r--   0        0        0     3950 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/workflow.py
--rw-r--r--   0        0        0      400 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/__init__.py
--rw-r--r--   0        0        0     1483 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/dataset.py
--rw-r--r--   0        0        0     1535 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/job.py
--rw-r--r--   0        0        0      845 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/project.py
--rw-r--r--   0        0        0     3257 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/task.py
--rw-r--r--   0        0        0     1256 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/models/v2/workflow.py
--rw-r--r--   0        0        0     2727 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/models/v2/workflowtask.py
--rw-r--r--   0        0        0        0 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0    13981 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/admin/v1.py
--rw-r--r--   0        0        0     9706 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/admin/v2.py
--rw-r--r--   0        0        0      315 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      958 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11955 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16911 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5436 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15765 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     6123 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8457 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10930 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5579 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     1217 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/__init__.py
--rw-r--r--   0        0        0    14218 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/_aux_functions.py
--rw-r--r--   0        0        0     9680 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/dataset.py
--rw-r--r--   0        0        0     5956 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/images.py
--rw-r--r--   0        0        0     5334 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/job.py
--rw-r--r--   0        0        0     6024 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/project.py
--rw-r--r--   0        0        0     7219 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/submit.py
--rw-r--r--   0        0        0     7130 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task.py
--rw-r--r--   0        0        0     8466 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task_collection.py
--rw-r--r--   0        0        0    11845 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflow.py
--rw-r--r--   0        0        0     8414 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0      829 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/async_wrap.py
--rw-r--r--   0        0        0      119 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/components.py
--rw-r--r--   0        0        0     4159 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/exceptions.py
--rw-r--r--   0        0        0       65 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/__init__.py
--rw-r--r--   0        0        0     8841 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_batching.py
--rw-r--r--   0        0        0     1908 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
--rw-r--r--   0        0        0     4421 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    15552 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_slurm_config.py
--rw-r--r--   0        0        0     5123 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    44504 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/remote.py
--rw-r--r--   0        0        0      206 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/filenames.py
--rw-r--r--   0        0        0     1254 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/set_start_and_last_task_index.py
--rw-r--r--   0        0        0     3219 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/task_files.py
--rw-r--r--   0        0        0    13608 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/__init__.py
--rw-r--r--   0        0        0    21238 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_common.py
--rw-r--r--   0        0        0     6919 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_local_config.py
--rw-r--r--   0        0        0     1493 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/executor.py
--rw-r--r--   0        0        0    10839 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/__init__.py
--rw-r--r--   0        0        0     2732 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5977 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0     3294 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/common.py
--rw-r--r--   0        0        0     4684 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/handle_failed_job.py
--rw-r--r--   0        0        0    12431 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/__init__.py
--rw-r--r--   0        0        0     6163 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/__init__.py
--rw-r--r--   0        0        0     3630 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_local_config.py
--rw-r--r--   0        0        0     1614 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/executor.py
--rw-r--r--   0        0        0     4395 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/__init__.py
--rw-r--r--   0        0        0     2847 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     6621 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0      571 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/deduplicate_list.py
--rw-r--r--   0        0        0     5149 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/handle_failed_job.py
--rw-r--r--   0        0        0     1281 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/merge_outputs.py
--rw-r--r--   0        0        0    11119 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner.py
--rw-r--r--   0        0        0    10087 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions.py
--rw-r--r--   0        0        0     3845 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions_low_level.py
--rw-r--r--   0        0        0     1376 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/task_interface.py
--rw-r--r--   0        0        0      511 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/v1_compat.py
--rw-r--r--   0        0        0      157 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     2549 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0     1787 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/json_schemas/manifest.json
--rw-r--r--   0        0        0      692 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3113 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     2078 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/__init__.py
--rw-r--r--   0        0        0     4302 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/applyworkflow.py
--rw-r--r--   0        0        0     3444 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dataset.py
--rw-r--r--   0        0        0     1274 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dumps.py
--rw-r--r--   0        0        0     3829 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/manifest.py
--rw-r--r--   0        0        0     1218 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/project.py
--rw-r--r--   0        0        0     3704 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task.py
--rw-r--r--   0        0        0     3057 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task_collection.py
--rw-r--r--   0        0        0     4618 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/workflow.py
--rw-r--r--   0        0        0     1704 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dataset.py
--rw-r--r--   0        0        0     2047 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dumps.py
--rw-r--r--   0        0        0     3250 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/job.py
--rw-r--r--   0        0        0     6243 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/manifest.py
--rw-r--r--   0        0        0      814 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/project.py
--rw-r--r--   0        0        0     3607 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/task.py
--rw-r--r--   0        0        0     2993 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/task_collection.py
--rw-r--r--   0        0        0     1831 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/workflow.py
--rw-r--r--   0        0        0     3903 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/workflowtask.py
--rw-r--r--   0        0        0    11203 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    15080 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/config.py
--rw-r--r--   0        0        0      398 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0       88 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/images/__init__.py
--rw-r--r--   0        0        0     1540 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/images/models.py
--rw-r--r--   0        0        0     2234 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/images/tools.py
--rw-r--r--   0        0        0     3924 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/logger.py
--rw-r--r--   0        0        0     3001 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/README
--rw-r--r--   0        0        0     2630 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     1632 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     2684 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0     8240 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/d71e732236cd_v2.py
--rw-r--r--   0        0        0      963 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/syringe.py
--rw-r--r--   0        0        0       23 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0     5379 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     3278 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     3775 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v1/_TaskCollectPip.py
--rw-r--r--   0        0        0    11725 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v1/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v1/get_collection_data.py
--rw-r--r--   0        0        0     3775 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v2/_TaskCollectPip.py
--rw-r--r--   0        0        0    12803 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v2/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v2/get_collection_data.py
--rw-r--r--   0        0        0     2115 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/utils.py
--rw-r--r--   0        0        0     2948 2024-04-09 08:34:24.924946 fractal_server-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 fractal_server-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/README.md
+-rw-r--r--   0        0        0       24 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1090 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0      413 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-10 10:17:25.445266 fractal_server-2.0.0a4/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     2782 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      400 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0     1483 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      845 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1256 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     2727 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/admin/__init__.py
+-rw-r--r--   0        0        0    13981 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0     9826 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11955 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16911 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5436 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15765 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6123 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8457 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10930 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1210 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14301 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0     9680 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     5956 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5334 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     6024 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     7171 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/submit.py
+-rw-r--r--   0        0        0     7130 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8466 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0    11845 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8414 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0      119 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/components.py
+-rw-r--r--   0        0        0     4159 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    44451 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3219 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13608 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21238 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6926 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/executor.py
+-rw-r--r--   0        0        0    10853 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2738 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-04-10 10:17:25.449266 fractal_server-2.0.0a4/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    12482 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/executor.py
+-rw-r--r--   0        0        0     4409 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2793 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6621 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      571 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5202 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1281 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    11119 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0    10087 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3845 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1376 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      511 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0      157 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     3264 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0      692 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     2078 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3731 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1704 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     2037 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3250 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     6243 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      814 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0     4574 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     3171 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1831 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     5051 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15080 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/config.py
+-rw-r--r--   0        0        0      398 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0       88 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     1969 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/images/models.py
+-rw-r--r--   0        0        0     2234 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     3924 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/logger.py
+-rw-r--r--   0        0        0     3001 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2630 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     1632 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     2684 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     1115 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0     1057 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1849 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0      867 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      949 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0     8240 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/d71e732236cd_v2.py
+-rw-r--r--   0        0        0      963 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/__init__.py
+-rw-r--r--   0        0        0    11725 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-04-10 10:17:25.453266 fractal_server-2.0.0a4/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/tasks/v2/__init__.py
+-rw-r--r--   0        0        0    12803 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0     2115 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/fractal_server/utils.py
+-rw-r--r--   0        0        0     2999 2024-04-10 10:17:25.457266 fractal_server-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 fractal_server-2.0.0a4/PKG-INFO
```

### Comparing `fractal_server-2.0.0a3/LICENSE` & `fractal_server-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/README.md` & `fractal_server-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/__main__.py` & `fractal_server-2.0.0a4/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/alembic.ini` & `fractal_server-2.0.0a4/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/db/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/linkuserproject.py` & `fractal_server-2.0.0a4/fractal_server/app/models/linkuserproject.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/security.py` & `fractal_server-2.0.0a4/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/state.py` & `fractal_server-2.0.0a4/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v1/dataset.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v1/job.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v1/project.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v1/task.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v1/workflow.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v2/dataset.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v2/job.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v2/project.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v2/task.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v2/workflow.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/models/v2/workflowtask.py` & `fractal_server-2.0.0a4/fractal_server/app/models/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/admin/v1.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/admin/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/admin/v2.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/admin/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from fastapi.responses import StreamingResponse
+from pydantic import BaseModel
 from sqlmodel import select
 
 from ....config import get_settings
 from ....syringe import Inject
 from ....utils import get_timestamp
 from ...db import AsyncSession
 from ...db import get_async_db
@@ -275,30 +276,34 @@
     return StreamingResponse(
         iter([byte_stream.getvalue()]),
         media_type="application/x-zip-compressed",
         headers={"Content-Disposition": f"attachment;filename={zip_filename}"},
     )
 
 
+class TaskCompatibility(BaseModel):
+    is_v2_compatible: bool
+
+
 @router_admin_v2.patch(
     "/task-v1/{task_id}/",
     status_code=status.HTTP_200_OK,
 )
 async def flag_task_v1_as_v2_compatible(
     task_id: int,
-    is_v2_compatible: bool,
+    compatibility: TaskCompatibility,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
 ) -> Response:
 
     task = await db.get(Task, task_id)
     if task is None:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"Task {task_id} not found",
         )
 
-    task.is_v2_compatible = is_v2_compatible
+    task.is_v2_compatible = compatibility.is_v2_compatible
     await db.commit()
     await db.close()
 
     return Response(status_code=status.HTTP_200_OK)
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 
 router_api_v2 = APIRouter()
 
 router_api_v2.include_router(dataset_router_v2, tags=["V2 Dataset"])
 router_api_v2.include_router(job_router_v2, tags=["V2 Job"])
 router_api_v2.include_router(images_routes_v2, tags=["V2 Images"])
 router_api_v2.include_router(project_router_v2, tags=["V2 Project"])
-router_api_v2.include_router(submit_job_router_v2, tags=["V2 Submit Job"])
+router_api_v2.include_router(submit_job_router_v2, tags=["V2 Job"])
 router_api_v2.include_router(task_router_v2, prefix="/task", tags=["V2 Task"])
 router_api_v2.include_router(
     task_collection_router_v2, prefix="/task", tags=["V2 Task Collection"]
 )
 router_api_v2.include_router(workflow_router_v2, tags=["V2 Workflow"])
 router_api_v2.include_router(workflowtask_router_v2, tags=["V2 WorkflowTask"])
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/_aux_functions.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/_aux_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     """
     Check that user is a member of project and return the project.
 
     Args:
         project_id:
         user_id:
         db:
-        version:
 
     Returns:
         The project object
 
     Raises:
         HTTPException(status_code=403_FORBIDDEN):
             If the user is not a member of the project
@@ -378,16 +377,16 @@
                 )
     return task
 
 
 def _get_submitted_jobs_statement() -> SelectOfScalar:
     """
     Returns:
-        A sqlmodel statement that selects all `ApplyWorkflow`s with
-        `ApplyWorkflow.status` equal to `submitted`.
+        A sqlmodel statement that selects all `Job`s with
+        `Job.status` equal to `submitted`.
     """
     stm = select(JobV2).where(JobV2.status == JobStatusTypeV1.SUBMITTED)
     return stm
 
 
 async def _workflow_insert_task(
     *,
@@ -402,19 +401,24 @@
     input_filters: Optional[Filters] = None,
     db: AsyncSession,
 ) -> WorkflowTaskV2:
     """
     Insert a new WorkflowTask into Workflow.task_list
 
     Args:
-        task_id: TBD
-        args: TBD
-        meta: TBD
-        order: TBD
-        db: TBD
+        workflow_id:
+        task_id:
+        is_legacy_task:
+        order:
+        meta_parallel:
+        meta_non_parallel:
+        args_non_parallel:
+        args_parallel:
+        input_filters:
+        db:
     """
     db_workflow = await db.get(WorkflowV2, workflow_id)
     if db_workflow is None:
         raise ValueError(f"Workflow {workflow_id} does not exist")
 
     if order is None:
         order = len(db_workflow.task_list)
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/dataset.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/images.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/images.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/job.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/project.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/submit.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                     "among those available to the current user"
                 ),
             )
     else:
         if len(user.slurm_accounts) > 0:
             job_create.slurm_account = user.slurm_accounts[0]
 
-    # Add new ApplyWorkflow object to DB
+    # Add new Job object to DB
     job = JobV2(
         project_id=project_id,
         dataset_id=dataset_id,
         workflow_id=workflow_id,
         user_email=user.email,
         dataset_dump=dict(
             **dataset.model_dump(exclude={"timestamp_created"}),
@@ -188,17 +188,16 @@
         )
         < timedelta(seconds=settings.FRACTAL_API_SUBMIT_RATE_LIMIT)
         for db_job in db_jobs
     ):
         raise HTTPException(
             status_code=status.HTTP_429_TOO_MANY_REQUESTS,
             detail=(
-                f"The endpoint 'POST /api/v2/project/{project_id}/workflow/"
-                f"{workflow_id}/apply/' "
-                "was called several times within an interval of less "
+                f"The endpoint 'POST /api/v2/project/{project_id}/job/submit/'"
+                " was called several times within an interval of less "
                 f"than {settings.FRACTAL_API_SUBMIT_RATE_LIMIT} seconds, using"
                 " the same foreign keys. If it was intentional, please wait "
                 "and try again."
             ),
         )
 
     db.add(job)
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task_collection.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflow.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflowtask.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/api/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/auth.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/aux/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.0a4/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/async_wrap.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/async_wrap.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/exceptions.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_batching.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_check_jobs_status.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_slurm_config.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/executor.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,16 +413,14 @@
             slurm_config:
                 A `SlurmConfig` object; if `None`, use
                 `get_default_slurm_config()`.
             task_files:
                 A `TaskFiles` object; if `None`, use
                 `self.get_default_task_files()`.
 
-        Returns:
-            An iterator of results.
         """
 
         def _result_or_cancel(fut):
             """
             This function is based on the Python Standard Library 3.11.
             Original Copyright 2009 Brian Quinlan. All Rights Reserved.
             Licensed to PSF under a Contributor Agreement.
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/remote.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/set_start_and_last_task_index.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/set_start_and_last_task_index.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/task_files.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/task_files.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_common.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     last_task_index: int,
 ) -> dict[str, Any]:
     """
     Internal processing routine
 
     Schedules the workflow using a `FractalThreadPoolExecutor`.
 
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
+    Cf.
+    [process_workflow][fractal_server.app.runner.v1._local.process_workflow]
     for the call signature.
     """
 
     with FractalThreadPoolExecutor() as executor:
         output_task_pars = execute_tasks(
             executor=executor,
             task_list=workflow.task_list[
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_local_config.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_submit_setup.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/executor.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,16 @@
     """
     Internal processing routine for the SLURM backend
 
     This function initialises the a FractalSlurmExecutor, setting logging,
     workflow working dir and user to impersonate. It then schedules the
     workflow tasks and returns the output dataset metadata.
 
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
+    Cf.
+    [process_workflow][fractal_server.app.runner.v1._local.process_workflow]
 
     Returns:
         output_dataset_metadata: Metadata of the output dataset
     """
 
     if not slurm_user:
         raise RuntimeError(
@@ -128,15 +129,16 @@
     worker_init: Optional[str] = None,
     first_task_index: Optional[int] = None,
     last_task_index: Optional[int] = None,
 ) -> dict[str, Any]:
     """
     Process workflow (SLURM backend public interface)
 
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
+    Cf.
+    [process_workflow][fractal_server.app.runner.v1._local.process_workflow]
     """
 
     # Set values of first_task_index and last_task_index
     num_tasks = len(workflow.task_list)
     first_task_index, last_task_index = set_start_and_last_task_index(
         num_tasks,
         first_task_index=first_task_index,
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/_submit_setup.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/_submit_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 Submodule to define _slurm_submit_setup, which is also the reference
 implementation of `submit_setup_call` in
-[fractal_server.app.runner._common][]).
+[fractal_server.app.runner.v1._common][]).
 """
 from pathlib import Path
 
 from ...task_files import get_task_file_paths
 from .get_slurm_config import get_slurm_config
 from fractal_server.app.models.v1 import WorkflowTask
 
@@ -34,15 +34,15 @@
     Here goes all the logic for reading attributes from the appropriate sources
     and transforming them into an appropriate `SlurmConfig` object (encoding
     SLURM configuration) and `TaskFiles` object (with details e.g. about file
     paths or filename prefixes).
 
     For now, this is the reference implementation for the argument
     `submit_setup_call` of
-    [fractal_server.app.runner._common.execute_tasks][].
+    [fractal_server.app.runner.v1._common.execute_tasks][].
 
     Arguments:
         wftask:
             WorkflowTask for which the configuration is to be assembled
         workflow_dir:
             Server-owned directory to store all task-execution-related relevant
             files (inputs, outputs, errors, and all meta files related to the
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/common.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v1/handle_failed_job.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         # Read dataset attributes produced by the last successful task, and
         # update the DB dataset accordingly
         failed_wftask = db_sync.get(WorkflowTaskV2, e.workflow_task_id)
         dataset.history = assemble_history_failed_job(
             job,
             dataset,
             workflow,
-            logger,
+            logger_name=logger_name,
             failed_wftask=failed_wftask,
         )
         latest_filters = assemble_filters_failed_job(job)
         if latest_filters is not None:
             dataset.filters = latest_filters
         latest_images = assemble_images_failed_job(job)
         if latest_images is not None:
@@ -279,15 +279,15 @@
 
         # Read dataset attributes produced by the last successful task, and
         # update the DB dataset accordingly
         dataset.history = assemble_history_failed_job(
             job,
             dataset,
             workflow,
-            logger,
+            logger_name=logger_name,
         )
         latest_filters = assemble_filters_failed_job(job)
         if latest_filters is not None:
             dataset.filters = latest_filters
         latest_images = assemble_images_failed_job(job)
         if latest_images is not None:
             dataset.images = latest_images
@@ -309,15 +309,15 @@
 
         # Read dataset attributes produced by the last successful task, and
         # update the DB dataset accordingly
         dataset.history = assemble_history_failed_job(
             job,
             dataset,
             workflow,
-            logger,
+            logger_name=logger_name,
         )
         latest_filters = assemble_filters_failed_job(job)
         if latest_filters is not None:
             dataset.filters = latest_filters
         latest_images = assemble_images_failed_job(job)
         if latest_images is not None:
             dataset.images = latest_images
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     last_task_index: int,
 ) -> dict:
     """
     Internal processing routine
 
     Schedules the workflow using a `FractalThreadPoolExecutor`.
 
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
+    Cf.
+    [process_workflow][fractal_server.app.runner.v2._local.process_workflow]
     for the call signature.
     """
 
     with FractalThreadPoolExecutor() as executor:
         new_dataset_attributes = execute_tasks_v2(
             wf_task_list=workflow.task_list[
                 first_task_index : (last_task_index + 1)  # noqa
@@ -87,29 +88,29 @@
 
     NOTE: This is the `local` backend's public interface, which also works as
     a reference implementation for other backends.
 
     Args:
         workflow:
             The workflow to be run
-        input_paths:
-            The paths to the input files to pass to the first task of the
-            workflow
-        output_path:
-            The destination path for the last task of the workflow
-        input_metadata:
-            Initial metadata, passed to the first task
-        logger_name:
-            Name of the logger to log information on the run to
+        dataset:
+            Initial dataset.
         workflow_dir:
             Working directory for this run.
         workflow_dir_user:
             Working directory for this run, on the user side. This argument is
             present for compatibility with the standard backend interface, but
             for the `local` backend it cannot be different from `workflow_dir`.
+        first_task_index:
+            Positional index of the first task to execute; if `None`, start
+            from `0`.
+        last_task_index:
+            Positional index of the last task to execute; if `None`, proceed
+            until the last task.
+        logger_name: Logger name
         slurm_user:
             Username to impersonate to run the workflow. This argument is
             present for compatibility with the standard backend interface, but
             is ignored in the `local` backend.
         slurm_account:
             SLURM account to use when running the workflow. This argument is
             present for compatibility with the standard backend interface, but
@@ -119,20 +120,14 @@
             argument is present for compatibility with the standard backend
             interface, but is ignored in the `local` backend.
         worker_init:
             Any additional, usually backend specific, information to be passed
             to the backend executor. This argument is present for compatibility
             with the standard backend interface, but is ignored in the `local`
             backend.
-        first_task_index:
-            Positional index of the first task to execute; if `None`, start
-            from `0`.
-        last_task_index:
-            Positional index of the last task to execute; if `None`, proceed
-            until the last task.
 
     Raises:
         TaskExecutionError: wrapper for errors raised during tasks' execution
                             (positive exit codes).
         JobExecutionError: wrapper for errors raised by the tasks' executors
                            (negative exit codes).
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_local_config.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_submit_setup.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/executor.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     """
     Internal processing routine for the SLURM backend
 
     This function initialises the a FractalSlurmExecutor, setting logging,
     workflow working dir and user to impersonate. It then schedules the
     workflow tasks and returns the new dataset attributes
 
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
+    Cf.
+    [process_workflow][fractal_server.app.runner.v2._local.process_workflow]
 
     Returns:
         new_dataset_attributes:
     """
 
     if not slurm_user:
         raise RuntimeError(
@@ -108,15 +109,16 @@
     slurm_user: Optional[str] = None,
     slurm_account: Optional[str] = None,
     worker_init: Optional[str] = None,
 ) -> dict:
     """
     Process workflow (SLURM backend public interface)
 
-    Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
+    Cf.
+    [process_workflow][fractal_server.app.runner.v2._local.process_workflow]
     """
 
     # Set values of first_task_index and last_task_index
     num_tasks = len(workflow.task_list)
     first_task_index, last_task_index = set_start_and_last_task_index(
         num_tasks,
         first_task_index=first_task_index,
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/_submit_setup.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 Submodule to define _slurm_submit_setup, which is also the reference
-implementation of `submit_setup_call` in
-[fractal_server.app.runner._common][]).
+implementation of `submit_setup_call`.
 """
 from pathlib import Path
 from typing import Literal
 
 from ...task_files import get_task_file_paths
 from .get_slurm_config import get_slurm_config
 from fractal_server.app.models.v2 import WorkflowTaskV2
@@ -36,15 +35,15 @@
     Here goes all the logic for reading attributes from the appropriate sources
     and transforming them into an appropriate `SlurmConfig` object (encoding
     SLURM configuration) and `TaskFiles` object (with details e.g. about file
     paths or filename prefixes).
 
     For now, this is the reference implementation for the argument
     `submit_setup_call` of
-    [fractal_server.app.runner._common.execute_tasks][].
+    [fractal_server.app.runner.v2.runner][].
 
     Arguments:
         wftask:
             WorkflowTask for which the configuration is to be assembled
         workflow_dir:
             Server-owned directory to store all task-execution-related relevant
             files (inputs, outputs, errors, and all meta files related to the
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/deduplicate_list.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/deduplicate_list.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/handle_failed_job.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/handle_failed_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,38 +28,40 @@
 from ..filenames import IMAGES_FILENAME
 
 
 def assemble_history_failed_job(
     job: JobV2,
     dataset: DatasetV2,
     workflow: WorkflowV2,
-    logger: logging.Logger,
+    logger_name: Optional[str] = None,
     failed_wftask: Optional[WorkflowTaskV2] = None,
 ) -> list[dict[str, Any]]:
     """
     Assemble `history` after a workflow-execution job fails.
 
     Args:
         job:
-            The failed `ApplyWorkflow` object.
-        output_dataset:
-            The `dataset` associated to `job`.
+            The failed `JobV2` object.
+        dataset:
+            The `DatasetV2` object associated to `job`.
         workflow:
-            The `workflow` associated to `job`.
-        logger: A logger instance.
+            The `WorkflowV2` object associated to `job`.
+        logger_name: A logger name.
         failed_wftask:
             If set, append it to `history` during step 3; if `None`, infer
             it by comparing the job task list and the one in
             `HISTORY_FILENAME`.
 
     Returns:
         The new value of `history`, to be merged into
-        `output_dataset.meta`.
+        `dataset.meta`.
     """
 
+    logger = logging.getLogger(logger_name)
+
     # The final value of the history attribute should include up to three
     # parts, coming from: the database, the temporary file, the failed-task
     # information.
 
     # Part 1: Read exising history from DB
     new_history = dataset.history
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/merge_outputs.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions_low_level.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/runner_functions_low_level.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/runner/v2/task_interface.py` & `fractal_server-2.0.0a4/fractal_server/app/runner/v2/task_interface.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from datetime import datetime
 from datetime import timezone
+from typing import Any
 
 
 def valstr(attribute: str, accept_none: bool = False):
     """
     Check that a string attribute is not an empty string, and remove the
     leading and trailing whitespace characters.
 
@@ -23,14 +24,35 @@
         if not s:
             raise ValueError(f"String attribute '{attribute}' cannot be empty")
         return s
 
     return val
 
 
+def valdictkeys(attribute: str):
+    def val(d: dict[str, Any]):
+        """
+        Apply valstr to every key of the dictionary, and fail if there are
+        identical keys.
+        """
+        if d is not None:
+            old_keys = list(d.keys())
+            new_keys = [valstr(f"{attribute}[{key}]")(key) for key in old_keys]
+            if len(new_keys) != len(set(new_keys)):
+                raise ValueError(
+                    f"Dictionary contains multiple identical keys: {d}."
+                )
+            for old_key, new_key in zip(old_keys, new_keys):
+                if new_key != old_key:
+                    d[new_key] = d.pop(old_key)
+        return d
+
+    return val
+
+
 def valint(attribute: str, min_val: int = 1):
     """
     Check that an integer attribute (e.g. if it is meant to be the ID of a
     database entry) is greater or equal to min_val.
     """
 
     def val(integer: int):
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/state.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/user.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/applyworkflow.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dataset.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dumps.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/manifest.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/project.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
     meta: Optional[dict[str, Any]] = Field(default={})
     owner: Optional[str]
     version: Optional[str]
     args_schema: Optional[dict[str, Any]]
     args_schema_version: Optional[str]
     docs_info: Optional[str]
     docs_link: Optional[HttpUrl]
+    is_v2_compatible: bool
 
 
 class TaskCreateV1(_TaskBaseV1):
     """
     Class for `Task` creation.
 
     Attributes:
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task_collection.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/workflow.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dataset.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dumps.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/dumps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 
 Dump models differ from their Read counterpart in that:
 * They are directly JSON-able, without any additional encoder.
 * They may only include a subset of the Read attributes.
 
 These models are used in at least two situations:
-1. In the "*_dump" attributes of ApplyWorkflow models;
+1. In the "*_dump" attributes of Job models;
 2. In the `_DatasetHistoryItem.workflowtask` model, to trim its size.
 """
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic import root_validator
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/job.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/manifest.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/project.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/task_collection.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/task_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Literal
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
+from .._validators import valdictkeys
 from .._validators import valstr
 from .task import TaskReadV2
 
 
 class TaskCollectPipV2(BaseModel):
     """
     TaskCollectPipV2 class
@@ -39,14 +40,17 @@
 
     package: str
     package_version: Optional[str] = None
     package_extras: Optional[str] = None
     python_version: Optional[str] = None
     pinned_package_versions: Optional[dict[str, str]] = None
 
+    _pinned_package_versions = validator(
+        "pinned_package_versions", allow_reuse=True
+    )(valdictkeys("pinned_package_versions"))
     _package_extras = validator("package_extras", allow_reuse=True)(
         valstr("package_extras")
     )
     _python_version = validator("python_version", allow_reuse=True)(
         valstr("python_version")
     )
```

### Comparing `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/workflow.py` & `fractal_server-2.0.0a4/fractal_server/app/schemas/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/app/security/__init__.py` & `fractal_server-2.0.0a4/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/config.py` & `fractal_server-2.0.0a4/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/images/models.py` & `fractal_server-2.0.0a4/fractal_server/images/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
+from fractal_server.app.schemas._validators import valdictkeys
+
 
 class SingleImage(BaseModel):
 
     zarr_url: str
     origin: Optional[str] = None
 
     attributes: dict[str, Any] = Field(default_factory=dict)
     types: dict[str, bool] = Field(default_factory=dict)
 
+    # Validators
+    _attributes = validator("attributes", allow_reuse=True)(
+        valdictkeys("attributes")
+    )
+    _types = validator("types", allow_reuse=True)(valdictkeys("types"))
+
     @validator("attributes")
     def validate_attributes(
         cls, v: dict[str, Any]
     ) -> dict[str, Union[int, float, str, bool]]:
         for key, value in v.items():
             if not isinstance(value, (int, float, str, bool)):
                 raise ValueError(
@@ -32,14 +40,19 @@
     attributes: dict[str, Any] = Field(default_factory=dict)
     types: dict[str, bool] = Field(default_factory=dict)
 
     class Config:
         extra = "forbid"
 
     # Validators
+    _attributes = validator("attributes", allow_reuse=True)(
+        valdictkeys("attributes")
+    )
+    _types = validator("types", allow_reuse=True)(valdictkeys("types"))
+
     @validator("attributes")
     def validate_attributes(
         cls, v: dict[str, Any]
     ) -> dict[str, Union[int, float, str, bool, None]]:
         for key, value in v.items():
             if not isinstance(value, (int, float, str, bool, type(None))):
                 raise ValueError(
```

### Comparing `fractal_server-2.0.0a3/fractal_server/images/tools.py` & `fractal_server-2.0.0a4/fractal_server/images/tools.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/logger.py` & `fractal_server-2.0.0a4/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/main.py` & `fractal_server-2.0.0a4/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/env.py` & `fractal_server-2.0.0a4/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.0a4/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/d71e732236cd_v2.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/d71e732236cd_v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.0a4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/syringe.py` & `fractal_server-2.0.0a4/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.0a4/fractal_server/tasks/endpoint_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/tasks/utils.py` & `fractal_server-2.0.0a4/fractal_server/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/tasks/v1/_TaskCollectPip.py` & `fractal_server-2.0.0a4/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/tasks/v1/background_operations.py` & `fractal_server-2.0.0a4/fractal_server/tasks/v1/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/tasks/v2/_TaskCollectPip.py` & `fractal_server-2.0.0a4/fractal_server/tasks/v2/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/tasks/v2/background_operations.py` & `fractal_server-2.0.0a4/fractal_server/tasks/v2/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/fractal_server/utils.py` & `fractal_server-2.0.0a4/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a3/pyproject.toml` & `fractal_server-2.0.0a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 [tool.poetry]
 name = "fractal-server"
-version = "2.0.0a3"
+version = "2.0.0a4"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
 homepage = "https://github.com/fractal-analytics-platform/fractal-server"
 repository = "https://github.com/fractal-analytics-platform/fractal-server"
 documentation = "https://fractal-analytics-platform.github.io/fractal-server"
 license = "BSD-3-Clause"
 exclude = [
 "fractal_server/.gitignore",
 "fractal_server/data_migrations/old",
+"fractal_server/json_schemas",
 ]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/fractal-analytics-platform/fractal-server/blob/main/CHANGELOG.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-python-dotenv = "^0.21.0"
-fastapi = "^0.109.0"
-sqlmodel = "^0.0.14"
+python-dotenv = "^1.0.0"
+fastapi = "^0.110.0"
+sqlmodel = "^0.0.16"
 sqlalchemy = {extras = ["asyncio"], version = ">=2.0.23,<2.1"}
 aiosqlite = "^0.19.0"
 fastapi-users = {extras = ["oauth"], version = "^12.1.0"}
-alembic = "^1.9.1"
-uvicorn = "^0.27.0"
+alembic = "^1.13.1"
+uvicorn = "^0.29.0"
 pydantic = ">=1.10.8,<2"
 bcrypt = "4.0.1"
 packaging = "^23.2"
 clusterfutures = "^0.5"
-cloudpickle = ">=2.2.1,<2.3.0"
+cloudpickle = ">=3.0.0,<3.1.0"
 
 asyncpg = { version = "^0.29.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
 gunicorn = { version = "^21.2.0", optional = true }
 
 [tool.poetry.extras]
 postgres = ["asyncpg", "psycopg2"]
@@ -50,29 +51,30 @@
 pytest = "^7.2"
 httpx = "^0.23"
 devtools = "^0.12"
 pytest-asyncio = "^0.21"
 bumpver = "^2022.1120"
 pre-commit = "^2.19"
 coverage = {extras = ["toml"], version = "^6.4.4"}
-mypy = "^0.982"
-pytest-subprocess = "^1.4"
 pytest-docker = {version = "^2.0"}
+mypy = "^1.9"
+pytest-subprocess = "^1.4"
 pyyaml="^6.0.1"
 a2wsgi = "^1.10.0"
 jinja2 = "^3.1.3"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.5.2"
-mkdocstrings = { extras = ["python"], version = "0.22.0" }
-mkdocs-material = "9.1.21"
-mkdocs-gen-files = "0.4.0"
-mkdocs-literate-nav = "0.5.0"
-mkdocs-section-index = "0.3.5"
-mkdocs-render-swagger-plugin = "0.1.0"
+
+mkdocs="1.5.3"
+mkdocstrings = { extras = ["python"], version = "0.24.3" }
+mkdocs-material="9.5.17"
+mkdocs-gen-files="0.5.0"
+mkdocs-literate-nav="0.6.1"
+mkdocs-section-index="0.3.8"
+mkdocs-render-swagger-plugin="0.1.1"
 pyyaml="^6.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -80,15 +82,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "2.0.0a3"
+current_version = "2.0.0a4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
@@ -102,12 +104,12 @@
 [tool.poetry.scripts]
 fractalctl = "fractal_server.__main__:run"
 
 [tool.coverage.run]
 branch = true
 parallel = true
 relative_files = true
-omit = ["tests/*", "benchmarks/*"]
+omit = ["tests/*", "benchmarks/*", "fractal_server/json_schemas/*"]
 
 [[tool.mypy.overrides]]
 module = ["devtools", "uvicorn", "pytest", "asgi_lifespan", "asyncpg"]
 ignore_missing_imports = true
```

### Comparing `fractal_server-2.0.0a3/PKG-INFO` & `fractal_server-2.0.0a4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -12,29 +12,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: gunicorn
 Provides-Extra: postgres
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
-Requires-Dist: alembic (>=1.9.1,<2.0.0)
+Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "postgres"
 Requires-Dist: bcrypt (==4.0.1)
-Requires-Dist: cloudpickle (>=2.2.1,<2.3.0)
+Requires-Dist: cloudpickle (>=3.0.0,<3.1.0)
 Requires-Dist: clusterfutures (>=0.5,<0.6)
-Requires-Dist: fastapi (>=0.109.0,<0.110.0)
+Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: fastapi-users[oauth] (>=12.1.0,<13.0.0)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0) ; extra == "gunicorn"
 Requires-Dist: packaging (>=23.2,<24.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
 Requires-Dist: pydantic (>=1.10.8,<2)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.23,<2.1)
-Requires-Dist: sqlmodel (>=0.0.14,<0.0.15)
-Requires-Dist: uvicorn (>=0.27.0,<0.28.0)
+Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Project-URL: Changelog, https://github.com/fractal-analytics-platform/fractal-server/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://fractal-analytics-platform.github.io/fractal-server
 Project-URL: Repository, https://github.com/fractal-analytics-platform/fractal-server
 Description-Content-Type: text/markdown
 
 # Fractal Server
```

