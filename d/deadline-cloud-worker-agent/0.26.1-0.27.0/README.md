# Comparing `tmp/deadline_cloud_worker_agent-0.26.1.tar.gz` & `tmp/deadline_cloud_worker_agent-0.27.0.tar.gz`

## Comparing `deadline_cloud_worker_agent-0.26.1.tar` & `deadline_cloud_worker_agent-0.27.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/_version.py
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/hatch_version_hook.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/__main__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/_version.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/api_models.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/errors.py
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/file_system_operations.py
--rw-r--r--   0        0        0    19180 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_messages.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/metrics.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/progress.py
--rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/session_events.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/utils.py
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/worker.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws/__init__.py
--rw-r--r--   0        0        0    36140 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws/deadline/__init__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/__init__.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/aws_configs.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/boto3_sessions.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/credentials_refresher.py
--rw-r--r--   0        0        0    23258 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/temporary_credentials.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/__init__.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/config.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/logger.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/retries.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/shim.py
--rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/__init__.py
--rwxr-xr-x   0        0        0    18766 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/install.sh
--rw-r--r--   0        0        0    38437 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/win_installer.py
--rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/worker.toml.example
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/__init__.py
--rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/cloudwatch.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/loggers.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/log.py
--rw-r--r--   0        0        0    61170 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/scheduler.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_action_status.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_cleanup.py
--rw-r--r--   0        0        0    19215 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_queue.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/active_action.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/errors.py
--rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/log_config.py
--rw-r--r--   0        0        0    53599 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/session.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/__init__.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/action_definition.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/enter_env.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/exit_env.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/openjd_action.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/run_step_task.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/__init__.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/environment_details.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py
--rw-r--r--   0        0        0    17689 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_details.py
--rw-r--r--   0        0        0    15220 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_entities.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_entity_type.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/step_details.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/validation.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/__init__.py
--rw-r--r--   0        0        0    20997 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/bootstrap.py
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/capabilities.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/cli_args.py
--rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config_file.py
--rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/entrypoint.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/host_properties.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/settings.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/__init__.py
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_credentials_resolver.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_service.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/NOTICE
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/README.md
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/hatch.toml
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/pyproject.toml
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/_version.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/hatch_version_hook.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/_version.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/api_models.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/errors.py
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/file_system_operations.py
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_messages.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/metrics.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/progress.py
+-rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/session_events.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/utils.py
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/worker.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws/__init__.py
+-rw-r--r--   0        0        0    36140 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws/deadline/__init__.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/__init__.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/aws_configs.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/boto3_sessions.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/credentials_refresher.py
+-rw-r--r--   0        0        0    23258 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/temporary_credentials.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/__init__.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/config.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/logger.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/retries.py
+-rw-r--r--   0        0        0    18821 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/shim.py
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/__init__.py
+-rwxr-xr-x   0        0        0    18766 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/install.sh
+-rw-r--r--   0        0        0    38437 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/win_installer.py
+-rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/worker.toml.example
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/__init__.py
+-rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/cloudwatch.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/loggers.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/log.py
+-rw-r--r--   0        0        0    64684 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/scheduler.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_action_status.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_cleanup.py
+-rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_queue.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/active_action.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/errors.py
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/log_config.py
+-rw-r--r--   0        0        0    54231 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/session.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/action_definition.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/enter_env.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/exit_env.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/openjd_action.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/run_step_task.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/__init__.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/environment_details.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py
+-rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_details.py
+-rw-r--r--   0        0        0    15220 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_entities.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_entity_type.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/step_details.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/validation.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/__init__.py
+-rw-r--r--   0        0        0    20997 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/bootstrap.py
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/capabilities.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/cli_args.py
+-rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config_file.py
+-rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/entrypoint.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/host_properties.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/settings.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/__init__.py
+-rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_credentials_resolver.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_service.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/NOTICE
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/README.md
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/hatch.toml
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/pyproject.toml
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/PKG-INFO
```

### Comparing `deadline_cloud_worker_agent-0.26.1/hatch_version_hook.py` & `deadline_cloud_worker_agent-0.27.0/hatch_version_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/api_models.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/api_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,22 +249,22 @@
     passwordArn: str
     """The ARN of a AWS Secrets Manager secret that the password of the user name to run actions as"""
 
 
 class JobRunAsUser(TypedDict):
     posix: NotRequired[PosixUser]
     windows: NotRequired[WindowsUser]
