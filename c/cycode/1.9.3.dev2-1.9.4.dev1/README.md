# Comparing `tmp/cycode-1.9.3.dev2.tar.gz` & `tmp/cycode-1.9.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-1.9.3.dev2.tar", max compression
+gzip compressed data, was "cycode-1.9.4.dev1.tar", max compression
```

## Comparing `cycode-1.9.3.dev2.tar` & `cycode-1.9.4.dev1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0    42529 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/README.md
--rw-r--r--   0        0        0      114 2024-04-05 09:56:52.765673 cycode-1.9.3.dev2/cycode/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/auth/__init__.py
--rw-r--r--   0        0        0     2897 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/auth/auth_command.py
--rw-r--r--   0        0        0     4722 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/auth/auth_manager.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/configure/__init__.py
--rw-r--r--   0        0        0     5423 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/configure/configure_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/ignore/__init__.py
--rw-r--r--   0        0        0     3873 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/ignore/ignore_command.py
--rw-r--r--   0        0        0     2497 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/main_cli.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/__init__.py
--rw-r--r--   0        0        0      563 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/report_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/__init__.py
--rw-r--r--   0        0        0     3429 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/common.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/path/__init__.py
--rw-r--r--   0        0        0     2821 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/path/path_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/repository_url/__init__.py
--rw-r--r--   0        0        0     2143 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
--rw-r--r--   0        0        0     2358 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/sbom_command.py
--rw-r--r--   0        0        0     1533 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/scan/__init__.py
--rw-r--r--   0        0        0    38706 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/scan/code_scanner.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/scan/commit_history/__init__.py
--rw-r--r--   0        0        0      975 2024-04-05 09:56:41.489692 cycode-1.9.3.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/path/__init__.py
--rw-r--r--   0        0        0      590 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/path/path_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/pre_commit/__init__.py
--rw-r--r--   0        0        0     1605 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/pre_receive/__init__.py
--rw-r--r--   0        0        0     2699 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/repository/__init__.py
--rw-r--r--   0        0        0     2710 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/repository/repository_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/scan_ci/__init__.py
--rw-r--r--   0        0        0     1588 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py
--rw-r--r--   0        0        0      552 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
--rw-r--r--   0        0        0     5082 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/scan/scan_command.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/version/__init__.py
--rw-r--r--   0        0        0      509 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/commands/version/version_command.py
--rw-r--r--   0        0        0      466 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/config.py
--rw-r--r--   0        0        0      463 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/config.yaml
--rw-r--r--   0        0        0     6154 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py
--rw-r--r--   0        0        0     2785 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/exceptions/handle_scan_errors.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/__init__.py
--rw-r--r--   0        0        0     5468 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/excluder.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/iac/__init__.py
--rw-r--r--   0        0        0     2457 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/iac/tf_content_generator.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/models/__init__.py
--rw-r--r--   0        0        0      922 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/models/in_memory_zip.py
--rw-r--r--   0        0        0     4393 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/path_documents.py
--rw-r--r--   0        0        0     4940 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/repository_documents.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/sca/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/sca/maven/__init__.py
--rw-r--r--   0        0        0     2417 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0     1136 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     3119 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     6398 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py
--rw-r--r--   0        0        0     1522 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/files_collector/zip_documents.py
--rw-r--r--   0        0        0      387 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/main.py
--rw-r--r--   0        0        0     2051 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0     2395 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     2290 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     1410 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/printer_base.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/tables/__init__.py
--rw-r--r--   0        0        0     7660 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/tables/sca_table_printer.py
--rw-r--r--   0        0        0     2281 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/tables/table.py
--rw-r--r--   0        0        0      480 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/tables/table_models.py
--rw-r--r--   0        0        0     5216 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/tables/table_printer.py
--rw-r--r--   0        0        0     2400 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/tables/table_printer_base.py
--rw-r--r--   0        0        0    10484 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      630 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4939 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7286 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     2987 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0      745 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/user_settings/jwt_creator.py
--rw-r--r--   0        0        0        0 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      211 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     1584 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/get_api_client.py
--rw-r--r--   0        0        0     1953 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     9716 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2794 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      978 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2034 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2748 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      934 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0       71 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1777 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     1072 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/client_creator.py
--rw-r--r--   0        0        0     2891 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      257 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     4073 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      670 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     3600 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0    13148 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/models.py
--rw-r--r--   0        0        0     3971 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/report_client.py
--rw-r--r--   0        0        0    13449 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0     1658 2024-04-05 09:56:41.493692 cycode-1.9.3.dev2/cycode/cyclient/scan_config_base.py
--rw-r--r--   0        0        0     3458 2024-04-05 09:56:52.765673 cycode-1.9.3.dev2/pyproject.toml
--rw-r--r--   0        0        0    44107 1970-01-01 00:00:00.000000 cycode-1.9.3.dev2/PKG-INFO
+-rw-r--r--   0        0        0    42529 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/README.md
+-rw-r--r--   0        0        0      114 2024-04-10 10:08:13.788381 cycode-1.9.4.dev1/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/auth/__init__.py
+-rw-r--r--   0        0        0     2897 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/auth/auth_command.py
+-rw-r--r--   0        0        0     4722 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/auth/auth_manager.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/configure/__init__.py
+-rw-r--r--   0        0        0     5423 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/configure/configure_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/ignore/__init__.py
+-rw-r--r--   0        0        0     3873 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/ignore/ignore_command.py
+-rw-r--r--   0        0        0     2497 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/main_cli.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/report_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/__init__.py
+-rw-r--r--   0        0        0     3429 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/common.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/path/__init__.py
+-rw-r--r--   0        0        0     2821 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/repository_url/__init__.py
+-rw-r--r--   0        0        0     2143 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
+-rw-r--r--   0        0        0     2358 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/sbom_command.py
+-rw-r--r--   0        0        0     1533 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/sbom_report_file.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/__init__.py
+-rw-r--r--   0        0        0    38706 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/code_scanner.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/commit_history/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/commit_history/commit_history_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/path/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/pre_commit/__init__.py
+-rw-r--r--   0        0        0     1605 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.040381 cycode-1.9.4.dev1/cycode/cli/commands/scan/pre_receive/__init__.py
+-rw-r--r--   0        0        0     2699 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/scan/repository/__init__.py
+-rw-r--r--   0        0        0     2710 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/scan/repository/repository_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/scan/scan_ci/__init__.py
+-rw-r--r--   0        0        0     1588 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/scan/scan_ci/ci_integrations.py
+-rw-r--r--   0        0        0      552 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
+-rw-r--r--   0        0        0     5082 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/scan/scan_command.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/version/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/commands/version/version_command.py
+-rw-r--r--   0        0        0      466 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/config.py
+-rw-r--r--   0        0        0      463 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     6194 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/exceptions/handle_report_sbom_errors.py
+-rw-r--r--   0        0        0     2785 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/exceptions/handle_scan_errors.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/__init__.py
+-rw-r--r--   0        0        0     5468 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/excluder.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/iac/__init__.py
+-rw-r--r--   0        0        0     2457 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/iac/tf_content_generator.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/models/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/models/in_memory_zip.py
+-rw-r--r--   0        0        0     4393 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/path_documents.py
+-rw-r--r--   0        0        0     4940 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/repository_documents.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/sca/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/sca/maven/__init__.py
+-rw-r--r--   0        0        0     2417 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0     1136 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     3119 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     6398 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/sca/sca_code_scanner.py
+-rw-r--r--   0        0        0     1836 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/files_collector/zip_documents.py
+-rw-r--r--   0        0        0      387 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/main.py
+-rw-r--r--   0        0        0     2051 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     2290 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     1410 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/printer_base.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/tables/__init__.py
+-rw-r--r--   0        0        0     7660 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/tables/sca_table_printer.py
+-rw-r--r--   0        0        0     2281 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/tables/table.py
+-rw-r--r--   0        0        0      480 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/tables/table_models.py
+-rw-r--r--   0        0        0     5216 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/tables/table_printer.py
+-rw-r--r--   0        0        0     2400 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/tables/table_printer_base.py
+-rw-r--r--   0        0        0    10484 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      630 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4939 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7591 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     2987 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0      745 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/user_settings/jwt_creator.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      211 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     1584 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/get_api_client.py
+-rw-r--r--   0        0        0     1953 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     9716 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2794 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      978 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2034 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2748 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      934 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0       71 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1777 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     1072 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/client_creator.py
+-rw-r--r--   0        0        0     2891 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      257 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     4073 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      670 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     3600 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0    13148 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     3971 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/report_client.py
+-rw-r--r--   0        0        0    13449 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0     1658 2024-04-10 10:07:59.044381 cycode-1.9.4.dev1/cycode/cyclient/scan_config_base.py
+-rw-r--r--   0        0        0     3458 2024-04-10 10:08:13.784381 cycode-1.9.4.dev1/pyproject.toml
+-rw-r--r--   0        0        0    44107 1970-01-01 00:00:00.000000 cycode-1.9.4.dev1/PKG-INFO
```

### Comparing `cycode-1.9.3.dev2/README.md` & `cycode-1.9.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/auth/auth_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/auth/auth_manager.py` & `cycode-1.9.4.dev1/cycode/cli/commands/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/configure/configure_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/configure/configure_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/ignore/ignore_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/ignore/ignore_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/main_cli.py` & `cycode-1.9.4.dev1/cycode/cli/commands/main_cli.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/report/report_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/report/report_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/common.py` & `cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/common.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/path/path_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/sbom_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/sbom_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py` & `cycode-1.9.4.dev1/cycode/cli/commands/report/sbom/sbom_report_file.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/code_scanner.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/commit_history/commit_history_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/path/path_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/pre_commit/pre_commit_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/pre_receive/pre_receive_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/repository/repository_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/repository/repository_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/scan_ci/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/scan_ci/scan_ci_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/commands/scan/scan_command.py` & `cycode-1.9.4.dev1/cycode/cli/commands/scan/scan_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/consts.py` & `cycode-1.9.4.dev1/cycode/cli/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 # env var names
 CYCODE_API_URL_ENV_VAR_NAME = 'CYCODE_API_URL'
 CYCODE_APP_URL_ENV_VAR_NAME = 'CYCODE_APP_URL'
 TIMEOUT_ENV_VAR_NAME = 'TIMEOUT'
 CYCODE_CLI_REQUEST_TIMEOUT_ENV_VAR_NAME = 'CYCODE_CLI_REQUEST_TIMEOUT'
 LOGGING_LEVEL_ENV_VAR_NAME = 'LOGGING_LEVEL'
 VERBOSE_ENV_VAR_NAME = 'CYCODE_CLI_VERBOSE'
