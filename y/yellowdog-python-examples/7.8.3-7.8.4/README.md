# Comparing `tmp/yellowdog-python-examples-7.8.3.tar.gz` & `tmp/yellowdog-python-examples-7.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-7.8.3.tar", last modified: Tue Apr  2 09:31:50 2024, max compression
+gzip compressed data, was "yellowdog-python-examples-7.8.4.tar", last modified: Wed Apr 10 07:24:58 2024, max compression
```

## Comparing `yellowdog-python-examples-7.8.3.tar` & `yellowdog-python-examples-7.8.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.902096 yellowdog-python-examples-7.8.3/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-7.8.3/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-02 09:31:50.902030 yellowdog-python-examples-7.8.3/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1442 2023-08-28 09:06:52.000000 yellowdog-python-examples-7.8.3/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   144187 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     2140 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.3/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)      242 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2024-04-02 09:31:50.902379 yellowdog-python-examples-7.8.3/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-7.8.3/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.880643 yellowdog-python-examples-7.8.3/tests/
--rw-r--r--   0 pwt        (501) staff       (20)     2092 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/tests/test_create_remove.py
--rw-r--r--   0 pwt        (501) staff       (20)     2374 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/tests/test_demos.py
--rw-r--r--   0 pwt        (501) staff       (20)     6017 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.3/tests/test_dryruns.py
--rw-r--r--   0 pwt        (501) staff       (20)     1656 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/tests/test_entrypoints.py
--rw-r--r--   0 pwt        (501) staff       (20)      604 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/tests/test_gui.py
--rw-r--r--   0 pwt        (501) staff       (20)     1705 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/tests/test_list.py
--rw-r--r--   0 pwt        (501) staff       (20)      857 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/tests/test_objects.py
--rw-r--r--   0 pwt        (501) staff       (20)     1683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/tests/test_variable_processing.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.900540 yellowdog-python-examples-7.8.3/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4179 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2024-03-25 12:45:42.000000 yellowdog-python-examples-7.8.3/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    45701 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/args.py
--rw-r--r--   0 pwt        (501) staff       (20)     1012 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/boost.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7489 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      607 2023-11-15 10:24:00.000000 yellowdog-python-examples-7.8.3/yd_commands/check_imports.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2502 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard.py
--rw-r--r--   0 pwt        (501) staff       (20)    38132 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_aws.py
--rw-r--r--   0 pwt        (501) staff       (20)      481 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_aws_types.py
--rw-r--r--   0 pwt        (501) staff       (20)    31534 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_azure.py
--rw-r--r--   0 pwt        (501) staff       (20)    13236 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_common.py
--rw-r--r--   0 pwt        (501) staff       (20)    12227 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_gcp.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.3/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)     3529 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/config_types.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    29810 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/create.py
--rw-r--r--   0 pwt        (501) staff       (20)    13603 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.3/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2479 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4715 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      329 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.3/yd_commands/follow.py
--rw-r--r--   0 pwt        (501) staff       (20)     3526 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.3/yd_commands/follow_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1494 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/format_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      290 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/hold.py
--rw-r--r--   0 pwt        (501) staff       (20)      842 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/id_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    12170 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.3/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     5005 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/interactive.py
--rw-r--r--   0 pwt        (501) staff       (20)     1007 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/items.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.3/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18464 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)    15959 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/load_config.py
--rw-r--r--   0 pwt        (501) staff       (20)     3861 2024-03-22 10:21:47.000000 yellowdog-python-examples-7.8.3/yd_commands/load_resources.py
--rw-r--r--   0 pwt        (501) staff       (20)     8703 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)    32348 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/printing.py
--rw-r--r--   0 pwt        (501) staff       (20)     5782 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/property_names.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17214 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     4748 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13555 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/remove.py
--rw-r--r--   0 pwt        (501) staff       (20)     5169 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.3/yd_commands/resize.py
--rw-r--r--   0 pwt        (501) staff       (20)     3261 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.3/yd_commands/settings.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4811 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.3/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      298 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/start.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5072 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/start_hold_common.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    52008 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.3/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)    10720 2024-02-14 11:33:32.000000 yellowdog-python-examples-7.8.3/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4797 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.3/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2023-11-24 13:35:57.000000 yellowdog-python-examples-7.8.3/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     5352 2023-11-18 08:50:59.000000 yellowdog-python-examples-7.8.3/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     6732 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2486 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    18199 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.3/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     3747 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.901675 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1934 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      860 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)      253 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-10 07:24:58.800492 yellowdog-python-examples-7.8.4/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-7.8.4/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-10 07:24:58.800336 yellowdog-python-examples-7.8.4/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1442 2023-08-28 09:06:52.000000 yellowdog-python-examples-7.8.4/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   144187 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.4/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     2140 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.4/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)      242 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2024-04-10 07:24:58.800887 yellowdog-python-examples-7.8.4/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-7.8.4/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-10 07:24:58.778094 yellowdog-python-examples-7.8.4/tests/
+-rw-r--r--   0 pwt        (501) staff       (20)     2092 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.4/tests/test_create_remove.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2636 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/tests/test_demos.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6489 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/tests/test_dryruns.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1656 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/tests/test_entrypoints.py
+-rw-r--r--   0 pwt        (501) staff       (20)      604 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/tests/test_gui.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1705 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.4/tests/test_list.py
+-rw-r--r--   0 pwt        (501) staff       (20)      857 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/tests/test_objects.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/tests/test_variable_processing.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-10 07:24:58.798961 yellowdog-python-examples-7.8.4/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4179 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.4/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2024-03-25 12:45:42.000000 yellowdog-python-examples-7.8.4/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    45713 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/yd_commands/args.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1012 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/boost.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7489 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.4/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      607 2023-11-15 10:24:00.000000 yellowdog-python-examples-7.8.4/yd_commands/check_imports.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2502 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/cloudwizard.py
+-rw-r--r--   0 pwt        (501) staff       (20)    38132 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_aws.py
+-rw-r--r--   0 pwt        (501) staff       (20)      481 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_aws_types.py
+-rw-r--r--   0 pwt        (501) staff       (20)    31534 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_azure.py
+-rw-r--r--   0 pwt        (501) staff       (20)    13236 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_common.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12227 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_gcp.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.4/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3529 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.4/yd_commands/config_types.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    29810 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.4/yd_commands/create.py
+-rw-r--r--   0 pwt        (501) staff       (20)    14060 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2479 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4715 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.4/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      329 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.4/yd_commands/follow.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3526 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.4/yd_commands/follow_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1494 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/format_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      290 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.4/yd_commands/hold.py
+-rw-r--r--   0 pwt        (501) staff       (20)      842 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/id_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    12170 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.4/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5005 2024-04-03 12:41:47.000000 yellowdog-python-examples-7.8.4/yd_commands/interactive.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1007 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.4/yd_commands/items.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.4/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18464 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)    15959 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/load_config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3861 2024-03-22 10:21:47.000000 yellowdog-python-examples-7.8.4/yd_commands/load_resources.py
+-rw-r--r--   0 pwt        (501) staff       (20)     8703 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.4/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)    32348 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/printing.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5782 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.4/yd_commands/property_names.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17214 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.4/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     4748 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13555 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.4/yd_commands/remove.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5169 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.4/yd_commands/resize.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3313 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/yd_commands/settings.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4811 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.4/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      298 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.4/yd_commands/start.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5072 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.4/yd_commands/start_hold_common.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    52008 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)    10720 2024-02-14 11:33:32.000000 yellowdog-python-examples-7.8.4/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4797 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.4/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2023-11-24 13:35:57.000000 yellowdog-python-examples-7.8.4/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5352 2023-11-18 08:50:59.000000 yellowdog-python-examples-7.8.4/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6732 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2486 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.4/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18350 2024-04-10 07:24:12.000000 yellowdog-python-examples-7.8.4/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.4/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3747 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.4/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-10 07:24:58.799883 yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-10 07:24:58.000000 yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1934 2024-04-10 07:24:58.000000 yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2024-04-10 07:24:58.000000 yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      860 2024-04-10 07:24:58.000000 yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      253 2024-04-10 07:24:58.000000 yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2024-04-10 07:24:58.000000 yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-7.8.3/LICENSE` & `yellowdog-python-examples-7.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/PKG-INFO` & `yellowdog-python-examples-7.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 7.8.3
+Version: 7.8.4
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-7.8.3/PYPI_README.md` & `yellowdog-python-examples-7.8.4/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/README.md` & `yellowdog-python-examples-7.8.4/README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/pyproject.toml` & `yellowdog-python-examples-7.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/setup.cfg` & `yellowdog-python-examples-7.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/tests/test_create_remove.py` & `yellowdog-python-examples-7.8.4/tests/test_create_remove.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/tests/test_demos.py` & `yellowdog-python-examples-7.8.4/tests/test_demos.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,22 @@
         result = shell(f"cd {DEMO_DIR}/powershell && {CMD_SEQ}")
         assert result.exit_code == 0
 
     def test_cmd_exe(self):
         result = shell(f"cd {DEMO_DIR}/cmd.exe && {CMD_SEQ}")
         assert result.exit_code == 0
 