-    runAs: NotRequired[Literal["QUEUE_CONFIGURED_USER", "WORKER_AGENT_USER"]]
+    runAs: Literal["QUEUE_CONFIGURED_USER", "WORKER_AGENT_USER"]
 
 
 class JobDetailsData(JobDetailsIdentifierFields):
     jobAttachmentSettings: NotRequired[JobAttachmentQueueSettings]
     """The queue's job attachment settings"""
 
-    jobRunAsUser: JobRunAsUser
+    jobRunAsUser: NotRequired[JobRunAsUser]
     """The queue's info on how to run the job processes (ie. posix or windows user/group)"""
 
     logGroupName: str
     """The name of the CloudWatch Log Group containing the Worker session's Log Stream"""
 
     schemaVersion: str
     """The Open Job Description job template schema version"""
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/file_system_operations.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/file_system_operations.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_messages.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,33 +462,38 @@
 
 
 class SessionActionLogKind(str, Enum):
     ENV_ENTER = "EnvEnter"
     ENV_EXIT = "EnvExit"
     TASK_RUN = "TaskRun"
     JA_SYNC = "JobAttachSyncInput"
+    JA_DEP_SYNC = "JobAttachSyncDeps"
 
 
 class SessionActionLogEvent(BaseLogEvent):
     type = "Action"
 
     queue_id: str
     job_id: str
+    step_id: Optional[str]
+    task_id: Optional[str]
     session_id: str
     kind: SessionActionLogKind
     action_id: str
     status: Optional[str]
     msg: str
 
     def __init__(
         self,
         *,
         subtype: SessionActionLogEventSubtype,
         queue_id: str,
         job_id: str,
+        step_id: Optional[str] = None,
+        task_id: Optional[str] = None,
         session_id: str,
         action_log_kind: SessionActionLogKind,
         action_id: str,
         message: str,
         status: Optional[str] = None,
     ) -> None:
         if subtype in (SessionActionLogEventSubtype.START,):
@@ -501,39 +506,52 @@
         else:
             self.ti = "🟣"
         self.subtype = subtype.value
         self.session_id = session_id
         self.kind = action_log_kind
         self.queue_id = queue_id
         self.job_id = job_id
+        self.step_id = step_id
+        self.task_id = task_id
         self.action_id = action_id
         self.msg = message
         self.status = status
 
     def getMessage(self) -> str:
         dd = self.asdict()
-        # TODO - Rearrange. Put (%(queue_id)s/%(job_id)s) after the message
+        if self.step_id is None:
+            resource_id = "[%(queue_id)s/%(job_id)s]"
+        elif self.task_id is None:
+            resource_id = "[%(queue_id)s/%(job_id)s/%(step_id)s]"
+        else:
+            resource_id = "[%(queue_id)s/%(job_id)s/%(step_id)s/%(task_id)s]"
         if self.subtype == SessionActionLogEventSubtype.END.value and self.status is not None:
-            fmt_str = "[%(session_id)s](%(action_id)s) %(message)s (Status: %(status)s) (Kind: %(kind)s) [%(queue_id)s/%(job_id)s]"
+            fmt_str = (
+                "[%(session_id)s](%(action_id)s) %(message)s (Status: %(status)s) (Kind: %(kind)s) "
+                + resource_id
+            )
         else:
-            fmt_str = "[%(session_id)s](%(action_id)s) %(message)s (Kind: %(kind)s) [%(queue_id)s/%(job_id)s]"
+            fmt_str = "[%(session_id)s](%(action_id)s) %(message)s (Kind: %(kind)s) " + resource_id
         return self.add_exception_to_message(fmt_str % dd)
 
     def asdict(self) -> dict[str, Any]:
         dd = super().asdict()
-        # TODO - Rearrange. Put (%(queue_id)s/%(job_id)s) after the message
         dd.update(
             session_id=self.session_id,
             action_id=self.action_id,
             kind=self.kind.value,
             message=self.msg,
         )
         if self.subtype == SessionActionLogEventSubtype.END.value and self.status is not None:
             dd.update(status=self.status)
         dd.update(queue_id=self.queue_id, job_id=self.job_id)
