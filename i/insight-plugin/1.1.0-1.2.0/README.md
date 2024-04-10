# Comparing `tmp/insight_plugin-1.1.0.tar.gz` & `tmp/insight_plugin-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insight_plugin-1.1.0.tar", last modified: Thu Mar 28 14:59:50 2024, max compression
+gzip compressed data, was "insight_plugin-1.2.0.tar", last modified: Wed Apr 10 10:32:33 2024, max compression
```

## Comparing `insight_plugin-1.1.0.tar` & `insight_plugin-1.2.0.tar`

### file list

```diff
@@ -1,177 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.186576 insight_plugin-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-28 14:59:50.186576 insight_plugin-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.166576 insight_plugin-1.1.0/insight_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16102 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.166576 insight_plugin-1.1.0/insight_plugin/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-28 14:59:50.000000 insight_plugin-1.1.0/insight_plugin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.166576 insight_plugin-1.1.0/insight_plugin/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/checksum_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/command_line_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/common_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/docker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/dockerspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/plugin_spec_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/schema_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/temp_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/common/template_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/create/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/help/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/help/connection_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/help/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/help/help_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/help/input_output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/json_generation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/plugin_to_helpmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/create/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/export/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/export/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/export/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/export/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/interactive/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/interactive/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/interactive/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/interactive/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.170576 insight_plugin-1.1.0/insight_plugin/features/refresh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/refresh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/refresh/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.174576 insight_plugin-1.1.0/insight_plugin/features/run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/run/bash_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/run/run_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/run/server_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.174576 insight_plugin-1.1.0/insight_plugin/features/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/samples/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.174576 insight_plugin-1.1.0/insight_plugin/features/samples/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/samples/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/samples/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/samples/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.174576 insight_plugin-1.1.0/insight_plugin/features/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/validate/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.174576 insight_plugin-1.1.0/insight_plugin/features/version/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/version/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.174576 insight_plugin-1.1.0/insight_plugin/features/version/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/version/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/version/util/helpmd_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/version/util/input_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/version/util/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/version/util/yaml_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.174576 insight_plugin-1.1.0/insight_plugin/features/view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/features/view/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/.dockerignore.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/Makefile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/assessment/assessment.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/bin/plugin.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/action/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/action/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/action/action.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/connection/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/connection/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/connection/connection.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/connection/schema.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/task/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/task/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/trigger/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/plugin/util/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/plugin/util/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/requirements.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/setup.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.178576 insight_plugin-1.1.0/insight_plugin/templates/unit_test/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/unit_test/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/insight_plugin/templates/unit_test/test_action.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.166576 insight_plugin-1.1.0/insight_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-28 14:59:50.000000 insight_plugin-1.1.0/insight_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-03-28 14:59:50.000000 insight_plugin-1.1.0/insight_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:59:50.000000 insight_plugin-1.1.0/insight_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 14:59:50.000000 insight_plugin-1.1.0/insight_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-28 14:59:50.000000 insight_plugin-1.1.0/insight_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 14:59:50.000000 insight_plugin-1.1.0/insight_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:59:50.186576 insight_plugin-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.182576 insight_plugin-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.182576 insight_plugin-1.1.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.182576 insight_plugin-1.1.0/tests/resources/export_test_base64/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.182576 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.182576 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.182576 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/decode/
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/decode/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.182576 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/encode/
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/encode/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.186576 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/connection/
--rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.186576 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.186576 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:50.186576 insight_plugin-1.1.0/tests/resources/export_test_base64/unit_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/unit_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/resources/export_test_base64/unit_test/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_gen_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_help_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_json_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_semver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_spec_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_temp_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-28 14:59:30.000000 insight_plugin-1.1.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.977923 insight_plugin-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-10 10:32:33.977923 insight_plugin-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18895 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/features/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/analysis/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/features/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/checksum_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/command_line_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/common_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/docker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/dockerspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/plugin_spec_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23952 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/schema_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/temp_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/template_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/create/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/connection_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/help_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/input_output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/json_generation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/plugin_to_helpmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/export/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/interactive/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/linter/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/refresh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/refresh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/refresh/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/bash_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/run_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/server_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/samples/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/validate/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/version/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/helpmd_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/input_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/yaml_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/view/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/.dockerignore.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/Makefile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/assessment/assessment.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/bin/plugin.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/action.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/connection.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/schema.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/util/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/requirements.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/setup.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/unit_test/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/unit_test/test_action.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:32:33.977923 insight_plugin-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/unit_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/unit_test/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_gen_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_help_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_json_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_semver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_spec_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_temp_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/util.py
```

### Comparing `insight_plugin-1.1.0/LICENSE` & `insight_plugin-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/PKG-INFO` & `insight_plugin-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight_plugin
-Version: 1.1.0
+Version: 1.2.0
 Summary: Plugin tooling for the Rapid7 Insight platform
 Home-page: https://github.com/rapid7/insight-plugin
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insight_plugin-1.1.0/README.md` & `insight_plugin-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/__main__.py` & `insight_plugin-1.2.0/insight_plugin/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,45 +2,54 @@
 import argparse
 import logging
 
 from argparse import Namespace
 
 from insight_plugin import VERSION
 
