# Comparing `tmp/robocorp_action_server-0.2.1.tar.gz` & `tmp/robocorp_action_server-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_action_server-0.2.1.tar", max compression
+gzip compressed data, was "robocorp_action_server-0.3.0.tar", max compression
```

## Comparing `robocorp_action_server-0.2.1.tar` & `robocorp_action_server-0.3.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     4055 2024-04-04 13:20:11.270397 robocorp_action_server-0.2.1/README.md
--rw-r--r--   0        0        0     1846 2024-04-04 13:20:11.270397 robocorp_action_server-0.2.1/build.py
--rw-r--r--   0        0        0     1551 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      894 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/README.md
--rw-r--r--   0        0        0      128 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/__init__.py
--rw-r--r--   0        0        0      284 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/__main__.py
--rw-r--r--   0        0        0    16696 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_import.py
--rw-r--r--   0        0        0    20512 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_process_pool.py
--rw-r--r--   0        0        0    11350 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_run.py
--rw-r--r--   0        0        0     1266 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_run_helpers.py
--rw-r--r--   0        0        0     1239 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_api_action_package.py
--rw-r--r--   0        0        0     7726 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_api_run.py
--rw-r--r--   0        0        0     2623 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_app.py
--rw-r--r--   0        0        0      775 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_cli_helpers.py
--rw-r--r--   0        0        0    21166 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_database.py
--rw-r--r--   0        0        0     1845 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_download_rcc.py
--rw-r--r--   0        0        0     3764 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_errors.py
--rw-r--r--   0        0        0      113 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_errors_action_server.py
--rw-r--r--   0        0        0      642 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_gen_ids.py
--rw-r--r--   0        0        0     5113 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_models.py
--rw-r--r--   0        0        0     2764 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_new_project.py
--rw-r--r--   0        0        0        0 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/__init__.py
--rw-r--r--   0        0        0      714 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions.py
--rw-r--r--   0        0        0     9519 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py
--rw-r--r--   0        0        0     7869 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions_streams.py
--rw-r--r--   0        0        0      587 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py
--rw-r--r--   0        0        0     4322 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_protocols.py
--rw-r--r--   0        0        0    10431 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_rcc.py
--rw-r--r--   0        0        0      426 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/auth.py
--rw-r--r--   0        0        0     1494 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/callback.py
--rw-r--r--   0        0        0     1282 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/constants.py
--rw-r--r--   0        0        0     1027 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/log_custom_handler.py
--rw-r--r--   0        0        0     1397 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/log_formatter.py
--rw-r--r--   0        0        0    19023 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/process.py
--rw-r--r--   0        0        0      692 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/run_in_thread.py
--rw-r--r--   0        0        0    13510 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/system_mutex.py
--rw-r--r--   0        0        0     4031 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_runs_state_cache.py
--rw-r--r--   0        0        0    15723 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_selftest.py
--rw-r--r--   0        0        0    11029 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_server.py
--rw-r--r--   0        0        0    16735 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_server_expose.py
--rw-r--r--   0        0        0    10278 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_server_websockets.py
--rw-r--r--   0        0        0     4746 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_settings.py
--rw-r--r--   0        0        0     1662 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_slugify.py
--rw-r--r--   0        0        0   874108 2024-04-04 13:20:57.026981 robocorp_action_server-0.2.1/src/robocorp/action_server/_static_contents.py
--rw-r--r--   0        0        0     2403 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/_whitelist.py
--rw-r--r--   0        0        0        6 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/bin/.gitignore
--rw-r--r--   0        0        0    25515 2024-04-04 13:20:11.278397 robocorp_action_server-0.2.1/src/robocorp/action_server/cli.py
--rw-r--r--   0        0        0     4611 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/migrations/__init__.py
--rw-r--r--   0        0        0      411 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/migrations/migration_add_action_enabled.py
--rw-r--r--   0        0        0      375 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/migrations/migration_add_is_consequential.py
--rw-r--r--   0        0        0      260 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/migrations/migration_initial.py
--rw-r--r--   0        0        0        0 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/package/__init__.py
--rw-r--r--   0        0        0      468 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/package/_ask_user.py
--rw-r--r--   0        0        0     7884 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/package/_package_build.py
--rw-r--r--   0        0        0     7666 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/package/_package_build_cli.py
--rw-r--r--   0        0        0     1494 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/package/_package_metadata.py
--rw-r--r--   0        0        0        0 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/py.typed
--rw-r--r--   0        0        0      349 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/README.md
--rw-r--r--   0        0        0        0 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/__init__.py
--rw-r--r--   0        0        0    14886 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py
--rw-r--r--   0        0        0      157 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/action_package_handling/cli_errors.py
--rw-r--r--   0        0        0        0 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py
--rw-r--r--   0        0        0     6112 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py
--rw-r--r--   0        0        0     1405 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py
--rw-r--r--   0        0        0     2331 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py
--rw-r--r--   0        0        0    23317 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py
--rw-r--r--   0        0        0    23813 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py
--rw-r--r--   0        0        0        0 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/__init__.py
--rw-r--r--   0        0        0      849 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
--rw-r--r--   0        0        0    11440 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
--rw-r--r--   0        0        0     9084 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
--rw-r--r--   0        0        0    13400 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
--rw-r--r--   0        0        0    25543 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
--rw-r--r--   0        0        0        0 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/__init__.py
--rw-r--r--   0        0        0     8976 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
--rw-r--r--   0        0        0     1431 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
--rw-r--r--   0        0        0    14693 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
--rw-r--r--   0        0        0     7245 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py
--rw-r--r--   0        0        0      319 2024-04-04 13:20:11.282398 robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/termcolors/__init__.py
--rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 robocorp_action_server-0.2.1/setup.py
--rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 robocorp_action_server-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4055 2024-04-10 19:55:15.126818 robocorp_action_server-0.3.0/README.md
+-rw-r--r--   0        0        0     1846 2024-04-10 19:55:15.126818 robocorp_action_server-0.3.0/build.py
+-rw-r--r--   0        0        0     1576 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      894 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/README.md
+-rw-r--r--   0        0        0      128 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/__main__.py
+-rw-r--r--   0        0        0    17906 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_import.py
+-rw-r--r--   0        0        0    20512 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_process_pool.py
+-rw-r--r--   0        0        0    11351 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_run.py
+-rw-r--r--   0        0        0     1266 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_run_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_api_action_package.py
+-rw-r--r--   0        0        0     7726 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_api_run.py
+-rw-r--r--   0        0        0     2623 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_app.py
+-rw-r--r--   0        0        0      775 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_cli_helpers.py
+-rw-r--r--   0        0        0    21166 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_database.py
+-rw-r--r--   0        0        0     1845 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_download_rcc.py
+-rw-r--r--   0        0        0     3764 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_errors.py
+-rw-r--r--   0        0        0      113 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_errors_action_server.py
+-rw-r--r--   0        0        0      642 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_gen_ids.py
+-rw-r--r--   0        0        0     5113 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_models.py
+-rw-r--r--   0        0        0     2764 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_new_project.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions.py
+-rw-r--r--   0        0        0     9519 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py
+-rw-r--r--   0        0        0     7869 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions_streams.py
+-rw-r--r--   0        0        0      587 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py
+-rw-r--r--   0        0        0     4322 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_protocols.py
+-rw-r--r--   0        0        0    10431 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_rcc.py
+-rw-r--r--   0        0        0      426 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/auth.py
+-rw-r--r--   0        0        0     1526 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/callback.py
+-rw-r--r--   0        0        0     1282 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/constants.py
+-rw-r--r--   0        0        0     1027 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/log_custom_handler.py
+-rw-r--r--   0        0        0     1397 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/log_formatter.py
+-rw-r--r--   0        0        0    19023 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/process.py
+-rw-r--r--   0        0        0      692 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/run_in_thread.py
+-rw-r--r--   0        0        0    13510 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/system_mutex.py
+-rw-r--r--   0        0        0     4031 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_runs_state_cache.py
+-rw-r--r--   0        0        0    15845 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_selftest.py
+-rw-r--r--   0        0        0    11168 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_server.py
+-rw-r--r--   0        0        0    16735 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_server_expose.py
+-rw-r--r--   0        0        0    10278 2024-04-10 19:55:15.134818 robocorp_action_server-0.3.0/src/robocorp/action_server/_server_websockets.py
+-rw-r--r--   0        0        0     4746 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/_settings.py
+-rw-r--r--   0        0        0     1662 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/_slugify.py
+-rw-r--r--   0        0        0   874108 2024-04-10 19:56:05.370564 robocorp_action_server-0.3.0/src/robocorp/action_server/_static_contents.py
+-rw-r--r--   0        0        0     2403 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/_whitelist.py
+-rw-r--r--   0        0        0        6 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/bin/.gitignore
+-rw-r--r--   0        0        0    25515 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/cli.py
+-rw-r--r--   0        0        0     4611 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/migrations/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/migrations/migration_add_action_enabled.py
+-rw-r--r--   0        0        0      375 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/migrations/migration_add_is_consequential.py
+-rw-r--r--   0        0        0      260 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/migrations/migration_initial.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/package/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/package/_ask_user.py
+-rw-r--r--   0        0        0     7884 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/package/_package_build.py
+-rw-r--r--   0        0        0     7666 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/package/_package_build_cli.py
+-rw-r--r--   0        0        0     2854 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/package/_package_metadata.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/py.typed
+-rw-r--r--   0        0        0      349 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/__init__.py
+-rw-r--r--   0        0        0    14886 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/action_package_handling/cli_errors.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py
+-rw-r--r--   0        0        0     6112 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py
+-rw-r--r--   0        0        0     1405 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py
+-rw-r--r--   0        0        0     2331 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py
+-rw-r--r--   0        0        0    23317 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py
+-rw-r--r--   0        0        0    23813 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
+-rw-r--r--   0        0        0    11440 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
+-rw-r--r--   0        0        0     9084 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
+-rw-r--r--   0        0        0    13400 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
+-rw-r--r--   0        0        0    25543 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/__init__.py
+-rw-r--r--   0        0        0     8976 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
+-rw-r--r--   0        0        0     1431 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
+-rw-r--r--   0        0        0    14693 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
+-rw-r--r--   0        0        0     7245 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py
+-rw-r--r--   0        0        0      319 2024-04-10 19:55:15.138818 robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/termcolors/__init__.py
+-rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 robocorp_action_server-0.3.0/setup.py
+-rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 robocorp_action_server-0.3.0/PKG-INFO
```

### Comparing `robocorp_action_server-0.2.1/README.md` & `robocorp_action_server-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/build.py` & `robocorp_action_server-0.3.0/build.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/pyproject.toml` & `robocorp_action_server-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-action-server"
-version = "0.2.1"
+version = "0.3.0"
 description = "Robocorp local task server"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