+        if self.step_id is not None:
+            dd.update(step_id=self.step_id)
+        if self.task_id is not None:
+            dd.update(task_id=self.task_id)
         return self.add_exception_to_dict(dd)
 
 
 # ===========================
 
 
 class LogRecordStringTranslationFilter(logging.Filter):
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/metrics.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/metrics.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/progress.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/progress.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/session_events.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/session_events.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/utils.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/worker.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/worker.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws/deadline/__init__.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws/deadline/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/aws_configs.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/aws_configs.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/boto3_sessions.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/boto3_sessions.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/credentials_refresher.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/credentials_refresher.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/temporary_credentials.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/temporary_credentials.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/config.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/retries.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/retries.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/shim.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/shim.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,15 @@
                             "schemaVersion": "jobtemplate-2023-09",
                             "jobAttachmentSettings": {
                                 "s3BucketName": "asset-bucket",
                                 "rootPrefix": "my-queue",
                             },
                             "logGroupName": "/aws/deadline/queue-abc",
                             "jobRunAsUser": {
+                                "runAs": "QUEUE_CONFIGURED_USER",
                                 "posix": {
                                     "user": "job-user",
                                     "group": "job-group",
                                 },
                                 "windows": {
                                     "user": "job-user",
                                     "group": "job-group",
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/__init__.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/install.sh` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/install.sh`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/win_installer.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/win_installer.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/worker.toml.example` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/worker.toml.example`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/cloudwatch.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/scheduler.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from ..sessions import JobEntities, Session
 from ..sessions.actions import SessionActionDefinition
 from ..sessions.log_config import (
     LogConfiguration,
     LogProvisioningError,
     SessionLogConfigurationParameters,
 )
+from ..sessions.job_entities.job_details import JobRunAsUser
 from ..api_models import (
     AssignedSession,
     UpdateWorkerScheduleResponse,
     UpdatedSessionActionInfo,
     WorkerStatus,
     EnvironmentAction,
     TaskRunAction,
@@ -664,14 +665,106 @@
                     ),
                 )
                 for action in actions
             }
         )
         self._wakeup.set()
 
+    @staticmethod
+    def _determine_user_for_session(
+        *,
+        host_is_posix: bool,
+        job_run_as_user: Optional[JobRunAsUser],
+        job_run_as_user_override: JobsRunAsUserOverride,
+        queue_id: str,
+        job_id: str,
+        session_id: str,
+    ) -> Optional[SessionUser]:
+        # Called only in self._create_new_sessions() to determine what os_user the Session should
+        # run as.
+        # Raises a ValueError if an impossible situation arises and we need to fail the Session.
+        os_user: Optional[SessionUser] = None
+        if not job_run_as_user_override.run_as_agent:
+            if job_run_as_user_override.job_user is not None:
+                os_user = job_run_as_user_override.job_user
+                logger.info(
+                    SessionLogEvent(
+                        subtype=SessionLogEventSubtype.USER,
+                        queue_id=queue_id,
+                        job_id=job_id,
+                        session_id=session_id,
+                        user=os_user.user,
+                        message="Running as host-configured override user.",
+                    )
+                )
+            elif job_run_as_user is None:
+                # Terminal error. We need to fail the Session.
+                # This should *never* happen; it occuring would mean that a service invariant has
+                # been violated.
+                message = (
+                    "FATAL: Queue does not have a jobRunAsUser. This should not be possible. "
+                    "Please report this to the service team."
+                )
+                raise ValueError(message)
+            elif not job_run_as_user.is_worker_agent_user:
+                # If we do not have a job-user override & we're not explicitly running
+                # as the agent's user, then we *MUST* have a jobRunAsUser from the JobDetails.
+                # Reasons:
+                #  1) The service always allows service-managed Fleets to associate with
+                #     a Queue. The SMF Worker Agent is *always* run with a local user override.
+                #  2) The service only allows a customer-managed Fleet to associate with a
+                #     Queue if either:
+                #       a) The jobRunAsUser is explicitly set to WORKER_AGENT_USER; or
+                #       b) The jobRunAsUser is explicitly set to QUEUE_CONFIGURED_USER and
+                #          a user has been defined for the CMF's OS Platform (Linux/MacOS Fleets must
+                #          have a "posix" user; and Windows Fleets must have a "windows" user)
+                #  3) The service does not allow a Queue's jobRunAsUser to be updated if the constraint
+                #     imposed by (2) above would be violated for one or more of that Queue's current QFAs.
+                if host_is_posix:
+                    os_user = job_run_as_user.posix
+                else:
+                    os_user = job_run_as_user.windows
+                if os_user is None:
+                    # Terminal error. We need to fail the Session.
+                    # This should *never* happen; it occuring would mean that a service invariant has
+                    # been violated.
+                    message = (
+                        "FATAL: Queue's jobRunAsUser does not define a QUEUE_CONFIGURED_USER for this platform. "
+                        "Please report this to the service team."
+                    )
+                    raise ValueError(message)
+                else:
+                    logger.info(
+                        SessionLogEvent(
+                            subtype=SessionLogEventSubtype.USER,
+                            queue_id=queue_id,
+                            job_id=job_id,
+                            session_id=session_id,
+                            user=os_user.user,
+                            message="Running as Queue's jobRunAsUser.",
+                        )
+                    )
+        if os_user is None:
+            try:
+                user_to_log = getpass.getuser()
+            except Exception:
+                # This is best-effort. If we cannot determine the user we will not log
+                user_to_log = "UNKNOWN"
+            logger.warning(
+                SessionLogEvent(
+                    subtype=SessionLogEventSubtype.USER,
+                    queue_id=queue_id,
+                    job_id=job_id,
+                    session_id=session_id,
+                    user=user_to_log,
+                    message="Running as the Worker Agent's user. This configuration is not recommended; please see the Security chapter of the User Guide.",
+                )
+            )
+        return os_user
+
     def _create_new_sessions(
         self,
         *,
         assigned_sessions: dict[str, AssignedSession],
     ) -> set[str]:
         new_session_ids = assigned_sessions.keys() - self._sessions.keys()
 