+DEBUG_ENV_VAR_NAME = 'CYCODE_CLI_DEBUG'
 
 CYCODE_CONFIGURATION_DIRECTORY: str = '.cycode'
 
 # user configuration sections names
 EXCLUSIONS_BY_VALUE_SECTION_NAME = 'values'
 EXCLUSIONS_BY_SHA_SECTION_NAME = 'shas'
 EXCLUSIONS_BY_PATH_SECTION_NAME = 'paths'
```

### Comparing `cycode-1.9.3.dev2/cycode/cli/exceptions/custom_exceptions.py` & `cycode-1.9.4.dev1/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py` & `cycode-1.9.4.dev1/cycode/cli/exceptions/handle_report_sbom_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/exceptions/handle_scan_errors.py` & `cycode-1.9.4.dev1/cycode/cli/exceptions/handle_scan_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/excluder.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/excluder.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/iac/tf_content_generator.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/iac/tf_content_generator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/models/in_memory_zip.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/models/in_memory_zip.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from io import BytesIO
 from sys import getsizeof
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 from zipfile import ZIP_DEFLATED, ZipFile
 
+from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 from cycode.cli.utils.path_utils import concat_unique_id
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 class InMemoryZip(object):
     def __init__(self) -> None:
+        self.configuration_manager = ConfigurationManager()
+
         # Create the in-memory file-like object
         self.in_memory_zip = BytesIO()
         self.zip = ZipFile(self.in_memory_zip, 'a', ZIP_DEFLATED, False)
 
     def append(self, filename: str, unique_id: Optional[str], content: str) -> None:
         # Write the file to the in-memory zip
         if unique_id:
