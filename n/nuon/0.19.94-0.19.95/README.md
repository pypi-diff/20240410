# Comparing `tmp/nuon-0.19.94.tar.gz` & `tmp/nuon-0.19.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuon-0.19.94.tar", last modified: Tue Apr  9 02:20:23 2024, max compression
+gzip compressed data, was "nuon-0.19.95.tar", last modified: Wed Apr 10 01:49:12 2024, max compression
```

## Comparing `nuon-0.19.94.tar` & `nuon-0.19.95.tar`

### file list

```diff
@@ -1,253 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:20:23.935819 nuon-0.19.94/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 02:20:23.935819 nuon-0.19.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 02:20:16.000000 nuon-0.19.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:20:23.895819 nuon-0.19.94/nuon/
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:20:23.899819 nuon-0.19.94/nuon/api/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   208357 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/apps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   230057 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/components_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31790 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/general_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   100599 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/installers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   263222 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/installs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    74180 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/orgs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55061 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/releases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30749 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54514 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api/vcs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24530 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:20:23.915819 nuon-0.19.94/nuon/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_config_fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_config_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_input_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_installer_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_runner_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_sandbox_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_app_sandbox_config_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_awsecr_image_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_component_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_component_config_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_component_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_component_release_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_connected_github_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_docker_build_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_external_image_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_helm_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_install_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_install_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_install_deploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_install_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_install_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_install_sandbox_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_job_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_operation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_org_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_org_health_check_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_public_git_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_sandbox_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_sandbox_run_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_terraform_module_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_token_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_user_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_vcs_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/app_vcs_connection_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/metrics_decr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/metrics_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/metrics_incr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/metrics_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/planv1_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_app_config_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_app_config_template_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_app_input_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_aws_ecr_image_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_connected_github_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_connected_github_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_app_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_app_input_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_app_runner_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_app_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_component_build_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_component_release_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_component_release_request_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_connection_callback_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_docker_build_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_external_image_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_helm_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_install_deploy_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_install_inputs_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_install_request_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_install_request_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_job_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_org_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_create_terraform_module_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_installer_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_public_git_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_public_git_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_publish_metric_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_rendered_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_rendered_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/service_update_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/statsd_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/statsd_event_alert_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/statsd_event_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/models/stderr_err_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-09 02:20:16.000000 nuon-0.19.94/nuon/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:20:23.935819 nuon-0.19.94/nuon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 02:20:23.000000 nuon-0.19.94/nuon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-09 02:20:23.000000 nuon-0.19.94/nuon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 02:20:23.000000 nuon-0.19.94/nuon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 02:20:23.000000 nuon-0.19.94/nuon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 02:20:23.000000 nuon-0.19.94/nuon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 02:20:16.000000 nuon-0.19.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 02:20:23.935819 nuon-0.19.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-09 02:20:16.000000 nuon-0.19.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:20:23.931819 nuon-0.19.94/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_config_fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_config_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_input_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_installer_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_runner_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_sandbox_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_app_sandbox_config_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_awsecr_image_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_component_build.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_component_config_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_component_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_component_release_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_connected_github_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_docker_build_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_external_image_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_helm_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_install_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_install_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_install_deploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_install_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_install_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_install_sandbox_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_job_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_operation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_org_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_org_health_check_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_public_git_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_sandbox_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_sandbox_run_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_terraform_module_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_token_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_user_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_vcs_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_app_vcs_connection_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_apps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_components_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_general_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_installers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_installs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_metrics_decr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_metrics_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_metrics_incr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_metrics_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_orgs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_planv1_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_releases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_app_config_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_app_config_template_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_app_input_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_aws_ecr_image_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_connected_github_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_connected_github_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_app_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_app_input_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_app_runner_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_app_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_component_build_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_component_release_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_component_release_request_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_connection_callback_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_docker_build_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_external_image_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_helm_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_install_deploy_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_install_inputs_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_install_request_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_install_request_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_job_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_org_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_create_terraform_module_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_installer_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_public_git_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_public_git_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_publish_metric_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_rendered_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_rendered_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_service_update_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_statsd_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_statsd_event_alert_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_statsd_event_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_stderr_err_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-09 02:20:16.000000 nuon-0.19.94/test/test_vcs_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:49:12.149687 nuon-0.19.95/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 01:49:12.149687 nuon-0.19.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 01:49:05.000000 nuon-0.19.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:49:12.105687 nuon-0.19.95/nuon/
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:49:12.109687 nuon-0.19.95/nuon/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   242441 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/apps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230057 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/components_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31790 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/general_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100599 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/installers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   263222 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/installs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74180 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/orgs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55061 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30749 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54514 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api/vcs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24530 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:49:12.129687 nuon-0.19.95/nuon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_config_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_config_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_input_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_installer_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_runner_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_sandbox_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_sandbox_config_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_app_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_awsecr_image_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_component_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_component_config_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_component_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_component_release_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_connected_github_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_docker_build_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_external_image_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_helm_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_install_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_install_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_install_deploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_install_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_install_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_install_sandbox_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_job_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_org_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_org_health_check_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_public_git_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_sandbox_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_sandbox_run_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_terraform_module_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_user_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_vcs_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/app_vcs_connection_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/metrics_decr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/metrics_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/metrics_incr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/metrics_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/planv1_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_app_config_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_app_config_template_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_app_input_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_aws_ecr_image_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_connected_github_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_connected_github_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_input_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_runner_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_app_secret_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_component_build_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_component_release_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_component_release_request_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_connection_callback_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_docker_build_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_external_image_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_helm_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_install_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_install_inputs_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_install_request_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_install_request_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_job_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_org_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_create_terraform_module_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_installer_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_public_git_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_public_git_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_publish_metric_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_rendered_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_rendered_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/service_update_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/statsd_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/statsd_event_alert_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/statsd_event_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/models/stderr_err_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-10 01:49:05.000000 nuon-0.19.95/nuon/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:49:12.149687 nuon-0.19.95/nuon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 01:49:12.000000 nuon-0.19.95/nuon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-10 01:49:12.000000 nuon-0.19.95/nuon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:49:12.000000 nuon-0.19.95/nuon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 01:49:12.000000 nuon-0.19.95/nuon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-10 01:49:12.000000 nuon-0.19.95/nuon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-10 01:49:05.000000 nuon-0.19.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 01:49:12.149687 nuon-0.19.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-10 01:49:05.000000 nuon-0.19.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:49:12.149687 nuon-0.19.95/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_config_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_config_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_input_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_installer_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_runner_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_sandbox_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_sandbox_config_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_app_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_awsecr_image_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_component_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_component_config_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_component_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_component_release_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_connected_github_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_docker_build_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_external_image_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_helm_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_install_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_install_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_install_deploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_install_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_install_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_install_sandbox_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_job_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_org_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_org_health_check_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_public_git_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_sandbox_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_sandbox_run_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_terraform_module_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_user_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_vcs_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_app_vcs_connection_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_apps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_components_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_general_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_installers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_installs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_metrics_decr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_metrics_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_metrics_incr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_metrics_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_orgs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_planv1_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_app_config_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_app_config_template_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_app_input_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_aws_ecr_image_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_connected_github_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_connected_github_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_input_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_runner_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_app_secret_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_component_build_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_component_release_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_component_release_request_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_connection_callback_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_docker_build_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_external_image_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_helm_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_install_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_install_inputs_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_install_request_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_install_request_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_job_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_org_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_create_terraform_module_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_installer_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_public_git_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_public_git_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_publish_metric_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_rendered_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_rendered_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_service_update_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_statsd_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_statsd_event_alert_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_statsd_event_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_stderr_err_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-10 01:49:05.000000 nuon-0.19.95/test/test_vcs_api.py
```

### Comparing `nuon-0.19.94/nuon/__init__.py` & `nuon-0.19.95/nuon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.19.94"
+__version__ = "0.19.95"
 
 # import apis into sdk package
 from nuon.api.apps_api import AppsApi
 from nuon.api.components_api import ComponentsApi
 from nuon.api.general_api import GeneralApi
 from nuon.api.installers_api import InstallersApi
 from nuon.api.installs_api import InstallsApi