@@ -838,60 +931,36 @@
                 job_entities=job_entities,
                 action_update_callback=self._handle_session_action_update,
             )
 
             queue.replace(actions=session_spec["sessionActions"])
 
             os_user: Optional[SessionUser] = None
-            if not self._job_run_as_user_override.run_as_agent:
-                if self._job_run_as_user_override.job_user is not None:
-                    os_user = self._job_run_as_user_override.job_user
-                    logger.info(
-                        SessionLogEvent(
-                            subtype=SessionLogEventSubtype.USER,
-                            queue_id=queue_id,
-                            job_id=job_id,
-                            session_id=new_session_id,
-                            user=os_user.user,
-                            message="Running as host-configured override user.",
-                        )
-                    )
-                elif job_details.job_run_as_user:
-                    if os.name == "posix":
-                        os_user = job_details.job_run_as_user.posix
-                    else:
-                        os_user = job_details.job_run_as_user.windows
-                    if os_user is not None:
-                        logger.info(
-                            SessionLogEvent(
-                                subtype=SessionLogEventSubtype.USER,
-                                queue_id=queue_id,
-                                job_id=job_id,
-                                session_id=new_session_id,
-                                user=os_user.user,
-                                message="Running as Queue's jobRunAsUser.",
-                            )
-                        )
-
-            if os_user is None:
-                try:
-                    user_to_log = getpass.getuser()
-                except Exception:
-                    # This is best-effort. If we cannot determine the user we will not log
-                    user_to_log = "UNKNOWN"
-                logger.warning(
+            try:
+                os_user = self._determine_user_for_session(
+                    host_is_posix=os.name == "posix",
+                    job_run_as_user=job_details.job_run_as_user,
+                    job_run_as_user_override=self._job_run_as_user_override,
+                    queue_id=queue_id,
+                    job_id=job_id,
+                    session_id=new_session_id,
+                )
+            except ValueError as e:
+                message = str(e)
+                self._fail_all_actions(session_spec, message)
+                logger.error(
                     SessionLogEvent(
                         subtype=SessionLogEventSubtype.USER,
                         queue_id=queue_id,
                         job_id=job_id,
                         session_id=new_session_id,
-                        user=user_to_log,
-                        message="Running as the Worker Agent's user.",
+                        message=message,
                     )
                 )
+                continue
 
             queue_credentials: QueueAwsCredentials | None = None
             asset_sync: AssetSync | None = None
             if job_details.queue_role_arn:
                 try:
                     queue_credentials = self._get_queue_aws_credentials(
                         queue_id,
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_action_status.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_action_status.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_cleanup.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_cleanup.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_queue.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -407,30 +407,40 @@
                     )
                 else:
                     raise ValueError(f'Unknown action type "{action_type}".')
             elif action_type == "TASK_RUN":
                 action_queue_entry = cast(TaskRunQueueEntry, action_queue_entry)
                 action_definition = action_queue_entry.definition
                 step_id = action_definition["stepId"]
+                task_id = action_definition["taskId"]
                 try:
                     step_details = self._job_entities.step_details(step_id=step_id)
                 except UnsupportedSchema as e:
                     raise JobEntityUnsupportedSchemaError(
-                        action_id, SessionActionLogKind.TASK_RUN, e._version
+                        action_id,
+                        SessionActionLogKind.TASK_RUN,
+                        e._version,
+                        step_id=step_id,
+                        task_id=task_id,
                     ) from e
                 except (ValueError, RuntimeError) as e:
-                    raise StepDetailsError(action_id, SessionActionLogKind.TASK_RUN, str(e)) from e
+                    raise StepDetailsError(
+                        action_id,
+                        SessionActionLogKind.TASK_RUN,
+                        str(e),
+                        step_id=step_id,
+                        task_id=task_id,
+                    ) from e
                 task_parameters_data: dict = action_definition.get("parameters", {})
                 task_parameters = parameters_from_api_response(task_parameters_data)
 
                 next_action = RunStepTaskAction(
                     id=action_id,
                     details=step_details,
                     task_parameter_values=task_parameters,
-                    step_id=step_id,
                     task_id=action_definition["taskId"],
                 )
             elif action_type == "SYNC_INPUT_JOB_ATTACHMENTS":
                 action_definition = action_queue_entry.definition
                 action_definition = cast(SyncInputJobAttachmentsActionApiModel, action_definition)
                 if "stepId" not in action_definition:
                     action_queue_entry = cast(SyncInputJobAttachmentsQueueEntry, action_queue_entry)
@@ -456,19 +466,25 @@
 
                     try:
                         step_details = self._job_entities.step_details(
                             step_id=action_definition["stepId"],
                         )
                     except UnsupportedSchema as e:
                         raise JobEntityUnsupportedSchemaError(
-                            action_id, SessionActionLogKind.JA_SYNC, e._version
+                            action_id,
+                            SessionActionLogKind.JA_DEP_SYNC,
+                            e._version,
+                            step_id=action_definition["stepId"],
                         ) from e
                     except ValueError as e:
                         raise StepDetailsError(
-                            action_id, SessionActionLogKind.JA_SYNC, str(e)
+                            action_id,
+                            SessionActionLogKind.JA_DEP_SYNC,
+                            str(e),
+                            step_id=action_definition["stepId"],
                         ) from e
                     next_action = SyncInputJobAttachmentsAction(
                         id=action_id,
                         session_id=self._session_id,
                         step_details=step_details,
                     )
             else:
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/log_config.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/log_config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/session.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,14 +552,16 @@
 
         # Cancel the action
         logger.info(
             SessionActionLogEvent(
                 subtype=SessionActionLogEventSubtype.CANCEL,
                 queue_id=self._queue_id,
                 job_id=self._job_id,
+                step_id=current_action.definition.step_id,
+                task_id=getattr(current_action.definition, "task_id", None),
                 session_id=self.id,
                 action_log_kind=current_action.definition.action_log_kind,
                 action_id=current_action.definition.id,
                 message="Canceling Action.",
             )
         )
         current_action.definition.cancel(session=self, time_limit=time_limit)
@@ -583,14 +585,16 @@
                 )
             )
             logger.error(
                 SessionActionLogEvent(
                     subtype=SessionActionLogEventSubtype.END,
                     queue_id=self._queue_id,
                     job_id=self._job_id,
+                    step_id=e.step_id,
+                    task_id=e.task_id,
                     session_id=self.id,
                     action_log_kind=e.action_log_kind,
                     action_id=e.action_id,
                     message="Failed to dequeue next Action: %s" % str(e),
                     status="FAILED",
                 )
             )