+from insight_plugin.features.analysis.controller import AnalysisController
 from insight_plugin.features.create.controller import CreateController
 from insight_plugin.features.samples.controller import GenSampleController
 from insight_plugin.features.export.controller import ExportController
+from insight_plugin.features.linter.controller import LinterController
 from insight_plugin.features.refresh.controller import RefreshController
 from insight_plugin.features.run.run_controller import RunController
 from insight_plugin.features.validate.controller import ValidateController
 from insight_plugin.features.run.server_controller import RunServerController
 from insight_plugin.features.run.bash_controller import RunShellController
 from insight_plugin.features.interactive.controller import InteractiveController
 from insight_plugin.features.common.exceptions import InsightException
 from insight_plugin.features.version.controller import VersionController
 from insight_plugin.features.view.controller import ViewController
 from typing import List
+from insight_plugin.constants import Color
 
 DEFAULT_JQ_STRING = ".body.output"
 
 
 def main():
     argparser = argparse.ArgumentParser(
         prog="insight-plugin",
         epilog=f"Version {VERSION}",
         description="Command-line tool to help develop plugins for the Rapid7 Insight Platform",
     )
 
     subparsers = argparser.add_subparsers(help="Commands")
     parsers_list = []
 
+    # Analysis
+    analysis_argparse(subparsers=subparsers, parsers_list=parsers_list)
+    # Checks
+    checks_argparse(subparsers=subparsers, parsers_list=parsers_list)
     # Create
     create_argparse(subparsers=subparsers, parsers_list=parsers_list)
     # Export
     export_argparse(subparsers=subparsers, parsers_list=parsers_list)
+    # Linter
+    linter_argparse(subparsers=subparsers, parsers_list=parsers_list)
     # Refresh
     refresh_argparse(subparsers=subparsers, parsers_list=parsers_list)
     # Validate
     validate_argparse(subparsers=subparsers, parsers_list=parsers_list)
     # Semantic version
     semver_argparse(subparsers=subparsers, parsers_list=parsers_list)
     # Gen Samples
@@ -503,16 +512,16 @@
 
 def validate(args: Namespace) -> None:
     """
     Validate insight plugin
     :param args: CLI args
     :return: None
     """