@@ -29,18 +29,19 @@
 jsonschema = "^4.19.2"
 msgspec = "^0.18"
 psutil = "^5"
 pydantic = "^2.4.2"
 pyyaml = "^6"
 python = "^3.10"
 requests = "^2"
-robocorp-actions = "^0.1.0"
+robocorp-actions = "^0.2.0"
 termcolor = "^2.4.0"
 uvicorn = "^0.23.2"
 websockets = "^12.0"
+cryptography = "^42.0.5"
 
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = { path = "../devutils/", develop = true }
 types-requests = "^2"
 types-PyYAML = "^6"
 robocorp-log-pytest = "^0.0.2"
```

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/README.md` & `robocorp_action_server-0.3.0/src/robocorp/action_server/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_import.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,56 @@
 import subprocess
 import sys
 import typing
 from pathlib import Path
 
 from termcolor import colored
 
+from robocorp.action_server._robo_utils.callback import Callback, OnExitContextManager
 from robocorp.action_server.vendored_deps.action_package_handling.cli_errors import (
     ActionPackageError,
 )
 from robocorp.action_server.vendored_deps.termcolors import bold_red, bold_yellow
 
 if typing.TYPE_CHECKING:
+    from robocorp.actions._protocols import ActionsListActionTypedDict
+
     from robocorp.action_server._models import ActionPackage
 
 log = logging.getLogger(__name__)
 
 
+class IHookOnActionsListCallback(typing.Protocol):
+    def __call__(
+        self,
+        action_package: "ActionPackage",
+        actions_list_result: list["ActionsListActionTypedDict"],
+    ):
+        ...
+
+
+class IHookOnActionsList(typing.Protocol):
+    def register(
+        self,
+        callback: IHookOnActionsListCallback,
+    ) -> OnExitContextManager:
+        ...
+
+    def __call__(
+        self,
+        action_package: "ActionPackage",
+        actions_list_result: list["ActionsListActionTypedDict"],
+    ):
+        ...
+
+
+# Called as: hook_on_actions_list(action_package, actions_list_result)
+hook_on_actions_list: IHookOnActionsList = Callback(raise_exceptions=True)
+
+
 def _log_deprecated_conda():
     from robocorp.action_server._settings import is_frozen
 
     if is_frozen():
         cmd = "action-server"
     else:
         cmd = "python -m robocorp.action_server"
@@ -341,22 +372,32 @@
 
     # If it didn't fail the import, consider as warning (and thus print in yellow).
     decoded_stderr = stderr.decode("utf-8", "replace").strip()
     if decoded_stderr:
         log.critical(bold_yellow(f"{decoded_stderr}\n"))
 
     try:
-        loaded = json.loads(stdout)
+        actions_list_result = json.loads(stdout)
     except json.JSONDecodeError:
         raise RuntimeError(
             f"It was not possible to load as json the contents >>{stdout!r}<<"
         )
     else:
+        if not isinstance(actions_list_result, list):
+            raise RuntimeError(
+                f"Expected robocorp.actions list to provide a list. Found: >>{stdout!r}<<"
+            )
+
+        hook_on_actions_list(
+            action_package,
+            typing.cast(list["ActionsListActionTypedDict"], actions_list_result),
+        )
+
         actions = []
-        for action_fields in loaded:
+        for action_fields in actions_list_result:
             action_name = action_fields["name"]
             if whitelist:
                 if not accept_action(whitelist, action_package.name, action_name):
                     log.info(
                         f"Action: {action_package.name}/{action_name} not imported because it has no match in the whitelist: {whitelist!r}"
                     )
                     continue
```

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_process_pool.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_process_pool.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_run.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         raise RuntimeError(
             f"Error making validator for input schema: {input_schema_dict}"
         )
     try:
         output_validator = fastjsonschema.compile(output_schema_dict)
     except Exception:
         raise RuntimeError(
-            f"Errormaking validator for output schema: {output_schema_dict}"
+            f"Error making validator for output schema: {output_schema_dict}"
         )
 
     # The returned function must be async because we have to request the `body`
 
     async def func(response: Response, request: Request):
         body = await request.body()