@@ -23,10 +29,14 @@
         self.zip.close()
 
     # to bytes
     def read(self) -> bytes:
         self.in_memory_zip.seek(0)
         return self.in_memory_zip.read()
 
+    def write_on_disk(self, path: 'Path') -> None:
+        with open(path, 'wb') as f:
+            f.write(self.read())
+
     @property
     def size(self) -> int:
         return getsizeof(self.in_memory_zip)
```

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/path_documents.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/path_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/repository_documents.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/repository_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/sca/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/files_collector/zip_documents.py` & `cycode-1.9.4.dev1/cycode/cli/files_collector/zip_documents.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from pathlib import Path
 from typing import List, Optional
 
 from cycode.cli import consts
 from cycode.cli.exceptions import custom_exceptions
 from cycode.cli.files_collector.models.in_memory_zip import InMemoryZip
 from cycode.cli.models import Document
 from cycode.cyclient import logger
@@ -33,8 +34,13 @@
 
     zip_file.close()
 
     end_zip_creation_time = time.time()
     zip_creation_time = int(end_zip_creation_time - start_zip_creation_time)
     logger.debug('finished to create zip file, %s', {'zip_creation_time': zip_creation_time})
 
+    if zip_file.configuration_manager.get_debug_flag():
+        zip_file_path = Path.joinpath(Path.cwd(), f'{scan_type}_scan_{end_zip_creation_time}.zip')
+        logger.debug('writing zip file to disk, %s', {'zip_file_path': zip_file_path})
+        zip_file.write_on_disk(zip_file_path)
+
     return zip_file
```