@@ -604,14 +608,16 @@
         now = datetime.now(tz=timezone.utc)
 
         logger.info(
             SessionActionLogEvent(
                 subtype=SessionActionLogEventSubtype.START,
                 queue_id=self._queue_id,
                 job_id=self._job_id,
+                step_id=action_definition.step_id,
+                task_id=getattr(action_definition, "task_id", None),
                 session_id=self.id,
                 action_id=action_definition.id,
                 action_log_kind=action_definition.action_log_kind,
                 message="Action started.",
             )
         )
 
@@ -626,14 +632,16 @@
             )
         except Exception as e:
             logger.error(
                 SessionActionLogEvent(
                     subtype=SessionActionLogEventSubtype.END,
                     queue_id=self._queue_id,
                     job_id=self._job_id,
+                    step_id=action_definition.step_id,
+                    task_id=getattr(action_definition, "task_id", None),
                     session_id=self.id,
                     action_id=action_definition.id,
                     action_log_kind=action_definition.action_log_kind,
                     message="Action failed to start: %s" % str(e),
                     status="FAILED",
                 )
             )
@@ -1137,14 +1145,16 @@
             # reading through the logs some context before they see a Session have actions
             # removed.
             logger.info(
                 SessionActionLogEvent(
                     subtype=SessionActionLogEventSubtype.END,
                     queue_id=self._queue_id,
                     job_id=self._job_id,
+                    step_id=current_action.definition.step_id,
+                    task_id=getattr(current_action.definition, "task_id", None),
                     session_id=self.id,
                     action_log_kind=current_action.definition.action_log_kind,
                     action_id=current_action.definition.id,
                     message="Action complete.",
                     status=completed_status,
                 )
             )