@@ -50,14 +50,15 @@
 from nuon.models.app_app_input_config import AppAppInputConfig
 from nuon.models.app_app_installer import AppAppInstaller
 from nuon.models.app_app_installer_metadata import AppAppInstallerMetadata
 from nuon.models.app_app_runner_config import AppAppRunnerConfig
 from nuon.models.app_app_runner_type import AppAppRunnerType
 from nuon.models.app_app_sandbox_config import AppAppSandboxConfig
 from nuon.models.app_app_sandbox_config_artifacts import AppAppSandboxConfigArtifacts
+from nuon.models.app_app_secret import AppAppSecret
 from nuon.models.app_azure_account import AppAzureAccount
 from nuon.models.app_cloud_platform import AppCloudPlatform
 from nuon.models.app_component import AppComponent
 from nuon.models.app_component_build import AppComponentBuild
 from nuon.models.app_component_config_connection import AppComponentConfigConnection
 from nuon.models.app_component_release import AppComponentRelease
 from nuon.models.app_component_release_step import AppComponentReleaseStep
@@ -103,14 +104,15 @@
 from nuon.models.service_create_app_config_request import ServiceCreateAppConfigRequest
 from nuon.models.service_create_app_input_config_request import ServiceCreateAppInputConfigRequest
 from nuon.models.service_create_app_installer_request import ServiceCreateAppInstallerRequest
 from nuon.models.service_create_app_installer_request_links import ServiceCreateAppInstallerRequestLinks
 from nuon.models.service_create_app_request import ServiceCreateAppRequest
 from nuon.models.service_create_app_runner_config_request import ServiceCreateAppRunnerConfigRequest
 from nuon.models.service_create_app_sandbox_config_request import ServiceCreateAppSandboxConfigRequest
+from nuon.models.service_create_app_secret_request import ServiceCreateAppSecretRequest
 from nuon.models.service_create_component_build_request import ServiceCreateComponentBuildRequest
 from nuon.models.service_create_component_release_request import ServiceCreateComponentReleaseRequest
 from nuon.models.service_create_component_release_request_strategy import ServiceCreateComponentReleaseRequestStrategy
 from nuon.models.service_create_component_request import ServiceCreateComponentRequest
 from nuon.models.service_create_connection_callback_request import ServiceCreateConnectionCallbackRequest
 from nuon.models.service_create_connection_request import ServiceCreateConnectionRequest
 from nuon.models.service_create_docker_build_component_config_request import ServiceCreateDockerBuildComponentConfigRequest
```

### Comparing `nuon-0.19.94/nuon/api/apps_api.py` & `nuon-0.19.95/nuon/api/apps_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -27,20 +27,22 @@
 from pydantic import Field, StrictStr, field_validator
 from typing_extensions import Annotated
 from nuon.models.app_app import AppApp
 from nuon.models.app_app_config import AppAppConfig
 from nuon.models.app_app_input_config import AppAppInputConfig
 from nuon.models.app_app_runner_config import AppAppRunnerConfig
 from nuon.models.app_app_sandbox_config import AppAppSandboxConfig