```

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_actions_run_helpers.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_actions_run_helpers.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_api_action_package.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_api_action_package.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_api_run.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_api_run.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_app.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_app.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_cli_helpers.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_cli_helpers.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_database.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_database.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_download_rcc.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_download_rcc.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_errors.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_errors.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_gen_ids.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_gen_ids.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_models.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_models.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_new_project.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_new_project.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions_streams.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions_streams.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_protocols.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_rcc.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_rcc.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/callback.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/callback.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     """
 
     def __init__(self, reversed=False, raise_exceptions=False):
         self.raise_exceptions = raise_exceptions
         self._reversed = reversed
         self._callbacks = ()
 
-    def register(self, callback):
+    def register(self, callback) -> OnExitContextManager:
         self._callbacks = self._callbacks + (callback,)
 
         # Enable using as a context manager to automatically call the unregister.
         return OnExitContextManager(lambda: self.unregister(callback))
 
-    def unregister(self, callback):
+    def unregister(self, callback) -> None:
         self._callbacks = tuple(x for x in self._callbacks if x != callback)
 
     def __len__(self):
         return len(self._callbacks)
 
     def __call__(self, *args, **kwargs):
         if self._reversed:
```

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/constants.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/constants.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/log_custom_handler.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/log_custom_handler.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/log_formatter.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/log_formatter.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/process.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/process.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/run_in_thread.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/run_in_thread.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_robo_utils/system_mutex.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_robo_utils/system_mutex.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_runs_state_cache.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_runs_state_cache.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_selftest.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_selftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         cwd: Optional[Path | str] = None,
         add_shutdown_api: bool = False,
         min_processes: int = 0,
         max_processes: int = 20,
         reuse_processes: bool = False,
         lint: bool = False,
         additional_args: Optional[list[str]] = None,