-    controller = ValidateController.new_from_cli(**{"spec_path": args.spec_path})
-    controller.validate()
+    controller = ValidateController.new_from_cli(**{"target_dir": args.target_dir})
+    controller.run()
 
 
 def view_argparse(subparsers, parsers_list: List) -> None:
     """
     Handle the arg-parsing for the view subcommand
     :param subparsers: List to be filled with commands
     :param parsers_list: List to be appended with parsed commands
@@ -534,9 +543,83 @@
             "verbose": args.verbose,
             "target_dir": args.target_dir,
         }
     )
     controller.run()
 
 
+def linter_argparse(subparsers, parsers_list: List) -> None:
+    """
+    Handle the arg-parsing for the linter subcommand
+    :param subparsers: List to be filled with commands
+    :param parsers_list: List to be appended with parsed commands
+    :return: None
+    """
+    command_view = subparsers.add_parser("linter", help=LinterController.HELP_MSG)
+    parsers_list.append(command_view)
+    command_view.set_defaults(func=linter)
+
+
+def linter(args: Namespace) -> None:
+    """
+    Run the linter
+    """
+    controller = LinterController.new_from_cli(**{"target_dir": args.target_dir})
+    controller.run()
+
+
+def analysis_argparse(subparsers, parsers_list: List) -> None:
+    """
+    Handle the arg-parsing for the analysis subcommand
+    :param subparsers: List to be filled with commands
+    :param parsers_list: List to be appended with parsed commands
+    :return: None
+    """
+    command_view = subparsers.add_parser("analysis", help=AnalysisController.HELP_MSG)
+    parsers_list.append(command_view)
+    command_view.set_defaults(func=analysis)
+
+
+def analysis(args: Namespace) -> None:
+    """
+    Run Static Code Analysis
+    """
+    controller = AnalysisController.new_from_cli(**{"target_dir": args.target_dir})
+    controller.run()
+
+
+def checks_argparse(subparsers, parsers_list: List) -> None:
+    """
+    Handle the arg-parsing for the checks subcommand
+    :param subparsers: List to be filled with commands
+    :param parsers_list: List to be appended with parsed commands
+    :return: None
+    """
+    command_view = subparsers.add_parser(
+        "checks", help="Run Linter, code analysis & validate on the plugin"
+    )
+    parsers_list.append(command_view)
+    command_view.set_defaults(func=checks)
+
+
+def checks(args: Namespace) -> None:
+    """
+    Run Linter, SCA & Validate
+    """
+    analysis_controller = AnalysisController.new_from_cli(
+        **{"target_dir": args.target_dir}
+    )
+    linter_controller = LinterController.new_from_cli(**{"target_dir": args.target_dir})
+    validate_controller = ValidateController.new_from_cli(
+        **{"target_dir": args.target_dir}
+    )
+
+    print(Color.BOLD + "\nAnalysis \n" + Color.END)
+    analysis_controller.run()
+    print(Color.BOLD + "\nLinter\n" + Color.END)
+    linter_controller.run()
+    print(Color.BOLD + "\nValidate\n" + Color.END)
+    validate_controller.run()
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `insight_plugin-1.1.0/insight_plugin/__pycache__/__init__.cpython-39.pyc` & `insight_plugin-1.2.0/insight_plugin/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar 28 14:59:30 2024 UTC, .py size: 429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 d285 0566 ad01 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 b06a 1666 ad01 0000  a........j.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 5a02 6500 6a03 a004 6500 6a03 a005 6506  Z.e.j...e.j...e.
 00000050: a101 a101 5a07 6403 5a08 6404 5a09 6405  ....Z.d.Z.d.Z.d.
 00000060: 5a0a 6406 5a0b 6407 5a0c 6408 5a0d 6408  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a0e 6501 6a03 a00f 6500 6a03 a004 6500  Z.e.j...e.j...e.
 00000080: 6a03 a004 6506 a101 a101 a101 0100 6401  j...e.........d.
-00000090: 5300 2909 e900 0000 004e 7a05 312e 312e  S.)......Nz.1.1.
+00000090: 5300 2909 e900 0000 004e 7a05 312e 322e  S.)......Nz.1.2.
 000000a0: 305a 0664 6f63 6b65 727a 0575 7466 2d38  0Z.dockerz.utf-8
 000000b0: 5a04 6963 6f6e 5a1d 696e 7369 6768 7463  Z.iconZ.insightc
 000000c0: 6f6e 6e65 6374 5f70 6c75 6769 6e5f 7275  onnect_plugin_ru
 000000d0: 6e74 696d 657a 1d69 6e73 6967 6874 636f  ntimez.insightco
 000000e0: 6e6e 6563 742d 706c 7567 696e 2d72 756e  nnect-plugin-run
 000000f0: 7469 6d65 5a06 6b6f 6d61 6e64 2910 da02  timeZ.komand)...
 00000100: 6f73 da03 7379 73da 0756 4552 5349 4f4e  os..sys..VERSION
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/builder.py` & `insight_plugin-1.2.0/insight_plugin/features/common/builder.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/checksum_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/checksum_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/command_line_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/command_line_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/common_feature.py` & `insight_plugin-1.2.0/insight_plugin/features/common/common_feature.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/docker_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/docker_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/dockerspec.py` & `insight_plugin-1.2.0/insight_plugin/features/common/dockerspec.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/exceptions.py` & `insight_plugin-1.2.0/insight_plugin/features/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/logging_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/plugin_spec_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/plugin_spec_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/schema_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/schema_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Dict, Union, List, Any
+from typing import Tuple, Dict, Union, Any
 from insight_plugin.features.common.plugin_spec_util import PluginSpecConstants
 from insight_plugin.features.common.exceptions import InsightException
 from insight_plugin.features.common.logging_util import BaseLoggingFeature
 
 
 class SchemaConstants:
     """