@@ -1245,15 +1255,15 @@
 
         assert isinstance(current_action.definition, RunStepTaskAction)
         upload_summary_statistics: SummaryStatistics = self._asset_sync.sync_outputs(
             s3_settings=s3_settings,
             attachments=attachments,
             queue_id=self._queue_id,
             job_id=self._queue._job_id,
-            step_id=current_action.definition.step_id,
+            step_id=current_action.definition.step_id,  # type: ignore[arg-type]
             task_id=current_action.definition.task_id,
             session_action_id=current_action.definition.id,
             start_time=current_action.start_time.timestamp(),
             session_dir=self._session.working_directory,
             storage_profiles_path_mapping_rules=storage_profiles_path_mapping_rules_dict,
             on_uploading_files=self._notifier_callback,
         )
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/__init__.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/action_definition.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/action_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 from __future__ import annotations
 from concurrent.futures import Executor
 from datetime import timedelta
+from typing import Optional
 
 from abc import ABC, abstractmethod
 
 from ..session import Session
 from ...log_messages import SessionActionLogKind
 
 
@@ -18,28 +19,36 @@
     ----------
     id : str
         The unique session action identifier
     """
 
     _id: str
     _action_log_kind: SessionActionLogKind
+    _step_id: Optional[str]
 
-    def __init__(self, *, id: str, action_log_kind: SessionActionLogKind) -> None:
+    def __init__(
+        self, *, id: str, action_log_kind: SessionActionLogKind, step_id: Optional[str] = None
+    ) -> None:
         self._id = id
         self._action_log_kind = action_log_kind
+        self._step_id = step_id
 
     @property
     def id(self) -> str:
         """The unique identifier of the SessionAction"""
         return self._id
 
     @property
     def action_log_kind(self) -> SessionActionLogKind:
         return self._action_log_kind
 
+    @property
+    def step_id(self) -> Optional[str]:
+        return self._step_id
+
     @abstractmethod
     def start(
         self,
         *,
         session: Session,
         executor: Executor,
     ) -> None:
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/enter_env.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/enter_env.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/exit_env.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/exit_env.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/openjd_action.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/openjd_action.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/run_step_task.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/run_step_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,33 +27,30 @@
         The environment details
     task_id : str
         The unique task identifier
     task_parameter_values : TaskParameterSet
         The task parameter values
     """
 
-    step_id: str
     task_id: str
     _details: StepDetails
     _task_parameter_values: TaskParameterSet
 
     def __init__(
         self,
         *,
         id: str,
-        step_id: str,
         details: StepDetails,
         task_id: str,
         task_parameter_values: TaskParameterSet,
     ) -> None:
         super(RunStepTaskAction, self).__init__(
-            id=id, action_log_kind=SessionActionLogKind.TASK_RUN
+            id=id, action_log_kind=SessionActionLogKind.TASK_RUN, step_id=details.step_id
         )
         self._details = details
-        self.step_id = step_id
         self.task_id = task_id
         self._task_parameter_values = task_parameter_values
 
     def __eq__(self, other: Any) -> bool:
         return (
             type(self) == type(other)
             and self._id == other._id
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,21 @@
         *,
         id: str,
         session_id: str,
         job_attachment_details: Optional[JobAttachmentDetails] = None,
         step_details: Optional[StepDetails] = None,
     ) -> None:
         super(SyncInputJobAttachmentsAction, self).__init__(
-            id=id, action_log_kind=SessionActionLogKind.JA_SYNC
+            id=id,
+            action_log_kind=(
+                SessionActionLogKind.JA_SYNC
+                if step_details is None
+                else SessionActionLogKind.JA_DEP_SYNC
+            ),
+            step_id=step_details.step_id if step_details is not None else None,
         )
         self._cancel = Event()
         self._job_attachment_details = job_attachment_details
         self._step_details = step_details
         self._logger = LoggerAdapter(OPENJD_LOG, extra={"session_id": session_id})
 
     def __eq__(self, other: Any) -> bool:
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/environment_details.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/environment_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_details.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_details.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,41 +87,47 @@
 
 def job_run_as_user_api_model_to_worker_agent(
     job_run_as_user_data: JobRunAsUserModel,
 ) -> JobRunAsUser | None:
     """Converts the 'JobRunAsUser' api model to the 'JobRunAsUser' dataclass
     expected by the Worker Agent.
     """