+from nuon.models.app_app_secret import AppAppSecret
 from nuon.models.service_app_config_template import ServiceAppConfigTemplate
 from nuon.models.service_create_app_config_request import ServiceCreateAppConfigRequest
 from nuon.models.service_create_app_input_config_request import ServiceCreateAppInputConfigRequest
 from nuon.models.service_create_app_request import ServiceCreateAppRequest
 from nuon.models.service_create_app_runner_config_request import ServiceCreateAppRunnerConfigRequest
 from nuon.models.service_create_app_sandbox_config_request import ServiceCreateAppSandboxConfigRequest
+from nuon.models.service_create_app_secret_request import ServiceCreateAppSecretRequest
 from nuon.models.service_update_app_request import ServiceUpdateAppRequest
 
 from nuon.api_client import ApiClient
 from nuon.api_response import ApiResponse
 from nuon.rest import RESTResponseType
 
 
@@ -1537,14 +1539,316 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def create_app_secret(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        service_create_app_secret_request: Annotated[ServiceCreateAppSecretRequest, Field(description="Input")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> AppAppSecret:
+        """create an app secret
+
+        Create an app secret that can be used to configure components. To reference an app secret, use `.nuon.secrets.<secret_name>`.  **NOTE** secrets can only be written, or deleted, not read. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param service_create_app_secret_request: Input (required)
+        :type service_create_app_secret_request: ServiceCreateAppSecretRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_app_secret_serialize(
+            app_id=app_id,
+            service_create_app_secret_request=service_create_app_secret_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "AppAppSecret",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def create_app_secret_with_http_info(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        service_create_app_secret_request: Annotated[ServiceCreateAppSecretRequest, Field(description="Input")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[AppAppSecret]:
+        """create an app secret
+
+        Create an app secret that can be used to configure components. To reference an app secret, use `.nuon.secrets.<secret_name>`.  **NOTE** secrets can only be written, or deleted, not read. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param service_create_app_secret_request: Input (required)
+        :type service_create_app_secret_request: ServiceCreateAppSecretRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_app_secret_serialize(
+            app_id=app_id,
+            service_create_app_secret_request=service_create_app_secret_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "AppAppSecret",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def create_app_secret_without_preload_content(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        service_create_app_secret_request: Annotated[ServiceCreateAppSecretRequest, Field(description="Input")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """create an app secret
+
+        Create an app secret that can be used to configure components. To reference an app secret, use `.nuon.secrets.<secret_name>`.  **NOTE** secrets can only be written, or deleted, not read. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param service_create_app_secret_request: Input (required)
+        :type service_create_app_secret_request: ServiceCreateAppSecretRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_app_secret_serialize(
+            app_id=app_id,
+            service_create_app_secret_request=service_create_app_secret_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "AppAppSecret",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _create_app_secret_serialize(
+        self,
+        app_id,
+        service_create_app_secret_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if app_id is not None:
+            _path_params['app_id'] = app_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if service_create_app_secret_request is not None:
+            _body_params = service_create_app_secret_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'APIKey', 
+            'OrgID'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/v1/apps/{app_id}/secret',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def delete_app(
         self,
         app_id: Annotated[StrictStr, Field(description="app ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -1808,14 +2112,303 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def delete_app_secret(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        secret_id: Annotated[StrictStr, Field(description="secret ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> bool:
+        """delete an app secret
+
+        Delete an app secret. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param secret_id: secret ID (required)
+        :type secret_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_app_secret_serialize(
+            app_id=app_id,
+            secret_id=secret_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "bool",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def delete_app_secret_with_http_info(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        secret_id: Annotated[StrictStr, Field(description="secret ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[bool]:
+        """delete an app secret
+
+        Delete an app secret. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param secret_id: secret ID (required)
+        :type secret_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_app_secret_serialize(
+            app_id=app_id,
+            secret_id=secret_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "bool",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def delete_app_secret_without_preload_content(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        secret_id: Annotated[StrictStr, Field(description="secret ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """delete an app secret
+
+        Delete an app secret. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param secret_id: secret ID (required)
+        :type secret_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_app_secret_serialize(
+            app_id=app_id,
+            secret_id=secret_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "bool",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _delete_app_secret_serialize(
+        self,
+        app_id,
+        secret_id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if app_id is not None:
+            _path_params['app_id'] = app_id
+        if secret_id is not None:
+            _path_params['secret_id'] = secret_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'APIKey', 
+            'OrgID'
+        ]
+
+        return self.api_client.param_serialize(
+            method='DELETE',
+            resource_path='/v1/apps/{app_id}/secret/{secret_id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def get_app(
         self,
         app_id: Annotated[StrictStr, Field(description="app ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -4824,14 +5417,288 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def get_app_secrets(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[AppAppSecret]:
+        """get app secrets
+
+        List all secrets for an app.  **NOTE** this does not return any sensitive values, as secrets are write only. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_app_secrets_serialize(
+            app_id=app_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[AppAppSecret]",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def get_app_secrets_with_http_info(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[AppAppSecret]]:
+        """get app secrets
+
+        List all secrets for an app.  **NOTE** this does not return any sensitive values, as secrets are write only. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_app_secrets_serialize(
+            app_id=app_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[AppAppSecret]",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def get_app_secrets_without_preload_content(
+        self,
+        app_id: Annotated[StrictStr, Field(description="app ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """get app secrets
+
+        List all secrets for an app.  **NOTE** this does not return any sensitive values, as secrets are write only. 
+
+        :param app_id: app ID (required)
+        :type app_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_app_secrets_serialize(
+            app_id=app_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[AppAppSecret]",
+            '400': "StderrErrResponse",
+            '401': "StderrErrResponse",
+            '403': "StderrErrResponse",
+            '404': "StderrErrResponse",
+            '500': "StderrErrResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _get_app_secrets_serialize(
+        self,
+        app_id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if app_id is not None:
+            _path_params['app_id'] = app_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'APIKey', 
+            'OrgID'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/v1/apps/{app_id}/secrets',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `nuon-0.19.94/nuon/api/components_api.py` & `nuon-0.19.95/nuon/api/components_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api/general_api.py` & `nuon-0.19.95/nuon/api/general_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api/installers_api.py` & `nuon-0.19.95/nuon/api/installers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api/installs_api.py` & `nuon-0.19.95/nuon/api/installs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api/orgs_api.py` & `nuon-0.19.95/nuon/api/orgs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api/releases_api.py` & `nuon-0.19.95/nuon/api/releases_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api/sandboxes_api.py` & `nuon-0.19.95/nuon/api/sandboxes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api/vcs_api.py` & `nuon-0.19.95/nuon/api/vcs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/api_client.py` & `nuon-0.19.95/nuon/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.19.94/python'
+        self.user_agent = 'OpenAPI-Generator/0.19.95/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `nuon-0.19.94/nuon/api_response.py` & `nuon-0.19.95/nuon/api_response.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/nuon/configuration.py` & `nuon-0.19.95/nuon/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -402,16 +402,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.19.94\n"\
-               "SDK Package Version: 0.19.94".\
+               "Version of the API: 0.19.95\n"\
+               "SDK Package Version: 0.19.95".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `nuon-0.19.94/nuon/exceptions.py` & `nuon-0.19.95/nuon/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `nuon-0.19.94/nuon/models/__init__.py` & `nuon-0.19.95/nuon/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -25,14 +25,15 @@
 from nuon.models.app_app_input_config import AppAppInputConfig
 from nuon.models.app_app_installer import AppAppInstaller
 from nuon.models.app_app_installer_metadata import AppAppInstallerMetadata
 from nuon.models.app_app_runner_config import AppAppRunnerConfig
 from nuon.models.app_app_runner_type import AppAppRunnerType
 from nuon.models.app_app_sandbox_config import AppAppSandboxConfig
 from nuon.models.app_app_sandbox_config_artifacts import AppAppSandboxConfigArtifacts
+from nuon.models.app_app_secret import AppAppSecret
 from nuon.models.app_azure_account import AppAzureAccount
 from nuon.models.app_cloud_platform import AppCloudPlatform
 from nuon.models.app_component import AppComponent
 from nuon.models.app_component_build import AppComponentBuild
 from nuon.models.app_component_config_connection import AppComponentConfigConnection
 from nuon.models.app_component_release import AppComponentRelease
 from nuon.models.app_component_release_step import AppComponentReleaseStep
@@ -78,14 +79,15 @@
 from nuon.models.service_create_app_config_request import ServiceCreateAppConfigRequest
 from nuon.models.service_create_app_input_config_request import ServiceCreateAppInputConfigRequest
 from nuon.models.service_create_app_installer_request import ServiceCreateAppInstallerRequest
 from nuon.models.service_create_app_installer_request_links import ServiceCreateAppInstallerRequestLinks
 from nuon.models.service_create_app_request import ServiceCreateAppRequest
 from nuon.models.service_create_app_runner_config_request import ServiceCreateAppRunnerConfigRequest
 from nuon.models.service_create_app_sandbox_config_request import ServiceCreateAppSandboxConfigRequest
+from nuon.models.service_create_app_secret_request import ServiceCreateAppSecretRequest
 from nuon.models.service_create_component_build_request import ServiceCreateComponentBuildRequest
 from nuon.models.service_create_component_release_request import ServiceCreateComponentReleaseRequest
 from nuon.models.service_create_component_release_request_strategy import ServiceCreateComponentReleaseRequestStrategy
 from nuon.models.service_create_component_request import ServiceCreateComponentRequest
 from nuon.models.service_create_connection_callback_request import ServiceCreateConnectionCallbackRequest
 from nuon.models.service_create_connection_request import ServiceCreateConnectionRequest
 from nuon.models.service_create_docker_build_component_config_request import ServiceCreateDockerBuildComponentConfigRequest
```

### Comparing `nuon-0.19.94/nuon/models/app_app.py` & `nuon-0.19.95/nuon/models/app_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_config.py` & `nuon-0.19.95/nuon/models/app_app_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_config_fmt.py` & `nuon-0.19.95/nuon/models/app_app_config_fmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_config_status.py` & `nuon-0.19.95/nuon/models/app_app_config_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_input.py` & `nuon-0.19.95/nuon/models/app_app_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_input_config.py` & `nuon-0.19.95/nuon/models/app_app_input_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_installer.py` & `nuon-0.19.95/nuon/models/app_app_installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_installer_metadata.py` & `nuon-0.19.95/nuon/models/app_app_installer_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_runner_config.py` & `nuon-0.19.95/nuon/models/app_app_runner_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_runner_type.py` & `nuon-0.19.95/nuon/models/app_app_runner_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_app_sandbox_config.py` & `nuon-0.19.95/nuon/models/app_app_sandbox_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -34,15 +34,15 @@
 except ImportError:
     from typing_extensions import Self
 
 class AppAppSandboxConfig(BaseModel):
     """
     AppAppSandboxConfig
     """ # noqa: E501
-    app_id: Optional[StrictStr] = Field(default=None, description="TODO(jm): add this back, once we have migrated all existing app sandbox configs `gorm:\"not null;default null\"`")
+    app_id: Optional[StrictStr] = Field(default=None, description="gorm:\"not null;default null\"`")
     artifacts: Optional[AppAppSandboxConfigArtifacts] = None
     cloud_platform: Optional[AppCloudPlatform] = None
     connected_github_vcs_config: Optional[AppConnectedGithubVCSConfig] = None
     created_at: Optional[StrictStr] = None
     created_by: Optional[AppUserToken] = None
     created_by_id: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
```

### Comparing `nuon-0.19.94/nuon/models/app_app_sandbox_config_artifacts.py` & `nuon-0.19.95/nuon/models/app_app_sandbox_config_artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_aws_account.py` & `nuon-0.19.95/nuon/models/app_aws_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_awsecr_image_config.py` & `nuon-0.19.95/nuon/models/app_awsecr_image_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_azure_account.py` & `nuon-0.19.95/nuon/models/app_azure_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_cloud_platform.py` & `nuon-0.19.95/nuon/models/app_cloud_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_component.py` & `nuon-0.19.95/nuon/models/app_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_component_build.py` & `nuon-0.19.95/nuon/models/app_component_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_component_config_connection.py` & `nuon-0.19.95/nuon/models/app_component_config_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_component_release.py` & `nuon-0.19.95/nuon/models/app_component_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_component_release_step.py` & `nuon-0.19.95/nuon/models/app_component_release_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_connected_github_vcs_config.py` & `nuon-0.19.95/nuon/models/app_connected_github_vcs_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_docker_build_component_config.py` & `nuon-0.19.95/nuon/models/app_docker_build_component_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_external_image_component_config.py` & `nuon-0.19.95/nuon/models/app_external_image_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_helm_component_config.py` & `nuon-0.19.95/nuon/models/app_helm_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_install.py` & `nuon-0.19.95/nuon/models/app_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_install_component.py` & `nuon-0.19.95/nuon/models/app_install_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_install_deploy.py` & `nuon-0.19.95/nuon/models/app_install_deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_install_deploy_type.py` & `nuon-0.19.95/nuon/models/app_install_deploy_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_install_event.py` & `nuon-0.19.95/nuon/models/app_install_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_install_inputs.py` & `nuon-0.19.95/nuon/models/app_install_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_install_sandbox_run.py` & `nuon-0.19.95/nuon/models/app_install_sandbox_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_job_component_config.py` & `nuon-0.19.95/nuon/models/app_job_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_operation_status.py` & `nuon-0.19.95/nuon/models/app_operation_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_org.py` & `nuon-0.19.95/nuon/models/app_org.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_org_health_check.py` & `nuon-0.19.95/nuon/models/app_org_health_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_org_health_check_status.py` & `nuon-0.19.95/nuon/models/app_org_health_check_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_public_git_vcs_config.py` & `nuon-0.19.95/nuon/models/app_public_git_vcs_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_sandbox.py` & `nuon-0.19.95/nuon/models/app_sandbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_sandbox_release.py` & `nuon-0.19.95/nuon/models/app_sandbox_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_sandbox_run_type.py` & `nuon-0.19.95/nuon/models/app_sandbox_run_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_terraform_module_component_config.py` & `nuon-0.19.95/nuon/models/app_terraform_module_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_token_type.py` & `nuon-0.19.95/nuon/models/app_token_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_user_org.py` & `nuon-0.19.95/nuon/models/app_user_org.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_user_token.py` & `nuon-0.19.95/nuon/models/app_user_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_vcs_connection.py` & `nuon-0.19.95/nuon/models/app_vcs_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/app_vcs_connection_commit.py` & `nuon-0.19.95/nuon/models/app_vcs_connection_commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py` & `nuon-0.19.95/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/metrics_decr.py` & `nuon-0.19.95/nuon/models/metrics_decr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/metrics_event.py` & `nuon-0.19.95/nuon/models/metrics_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/metrics_incr.py` & `nuon-0.19.95/nuon/models/metrics_incr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/metrics_timing.py` & `nuon-0.19.95/nuon/models/metrics_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/planv1_plan.py` & `nuon-0.19.95/nuon/models/planv1_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_app_config_template.py` & `nuon-0.19.95/nuon/models/service_app_config_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_app_config_template_type.py` & `nuon-0.19.95/nuon/models/service_app_config_template_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_app_input_request.py` & `nuon-0.19.95/nuon/models/service_app_input_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_app_installer.py` & `nuon-0.19.95/nuon/models/service_app_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/nuon/models/service_aws_ecr_image_config_request.py` & `nuon-0.19.95/nuon/models/service_aws_ecr_image_config_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_cli_config.py` & `nuon-0.19.95/nuon/models/service_cli_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_connected_github_vcs_config_request.py` & `nuon-0.19.95/nuon/models/service_connected_github_vcs_config_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_connected_github_vcs_sandbox_config_request.py` & `nuon-0.19.95/nuon/models/service_connected_github_vcs_sandbox_config_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_app_config_request.py` & `nuon-0.19.95/nuon/models/service_create_app_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_app_input_config_request.py` & `nuon-0.19.95/nuon/models/service_create_app_input_config_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_app_installer_request.py` & `nuon-0.19.95/nuon/models/service_create_app_installer_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_app_installer_request_links.py` & `nuon-0.19.95/nuon/models/service_create_app_installer_request_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_app_request.py` & `nuon-0.19.95/nuon/models/service_create_app_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_app_runner_config_request.py` & `nuon-0.19.95/nuon/models/service_create_app_runner_config_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_app_sandbox_config_request.py` & `nuon-0.19.95/nuon/models/service_create_app_sandbox_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_component_build_request.py` & `nuon-0.19.95/nuon/models/service_create_component_build_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_component_release_request.py` & `nuon-0.19.95/nuon/models/service_create_component_release_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_component_release_request_strategy.py` & `nuon-0.19.95/nuon/models/service_create_component_release_request_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_component_request.py` & `nuon-0.19.95/nuon/models/service_create_component_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_connection_callback_request.py` & `nuon-0.19.95/nuon/models/service_create_connection_callback_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_connection_request.py` & `nuon-0.19.95/nuon/models/service_create_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_docker_build_component_config_request.py` & `nuon-0.19.95/nuon/models/service_create_docker_build_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_external_image_component_config_request.py` & `nuon-0.19.95/nuon/models/service_create_external_image_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_helm_component_config_request.py` & `nuon-0.19.95/nuon/models/service_create_helm_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_install_deploy_request.py` & `nuon-0.19.95/nuon/models/service_create_install_deploy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_install_inputs_request.py` & `nuon-0.19.95/nuon/models/service_create_install_inputs_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_install_request.py` & `nuon-0.19.95/nuon/models/service_create_install_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_install_request_aws_account.py` & `nuon-0.19.95/nuon/models/service_create_install_request_aws_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_install_request_azure_account.py` & `nuon-0.19.95/nuon/models/service_create_install_request_azure_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_job_component_config_request.py` & `nuon-0.19.95/nuon/models/service_create_job_component_config_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_org_request.py` & `nuon-0.19.95/nuon/models/service_create_org_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_org_user_request.py` & `nuon-0.19.95/nuon/models/service_create_org_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_create_terraform_module_component_config_request.py` & `nuon-0.19.95/nuon/models/service_create_terraform_module_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_installer_create_install_request.py` & `nuon-0.19.95/nuon/models/service_installer_create_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/nuon/models/service_public_git_vcs_config_request.py` & `nuon-0.19.95/nuon/models/service_public_git_vcs_config_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_public_git_vcs_sandbox_config_request.py` & `nuon-0.19.95/nuon/models/service_public_git_vcs_sandbox_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_publish_metric_input.py` & `nuon-0.19.95/nuon/models/service_publish_metric_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_rendered_install.py` & `nuon-0.19.95/nuon/models/service_rendered_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_rendered_installer.py` & `nuon-0.19.95/nuon/models/service_rendered_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_repository.py` & `nuon-0.19.95/nuon/models/service_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_update_app_installer_request.py` & `nuon-0.19.95/nuon/models/service_update_app_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/nuon/models/service_update_app_installer_request_links.py` & `nuon-0.19.95/nuon/models/service_update_app_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/nuon/models/service_update_app_request.py` & `nuon-0.19.95/nuon/models/service_update_app_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_update_component_request.py` & `nuon-0.19.95/nuon/models/service_update_component_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_update_install_request.py` & `nuon-0.19.95/nuon/models/service_update_install_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_update_installer_request.py` & `nuon-0.19.95/nuon/models/service_update_installer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_update_installer_request_links.py` & `nuon-0.19.95/nuon/models/service_update_installer_request_links.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/service_update_org_request.py` & `nuon-0.19.95/nuon/models/service_update_org_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/statsd_event.py` & `nuon-0.19.95/nuon/models/statsd_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/statsd_event_alert_type.py` & `nuon-0.19.95/nuon/models/statsd_event_alert_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/statsd_event_priority.py` & `nuon-0.19.95/nuon/models/statsd_event_priority.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/models/stderr_err_response.py` & `nuon-0.19.95/nuon/models/stderr_err_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon/rest.py` & `nuon-0.19.95/nuon/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.94/nuon.egg-info/SOURCES.txt` & `nuon-0.19.95/nuon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 nuon/models/app_app_input_config.py
 nuon/models/app_app_installer.py
 nuon/models/app_app_installer_metadata.py
 nuon/models/app_app_runner_config.py
 nuon/models/app_app_runner_type.py
 nuon/models/app_app_sandbox_config.py
 nuon/models/app_app_sandbox_config_artifacts.py
+nuon/models/app_app_secret.py
 nuon/models/app_aws_account.py
 nuon/models/app_awsecr_image_config.py
 nuon/models/app_azure_account.py
 nuon/models/app_cloud_platform.py
 nuon/models/app_component.py
 nuon/models/app_component_build.py
 nuon/models/app_component_config_connection.py
@@ -89,14 +90,15 @@
 nuon/models/service_create_app_config_request.py
 nuon/models/service_create_app_input_config_request.py
 nuon/models/service_create_app_installer_request.py
 nuon/models/service_create_app_installer_request_links.py
 nuon/models/service_create_app_request.py
 nuon/models/service_create_app_runner_config_request.py
 nuon/models/service_create_app_sandbox_config_request.py
+nuon/models/service_create_app_secret_request.py
 nuon/models/service_create_component_build_request.py
 nuon/models/service_create_component_release_request.py
 nuon/models/service_create_component_release_request_strategy.py
 nuon/models/service_create_component_request.py
 nuon/models/service_create_connection_callback_request.py
 nuon/models/service_create_connection_request.py
 nuon/models/service_create_docker_build_component_config_request.py
@@ -138,14 +140,15 @@
 test/test_app_app_input_config.py
 test/test_app_app_installer.py
 test/test_app_app_installer_metadata.py
 test/test_app_app_runner_config.py
 test/test_app_app_runner_type.py
 test/test_app_app_sandbox_config.py
 test/test_app_app_sandbox_config_artifacts.py
+test/test_app_app_secret.py
 test/test_app_aws_account.py
 test/test_app_awsecr_image_config.py
 test/test_app_azure_account.py
 test/test_app_cloud_platform.py
 test/test_app_component.py
 test/test_app_component_build.py
 test/test_app_component_config_connection.py
@@ -202,14 +205,15 @@
 test/test_service_create_app_config_request.py
 test/test_service_create_app_input_config_request.py
 test/test_service_create_app_installer_request.py
 test/test_service_create_app_installer_request_links.py
 test/test_service_create_app_request.py
 test/test_service_create_app_runner_config_request.py
 test/test_service_create_app_sandbox_config_request.py
+test/test_service_create_app_secret_request.py
 test/test_service_create_component_build_request.py
 test/test_service_create_component_release_request.py
 test/test_service_create_component_release_request_strategy.py
 test/test_service_create_component_request.py
 test/test_service_create_connection_callback_request.py
 test/test_service_create_connection_request.py
 test/test_service_create_docker_build_component_config_request.py
```

### Comparing `nuon-0.19.94/pyproject.toml` & `nuon-0.19.95/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuon"
-version = "0.19.94"
+version = "0.19.95"
 description = "Nuon"
 authors = ["Nuon Support <support@nuon.co>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Nuon"]
 include = ["nuon/py.typed"]
```

### Comparing `nuon-0.19.94/setup.py` & `nuon-0.19.95/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.94
+    The version of the OpenAPI document: 0.19.95
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "nuon"
-VERSION = "0.19.94"
+VERSION = "0.19.95"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `nuon-0.19.94/test/test_app_app.py` & `nuon-0.19.95/test/test_app_app.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_config.py` & `nuon-0.19.95/test/test_app_app_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_config_fmt.py` & `nuon-0.19.95/test/test_app_app_config_fmt.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_config_status.py` & `nuon-0.19.95/test/test_app_app_config_status.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_input.py` & `nuon-0.19.95/test/test_app_app_input.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_input_config.py` & `nuon-0.19.95/test/test_app_app_input_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_installer.py` & `nuon-0.19.95/test/test_app_app_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_installer_metadata.py` & `nuon-0.19.95/test/test_app_app_installer_metadata.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_runner_config.py` & `nuon-0.19.95/test/test_app_app_runner_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_runner_type.py` & `nuon-0.19.95/test/test_app_app_runner_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_sandbox_config.py` & `nuon-0.19.95/test/test_app_app_sandbox_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_app_sandbox_config_artifacts.py` & `nuon-0.19.95/test/test_app_app_sandbox_config_artifacts.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_aws_account.py` & `nuon-0.19.95/test/test_app_aws_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_awsecr_image_config.py` & `nuon-0.19.95/test/test_app_awsecr_image_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_azure_account.py` & `nuon-0.19.95/test/test_app_azure_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_cloud_platform.py` & `nuon-0.19.95/test/test_app_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_component.py` & `nuon-0.19.95/test/test_app_component.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_component_build.py` & `nuon-0.19.95/test/test_app_component_build.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_component_config_connection.py` & `nuon-0.19.95/test/test_app_component_config_connection.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_component_release.py` & `nuon-0.19.95/test/test_app_component_release.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_component_release_step.py` & `nuon-0.19.95/test/test_app_component_release_step.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_connected_github_vcs_config.py` & `nuon-0.19.95/test/test_app_connected_github_vcs_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_docker_build_component_config.py` & `nuon-0.19.95/test/test_app_docker_build_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_external_image_component_config.py` & `nuon-0.19.95/test/test_app_external_image_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_helm_component_config.py` & `nuon-0.19.95/test/test_app_helm_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_install.py` & `nuon-0.19.95/test/test_app_install.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_install_component.py` & `nuon-0.19.95/test/test_app_install_component.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_install_deploy.py` & `nuon-0.19.95/test/test_app_install_deploy.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_install_deploy_type.py` & `nuon-0.19.95/test/test_app_install_deploy_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_install_event.py` & `nuon-0.19.95/test/test_app_install_event.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_install_inputs.py` & `nuon-0.19.95/test/test_app_install_inputs.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_install_sandbox_run.py` & `nuon-0.19.95/test/test_app_install_sandbox_run.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_job_component_config.py` & `nuon-0.19.95/test/test_app_job_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_operation_status.py` & `nuon-0.19.95/test/test_app_operation_status.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_org.py` & `nuon-0.19.95/test/test_app_org.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_org_health_check.py` & `nuon-0.19.95/test/test_app_org_health_check.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_org_health_check_status.py` & `nuon-0.19.95/test/test_app_org_health_check_status.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_public_git_vcs_config.py` & `nuon-0.19.95/test/test_app_public_git_vcs_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_sandbox.py` & `nuon-0.19.95/test/test_app_sandbox.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_sandbox_release.py` & `nuon-0.19.95/test/test_app_sandbox_release.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_sandbox_run_type.py` & `nuon-0.19.95/test/test_app_sandbox_run_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_terraform_module_component_config.py` & `nuon-0.19.95/test/test_app_terraform_module_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_token_type.py` & `nuon-0.19.95/test/test_app_token_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_user_org.py` & `nuon-0.19.95/test/test_app_user_org.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_user_token.py` & `nuon-0.19.95/test/test_app_user_token.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_vcs_connection.py` & `nuon-0.19.95/test/test_app_vcs_connection.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_app_vcs_connection_commit.py` & `nuon-0.19.95/test/test_app_vcs_connection_commit.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_apps_api.py` & `nuon-0.19.95/test/test_apps_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_components_api.py` & `nuon-0.19.95/test/test_components_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_general_api.py` & `nuon-0.19.95/test/test_general_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py` & `nuon-0.19.95/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_installers_api.py` & `nuon-0.19.95/test/test_installers_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_installs_api.py` & `nuon-0.19.95/test/test_installs_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_metrics_decr.py` & `nuon-0.19.95/test/test_metrics_decr.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_metrics_event.py` & `nuon-0.19.95/test/test_metrics_event.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_metrics_incr.py` & `nuon-0.19.95/test/test_metrics_incr.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_metrics_timing.py` & `nuon-0.19.95/test/test_metrics_timing.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_orgs_api.py` & `nuon-0.19.95/test/test_orgs_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_planv1_plan.py` & `nuon-0.19.95/test/test_planv1_plan.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_releases_api.py` & `nuon-0.19.95/test/test_releases_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_sandboxes_api.py` & `nuon-0.19.95/test/test_sandboxes_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_app_config_template.py` & `nuon-0.19.95/test/test_service_app_config_template.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_app_config_template_type.py` & `nuon-0.19.95/test/test_service_app_config_template_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_app_input_request.py` & `nuon-0.19.95/test/test_service_app_input_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_app_installer.py` & `nuon-0.19.95/test/test_service_app_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_aws_ecr_image_config_request.py` & `nuon-0.19.95/test/test_service_aws_ecr_image_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_cli_config.py` & `nuon-0.19.95/test/test_service_cli_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_connected_github_vcs_config_request.py` & `nuon-0.19.95/test/test_service_connected_github_vcs_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_connected_github_vcs_sandbox_config_request.py` & `nuon-0.19.95/test/test_service_connected_github_vcs_sandbox_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_app_config_request.py` & `nuon-0.19.95/test/test_service_create_app_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_app_input_config_request.py` & `nuon-0.19.95/test/test_service_create_app_input_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_app_installer_request.py` & `nuon-0.19.95/test/test_service_create_app_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_app_installer_request_links.py` & `nuon-0.19.95/test/test_service_create_app_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_app_request.py` & `nuon-0.19.95/test/test_service_create_app_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_app_runner_config_request.py` & `nuon-0.19.95/test/test_service_create_app_runner_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_app_sandbox_config_request.py` & `nuon-0.19.95/test/test_service_create_app_sandbox_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_component_build_request.py` & `nuon-0.19.95/test/test_service_create_component_build_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_component_release_request.py` & `nuon-0.19.95/test/test_service_create_component_release_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_component_release_request_strategy.py` & `nuon-0.19.95/test/test_service_create_component_release_request_strategy.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_component_request.py` & `nuon-0.19.95/test/test_service_create_component_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_connection_callback_request.py` & `nuon-0.19.95/test/test_service_create_connection_callback_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_connection_request.py` & `nuon-0.19.95/test/test_service_create_connection_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_docker_build_component_config_request.py` & `nuon-0.19.95/test/test_service_create_docker_build_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_external_image_component_config_request.py` & `nuon-0.19.95/test/test_service_create_external_image_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_helm_component_config_request.py` & `nuon-0.19.95/test/test_service_create_helm_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_install_deploy_request.py` & `nuon-0.19.95/test/test_service_create_install_deploy_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_install_inputs_request.py` & `nuon-0.19.95/test/test_service_create_install_inputs_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_install_request.py` & `nuon-0.19.95/test/test_service_create_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_install_request_aws_account.py` & `nuon-0.19.95/test/test_service_create_install_request_aws_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_install_request_azure_account.py` & `nuon-0.19.95/test/test_service_create_install_request_azure_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_job_component_config_request.py` & `nuon-0.19.95/test/test_service_create_job_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_org_request.py` & `nuon-0.19.95/test/test_service_create_org_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_org_user_request.py` & `nuon-0.19.95/test/test_service_create_org_user_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_create_terraform_module_component_config_request.py` & `nuon-0.19.95/test/test_service_create_terraform_module_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_installer_create_install_request.py` & `nuon-0.19.95/test/test_service_installer_create_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_public_git_vcs_config_request.py` & `nuon-0.19.95/test/test_service_public_git_vcs_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_public_git_vcs_sandbox_config_request.py` & `nuon-0.19.95/test/test_service_public_git_vcs_sandbox_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_publish_metric_input.py` & `nuon-0.19.95/test/test_service_publish_metric_input.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_rendered_install.py` & `nuon-0.19.95/test/test_service_rendered_install.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_rendered_installer.py` & `nuon-0.19.95/test/test_service_rendered_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_repository.py` & `nuon-0.19.95/test/test_service_repository.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_app_installer_request.py` & `nuon-0.19.95/test/test_service_update_app_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_app_installer_request_links.py` & `nuon-0.19.95/test/test_service_update_app_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_app_request.py` & `nuon-0.19.95/test/test_service_update_app_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_component_request.py` & `nuon-0.19.95/test/test_service_update_component_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_install_request.py` & `nuon-0.19.95/test/test_service_update_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_installer_request.py` & `nuon-0.19.95/test/test_service_update_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_installer_request_links.py` & `nuon-0.19.95/test/test_service_update_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_service_update_org_request.py` & `nuon-0.19.95/test/test_service_update_org_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_statsd_event.py` & `nuon-0.19.95/test/test_statsd_event.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_statsd_event_alert_type.py` & `nuon-0.19.95/test/test_statsd_event_alert_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_statsd_event_priority.py` & `nuon-0.19.95/test/test_statsd_event_priority.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_stderr_err_response.py` & `nuon-0.19.95/test/test_stderr_err_response.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.94/test/test_vcs_api.py` & `nuon-0.19.95/test/test_vcs_api.py`

 * *Files identical despite different names*