@@ -283,17 +283,17 @@
                     troubleshooting=f'Please add "type" to {key} in plugin.spec.yaml',
                 )
             # If this property is a primitive type, then we do not need to add it to the definitions section.
             if current_type in SchemaUtil.PRIMITIVE_TYPES:
                 # Primitive type definitions are only either strings or dicts.
                 if isinstance(SchemaUtil.PRIMITIVE_TYPES[current_type], str):
                     # If this type definition is a string, we simply assign the value to the type property.
-                    parent_object[key][
-                        PluginSpecConstants.TYPE
-                    ] = SchemaUtil.PRIMITIVE_TYPES[current_type]
+                    parent_object[key][PluginSpecConstants.TYPE] = (
+                        SchemaUtil.PRIMITIVE_TYPES[current_type]
+                    )
                 # This parameter's primitive type is one defined as a dict object with multiple properties.
                 elif isinstance(SchemaUtil.PRIMITIVE_TYPES[current_type], dict):
                     # Add each property of this primitive type's dict definition to the current parameter schema.
                     for primitive_key in SchemaUtil.PRIMITIVE_TYPES[current_type]:
                         # Dict-defined primitive type properties have primitive_keys type, displayType, and format.
                         parent_object[key][primitive_key] = SchemaUtil.PRIMITIVE_TYPES[
                             current_type
@@ -354,41 +354,41 @@
                 # Remove the [] array indicator and extract the parameter array contents type.
                 final_type = current_type[len(SchemaConstants.TYPE_ARRAY) :]
                 # Is this parameter an array of a primitive type?
                 if final_type in SchemaUtil.PRIMITIVE_TYPES:
                     # Is this an array of strings?
                     if isinstance(SchemaUtil.PRIMITIVE_TYPES[final_type], str):
                         # Set this array's items: type value to string.
-                        current_item[
-                            PluginSpecConstants.TYPE
-                        ] = SchemaUtil.PRIMITIVE_TYPES[final_type]
+                        current_item[PluginSpecConstants.TYPE] = (
+                            SchemaUtil.PRIMITIVE_TYPES[final_type]
+                        )
                     # Is this an array of dict objects?
                     elif isinstance(SchemaUtil.PRIMITIVE_TYPES[final_type], dict):
                         for primitive_key in SchemaUtil.PRIMITIVE_TYPES[final_type]:
                             current_item[primitive_key] = SchemaUtil.PRIMITIVE_TYPES[
                                 final_type
                             ][primitive_key]
                 # Is this parameter an array of a base type?
                 elif final_type in SchemaUtil.BASE_TYPES:
                     # Non-primitive types use $ref instead of type, here we set the definition reference.
-                    current_item[
-                        SchemaConstants.REF
-                    ] = f"{SchemaConstants.REF_DEF}{final_type}"
+                    current_item[SchemaConstants.REF] = (
+                        f"{SchemaConstants.REF_DEF}{final_type}"
+                    )
                     # Non-primitive types must be defined in the schema, here we get this base type definition.
                     if final_type not in definitions:
                         definitions[final_type] = SchemaUtil.BASE_TYPES[final_type]
                 # Is this parameter an array of a custom type defined in the plugin spec?
                 elif (
                     PluginSpecConstants.TYPES in spec
                     and final_type in spec[PluginSpecConstants.TYPES]
                 ):
                     # Non-primitive types use $ref instead of type, here we set the definition reference.
-                    current_item[
-                        SchemaConstants.REF
-                    ] = f"{SchemaConstants.REF_DEF}{final_type}"
+                    current_item[SchemaConstants.REF] = (
+                        f"{SchemaConstants.REF_DEF}{final_type}"
+                    )
                     # Have we not yet added this custom type definition to the schema?
                     if final_type not in definitions:
                         # We have not yet defined this custom type, prepare to recurse.
                         # Instantiate the nested schema with attributes like those set at the top level in build_inner()
                         # Custom type definitions are objects which all start with type = "object" and title = its name
                         definitions[final_type] = {}
                         definitions[final_type][SchemaConstants.TYPE] = "object"
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/temp_file_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/temp_file_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/common/template_util.py` & `insight_plugin-1.2.0/insight_plugin/features/common/template_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,17 @@
             autoescape=select_autoescape(),
         )  # nosec
         # Add methods to the Jinja global environment, allowing us to call these methods in templates
         self._env.globals["camel_case"] = Templates.camel_case
         self._env.globals["upper_camel_case"] = Templates.upper_camel_case
         self._env.globals["json_schema_connection"] = self.json_schema_connection
         self._env.globals["json_schema_trigger_input"] = self.json_schema_trigger_input