+    def test_blender(self):
+        result = shell(f"cd {DEMO_DIR}/blender && {CMD_SEQ}")
+        assert result.exit_code == 0
+
+    def test_montecarlo(self):
+        result = shell(f"cd {DEMO_DIR}/montecarlo && {CMD_SEQ}")
+        assert result.exit_code == 0
+
     def test_nextflow_image_montage(self):
         result = shell(
             f"cd {DEMO_DIR}/nextflow/image-montage && {NEXTFLOW} main.nf "
             "&& cd .. && ./cleanup.sh"
         )
         assert result.exit_code == 0
```

### Comparing `yellowdog-python-examples-7.8.3/tests/test_dryruns.py` & `yellowdog-python-examples-7.8.4/tests/test_dryruns.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,18 @@
         result = shell(f"cd {DEMO_DIR}/cmd.exe && {CMD_SEQ}")
         assert result.exit_code == 0
 
     def test_blender(self):
         result = shell(f"cd {DEMO_DIR}/blender && {CMD_SEQ}")
         assert result.exit_code == 0
 
+    def test_montecarlo(self):
+        result = shell(f"cd {DEMO_DIR}/montecarlo && {CMD_SEQ}")
+        assert result.exit_code == 0
+
     # Tests run from outside the demo directories
     def test_bash_out(self):
         demo_name = "bash"
         result = shell(
             f"cd {DEMO_DIR} && yd-provision -D -c {demo_name}/config.toml && yd-submit"
             f" -D -c {demo_name}/config.toml && yd-instantiate -D -c"
             f" {demo_name}/config.toml"
@@ -165,7 +169,16 @@
         demo_name = "blender"
         result = shell(
             f"cd {DEMO_DIR} && yd-provision -D -c {demo_name}/config.toml && yd-submit"
             f" -D -c {demo_name}/config.toml && yd-instantiate -D -c"
             f" {demo_name}/config.toml"
         )
         assert result.exit_code == 0
+
+    def test_montecarlo_out(self):
+        demo_name = "montecarlo"
+        result = shell(
+            f"cd {DEMO_DIR} && yd-provision -D -c {demo_name}/config.toml && yd-submit"
+            f" -D -c {demo_name}/config.toml && yd-instantiate -D -c"
+            f" {demo_name}/config.toml"
+        )
+        assert result.exit_code == 0
```

### Comparing `yellowdog-python-examples-7.8.3/tests/test_entrypoints.py` & `yellowdog-python-examples-7.8.4/tests/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/tests/test_gui.py` & `yellowdog-python-examples-7.8.4/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/tests/test_list.py` & `yellowdog-python-examples-7.8.4/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/tests/test_objects.py` & `yellowdog-python-examples-7.8.4/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/tests/test_variable_processing.py` & `yellowdog-python-examples-7.8.4/tests/test_variable_processing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/abort.py` & `yellowdog-python-examples-7.8.4/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/admin.py` & `yellowdog-python-examples-7.8.4/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/args.py` & `yellowdog-python-examples-7.8.4/yd_commands/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,16 +806,16 @@
         ):
             parser.add_argument(
                 "--content-path",
                 "-F",
                 type=str,
                 required=False,
                 help=(
-                    "the directory in which files for upload (or for user data) are"
-                    " found"
+                    "the directory in which files for upload (or for user data "
+                    "or CSV data) are found"
                 ),
                 metavar="<directory>",
             )
 
         if any(module in sys.argv[0] for module in ["provision", "instantiate"]):
             parser.add_argument(
                 "--follow",
```

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/boost.py` & `yellowdog-python-examples-7.8.4/yd_commands/boost.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/cancel.py` & `yellowdog-python-examples-7.8.4/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/check_imports.py` & `yellowdog-python-examples-7.8.4/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard.py` & `yellowdog-python-examples-7.8.4/yd_commands/cloudwizard.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_aws.py` & `yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_aws.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_azure.py` & `yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_azure.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_common.py` & `yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_common.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_gcp.py` & `yellowdog-python-examples-7.8.4/yd_commands/cloudwizard_gcp.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/compact_json.py` & `yellowdog-python-examples-7.8.4/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/config_types.py` & `yellowdog-python-examples-7.8.4/yd_commands/config_types.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/create.py` & `yellowdog-python-examples-7.8.4/yd_commands/create.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/csv_data.py` & `yellowdog-python-examples-7.8.4/yd_commands/csv_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from yd_commands.config_types import ConfigWorkRequirement
 from yd_commands.printing import print_json, print_log
 from yd_commands.property_names import *
 from yd_commands.settings import (
     BOOL_TYPE_TAG,
     CSV_VAR_CLOSING_DELIMITER,
     CSV_VAR_OPENING_DELIMITER,
+    LOWER_CASE_TYPE_TAG,
     NUMBER_TYPE_TAG,
 )
 from yd_commands.variables import (
     load_jsonnet_file_with_variable_substitutions,
     process_variable_substitutions_insitu,
     resolve_filename,
 )
@@ -162,15 +163,15 @@
     from CSV files. Return the expanded and variables-processed Work Requirement
     data.
     """
 
     with open(resolve_filename(files_directory, toml_file), "r") as f:
         wr_data = toml_load(f)
 
-    return perform_csv_task_expansion(wr_data, csv_files, f)
+    return perform_csv_task_expansion(wr_data, csv_files, files_directory)
 
 
 def perform_csv_task_expansion(
     wr_data: Dict, csv_files: List[str], files_directory: str = ""
 ) -> Dict:
     """
     Expand a Work Requirement using CSV data.
@@ -269,14 +270,18 @@
             value = "True"
         elif value.lower() == "false":
             value = "False"
         else:
             raise Exception(f"Invalid Boolean substitution in CSV: '{value}'")
         input = input.replace(f"'{bool_sub_str}'", value)
 
+    lower_sub_str = f"{CSV_VAR_OPENING_DELIMITER}{LOWER_CASE_TYPE_TAG}{var_name}{CSV_VAR_CLOSING_DELIMITER}"
+    if lower_sub_str in input:
+        input = input.replace(f"{lower_sub_str}", value.lower())
+
     return input
 
 
 USED_FILE_INDEXES = []
 
 
 def get_csv_file_index(
@@ -340,14 +345,19 @@
             for var_name in var_names
         )
         or any(
             f"{CSV_VAR_OPENING_DELIMITER}{BOOL_TYPE_TAG}{var_name}{CSV_VAR_CLOSING_DELIMITER}"
             in task_prototype
             for var_name in var_names
         )
+        or any(
+            f"{CSV_VAR_OPENING_DELIMITER}{LOWER_CASE_TYPE_TAG}{var_name}{CSV_VAR_CLOSING_DELIMITER}"
+            in task_prototype
+            for var_name in var_names
+        )
     )
 
 
 def csv_expand_toml_tasks(
     config_wr: ConfigWorkRequirement, csv_file: str, files_directory=""
 ) -> Dict:
     """
@@ -391,8 +401,8 @@
         # Note: not TASK_COUNT; count determined by CSV data
     ]:
         if config_value is not None and substitions_present(
             csv_data.var_names, str(config_value)
         ):
             task_proto[config_name] = config_value
 
-    return perform_csv_task_expansion(wr_data, [csv_file])
+    return perform_csv_task_expansion(wr_data, [csv_file], files_directory)
```

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/delete.py` & `yellowdog-python-examples-7.8.4/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/download.py` & `yellowdog-python-examples-7.8.4/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/follow_utils.py` & `yellowdog-python-examples-7.8.4/yd_commands/follow_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/format_json.py` & `yellowdog-python-examples-7.8.4/yd_commands/format_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/id_utils.py` & `yellowdog-python-examples-7.8.4/yd_commands/id_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/instantiate.py` & `yellowdog-python-examples-7.8.4/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/interactive.py` & `yellowdog-python-examples-7.8.4/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/items.py` & `yellowdog-python-examples-7.8.4/yd_commands/items.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-7.8.4/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/list.py` & `yellowdog-python-examples-7.8.4/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/load_config.py` & `yellowdog-python-examples-7.8.4/yd_commands/load_config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/load_resources.py` & `yellowdog-python-examples-7.8.4/yd_commands/load_resources.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/object_utilities.py` & `yellowdog-python-examples-7.8.4/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/printing.py` & `yellowdog-python-examples-7.8.4/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/property_names.py` & `yellowdog-python-examples-7.8.4/yd_commands/property_names.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/provision.py` & `yellowdog-python-examples-7.8.4/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/provision_utils.py` & `yellowdog-python-examples-7.8.4/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/remove.py` & `yellowdog-python-examples-7.8.4/yd_commands/remove.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/resize.py` & `yellowdog-python-examples-7.8.4/yd_commands/resize.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/settings.py` & `yellowdog-python-examples-7.8.4/yd_commands/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 VAR_DEFAULT_SEPARATOR = ":="
 TYPE_TAG_TERMINATOR = ":"
 TAG_DEFAULT_DIFF = "="
 NUMBER_TYPE_TAG = "num" + TYPE_TAG_TERMINATOR
 BOOL_TYPE_TAG = "bool" + TYPE_TAG_TERMINATOR
 ARRAY_TYPE_TAG = "array" + TYPE_TAG_TERMINATOR
 TABLE_TYPE_TAG = "table" + TYPE_TAG_TERMINATOR
+LOWER_CASE_TYPE_TAG = "lower" + TYPE_TAG_TERMINATOR
 TOML_VAR_NESTED_DEPTH = 3
 
 DEFAULT_LOG_WIDTH = 120
 MAX_LINES_COLOURED_JSON = 1024
 ERROR_STYLE = "bold red3"
 WARNING_STYLE = "red3"
 JSON_INDENT = 2
```

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/shutdown.py` & `yellowdog-python-examples-7.8.4/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/start_hold_common.py` & `yellowdog-python-examples-7.8.4/yd_commands/start_hold_common.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/submit.py` & `yellowdog-python-examples-7.8.4/yd_commands/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         if ARGS_PARSER.content_path is None
         else ARGS_PARSER.content_path
     )
 
     if wr_data_file is None and csv_files is not None:
         wr_data = csv_expand_toml_tasks(CONFIG_WR, csv_files[0], files_directory)
         submit_work_requirement(
-            files_directory=CONFIG_FILE_DIR,
+            files_directory=files_directory,
             wr_data=wr_data,
         )
 
     elif wr_data_file is not None:
 
         if ARGS_PARSER.jsonnet_dry_run and not wr_data_file.lower().endswith("jsonnet"):
             raise Exception(
```

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/submit_utils.py` & `yellowdog-python-examples-7.8.4/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/terminate.py` & `yellowdog-python-examples-7.8.4/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/type_check.py` & `yellowdog-python-examples-7.8.4/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/upload.py` & `yellowdog-python-examples-7.8.4/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/upload_utils.py` & `yellowdog-python-examples-7.8.4/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/utils.py` & `yellowdog-python-examples-7.8.4/yd_commands/utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/validate_properties.py` & `yellowdog-python-examples-7.8.4/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/variables.py` & `yellowdog-python-examples-7.8.4/yd_commands/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from yd_commands.check_imports import check_jsonnet_import
 from yd_commands.printing import print_error, print_json, print_log
 from yd_commands.property_names import *
 from yd_commands.settings import (
     ARRAY_TYPE_TAG,
     BOOL_TYPE_TAG,
     ENV_VAR_PREFIX,
+    LOWER_CASE_TYPE_TAG,
     NUMBER_TYPE_TAG,
     RAND_VAR_SIZE,
     TABLE_TYPE_TAG,
     TAG_DEFAULT_DIFF,
     TOML_VAR_NESTED_DEPTH,
     VAR_CLOSING_DELIMITER,
     VAR_DEFAULT_SEPARATOR,
@@ -181,15 +182,16 @@
             return_str += element
             continue
 
         try:  # Find the type tag in the element, if present
             type_tag = (
                 re.match(
                     f"^{opening_delimiter}({NUMBER_TYPE_TAG}|{BOOL_TYPE_TAG}"
-                    f"|{TABLE_TYPE_TAG}|{ARRAY_TYPE_TAG})(?!{TAG_DEFAULT_DIFF})",
+                    f"|{TABLE_TYPE_TAG}|{ARRAY_TYPE_TAG}|{LOWER_CASE_TYPE_TAG})"
+                    f"(?!{TAG_DEFAULT_DIFF})",
                     element,
                 )
                 .group(0)
                 .replace(opening_delimiter, "")
             )
         except AttributeError:  # No type-tag matches
             type_tag = ""
@@ -309,14 +311,17 @@
 def process_typed_variable_substitution(
     type_string: str, input_string: str
 ) -> Optional[Union[str, int, bool, float, List, Dict]]:
     """
     Process a single typed substitution, returning the appropriate type.
     Assumes there is a substitution present.
     """
+    if type_string == LOWER_CASE_TYPE_TAG:
+        return input_string.lower()
+
     if type_string == NUMBER_TYPE_TAG:
         try:
             return int(input_string)
         except ValueError:
             try:
                 return float(input_string)
             except ValueError:
```

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/version.py` & `yellowdog-python-examples-7.8.4/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yd_commands/wrapper.py` & `yellowdog-python-examples-7.8.4/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 7.8.3
+Version: 7.8.4
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-7.8.4/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

