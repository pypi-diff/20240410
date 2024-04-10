# Comparing `tmp/bttc-0.0.73.3.tar.gz` & `tmp/bttc-0.0.73.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.73.3.tar", last modified: Wed Apr 10 01:57:15 2024, max compression
+gzip compressed data, was "bttc-0.0.73.4.tar", last modified: Wed Apr 10 02:12:35 2024, max compression
```

## Comparing `bttc-0.0.73.3.tar` & `bttc-0.0.73.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.384922 bttc-0.0.73.3/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.3/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 01:57:15.384922 bttc-0.0.73.3/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.3/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-10 01:55:39.000000 bttc-0.0.73.3/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.3/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16092 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2290 2024-04-10 01:55:39.000000 bttc-0.0.73.3/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22552 2024-04-10 00:48:38.000000 bttc-0.0.73.3/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.376922 bttc-0.0.73.3/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.384922 bttc-0.0.73.3/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.384922 bttc-0.0.73.3/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 01:57:15.384922 bttc-0.0.73.3/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.3/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.388174 bttc-0.0.73.4/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.4/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 02:12:35.388174 bttc-0.0.73.4/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.4/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.384174 bttc-0.0.73.4/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-10 02:12:25.000000 bttc-0.0.73.4/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.4/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.4/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16092 2024-04-08 13:33:17.000000 bttc-0.0.73.4/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.384174 bttc-0.0.73.4/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2155 2024-04-10 02:08:56.000000 bttc-0.0.73.4/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22387 2024-04-10 02:08:56.000000 bttc-0.0.73.4/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.4/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.384174 bttc-0.0.73.4/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.384174 bttc-0.0.73.4/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.380174 bttc-0.0.73.4/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.384174 bttc-0.0.73.4/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.384174 bttc-0.0.73.4/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.388174 bttc-0.0.73.4/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.388174 bttc-0.0.73.4/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.4/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.4/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 02:12:35.384174 bttc-0.0.73.4/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 02:12:35.000000 bttc-0.0.73.4/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 02:12:35.000000 bttc-0.0.73.4/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 02:12:35.000000 bttc-0.0.73.4/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 02:12:35.000000 bttc-0.0.73.4/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 02:12:35.000000 bttc-0.0.73.4/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 02:12:35.388174 bttc-0.0.73.4/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.4/setup.py
```

### Comparing `bttc-0.0.73.3/LICENSE` & `bttc-0.0.73.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/PKG-INFO` & `bttc-0.0.73.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.3
+Version: 0.0.73.4
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.3/README.md` & `bttc-0.0.73.4/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/__init__.py` & `bttc-0.0.73.4/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.73.3'
+__version__ = '0.0.73.4'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.73.3/bttc/apk_utils.py` & `bttc-0.0.73.4/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/ble_data.py` & `bttc-0.0.73.4/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/ble_utils.py` & `bttc-0.0.73.4/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/bt_data.py` & `bttc-0.0.73.4/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/bt_utils.py` & `bttc-0.0.73.4/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/cli/__init__.py` & `bttc-0.0.73.4/bttc/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Entry point of BTTC Cli."""
 
 from bttc.cli import constants
+from bttc.cli import main
 import cmd2
 from typing import (
     Callable,
     Type,
 )
 
 
+BttcCmdApp = main.BttcCmdApp
 CommandSet = cmd2.CommandSet
 Color = constants.Color
 
 
-class BttcCommandSet(CommandSet):
-  """BTTC Command set base class."""
-
-  def __init__(self, app: 'BttcCmdApp'):
-    super().__init__()
-    self._app = app
-    self.namespace_history = []
-
-
 def with_default_category(
     category: str, *, heritable: bool = True) -> Callable[
         [Type['CommandSet']], Type['CommandSet']]:
     """
     Decorator that applies a category to all ``do_*`` command methods in a class
     that do not already have a category specified.