+        env: Optional[Dict[str, str]] = None,
     ) -> None:
         from robocorp.action_server._robo_utils.process import Process
         from robocorp.action_server._settings import is_frozen
 
         if self.started:
             raise RuntimeError("The action process was already started.")
 
@@ -120,18 +121,20 @@
         new_args.append(f"--max-processes={max_processes}")
         if reuse_processes:
             new_args.append("--reuse-processes")
 
         if additional_args:
             new_args = new_args + additional_args
 
-        env = {}
+        use_env: Dict[str, str] = {}
         if add_shutdown_api:
-            env["RC_ADD_SHUTDOWN_API"] = "1"
-        process = self._process = Process(new_args, cwd=cwd, env=env)
+            use_env["RC_ADD_SHUTDOWN_API"] = "1"
+        if env:
+            use_env.update(env)
+        process = self._process = Process(new_args, cwd=cwd, env=use_env)
 
         compiled = re.compile(r"Local Action Server: http://([\w.-]+):(\d+)")
         future: Future[Tuple[str, str]] = Future()
 
         def collect_port_from_stdout(line):
             # Note: this is called in a thread.
             matches = re.findall(compiled, line)
```

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_server.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 def _name_to_url(name):
     from robocorp.action_server._slugify import slugify
 
     return slugify(name.replace("_", "-"))
 
 
+def build_url_api_run(action_package_name: str, action_name: str) -> str:
+    return f"/api/actions/{_name_to_url(action_package_name)}/{_name_to_url(action_name)}/run"
+
+
 def get_action_description_from_docs(docs: str) -> str:
     import docstring_parser
 
     doc_desc: str
     try:
         parsed = docstring_parser.parse(docs)
         if parsed.short_description and parsed.long_description:
@@ -134,15 +138,15 @@
                 continue
 
         func, openapi_extra = _actions_run.generate_func_from_action(action)
         if action.is_consequential is not None:
             openapi_extra["x-openai-isConsequential"] = action.is_consequential
 
         app.add_api_route(
-            f"/api/actions/{_name_to_url(action_package.name)}/{_name_to_url(action.name)}/run",
+            build_url_api_run(action_package.name, action.name),
             func,
             name=action.name,
             summary=_name_as_summary(action.name),
             description=doc_desc,
             operation_id=action.name,
             methods=["POST"],
             dependencies=endpoint_dependencies,
```

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_server_expose.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_server_expose.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_server_websockets.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_server_websockets.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_settings.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_settings.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_slugify.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_slugify.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_static_contents.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_static_contents.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/_whitelist.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/_whitelist.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/cli.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/migrations/__init__.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/package/_package_build.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/package/_package_build.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/package/_package_build_cli.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/package/_package_build_cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py` & `robocorp_action_server-0.3.0/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.2.1/setup.py` & `robocorp_action_server-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,33 +19,34 @@
  'robocorp.action_server.vendored_deps.termcolors']
 
 package_data = \
 {'': ['*'], 'robocorp.action_server': ['bin/*']}
 
 install_requires = \
 ['aiohttp>=3.9.3,<4.0.0',
+ 'cryptography>=42.0.5,<43.0.0',
  'fastapi>=0.110.0,<0.111.0',
  'fastjsonschema>=2.19.1,<3.0.0',
  'jsonschema>=4.19.2,<5.0.0',
  'msgspec>=0.18,<0.19',
  'psutil>=5,<6',
  'pydantic>=2.4.2,<3.0.0',
  'pyyaml>=6,<7',
  'requests>=2,<3',
- 'robocorp-actions>=0.1.0,<0.2.0',
+ 'robocorp-actions>=0.2.0,<0.3.0',
  'termcolor>=2.4.0,<3.0.0',
  'uvicorn>=0.23.2,<0.24.0',
  'websockets>=12.0,<13.0']
 
 entry_points = \
 {'console_scripts': ['action-server = robocorp.action_server.cli:main']}
 
 setup_kwargs = {
     'name': 'robocorp-action-server',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Robocorp local task server',
     'long_description': '# robocorp-action-server\n\n[Robocorp Action Server](https://github.com/robocorp/robocorp#readme) is a Python framework designed to simplify the deployment of actions (AI or otherwise).\n\nAn `action` in this case is defined as a Python function (which has inputs/outputs defined), which is served by the `Robocorp Action Server`.\n\nThe `Robocorp Action Server` automatically generates an OpenAPI spec for your Python code, enabling different AI/LLM Agents to understand and call your Action. It also manages the Action lifecycle and provides full traceability of what happened during runs.\n\n## 1. Install Action Server\n\nAction Server is available as a stand-alone fully signed executable and via `pip install robocorp-action-server`.\n> We recommend the executable to prevent confusion in case you have multiple/crowded Python environments, etc.\n\n#### For macOS\n\n```sh\n# Install Robocorp Action Server\nbrew update\nbrew install robocorp/tools/action-server \n```\n\n#### For Windows\n\n```sh\n# Download Robocorp Action Server\ncurl -o action-server.exe https://downloads.robocorp.com/action-server/releases/latest/windows64/action-server.exe\n\n# Add to PATH or move to a folder that is in PATH\nsetx PATH=%PATH%;%CD%\n```\n\n#### For Linux\n\n```sh\n# Download Robocorp Action Server\ncurl -o action-server https://downloads.robocorp.com/action-server/releases/latest/linux64/action-server\nchmod a+x action-server\n\n# Add to PATH or move to a folder that is in PATH\nsudo mv action-server /usr/local/bin/\n```\n\n## 2. Run your first Action\n\n```sh\n# Bootstrap a new project using this template.\n# You\'ll be prompted for the name of the project (directory):\naction-server new\n\n# Start Action Server \ncd my-project\naction-server start --expose\n```\n\n👉 You should now have an Action Server running locally at: [http://localhost:8080](http://localhost:8080), so open that in your browser and the web UI will guide you further.\n\n👉 Using the `--expose` -flag, you also get a public internet-facing URL (something like "https://twently-cuddly-dinosaurs.robocorp.link") and the related token. These are the details that you need to configure your AI Agent to have access to your Action\n\n## What do you need in your Action Package\n\nAn `Action Package` is currently defined as a local folder that contains at least one Python file containing an action entry point (a Python function marked with `@action` -decorator from `robocorp.actions`).\n\nThe `package.yaml` file is required for specifying the Python environment and dependencies for your Action ([RCC](https://github.com/robocorp/rcc/) will be used to automatically bootstrap it and keep it updated given the `package.yaml` contents).\n\n> Note: the `package.yaml` is optional if the action server is not being used as a standalone (i.e.: if it was pip-installed it can use the same python environment where it\'s installed).\n\n### Bootstrapping a new Action\n\nStart new projects with:\n\n`action-server new`\n\nNote: the `action-server` executable should be automatically added to your python installation after `pip install robocorp-action-server`, but if for some reason it wasn\'t pip-installed, it\'s also possible to use `python -m robocorp.action_server` instead of `action-server`.\n\nAfter creating the project, it\'s possible to serve the actions under the current directory with:\n\n`action-server start`\n\nFor example: When running `action-server start`, the action server will scan for existing actions under the current directory, and it\'ll start serving those.\n\nAfter it\'s started, it\'s possible to access the following URLs:\n\n- `/index.html`: UI for the Action Server.\n- `/openapi.json`: Provides the openapi spec for the action server.\n- `/docs`: Provides access to the APIs available in the server and a UI to test it.\n\n## Documentation\n\nExplore our [docs](https://github.com/robocorp/robocorp/tree/master/action_server/docs) for extensive documentation.\n\n## Changelog\n\nA list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/action_server/docs/CHANGELOG.md).\n',
     'author': 'Fabio Z.',
     'author_email': 'fabio@robocorp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/robocorp/robocorp/',
```

### Comparing `robocorp_action_server-0.2.1/PKG-INFO` & `robocorp_action_server-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: robocorp-action-server
-Version: 0.2.1
+Version: 0.3.0
 Summary: Robocorp local task server
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: fastjsonschema (>=2.19.1,<3.0.0)
 Requires-Dist: jsonschema (>=4.19.2,<5.0.0)
 Requires-Dist: msgspec (>=0.18,<0.19)
 Requires-Dist: psutil (>=5,<6)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: requests (>=2,<3)
-Requires-Dist: robocorp-actions (>=0.1.0,<0.2.0)
+Requires-Dist: robocorp-actions (>=0.2.0,<0.3.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp-action-server
```

