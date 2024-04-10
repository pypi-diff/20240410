# Comparing `tmp/hahomematic-2024.4.5.tar.gz` & `tmp/hahomematic-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.5.tar", last modified: Tue Apr  9 17:31:47 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.6.tar", last modified: Wed Apr 10 17:57:07 2024, max compression
```

## Comparing `hahomematic-2024.4.5.tar` & `hahomematic-2024.4.6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.863688 hahomematic-2024.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 17:31:47.863688 hahomematic-2024.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.851688 hahomematic-2024.4.5/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.851688 hahomematic-2024.4.5/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.855688 hahomematic-2024.4.5/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    58726 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.855688 hahomematic-2024.4.5/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.855688 hahomematic-2024.4.5/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.855688 hahomematic-2024.4.5/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33402 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    29012 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.859688 hahomematic-2024.4.5/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.859688 hahomematic-2024.4.5/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.859688 hahomematic-2024.4.5/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.863688 hahomematic-2024.4.5/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 17:31:47.000000 hahomematic-2024.4.5/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-09 17:31:47.000000 hahomematic-2024.4.5/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:31:47.000000 hahomematic-2024.4.5/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:31:47.000000 hahomematic-2024.4.5/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 17:31:47.000000 hahomematic-2024.4.5/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 17:31:47.000000 hahomematic-2024.4.5/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.859688 hahomematic-2024.4.5/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 17:31:47.863688 hahomematic-2024.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:31:47.863688 hahomematic-2024.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-09 17:31:23.000000 hahomematic-2024.4.5/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    57524 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.855441 hahomematic-2024.4.6/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    41426 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.859441 hahomematic-2024.4.6/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.859441 hahomematic-2024.4.6/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33468 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28733 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 17:57:07.000000 hahomematic-2024.4.6/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.863441 hahomematic-2024.4.6/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:57:07.867441 hahomematic-2024.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 17:56:44.000000 hahomematic-2024.4.6/tests/test_text.py
```

### Comparing `hahomematic-2024.4.5/LICENSE` & `hahomematic-2024.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/PKG-INFO` & `hahomematic-2024.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.5
+Version: 2024.4.6
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.5/README.md` & `hahomematic-2024.4.6/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/__init__.py` & `hahomematic-2024.4.6/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.6/hahomematic/caches/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     NO_CACHE_ENTRY,
     CallSource,
     EventType,
     InterfaceEventType,
     InterfaceName,
 )
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import changed_within_seconds
+from hahomematic.support import changed_within_seconds, loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class DeviceDetailsCache:
     """Cache for device/channel details."""
 
@@ -250,28 +250,30 @@
     def clear(self) -> None:
         """Clear the cache."""
         self._pending_pongs.clear()
         self._unknown_pongs.clear()
         self._pending_pong_logged = False
         self._unknown_pong_logged = False
 
+    @loop_safe
     def handle_send_ping(self, ping_ts: datetime) -> None:
         """Handle send ping timestamp."""
         self._pending_pongs.add(ping_ts)
         self._check_and_fire_pong_event(
             event_type=InterfaceEventType.PENDING_PONG,
             pong_mismatch_count=self.pending_pong_count,
         )
         _LOGGER.debug(
             "PING PONG CACHE: Increase pending PING count: %s - %i for ts: %s",
             self._interface_id,
             self.pending_pong_count,
             ping_ts,
         )
 