### Comparing `cycode-1.9.3.dev2/cycode/cli/models.py` & `cycode-1.9.4.dev1/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/console_printer.py` & `cycode-1.9.4.dev1/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/json_printer.py` & `cycode-1.9.4.dev1/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/printer_base.py` & `cycode-1.9.4.dev1/cycode/cli/printers/printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/tables/sca_table_printer.py` & `cycode-1.9.4.dev1/cycode/cli/printers/tables/sca_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/tables/table.py` & `cycode-1.9.4.dev1/cycode/cli/printers/tables/table.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/tables/table_printer.py` & `cycode-1.9.4.dev1/cycode/cli/printers/tables/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/tables/table_printer_base.py` & `cycode-1.9.4.dev1/cycode/cli/printers/tables/table_printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/printers/text_printer.py` & `cycode-1.9.4.dev1/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/user_settings/base_file_manager.py` & `cycode-1.9.4.dev1/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/user_settings/config_file_manager.py` & `cycode-1.9.4.dev1/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/user_settings/configuration_manager.py` & `cycode-1.9.4.dev1/cycode/cli/user_settings/configuration_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 
         app_url = self.global_config_file_manager.get_app_url()
         if app_url is not None:
             return app_url
 
         return consts.DEFAULT_CYCODE_APP_URL
 
+    def get_debug_flag_from_environment_variables(self) -> bool:
+        value = self._get_value_from_environment_variables(consts.DEBUG_ENV_VAR_NAME, '')
+        return value.lower() in {'true', '1'}
+
+    def get_debug_flag(self) -> bool:
+        return self.get_debug_flag_from_environment_variables()
+
     def get_verbose_flag(self) -> bool:
         verbose_flag_env_var = self.get_verbose_flag_from_environment_variables()
         verbose_flag_local_config = self.local_config_file_manager.get_verbose_flag()
         verbose_flag_global_config = self.global_config_file_manager.get_verbose_flag()
         return verbose_flag_env_var or verbose_flag_local_config or verbose_flag_global_config
 
     def get_api_url_from_environment_variables(self) -> Optional[str]:
```

### Comparing `cycode-1.9.3.dev2/cycode/cli/user_settings/credentials_manager.py` & `cycode-1.9.4.dev1/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/user_settings/jwt_creator.py` & `cycode-1.9.4.dev1/cycode/cli/user_settings/jwt_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/get_api_client.py` & `cycode-1.9.4.dev1/cycode/cli/utils/get_api_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/path_utils.py` & `cycode-1.9.4.dev1/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/progress_bar.py` & `cycode-1.9.4.dev1/cycode/cli/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/scan_batch.py` & `cycode-1.9.4.dev1/cycode/cli/utils/scan_batch.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/shell_executor.py` & `cycode-1.9.4.dev1/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/string_utils.py` & `cycode-1.9.4.dev1/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/task_timer.py` & `cycode-1.9.4.dev1/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cli/utils/yaml_utils.py` & `cycode-1.9.4.dev1/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/auth_client.py` & `cycode-1.9.4.dev1/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/client_creator.py` & `cycode-1.9.4.dev1/cycode/cyclient/client_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/config.py` & `cycode-1.9.4.dev1/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/cycode_client_base.py` & `cycode-1.9.4.dev1/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/cycode_dev_based_client.py` & `cycode-1.9.4.dev1/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/cycode_token_based_client.py` & `cycode-1.9.4.dev1/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/models.py` & `cycode-1.9.4.dev1/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/report_client.py` & `cycode-1.9.4.dev1/cycode/cyclient/report_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/scan_client.py` & `cycode-1.9.4.dev1/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/cycode/cyclient/scan_config_base.py` & `cycode-1.9.4.dev1/cycode/cyclient/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.3.dev2/pyproject.toml` & `cycode-1.9.4.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "1.9.3.dev2" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "1.9.4.dev1" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning."
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-1.9.3.dev2/PKG-INFO` & `cycode-1.9.4.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 1.9.3.dev2
+Version: 1.9.4.dev1
 Summary: Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning.
 Home-page: https://github.com/cycodehq/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.13
```

