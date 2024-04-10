# Comparing `tmp/bttc-0.0.73.1.tar.gz` & `tmp/bttc-0.0.73.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.73.1.tar", last modified: Tue Apr  9 04:37:46 2024, max compression
+gzip compressed data, was "bttc-0.0.73.3.tar", last modified: Wed Apr 10 01:57:15 2024, max compression
```

## Comparing `bttc-0.0.73.1.tar` & `bttc-0.0.73.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.354849 bttc-0.0.73.1/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.1/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-09 04:37:46.354849 bttc-0.0.73.1/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.1/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-09 04:28:05.000000 bttc-0.0.73.1/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.1/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16092 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22466 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.346849 bttc-0.0.73.1/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.354849 bttc-0.0.73.1/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.354849 bttc-0.0.73.1/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      164 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-09 04:37:46.354849 bttc-0.0.73.1/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1682 2024-04-09 04:37:34.000000 bttc-0.0.73.1/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.384922 bttc-0.0.73.3/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.3/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 01:57:15.384922 bttc-0.0.73.3/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.3/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-10 01:55:39.000000 bttc-0.0.73.3/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.3/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16092 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2290 2024-04-10 01:55:39.000000 bttc-0.0.73.3/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22552 2024-04-10 00:48:38.000000 bttc-0.0.73.3/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.376922 bttc-0.0.73.3/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.384922 bttc-0.0.73.3/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.384922 bttc-0.0.73.3/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.3/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.3/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 01:57:15.380922 bttc-0.0.73.3/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 01:57:15.000000 bttc-0.0.73.3/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 01:57:15.384922 bttc-0.0.73.3/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.3/setup.py
```

### Comparing `bttc-0.0.73.1/LICENSE` & `bttc-0.0.73.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/PKG-INFO` & `bttc-0.0.73.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.1
+Version: 0.0.73.3
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.1/README.md` & `bttc-0.0.73.3/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/__init__.py` & `bttc-0.0.73.3/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.73.1'
+__version__ = '0.0.73.3'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.73.1/bttc/apk_utils.py` & `bttc-0.0.73.3/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/ble_data.py` & `bttc-0.0.73.3/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/ble_utils.py` & `bttc-0.0.73.3/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/bt_data.py` & `bttc-0.0.73.3/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/bt_utils.py` & `bttc-0.0.73.3/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/cli/__init__.py` & `bttc-0.0.73.3/bttc/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,23 @@
 )
 
 
 CommandSet = cmd2.CommandSet
 Color = constants.Color
 
 
+class BttcCommandSet(CommandSet):
+  """BTTC Command set base class."""
+
+  def __init__(self, app: 'BttcCmdApp'):
+    super().__init__()
+    self._app = app
+    self.namespace_history = []
+
+
 def with_default_category(
     category: str, *, heritable: bool = True) -> Callable[
         [Type['CommandSet']], Type['CommandSet']]:
     """
     Decorator that applies a category to all ``do_*`` command methods in a class
     that do not already have a category specified.
```

### Comparing `bttc-0.0.73.1/bttc/cli/constants.py` & `bttc-0.0.73.3/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/cli/main.py` & `bttc-0.0.73.3/bttc/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import mobly
 import os
 import pathlib
 from ppadb import client
 from pprint import pprint
 import re
 import sys
+from typing import Any
 
 import bttc
 from bttc import constants as bttc_constants
 from bttc.cli import constants
 from bttc.utils import device_factory
 
 
@@ -466,22 +467,26 @@
             'dut_init_snippet_uiautomator', bool,
             'Initialize snippet_uiautomator in DUT during selection.', self))
     self.add_settable(
         cmd2.Settable(
             'dut_init_sl4a', bool,
             'Initialize SL4A in DUT during selection.', self))
 
-    self._dut = None
+    self._dut: Any = None
     if serial:
       self._init_dut(serial)
 
     self.logcat_pattern_history = []
     self.selected_device_history = [
         device.serial for device in self.adb.devices()]
 
+  @property
+  def dut(self) -> Any:
+    return self._dut
+
   def _init_dut(self, serial: str):
     self._dut = bttc.get(
         serial,
         init_snippet_uiautomator=self.dut_init_snippet_uiautomator,
         init_sl4a=self.dut_init_sl4a)
     self.prompt = BttcCmdApp.DEVICE_PROMPT_PROMPT.format(serial=serial)
```

### Comparing `bttc-0.0.73.1/bttc/common_data.py` & `bttc-0.0.73.3/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/constants.py` & `bttc-0.0.73.3/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/core.py` & `bttc-0.0.73.3/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/errors.py` & `bttc-0.0.73.3/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/general_utils.py` & `bttc-0.0.73.3/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.73.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.73.3/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.73.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.73.3/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.73.3/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/avrcp/errors.py` & `bttc-0.0.73.3/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/hfp/__init__.py` & `bttc-0.0.73.3/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/hfp/constants.py` & `bttc-0.0.73.3/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/hfp/errors.py` & `bttc-0.0.73.3/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.73.3/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.73.3/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.73.3/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.73.3/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/strategy.py` & `bttc-0.0.73.3/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/ad_checker.py` & `bttc-0.0.73.3/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/device_factory.py` & `bttc-0.0.73.3/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/iperf/__init__.py` & `bttc-0.0.73.3/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/iperf/errors.py` & `bttc-0.0.73.3/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/key_events_handler.py` & `bttc-0.0.73.3/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/log_parser.py` & `bttc-0.0.73.3/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/logcat.py` & `bttc-0.0.73.3/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/retry.py` & `bttc-0.0.73.3/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils/typing_utils.py` & `bttc-0.0.73.3/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/utils_loader.py` & `bttc-0.0.73.3/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc/wifi_utils.py` & `bttc-0.0.73.3/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/bttc.egg-info/PKG-INFO` & `bttc-0.0.73.3/bttc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.1
+Version: 0.0.73.3
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.1/bttc.egg-info/SOURCES.txt` & `bttc-0.0.73.3/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.1/setup.py` & `bttc-0.0.73.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         'bttc.mobly_android_device_lib.services'],
     install_requires=[
         'cmd2==2.4.3',
         'deprecation==2.1.0',
         'mobly>=1.12.2',
         'portpicker==1.6.0',
         'psutil==5.9.8',
+        'python-dotenv==1.0.1',
         'PyYAML==6.0.1',
         'numpy',
         'six==1.16.0',
         'pure-python-adb==0.3.0.dev0',
         'snippet-uiautomator>=1.1.0',
     ],
     classifiers=[
```