-    if "runAs" in job_run_as_user_data and job_run_as_user_data["runAs"] == "WORKER_AGENT_USER":
+    # Only two options for "runAs": WORKER_AGENT_USER & QUEUE_CONFIGURED_USER
+    if job_run_as_user_data["runAs"] == "WORKER_AGENT_USER":
         job_run_as_user = JobRunAsUser(is_worker_agent_user=True)
         return job_run_as_user
 
+    # We have a QUEUE_CONFIGURED_USER, so extract the data for this platform.
     if os.name == "posix":
-        user = ""
-        group = ""
-        if job_run_as_user_posix := job_run_as_user_data.get("posix", None):
-            user = job_run_as_user_posix["user"]
-            group = job_run_as_user_posix["group"]
-        else:
+        job_run_as_user_posix = job_run_as_user_data.get("posix", None)
+        if job_run_as_user_posix is None:
+            # Note: This may happen in an SMF case as follows:
+            #  Customer has a Windows-based CMF, and configures the QUEUE_CONFIGURED_USER
+            # for Windows, but also connects the Queue to a posix-based SMF.
+            #  So, this would mean that we're in a posix-based SMF. Return None; the agent
+            # must have been started with a jobRunAsUser override.
             return None
 
-        if "runAs" not in job_run_as_user_data and not group and not user:
-            return None
         job_run_as_user = JobRunAsUser(
             posix=PosixSessionUser(
-                user=user,
-                group=group,
+                user=job_run_as_user_posix["user"],
+                group=job_run_as_user_posix["group"],
             ),
         )
     else:
-        job_run_as_user_windows = job_run_as_user_data.get("windows", {})
-        user = job_run_as_user_windows.get("user", "")
-        passwordArn = job_run_as_user_windows.get("passwordArn", "")
-        if not (user and passwordArn):
+        job_run_as_user_windows = job_run_as_user_data.get("windows", None)
+        if job_run_as_user_windows is None:
+            # Note: This may happen in an SMF case as follows:
+            #  Customer has a posix-based CMF, and configures the QUEUE_CONFIGURED_USER
+            # for posix, but also connects the Queue to a Windows-based SMF.
+            #  So, this would mean that we're in a Windows-based SMF. Return None; the agent
+            # must have been started with a jobRunAsUser override.
             return None
+        user = job_run_as_user_windows["user"]
+        passwordArn = job_run_as_user_windows["passwordArn"]
         job_run_as_user = JobRunAsUser(
             windows_settings=JobRunAsWindowsUser(user=user, passwordArn=passwordArn),
         )
 
     return job_run_as_user
 
 
@@ -234,17 +240,19 @@
         if path_mapping_rules_data:
             path_mapping_rules = path_mapping_api_model_to_openjd(path_mapping_rules_data)
 
         job_attachment_settings: JobAttachmentSettings | None = None
         if job_attachment_settings_boto := job_details_data.get("jobAttachmentSettings", None):
             job_attachment_settings = JobAttachmentSettings.from_boto(job_attachment_settings_boto)
 