+    @loop_safe
     def handle_received_pong(self, pong_ts: datetime) -> None:
         """Handle received pong timestamp."""
         if pong_ts in self._pending_pongs:
             self._pending_pongs.remove(pong_ts)
             self._check_and_fire_pong_event(
                 event_type=InterfaceEventType.PENDING_PONG,
                 pong_mismatch_count=self.pending_pong_count,
@@ -320,14 +322,15 @@
                 _LOGGER.debug(
                     "PING PONG CACHE: Removing expired unknown PONG: %s - %i or ts: %s",
                     self._interface_id,
                     self.unknown_pong_count,
                     pong_ts,
                 )
 
+    @loop_safe
     def _check_and_fire_pong_event(
         self, event_type: InterfaceEventType, pong_mismatch_count: int
     ) -> None:
         """Fire an event about the pong status."""
 
         def _fire_event(mismatch_count: int) -> None:
             self._central.fire_ha_event_callback(
```

### Comparing `hahomematic-2024.4.5/hahomematic/caches/persistent.py` & `hahomematic-2024.4.6/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/caches/visibility.py` & `hahomematic-2024.4.6/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/central/__init__.py` & `hahomematic-2024.4.6/hahomematic/central/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,21 @@
 from hahomematic.platforms.device import HmDevice
 from hahomematic.platforms.entity import BaseEntity, CallbackEntity
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.hub import Hub
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
-from hahomematic.support import cancelling, check_config, get_device_address, reduce_args
+from hahomematic.support import (
+    cancelling,
+    check_config,
+    get_device_address,
+    loop_safe,
+    reduce_args,
+)
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _R = TypeVar("_R")
 _T = TypeVar("_T")
 
 # {instance_name, central}
@@ -144,17 +150,14 @@
         self.last_events: Final[dict[str, datetime]] = {}
         # Signature: (name, *args)
         # e.g. DEVICES_CREATED, HUB_REFRESHED
         self._system_event_callbacks: Final[set[Callable]] = set()
         # Signature: (interface_id, channel_address, parameter, value)
         # Re-Fired events from CCU for parameter updates
         self._entity_event_callbacks: Final[set[Callable]] = set()
-        # Signature: (interface_id, entity)
-        # Fires parameter data updates as events with entity.
-        self._entity_data_event_callbacks: Final[set[Callable]] = set()
         # Signature: (event_type, event_data)
         # Events like INTERFACE, KEYPRESS, ...
         self._ha_event_callbacks: Final[set[Callable]] = set()
 
         self.json_rpc_client: Final[JsonRpcAioHttpClient] = central_config.create_json_rpc_client()
 
         CENTRAL_INSTANCES[self._name] = self
@@ -471,14 +474,15 @@
                 _LOGGER.debug("DE_INIT_CLIENTS: Proxy de-initialized: %s", name)
 
     async def _init_hub(self) -> None:
         """Init the hub."""
         await self._hub.fetch_program_data()
         await self._hub.fetch_sysvar_data()
 
+    @loop_safe
     def fire_interface_event(
         self,
         interface_id: str,
         interface_event_type: InterfaceEventType,
         data: dict[str, Any] | None = None,
     ) -> None:
         """Fire an event about the interface status."""
@@ -957,14 +961,15 @@
         except CancelledError:
             _LOGGER.debug(
                 "create_task: task cancelled for %s",
                 self._name,
             )
             return
 
+    @loop_safe
     def _async_create_task(self, target: Coroutine[Any, Any, _R], name: str) -> asyncio.Task[_R]:
         """Create a task from within the event_loop. This method must be run in the event_loop."""
         task = self._loop.create_task(target, name=name)
         self._tasks.add(task)
         task.add_done_callback(self._tasks.remove)
         return task
 
@@ -975,14 +980,15 @@
         except CancelledError:  # pragma: no cover
             _LOGGER.debug(
                 "run_coroutine: coroutine interrupted for %s",
                 self._name,
             )
             return None
 
+    @loop_safe
     def async_add_executor_job(self, target: Callable[..., _T], *args: Any) -> asyncio.Future[_T]:
         """Add an executor job from within the event_loop."""
         try:
             task = self._loop.run_in_executor(None, target, *args)
             self._tasks.add(task)
             task.add_done_callback(self._tasks.remove)
             return task
@@ -1096,14 +1102,15 @@
         self._ha_event_callbacks.add(ha_event_callback)
 
     def unregister_ha_event_callback(self, ha_event_callback: Callable) -> None:
         """RUn register ha_event callback in central."""
         if ha_event_callback in self._ha_event_callbacks:
             self._ha_event_callbacks.remove(ha_event_callback)
 
+    @loop_safe
     def fire_ha_event_callback(self, event_type: EventType, event_data: dict[str, str]) -> None:
         """
         Fire ha_event callback in central.
 
         # Events like INTERFACE, KEYPRESS, ...
         """
         for callback_handler in self._ha_event_callbacks:
@@ -1119,14 +1126,15 @@
         self._entity_event_callbacks.add(entity_event_callback)
 
     def unregister_entity_event_callback(self, entity_event_callback: Callable) -> None:
         """Un register entity_event callback in central."""
         if entity_event_callback in self._entity_event_callbacks:
             self._entity_event_callbacks.remove(entity_event_callback)
 
+    @loop_safe
     def fire_entity_event_callback(
         self, interface_id: str, channel_address: str, parameter: str, value: Any
     ) -> None:
         """
         Fire entity callback in central.
 
         Not used by HA.
@@ -1137,48 +1145,24 @@
                 callback_handler(interface_id, channel_address, parameter, value)
             except Exception as ex:
                 _LOGGER.error(
                     "FIRE_ENTITY_EVENT_CALLBACK: Unable to call handler: %s",
                     reduce_args(args=ex.args),
                 )
 
-    def register_entity_data_event_callback(self, entity_data_event_callback: Callable) -> None:
-        """Register entity_event callback in central."""
-        self._entity_data_event_callbacks.add(entity_data_event_callback)
-
-    def unregister_entity_data_event_callback(self, entity_data_event_callback: Callable) -> None:
-        """Un register entity_event callback in central."""
-        if entity_data_event_callback in self._entity_data_event_callbacks:
-            self._entity_data_event_callbacks.remove(entity_data_event_callback)
-
-    def fire_entity_data_event_callback(self, interface_id: str, entity: BaseEntity) -> None:
-        """
-        Fire entity_data callback in central.
-
-        Not used by HA.
-        Fires parameter data updates as events with entity.
-        """
-        for callback_handler in self._entity_data_event_callbacks:
-            try:
-                callback_handler(interface_id, entity)
-            except Exception as ex:
-                _LOGGER.error(
-                    "FIRE_ENTITY_DATA_EVENT_CALLBACK: Unable to call handler: %s",
-                    reduce_args(args=ex.args),
-                )
-
     def register_system_event_callback(self, system_event_callback: Callable) -> None:
         """Register system_event callback in central."""
         self._system_event_callbacks.add(system_event_callback)
 
     def unregister_system_event_callback(self, system_event_callback: Callable) -> None:
         """Un register system_event callback in central."""
         if system_event_callback in self._system_event_callbacks:
             self._system_event_callbacks.remove(system_event_callback)
 
+    @loop_safe
     def fire_system_event_callback(self, system_event: SystemEvent, **kwargs: Any) -> None:
         """
         Fire system_event callback in central.
 
         e.g. DEVICES_CREATED, HUB_REFRESHED
         """
         for callback_handler in self._system_event_callbacks:
```

### Comparing `hahomematic-2024.4.5/hahomematic/central/decorators.py` & `hahomematic-2024.4.6/hahomematic/central/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,97 +5,115 @@
 import asyncio
 from collections.abc import Awaitable, Callable
 from datetime import datetime
 from functools import wraps
 import logging
 from typing import Any, Final, ParamSpec, TypeVar, cast
 
-from hahomematic import client as hmcl
+from hahomematic import central as hmcu, client as hmcl
+import hahomematic.central.xml_rpc_server as xmlrpc
 from hahomematic.const import SystemEvent
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.support import reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 _INTERFACE_ID: Final = "interface_id"
 
 
 def callback_system_event(system_event: SystemEvent) -> Callable:
-    """Check if callback_system is set and call it AFTER original function."""
+    """Check if system_event_callback is set and call it AFTER original function."""
 
-    def decorator_callback_system_event(
+    def decorator_system_event_callback(
         func: Callable[_P, _R | Awaitable[_R]],
     ) -> Callable[_P, _R | Awaitable[_R]]:
         """Decorate callback system events."""
 
         @wraps(func)
-        async def async_wrapper_callback_system_event(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+        async def async_wrapper_system_event_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
             """Wrap async callback system events."""
             return_value = cast(_R, await func(*args, **kwargs))  # type: ignore[misc]
-            _exec_callback_system_event(*args, **kwargs)
+            await _exec_system_event_callback(*args, **kwargs)
             return return_value
 
         @wraps(func)
-        def wrapper_callback_system_event(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+        def wrapper_system_event_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
             """Wrap callback system events."""
             return_value = cast(_R, func(*args, **kwargs))
-            _exec_callback_system_event(*args, **kwargs)
+            try:
+                unit = args[0]
+                central: hmcu.CentralUnit | None = None
+                if isinstance(unit, hmcu.CentralUnit):
+                    central = unit
+                if central is None and isinstance(unit, xmlrpc.RPCFunctions):
+                    central = unit.get_central(interface_id=str(args[1]))
+                if central:
+                    central.create_task(
+                        _exec_system_event_callback(*args, **kwargs),
+                        name="wrapper_system_event_callback",
+                    )
+            except Exception as ex:
+                _LOGGER.warning(
+                    "EXEC_SYSTEM_EVENT_CALLBACK failed: Problem with identifying central: %s",
+                    reduce_args(args=ex.args),
+                )
             return return_value
 
-        def _exec_callback_system_event(*args: Any, **kwargs: Any) -> None:
+        async def _exec_system_event_callback(*args: Any, **kwargs: Any) -> None:
             """Execute the callback for a system event."""
-            if len(args) > 1:
+
+            if not ((len(args) > 1 and not kwargs) or (len(args) == 1 and kwargs)):
                 _LOGGER.warning(
-                    "EXEC_CALLBACK_SYSTEM_EVENT failed: *args not supported for callback_system_event"
+                    "EXEC_SYSTEM_EVENT_CALLBACK failed: *args not supported for callback_system_event"
                 )
             try:
                 args = args[1:]
-                interface_id: str = args[0] if len(args) > 1 else str(kwargs[_INTERFACE_ID])
+                interface_id: str = args[0] if len(args) > 0 else str(kwargs[_INTERFACE_ID])
                 if client := hmcl.get_client(interface_id=interface_id):
                     client.last_updated = datetime.now()
                     client.central.fire_system_event_callback(system_event=system_event, **kwargs)
             except Exception as err:  # pragma: no cover
                 _LOGGER.warning(
-                    "EXEC_CALLBACK_SYSTEM_EVENT failed: Unable to reduce kwargs for callback_system_event"
+                    "EXEC_SYSTEM_EVENT_CALLBACK failed: Unable to reduce kwargs for system_event_callback"
                 )
                 raise HaHomematicException(
-                    f"args-exception callback_system_event [{reduce_args(args=err.args)}]"
+                    f"args-exception system_event_callback [{reduce_args(args=err.args)}]"
                 ) from err
 
         if asyncio.iscoroutinefunction(func):
-            return async_wrapper_callback_system_event
-        return wrapper_callback_system_event
+            return async_wrapper_system_event_callback
+        return wrapper_system_event_callback
 
-    return decorator_callback_system_event
+    return decorator_system_event_callback
 
 
 def callback_event(
     func: Callable[_P, _R],
 ) -> Callable:
-    """Check if callback_event is set and call it AFTER original function."""
+    """Check if event_callback is set and call it AFTER original function."""
 
     @wraps(func)
-    async def async_wrapper_callback_event(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+    async def async_wrapper_event_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         """Wrap callback events."""
         return_value = cast(_R, await func(*args, **kwargs))  # type: ignore[misc]
-        _exec_callback_entity_event(*args, **kwargs)
+        _exec_event_callback(*args, **kwargs)
         return return_value
 
-    def _exec_callback_entity_event(*args: Any, **kwargs: Any) -> None:
+    def _exec_event_callback(*args: Any, **kwargs: Any) -> None:
         """Execute the callback for an entity event."""
         try:
             args = args[1:]
             interface_id: str = args[0] if len(args) > 1 else str(kwargs[_INTERFACE_ID])
             if client := hmcl.get_client(interface_id=interface_id):
                 client.last_updated = datetime.now()
                 client.central.fire_entity_event_callback(*args, **kwargs)
         except Exception as err:  # pragma: no cover
             _LOGGER.warning(
-                "EXEC_CALLBACK_ENTITY_EVENT failed: Unable to reduce kwargs for callback_event"
+                "EXEC_ENTITY_EVENT_CALLBACK failed: Unable to reduce kwargs for event_callback"
             )
             raise HaHomematicException(
-                f"args-exception callback_event [{reduce_args(args=err.args)}]"
+                f"args-exception event_callback [{reduce_args(args=err.args)}]"
             ) from err
 
-    return async_wrapper_callback_event
+    return async_wrapper_event_callback
```

### Comparing `hahomematic-2024.4.5/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.6/hahomematic/central/xml_rpc_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def __init__(self, xml_rpc_server: XmlRpcServer) -> None:
         """Init RPCFunctions."""
         self._xml_rpc_server: Final = xml_rpc_server
 
     def event(self, interface_id: str, channel_address: str, parameter: str, value: Any) -> None:
         """If a device emits some sort event, we will handle it here."""
-        if central := self._xml_rpc_server.get_central(interface_id):
+        if central := self.get_central(interface_id):
             central.create_task(
                 central.event(
                     interface_id=interface_id,
                     channel_address=channel_address,
                     parameter=parameter,
                     value=value,
                 ),
@@ -49,33 +49,33 @@
             interface_id,
             int(error_code),
             str(msg),
         )
 
     def listDevices(self, interface_id: str) -> list[dict[str, Any]]:
         """Return already existing devices to CCU / Homegear."""
-        if central := self._xml_rpc_server.get_central(interface_id):
+        if central := self.get_central(interface_id):
             return central.list_devices(interface_id=interface_id)  # type: ignore[no-any-return]
         return []
 
     def newDevices(self, interface_id: str, device_descriptions: list[dict[str, Any]]) -> None:
         """Add new devices send from backend."""
         central: hmcu.CentralUnit | None
-        if central := self._xml_rpc_server.get_central(interface_id):
+        if central := self.get_central(interface_id):
             central.create_task(
                 central.add_new_devices(
                     interface_id=interface_id, device_descriptions=tuple(device_descriptions)
                 ),
                 name=f"newDevices-{interface_id}",
             )
 
     def deleteDevices(self, interface_id: str, addresses: list[str]) -> None:
         """Delete devices send from backend."""
         central: hmcu.CentralUnit | None
-        if central := self._xml_rpc_server.get_central(interface_id):
+        if central := self.get_central(interface_id):
             central.create_task(
                 central.delete_devices(interface_id=interface_id, addresses=tuple(addresses)),
                 name=f"deleteDevices-{interface_id}",
             )
 
     @callback_system_event(system_event=SystemEvent.UPDATE_DEVICE)
     def updateDevice(self, interface_id: str, address: str, hint: int) -> None:
@@ -115,14 +115,18 @@
         """
         _LOGGER.debug(
             "READDEDDEVICES: interface_id = %s, addresses = %s",
             interface_id,
             str(addresses),
         )
 
+    def get_central(self, interface_id: str) -> hmcu.CentralUnit | None:
+        """Return the central by interface_id."""
+        return self._xml_rpc_server.get_central(interface_id)
+
 
 # Restrict to specific paths.
 class RequestHandler(SimpleXMLRPCRequestHandler):
     """We handle requests to / and /RPC2."""
 
     rpc_paths = (
         "/",
```

### Comparing `hahomematic-2024.4.5/hahomematic/client/__init__.py` & `hahomematic-2024.4.6/hahomematic/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,21 @@
     ProxyInitState,
     SystemInformation,
     SystemVariableData,
 )
 from hahomematic.exceptions import BaseHomematicException, NoConnection
 from hahomematic.performance import measure_execution_time
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import build_headers, build_xml_rpc_uri, get_channel_no, reduce_args
+from hahomematic.support import (
+    build_headers,
+    build_xml_rpc_uri,
+    get_channel_no,
+    loop_safe,
+    reduce_args,
+)
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _ADDRESS: Final = "address"
 _CHANNELS: Final = "channels"
 _ID: Final = "id"
 _INTERFACE: Final = "interface"
@@ -164,14 +170,15 @@
 
     async def proxy_re_init(self) -> ProxyInitState:
         """Reinit Proxy."""
         if await self.proxy_de_init() != ProxyInitState.DE_INIT_FAILED:
             return await self.proxy_init()
         return ProxyInitState.DE_INIT_FAILED
 
+    @loop_safe
     def _mark_all_devices_forced_availability(
         self, forced_availability: ForcedDeviceAvailability
     ) -> None:
         """Mark device's availability state for this interface."""
         available = forced_availability != ForcedDeviceAvailability.FORCE_FALSE
         if self._available != available:
             for device in self.central.devices:
@@ -238,14 +245,15 @@
             )
             return False
 
         if (datetime.now() - self.last_updated).total_seconds() < CALLBACK_WARN_INTERVAL:
             return True
         return False
 
+    @loop_safe
     def is_callback_alive(self) -> bool:
         """Return if XmlRPC-Server is alive based on received events for this client."""
         if last_events_time := self.central.last_events.get(self.interface_id):
             seconds_since_last_event = (datetime.now() - last_events_time).total_seconds()
             if seconds_since_last_event > CALLBACK_WARN_INTERVAL:
                 if self._is_callback_alive:
                     self.central.fire_interface_event(
```

### Comparing `hahomematic-2024.4.5/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.6/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.6/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/config.py` & `hahomematic-2024.4.6/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/const.py` & `hahomematic-2024.4.6/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/exceptions.py` & `hahomematic-2024.4.6/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/hmcli.py` & `hahomematic-2024.4.6/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/performance.py` & `hahomematic-2024.4.6/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.6/hahomematic/platforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     Operations,
     ParamsetKey,
 )
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import create_custom_entity_and_append_to_device
 from hahomematic.platforms.event import create_event_and_append_to_device
 from hahomematic.platforms.generic import create_entity_and_append_to_device
+from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
+@loop_safe
 def create_entities_and_append_to_device(device: hmd.HmDevice) -> None:
     """Create the entities associated to this device."""
     for channel_address in device.channels:
         channel_no = hms.get_channel_no(channel_address)
 
         if not device.central.paramset_descriptions.get_paramset_keys(
             interface_id=device.interface_id, channel_address=channel_address
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 import importlib
 import logging
 from typing import Final
 
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom.definition import entity_definition_exists, get_entity_configs
 from hahomematic.platforms.custom.support import CustomConfig
+from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
+@loop_safe
 def create_custom_entity_and_append_to_device(
     device: hmd.HmDevice,
 ) -> None:
     """Decides which default platform should be used, and creates the required entities."""
 
     if device.ignore_for_custom_entity:
         _LOGGER.debug(
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.6/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.6/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/device.py` & `hahomematic-2024.4.6/hahomematic/platforms/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,21 @@
 from hahomematic.platforms.custom import definition as hmed, entity as hmce
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.entity import BaseEntity, CallbackEntity
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.support import PayloadMixin, get_device_name
 from hahomematic.platforms.update import HmUpdate
-from hahomematic.support import CacheEntry, Channel, check_or_create_directory, reduce_args
+from hahomematic.support import (
+    CacheEntry,
+    Channel,
+    check_or_create_directory,
+    loop_safe,
+    reduce_args,
+)
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class HmDevice(PayloadMixin):
     """Object to hold information about a device and associated entities."""
 
@@ -494,14 +500,15 @@
         """Return the list of readable master entities."""
         return tuple(
             ge
             for ge in self._generic_entities.values()
             if ge.is_readable and ge.paramset_key == paramset_key
         )
 
+    @loop_safe
     def set_forced_availability(self, forced_availability: ForcedDeviceAvailability) -> None:
         """Set the availability of the device."""
         if self._forced_availability != forced_availability:
             self._forced_availability = forced_availability
             for entity in self.generic_entities:
                 entity.fire_entity_updated_callback()
 
@@ -571,14 +578,15 @@
                     save_to_file=False,
                 )
         await self.central.paramset_descriptions.save()
         for entity in self.generic_entities:
             entity.update_parameter_data()
         self.fire_device_updated_callback()
 
+    @loop_safe
     def fire_device_updated_callback(self, *args: Any) -> None:
         """Do what is needed when the state of the device has been updated."""
         self._set_last_updated()
         for callback_handler in self._device_updated_callbacks:
             try:
                 callback_handler(*args)
             except Exception as ex:
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/entity.py` & `hahomematic-2024.4.6/hahomematic/platforms/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.support import (
     EntityNameData,
     PayloadMixin,
     convert_value,
     generate_channel_unique_id,
 )
-from hahomematic.support import reduce_args
+from hahomematic.support import loop_safe, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 
 _CONFIGURABLE_CHANNEL: Final[tuple[str, ...]] = (
     "KEY_TRANSCEIVER",
@@ -225,22 +225,24 @@
             self._device_removed_callbacks.append(device_removed_callback)
 
     def unregister_device_removed_callback(self, device_removed_callback: Callable) -> None:
         """Unregister the device removed callback."""
         if device_removed_callback in self._device_removed_callbacks:
             self._device_removed_callbacks.remove(device_removed_callback)
 
+    @loop_safe
     def fire_entity_updated_callback(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been updated/refreshed."""
         for callback_handler in self._entity_updated_callbacks:
             try:
                 callback_handler(*args, **kwargs)
             except Exception as ex:
                 _LOGGER.warning("FIRE_entity_updated_EVENT failed: %s", reduce_args(args=ex.args))
 
+    @loop_safe
     def fire_device_removed_callback(self, *args: Any) -> None:
         """Do what is needed when the entity has been removed."""
         for callback_handler in self._device_removed_callbacks:
             try:
                 callback_handler(*args)
             except Exception as ex:
                 _LOGGER.warning("FIRE_DEVICE_REMOVED_EVENT failed: %s", reduce_args(args=ex.args))
@@ -368,21 +370,14 @@
         """Return the entity usage."""
         return self._usage
 
     def set_usage(self, usage: EntityUsage) -> None:
         """Set the entity usage."""
         self._usage = usage
 
-    def fire_entity_updated_callback(self, *args: Any, **kwargs: Any) -> None:
-        """Do what is needed when the value of the entity has been updated."""
-        super().fire_entity_updated_callback(*args, **kwargs)
-        self._central.fire_entity_data_event_callback(
-            interface_id=self._device.interface_id, entity=self
-        )
-
     @abstractmethod
     async def load_entity_value(self, call_source: CallSource, direct_call: bool = False) -> None:
         """Init the entity data."""
 
     @abstractmethod
     def _get_entity_name(self) -> EntityNameData:
         """Generate the name for the entity."""
@@ -649,14 +644,15 @@
         """Replace given unit."""
         if not raw_unit:
             return 1
         if multiplier := _MULTIPLIER_UNIT.get(raw_unit):
             return multiplier
         return 1
 
+    @loop_safe
     @abstractmethod
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
 
     async def load_entity_value(self, call_source: CallSource, direct_call: bool = False) -> None:
         """Init the entity data."""
         if direct_call is False and hms.changed_within_seconds(last_change=self._last_refreshed):
@@ -672,14 +668,15 @@
                 paramset_key=self._paramset_key,
                 parameter=self._parameter,
                 call_source=call_source,
                 direct_call=direct_call,
             )
         )
 
+    @loop_safe
     def write_value(self, value: Any) -> tuple[ParameterT | None, ParameterT | None]:
         """Update value of the entity."""
         old_value = self._value
         if value == NO_CACHE_ENTRY:
             if self.last_refreshed != INIT_DATETIME:
                 self._state_uncertain = True
                 self.fire_entity_updated_callback()
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/event.py` & `hahomematic-2024.4.6/hahomematic/platforms/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Operations,
     ParamsetKey,
 )
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.entity import BaseParameterEntity
 from hahomematic.platforms.support import EntityNameData, generate_unique_id, get_event_name
+from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class GenericEvent(BaseParameterEntity[Any, Any]):
     """Base class for events."""
 
@@ -59,21 +60,23 @@
         return EntityUsage.EVENT if force_enabled else EntityUsage.NO_CREATE
 
     @config_property
     def event_type(self) -> EventType:
         """Return the event_type of the event."""
         return self._event_type
 
+    @loop_safe
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
         if self.event_type in ENTITY_EVENTS:
             self.fire_entity_updated_callback(parameter=self.parameter.lower())
         self._set_last_updated()
         self.fire_event(value)
 
+    @loop_safe
     def fire_event(self, value: Any) -> None:
         """Do what is needed to fire an event."""
         self._central.fire_ha_event_callback(
             event_type=self.event_type, event_data=self.get_event_data(value=value)
         )
 
     def _get_entity_name(self) -> EntityNameData:
@@ -97,14 +100,15 @@
 
 
 class DeviceErrorEvent(GenericEvent):
     """class for handling device error events."""
 
     _event_type = EventType.DEVICE_ERROR
 
+    @loop_safe
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
 
         old_value, new_value = self.write_value(value=value)
 
         if (
             isinstance(new_value, bool)
@@ -124,14 +128,15 @@
 
 class ImpulseEvent(GenericEvent):
     """class for handling impulse events."""
 
     _event_type = EventType.IMPULSE
 
 
+@loop_safe
 def create_event_and_append_to_device(
     device: hmd.HmDevice, channel_address: str, parameter: str, parameter_data: Mapping[str, Any]
 ) -> None:
     """Create action event entity."""
     if device.central.parameter_visibility.parameter_is_ignored(
         device_type=device.device_type,
         channel_no=hms.get_channel_no(address=channel_address),
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 from hahomematic.platforms.generic.button import HmButton
 from hahomematic.platforms.generic.number import HmFloat, HmInteger
 from hahomematic.platforms.generic.select import HmSelect
 from hahomematic.platforms.generic.sensor import HmSensor
 from hahomematic.platforms.generic.switch import HmSwitch
 from hahomematic.platforms.generic.text import HmText
 from hahomematic.platforms.support import generate_unique_id, is_binary_sensor
+from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 _BUTTON_ACTIONS: Final[tuple[str, ...]] = ("RESET_MOTION", "RESET_PRESENCE")
 
 # Entities that should be wrapped in a new entity on a new platform.
 _SWITCH_ENTITY_TO_SENSOR: Final[Mapping[str | tuple[str, ...], Parameter]] = {
     ("HmIP-eTRV", "HmIP-HEATING"): Parameter.LEVEL,
 }
 
 
+@loop_safe
 def create_entity_and_append_to_device(
     device: hmd.HmDevice,
     channel_address: str,
     paramset_key: str,
     parameter: str,
     parameter_data: dict[str, Any],
 ) -> None:
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 from typing import Any, Final
 
 from hahomematic.const import CallSource, EntityUsage, EventType, Parameter, ParamsetKey
 from hahomematic.platforms import device as hmd, entity as hme
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.support import EntityNameData, get_entity_name
+from hahomematic.support import loop_safe
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class GenericEntity(hme.BaseParameterEntity[hme.ParameterT, hme.InputParameterT]):
     """Base class for generic entities."""
 
@@ -44,14 +45,15 @@
         """Return the entity usage."""
         if self._is_forced_sensor or self._is_un_ignored:
             return EntityUsage.ENTITY
         if (force_enabled := self._enabled_by_channel_operation_mode) is None:
             return self._usage
         return EntityUsage.ENTITY if force_enabled else EntityUsage.NO_CREATE
 
+    @loop_safe
     def event(self, value: Any) -> None:
         """Handle event for which this entity has subscribed."""
 
         old_value, new_value = self.write_value(value=value)
         if old_value == new_value:
             return
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.6/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import annotations
 
 from typing import Final
 
 from hahomematic import central as hmcu
 from hahomematic.const import PROGRAM_ADDRESS, HmPlatform, HubData, ProgramData
 from hahomematic.platforms.hub.entity import GenericHubEntity
+from hahomematic.support import loop_safe
 
 
 class HmProgramButton(GenericHubEntity):
     """Class for a HomeMatic program button."""
 
     _platform = HmPlatform.HUB_BUTTON
 
@@ -42,14 +43,15 @@
 
     def get_name(self, data: HubData) -> str:
         """Return the name of the program button entity."""
         if data.name.lower().startswith(tuple({"p_", "prg_"})):
             return data.name
         return f"P_{data.name}"
 
+    @loop_safe
     def update_data(self, data: ProgramData) -> None:
         """Set variable value on CCU/Homegear."""
         do_update: bool = False
         if self.is_active != data.is_active:
             self.is_active = data.is_active
             do_update = True
         if self.is_internal != data.is_internal:
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from slugify import slugify
 
 from hahomematic import central as hmcu
 from hahomematic.const import SYSVAR_ADDRESS, HubData, SystemVariableData
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.entity import CallbackEntity
 from hahomematic.platforms.support import generate_unique_id
-from hahomematic.support import parse_sys_var
+from hahomematic.support import loop_safe, parse_sys_var
 
 
 class GenericHubEntity(CallbackEntity):
     """Class for a HomeMatic system variable."""
 
     def __init__(
         self,
@@ -112,14 +112,15 @@
 
     def get_name(self, data: HubData) -> str:
         """Return the name of the sysvar entity."""
         if data.name.lower().startswith(tuple({"v_", "sv_", "sv"})):
             return data.name
         return f"Sv_{data.name}"
 
+    @loop_safe
     def write_value(self, value: Any) -> None:
         """Set variable value on CCU/Homegear."""
         old_value = self._value
         if self.data_type:
             value = parse_sys_var(data_type=self.data_type, raw_value=value)
         elif isinstance(old_value, bool):
             value = bool(value)
```

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.6/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/support.py` & `hahomematic-2024.4.6/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/platforms/update.py` & `hahomematic-2024.4.6/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.6/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.6/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.6/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic/support.py` & `hahomematic-2024.4.6/hahomematic/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 """Helper functions used within hahomematic."""
 
 from __future__ import annotations
 
 import asyncio
 import base64
-from collections.abc import Collection
+from collections.abc import Callable, Collection
 import contextlib
 from dataclasses import dataclass
 from datetime import datetime
 from functools import lru_cache
 import logging
 import os
 import re
 import socket
 import ssl
-from typing import Any, Final
+from typing import Any, Final, TypeVar
 
 from hahomematic.const import (
     CCU_PASSWORD_PATTERN,
     FILE_DEVICES,
     FILE_PARAMSETS,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     SysvarType,
 )
 from hahomematic.exceptions import BaseHomematicException, HaHomematicException
 
+_CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 def reduce_args(args: tuple[Any, ...]) -> tuple[Any, ...] | Any:
     """Return the first arg, if there is only one arg."""
     return args[0] if len(args) == 1 else args
 
@@ -291,7 +292,13 @@
             return False
         return changed_within_seconds(last_change=self.last_refresh)
 
 
 def cancelling(task: asyncio.Future[Any]) -> bool:
     """Return True if task is cancelling."""
     return bool((cancelling_ := getattr(task, "cancelling", None)) and cancelling_())
+
+
+def loop_safe(func: _CallableT) -> _CallableT:
+    """Annotation to mark method as safe to call from within the event loop."""
+    setattr(func, "_loop_safe", True)
+    return func
```

### Comparing `hahomematic-2024.4.5/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.6/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.5
+Version: 2024.4.6
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.5/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.6/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/hahomematic_support/client_local.py` & `hahomematic-2024.4.6/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/pyproject.toml` & `hahomematic-2024.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.5"
+version     = "2024.4.6"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.4.5/tests/test_action.py` & `hahomematic-2024.4.6/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_binary_sensor.py` & `hahomematic-2024.4.6/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_button.py` & `hahomematic-2024.4.6/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_central.py` & `hahomematic-2024.4.6/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_central_pydevccu.py` & `hahomematic-2024.4.6/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_climate.py` & `hahomematic-2024.4.6/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_cover.py` & `hahomematic-2024.4.6/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_decorator.py` & `hahomematic-2024.4.6/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_device.py` & `hahomematic-2024.4.6/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_entity.py` & `hahomematic-2024.4.6/tests/test_entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,22 +48,16 @@
     switch.register_device_removed_callback(device_removed_callback=device_removed_mock)
     assert switch.value is None
     assert (
         str(switch) == "address_path: switch/CentralTest-BidCos-RF/vcu2128127_4/, "
         "type: HmIP-BSM, name: HmIP-BSM_VCU2128127"
     )
     await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
-    assert factory.entity_event_mock.call_args_list[-1] == call(
-        const.INTERFACE_ID, "VCU2128127:4", "STATE", 1
-    )
     assert switch.value is True
     await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 0)
-    assert factory.entity_event_mock.call_args_list[-1] == call(
-        const.INTERFACE_ID, "VCU2128127:4", "STATE", 0
-    )
     assert switch.value is False
     await central.delete_devices(
         interface_id=const.INTERFACE_ID, addresses=[switch.device.device_address]
     )
     assert factory.system_event_mock.call_args_list[-1] == call(
         "deleteDevices", interface_id="CentralTest-BidCos-RF", addresses=["VCU2128127"]
     )
@@ -92,22 +86,16 @@
     switch.register_device_removed_callback(device_removed_callback=device_removed_mock)
     assert switch.value is None
     assert (
         str(switch) == "address_path: switch/CentralTest-BidCos-RF/vcu2128127_4_state/, "
         "type: HmIP-BSM, name: HmIP-BSM_VCU2128127 State ch4"
     )
     await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
-    assert factory.entity_event_mock.call_args_list[-1] == call(
-        const.INTERFACE_ID, "VCU2128127:4", "STATE", 1
-    )
     assert switch.value is True
     await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 0)
-    assert factory.entity_event_mock.call_args_list[-1] == call(
-        const.INTERFACE_ID, "VCU2128127:4", "STATE", 0
-    )
     assert switch.value is False
     await central.delete_devices(
         interface_id=const.INTERFACE_ID, addresses=[switch.device.device_address]
     )
     assert factory.system_event_mock.call_args_list[-1] == call(
         "deleteDevices", interface_id="CentralTest-BidCos-RF", addresses=["VCU2128127"]
     )
```

### Comparing `hahomematic-2024.4.5/tests/test_event.py` & `hahomematic-2024.4.6/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_json_rpc.py` & `hahomematic-2024.4.6/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_light.py` & `hahomematic-2024.4.6/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_lock.py` & `hahomematic-2024.4.6/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_number.py` & `hahomematic-2024.4.6/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_select.py` & `hahomematic-2024.4.6/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_sensor.py` & `hahomematic-2024.4.6/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_siren.py` & `hahomematic-2024.4.6/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_support.py` & `hahomematic-2024.4.6/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_switch.py` & `hahomematic-2024.4.6/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.5/tests/test_text.py` & `hahomematic-2024.4.6/tests/test_text.py`

 * *Files identical despite different names*