```

### Comparing `bttc-0.0.73.3/bttc/cli/constants.py` & `bttc-0.0.73.4/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/cli/main.py` & `bttc-0.0.73.4/bttc/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 import bttc
 from bttc import constants as bttc_constants
 from bttc.cli import constants
 from bttc.utils import device_factory
 
 
+CommandSet = cmd2.CommandSet
 Color = constants.Color
 EXIST_MSG = 'Welcome to use BTTC Cli and see you next time!'
 MAIN_COMMANDS = "Main Commands"
 
 select_parser = cmd2.Cmd2ArgumentParser()
 select_parser.add_argument(
     '-s', '--serial', type=str, default=None, help='DUT serial')
@@ -93,24 +94,22 @@
       return
 
     return func(*args, **kwargs)
 
   return wrapper
 
 
-@cmd2.with_default_category('john_manual')
-class TestCommandSet(cmd2.CommandSet):
+class BttcCommandSet(CommandSet):
+  """BTTC Command set base class."""
+
   def __init__(self, app: 'BttcCmdApp'):
     super().__init__()
     self._app = app
     self.namespace_history = []
 
-  def do_john_work(self, args):
-    print("!!! Do john's Customized command test works !!!")
-
 
 @cmd2.with_default_category('device_config')
 class DeviceConfigCommandSet(cmd2.CommandSet):
   def __init__(self, app: 'BttcCmdApp'):
     super().__init__()
     self._app = app
     self.namespace_history = []
@@ -486,17 +485,14 @@
   def _init_dut(self, serial: str):
     self._dut = bttc.get(
         serial,
         init_snippet_uiautomator=self.dut_init_snippet_uiautomator,
         init_sl4a=self.dut_init_sl4a)
     self.prompt = BttcCmdApp.DEVICE_PROMPT_PROMPT.format(serial=serial)
 
-  def do_load_test_cmd2(self, args):
-    self.register_command_set(TestCommandSet(self))
-
   @dec_require_dut
   def do_device_time(self, args):
     self.poutput(f'{self._dut.gm.device_datetime}\n')
 
   @cmd2.with_argparser(load_cmd2_commandset_parser)
   def do_load_cmd2_command_set(self, args):
     """Loads cmd2 command set from given module path."""
```

### Comparing `bttc-0.0.73.3/bttc/common_data.py` & `bttc-0.0.73.4/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/constants.py` & `bttc-0.0.73.4/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/core.py` & `bttc-0.0.73.4/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/errors.py` & `bttc-0.0.73.4/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/general_utils.py` & `bttc-0.0.73.4/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.73.4/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.73.4/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.73.4/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.73.4/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.73.4/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.73.4/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.73.4/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/avrcp/errors.py` & `bttc-0.0.73.4/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/hfp/__init__.py` & `bttc-0.0.73.4/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/hfp/constants.py` & `bttc-0.0.73.4/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/hfp/errors.py` & `bttc-0.0.73.4/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.73.4/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.73.4/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.73.4/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.73.4/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/strategy.py` & `bttc-0.0.73.4/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/ad_checker.py` & `bttc-0.0.73.4/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/device_factory.py` & `bttc-0.0.73.4/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/iperf/__init__.py` & `bttc-0.0.73.4/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/iperf/errors.py` & `bttc-0.0.73.4/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/key_events_handler.py` & `bttc-0.0.73.4/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/log_parser.py` & `bttc-0.0.73.4/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/logcat.py` & `bttc-0.0.73.4/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/retry.py` & `bttc-0.0.73.4/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils/typing_utils.py` & `bttc-0.0.73.4/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/utils_loader.py` & `bttc-0.0.73.4/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc/wifi_utils.py` & `bttc-0.0.73.4/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/bttc.egg-info/PKG-INFO` & `bttc-0.0.73.4/bttc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.3
+Version: 0.0.73.4
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.3/bttc.egg-info/SOURCES.txt` & `bttc-0.0.73.4/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.3/setup.py` & `bttc-0.0.73.4/setup.py`

 * *Files identical despite different names*