-        job_run_as_user_data = job_details_data["jobRunAsUser"]
-        job_run_as_user: JobRunAsUser | None = job_run_as_user_api_model_to_worker_agent(
-            job_run_as_user_data
+        job_run_as_user_data = job_details_data.get("jobRunAsUser", None)
+        job_run_as_user: JobRunAsUser | None = (
+            job_run_as_user_api_model_to_worker_agent(job_run_as_user_data)
+            if job_run_as_user_data is not None
+            else None
         )
 
         # Note: Record the empty string as a None as well.
         queue_role_arn: str | None = job_details_data.get("queueRoleArn", None)
 
         given_schema_version = TemplateSpecificationVersion(job_details_data["schemaVersion"])
 
@@ -286,43 +294,42 @@
 
         validate_object(
             data=entity_data,
             fields=(
                 Field(key="jobId", expected_type=str, required=True),
                 Field(key="logGroupName", expected_type=str, required=True),
                 Field(key="schemaVersion", expected_type=str, required=True),
-                Field(key="osUser", expected_type=str, required=False),
                 Field(
                     key="parameters",
                     expected_type=dict,
                     required=False,
                 ),
                 Field(
                     key="pathMappingRules",
                     expected_type=list,
                     required=False,
                 ),
                 Field(
                     key="jobRunAsUser",
                     expected_type=dict,
-                    required=True,
+                    required=False,
                     fields=(
                         Field(
                             key="posix",
                             expected_type=dict,
                             required=False,
                             fields=(
                                 Field(key="user", expected_type=str, required=True),
                                 Field(key="group", expected_type=str, required=True),
                             ),
                         ),
                         Field(
                             key="runAs",
                             expected_type=str,
-                            required=False,
+                            required=True,
                         ),
                         Field(
                             key="windows",
                             expected_type=dict,
                             required=False,
                             fields=(
                                 Field(key="user", expected_type=str, required=True),
@@ -363,15 +370,15 @@
                         Field(key="sourcePathFormat", expected_type=str, required=True),
                         Field(key="sourcePath", expected_type=str, required=True),
                         Field(key="destinationPath", expected_type=str, required=True),
                     ),
                 )
 
         # Validate jobRunAsUser -> runAs is one of ("QUEUE_CONFIGURED_USER" / "WORKER_AGENT_USER")
-        if run_as_value := entity_data["jobRunAsUser"].get("runAs", None):
+        if run_as_value := entity_data.get("jobRunAsUser", dict()).get("runAs", None):
             if run_as_value not in ("QUEUE_CONFIGURED_USER", "WORKER_AGENT_USER"):
                 raise ValueError(
                     f'Expected "jobRunAs" -> "runAs" to be one of "QUEUE_CONFIGURED_USER", "WORKER_AGENT_USER" but got "{run_as_value}"'
                 )
             elif run_as_value == "QUEUE_CONFIGURED_USER":
                 run_as_posix = entity_data["jobRunAsUser"].get("posix", None)
                 run_as_windows = entity_data["jobRunAsUser"].get("windows", None)
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_entities.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_entities.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/step_details.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/step_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     ENTITY_TYPE = JobEntityType.STEP_DETAILS.value
     """The JobEntityType handled by this class"""
 
     step_template: StepTemplate
     """The step's Open Job Description step template.
     """
 
+    step_id: str
+    """The AWS Deadline Cloud resource ID for the Step.
+    """
+
     dependencies: list[str] = field(default_factory=list)
     """The dependencies (a list of IDs) that the step depends on"""
 
     @classmethod
     def from_boto(cls, step_details_data: StepDetailsData) -> StepDetails:
         """Converts an stepDetails entity received from BatchGetJobEntity API response into a
         StepDetails instance
@@ -69,14 +73,15 @@
                     model=StepTemplate_2023_09, obj={"name": "Placeholder", "script": details_data}
                 )
         else:
             raise UnsupportedSchema(schema_version.value)
 
         return StepDetails(
             step_template=step_template,
+            step_id=step_details_data["stepId"],
             dependencies=step_details_data["dependencies"],
         )
 
     @classmethod
     def validate_entity_data(cls, entity_data: dict[str, Any]) -> StepDetailsData:
         """Performs input validation on a response element recceived from boto3's call to
         the BatchGetJobEntity AWS Deadline Cloud API.
```

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/validation.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/validation.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/bootstrap.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/bootstrap.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/capabilities.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/capabilities.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/cli_args.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/cli_args.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config_file.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config_file.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/entrypoint.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/host_properties.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/host_properties.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/settings.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/settings.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_credentials_resolver.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_credentials_resolver.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_service.py` & `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_service.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/LICENSE` & `deadline_cloud_worker_agent-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/README.md` & `deadline_cloud_worker_agent-0.27.0/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/hatch.toml` & `deadline_cloud_worker_agent-0.27.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/pyproject.toml` & `deadline_cloud_worker_agent-0.27.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.1/PKG-INFO` & `deadline_cloud_worker_agent-0.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-worker-agent
-Version: 0.26.1
+Version: 0.27.0
 Summary: The AWS Deadline Cloud worker agent can be used to run a worker in an AWS Deadline Cloud fleet
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-worker-agent
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-worker-agent
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