-        self._env.globals[
-            "json_schema_trigger_output"
-        ] = self.json_schema_trigger_output
+        self._env.globals["json_schema_trigger_output"] = (
+            self.json_schema_trigger_output
+        )
         self._env.globals["json_schema_action_input"] = self.json_schema_action_input
         self._env.globals["json_schema_action_output"] = self.json_schema_action_output
         self._env.globals["json_schema_task_input"] = self.json_schema_task_input
         self._env.globals["json_schema_task_state"] = self.json_schema_task_state
         self._env.globals["json_schema_task_output"] = self.json_schema_task_output
 
     def fill(self, template_name: str, inputs: {str: str}) -> str:
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/controller.py` & `insight_plugin-1.2.0/insight_plugin/features/create/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     PluginSpecTypes,
 )
 from insight_plugin.features.common.common_feature import CommonFeature
 from insight_plugin.features.common.template_util import Templates
 from insight_plugin.features.common.temp_file_util import SafeTempDirectory
 from insight_plugin.features.common.exceptions import InsightException
 from insight_plugin.features.create import util
-from insight_plugin.constants import CREATE_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 
 
 class CreateController(CommonFeature):
     """
     Controls the subcommand to create a new skeleton plugin file structure.
     Depends on plugin spec dictionary values to fill templates.
     """
 
-    HELP_MSG = CREATE_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.CREATE_DESCRIPTION
 
     def __init__(self, spec_path: Optional[str], verbose: bool, target_dir: str):
         super().__init__(verbose, target_dir)
         self._spec_path = spec_path
         self._templates = Templates(os.path.join(ROOT_DIR, "templates"))
 
     @classmethod
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/help/components.py` & `insight_plugin-1.2.0/insight_plugin/features/create/help/components.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/help/connection_help.py` & `insight_plugin-1.2.0/insight_plugin/features/create/help/connection_help.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/help/constants.py` & `insight_plugin-1.2.0/insight_plugin/features/create/help/constants.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/help/help_util.py` & `insight_plugin-1.2.0/insight_plugin/features/create/help/help_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/help/input_output_helpers.py` & `insight_plugin-1.2.0/insight_plugin/features/create/help/input_output_helpers.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/json_generation_util.py` & `insight_plugin-1.2.0/insight_plugin/features/create/json_generation_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/plugin_to_helpmd.py` & `insight_plugin-1.2.0/insight_plugin/features/create/plugin_to_helpmd.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/create/util.py` & `insight_plugin-1.2.0/insight_plugin/features/create/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/export/controller.py` & `insight_plugin-1.2.0/insight_plugin/features/export/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import shutil
 from insight_plugin.features.common.plugin_spec_util import PluginSpecUtil
 from insight_plugin.features.common.builder import Builder, BuilderOperation
 from insight_plugin.features.common.common_feature import CommonFeature
 from insight_plugin.features.common.command_line_util import CommandLineUtil
 from insight_plugin.features.common.temp_file_util import SafeTempDirectory
 from insight_plugin.features.common.exceptions import InsightException
-from insight_plugin.constants import EXPORT_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 
 
 class ExportController(CommonFeature):
     """
     Controls the subcommand for export
     Allows the user to export the plugin image to a tarball
     """
 
-    HELP_MSG = EXPORT_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.EXPORT_DESCRIPTION
 
     def __init__(
         self,
         no_pull: bool,
         verbose: bool,
         target_dir: str,
     ):
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/interactive/controller.py` & `insight_plugin-1.2.0/insight_plugin/features/interactive/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 import sys
 from insight_plugin.features.create.controller import CreateController
 from insight_plugin.features.validate.controller import ValidateController
 from insight_plugin.features.refresh.controller import RefreshController
 from insight_plugin.features.run.run_controller import RunController
 from insight_plugin.features.export.controller import ExportController
 from typing import Tuple, Optional, Union
-from insight_plugin.constants import (
-    CREATE_DESCRIPTION,
-    REFRESH_DESCRIPTION,
-    RUN_DESCRIPTION,
-    EXPORT_DESCRIPTION,
-    VALIDATE_DESCRIPTION,
-)
+from insight_plugin.constants import SubcommandDescriptions
 from insight_plugin.features.interactive.util.util import (
     retrieve_bool_input,
     retrieve_path_input,
     retrieve_jq_input,
     create_and_refresh_cli_controller,
     export_cli_controller,
     run_cli_controller,
@@ -29,23 +23,23 @@
         self.title = title
         self.description = description
 
 
 # TODO: Make this dynamic instead of hardcoded
 _OPTIONS = [
     # 1
-    _Option(title="Create", description=CREATE_DESCRIPTION),
+    _Option(title="Create", description=SubcommandDescriptions.CREATE_DESCRIPTION),
     # 2
-    _Option(title="Refresh", description=REFRESH_DESCRIPTION),
+    _Option(title="Refresh", description=SubcommandDescriptions.REFRESH_DESCRIPTION),
     # 3
-    _Option(title="Run", description=RUN_DESCRIPTION),
+    _Option(title="Run", description=SubcommandDescriptions.RUN_DESCRIPTION),
     # 4
-    _Option(title="Validate", description=VALIDATE_DESCRIPTION),
+    _Option(title="Validate", description=SubcommandDescriptions.VALIDATE_DESCRIPTION),
     # 5
-    _Option(title="Export", description=EXPORT_DESCRIPTION),
+    _Option(title="Export", description=SubcommandDescriptions.EXPORT_DESCRIPTION),
 ]
 
 
 class InteractiveController(object):
     @staticmethod
     def prompt_menu():
         """
@@ -197,24 +191,22 @@
 
         # Handle path to spec file input
         path_to_spec = retrieve_path_input("plugin.spec.yaml")
 
         return path_to_spec
 
     @staticmethod
-    def _get_run_controller_menu() -> (
-        Tuple[
-            str,
-            Union[str, None],
-            bool,
-            bool,
-            bool,
-            Optional[str],
-        ]
-    ):
+    def _get_run_controller_menu() -> Tuple[
+        str,
+        Union[str, None],
+        bool,
+        bool,
+        bool,
+        Optional[str],
+    ]:
         """
         Method to handle the run subcommand inputs.
         :return: User inputs for verbose, target_dir, assessment, is_test, jq & json_target
         """
 
         # Handle json_files input
         json_target = retrieve_path_input("json_files")
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/interactive/util/util.py` & `insight_plugin-1.2.0/insight_plugin/features/interactive/util/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/refresh/controller.py` & `insight_plugin-1.2.0/insight_plugin/features/refresh/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     PluginSpecUtil,
     PluginSpecTypes,
 )
 from insight_plugin.features.common.common_feature import CommonFeature
 from insight_plugin.features.common.template_util import Templates
 from insight_plugin.features.common.exceptions import InsightException
 from insight_plugin.features.create import util
-from insight_plugin.constants import REFRESH_DESCRIPTION, VALID_IGNORE_FILES
+from insight_plugin.constants import SubcommandDescriptions, VALID_IGNORE_FILES
 
 
 class RefreshController(CommonFeature):
     """
     Controls the subcommand to refresh plugin file structure.
     Depends on plugin spec dictionary values to fill templates.
     """
 
-    HELP_MSG = REFRESH_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.REFRESH_DESCRIPTION
 
     def __init__(
         self, spec_path: Optional[str], verbose: bool, target_dir: str, ignore: list
     ):
         super().__init__(verbose, target_dir)
         self._spec_path = spec_path
         self._templates = Templates(os.path.join(ROOT_DIR, "templates"))
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/run/bash_controller.py` & `insight_plugin-1.2.0/insight_plugin/features/run/bash_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from insight_plugin.features.common.common_feature import CommonFeature
-from insight_plugin.constants import SHELL_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 from insight_plugin.features.common.docker_util import DockerUtil
 
 
 class RunShellController(CommonFeature):
     """
     Controls the subcommand for Run Shell
     Allows the user to run the plugin via the docker shell
     """
 
-    HELP_MSG = SHELL_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.SHELL_DESCRIPTION
 
     def __init__(
         self,
         verbose: bool,
         target_dir: str,
         rebuild: bool = False,
         volumes: [str] = None,
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/run/run_controller.py` & `insight_plugin-1.2.0/insight_plugin/features/run/run_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from insight_plugin.features.common.common_feature import CommonFeature
-from insight_plugin.constants import RUN_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 from insight_plugin.features.common.docker_util import DockerUtil
 
 
 class RunController(CommonFeature):
     """
     Controls the subcommand for run
     Allows the user to run the plugin
     """
 
-    HELP_MSG = RUN_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.RUN_DESCRIPTION
 
     def __init__(
         self,
         verbose: bool,
         target_dir: str,
         rebuild: bool,
         assessment: bool,
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/run/server_controller.py` & `insight_plugin-1.2.0/insight_plugin/features/run/server_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from insight_plugin.features.common.common_feature import CommonFeature
-from insight_plugin.constants import SERVER_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 from insight_plugin.features.common.docker_util import DockerUtil
 
 
 class RunServerController(CommonFeature):
     """
     Controls the subcommand for Run Server
     Allows the user to run the plugin as a webserver
     """
 
-    HELP_MSG = SERVER_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.SERVER_DESCRIPTION
 
     def __init__(
         self,
         target_dir: str,
         volumes: [str],
         ports: [str],
         rebuild: bool,
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/samples/controller.py` & `insight_plugin-1.2.0/insight_plugin/features/samples/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional
 from insight_plugin.features.common.common_feature import CommonFeature
-from insight_plugin.constants import SAMPLES_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 from insight_plugin.features.samples.util.util import SamplesUtil
 
 
 class GenSampleController(CommonFeature):
     """
     Controls the subcommand to create samples for testing.
     Depends on plugin spec dictionary values to fill templates.
     """
 
-    HELP_MSG = SAMPLES_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.SAMPLES_DESCRIPTION
 
     def __init__(
         self,
         verbose: bool,
         target_dir: str,
         target_component: Optional[str],
     ):
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/samples/util/constants.py` & `insight_plugin-1.2.0/insight_plugin/features/samples/util/constants.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/samples/util/util.py` & `insight_plugin-1.2.0/insight_plugin/features/samples/util/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/version/controller.py` & `insight_plugin-1.2.0/insight_plugin/features/version/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from insight_plugin.features.common.common_feature import CommonFeature
-from insight_plugin.constants import VERSION_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 from insight_plugin.features.version.util.version_util import VersionUtil
 
 
 class VersionController(CommonFeature):
     """
     Controls the subcommand to modify the plugin version & write to help.md
     Must be used within the directory that contains the plugin.spec.yaml
     """
 
-    HELP_MSG = VERSION_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.VERSION_DESCRIPTION
 
     def __init__(
         self,
         version_num: str,
         changelog_desc: str,
         verbose: bool,
         target_dir: str,
```

### Comparing `insight_plugin-1.1.0/insight_plugin/features/version/util/helpmd_util.py` & `insight_plugin-1.2.0/insight_plugin/features/version/util/helpmd_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/version/util/input_util.py` & `insight_plugin-1.2.0/insight_plugin/features/version/util/input_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/version/util/version_util.py` & `insight_plugin-1.2.0/insight_plugin/features/version/util/version_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/version/util/yaml_util.py` & `insight_plugin-1.2.0/insight_plugin/features/version/util/yaml_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/features/view/controller.py` & `insight_plugin-1.2.0/insight_plugin/features/view/controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from insight_plugin.features.common.common_feature import CommonFeature
-from insight_plugin.constants import VIEW_DESCRIPTION
+from insight_plugin.constants import SubcommandDescriptions
 from insight_plugin.features.common.docker_util import DockerUtil
 
 
 class ViewController(CommonFeature):
-    HELP_MSG = VIEW_DESCRIPTION
+    HELP_MSG = SubcommandDescriptions.VIEW_DESCRIPTION
 
     def __init__(self, verbose: bool, target_dir: str):
         super().__init__(verbose=verbose, target_dir=target_dir)
         self._verbose = verbose
         self._target_dir = target_dir
 
     @classmethod
```

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/Dockerfile.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/Makefile.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/Makefile.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/assessment/assessment.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/assessment/assessment.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/bin/plugin.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/bin/plugin.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/action/action.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/action.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/plugin/connection/connection.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/connection.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin/templates/unit_test/test_action.py.jinja` & `insight_plugin-1.2.0/insight_plugin/templates/unit_test/test_action.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/insight_plugin.egg-info/PKG-INFO` & `insight_plugin-1.2.0/insight_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight-plugin
-Version: 1.1.0
+Version: 1.2.0
 Summary: Plugin tooling for the Rapid7 Insight platform
 Home-page: https://github.com/rapid7/insight-plugin
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insight_plugin-1.1.0/insight_plugin.egg-info/SOURCES.txt` & `insight_plugin-1.2.0/insight_plugin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 insight_plugin.egg-info/SOURCES.txt
 insight_plugin.egg-info/dependency_links.txt
 insight_plugin.egg-info/entry_points.txt
 insight_plugin.egg-info/requires.txt
 insight_plugin.egg-info/top_level.txt
 insight_plugin/__pycache__/__init__.cpython-39.pyc
 insight_plugin/features/__init__.py
+insight_plugin/features/analysis/__init__.py
+insight_plugin/features/analysis/controller.py
 insight_plugin/features/common/__init__.py
 insight_plugin/features/common/builder.py
 insight_plugin/features/common/checksum_util.py
 insight_plugin/features/common/command_line_util.py
 insight_plugin/features/common/common_feature.py
 insight_plugin/features/common/docker_util.py
 insight_plugin/features/common/dockerspec.py
@@ -41,14 +43,16 @@
 insight_plugin/features/export/controller.py
 insight_plugin/features/export/util/__init__.py
 insight_plugin/features/export/util/util.py
 insight_plugin/features/interactive/__init__.py
 insight_plugin/features/interactive/controller.py
 insight_plugin/features/interactive/util/__init__.py
 insight_plugin/features/interactive/util/util.py
+insight_plugin/features/linter/__init__.py
+insight_plugin/features/linter/controller.py
 insight_plugin/features/refresh/__init__.py
 insight_plugin/features/refresh/controller.py
 insight_plugin/features/run/__init__.py
 insight_plugin/features/run/bash_controller.py
 insight_plugin/features/run/run_controller.py
 insight_plugin/features/run/server_controller.py
 insight_plugin/features/samples/__init__.py
```

### Comparing `insight_plugin-1.1.0/pyproject.toml` & `insight_plugin-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/setup.py` & `insight_plugin-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py` & `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py` & `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py` & `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py` & `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_checksum.py` & `insight_plugin-1.2.0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_create.py` & `insight_plugin-1.2.0/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_export.py` & `insight_plugin-1.2.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_gen_samples.py` & `insight_plugin-1.2.0/tests/test_gen_samples.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_help_creation.py` & `insight_plugin-1.2.0/tests/test_help_creation.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_interactive.py` & `insight_plugin-1.2.0/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_json_generate.py` & `insight_plugin-1.2.0/tests/test_json_generate.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_refresh.py` & `insight_plugin-1.2.0/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_run.py` & `insight_plugin-1.2.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_schema.py` & `insight_plugin-1.2.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_semver.py` & `insight_plugin-1.2.0/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/test_spec_order.py` & `insight_plugin-1.2.0/tests/test_spec_order.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.1.0/tests/util.py` & `insight_plugin-1.2.0/tests/util.py`

 * *Files identical despite different names*

