# Comparing `tmp/bttc-0.0.73.7.tar.gz` & `tmp/bttc-0.0.73.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.73.7.tar", last modified: Wed Apr 10 05:55:08 2024, max compression
+gzip compressed data, was "bttc-0.0.73.8.tar", last modified: Wed Apr 10 06:02:37 2024, max compression
```

## Comparing `bttc-0.0.73.7.tar` & `bttc-0.0.73.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.050225 bttc-0.0.73.7/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.7/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 05:55:08.050225 bttc-0.0.73.7/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.7/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.046225 bttc-0.0.73.7/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-10 05:54:23.000000 bttc-0.0.73.7/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.7/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.7/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-10 05:33:38.000000 bttc-0.0.73.7/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.046225 bttc-0.0.73.7/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2155 2024-04-10 02:58:12.000000 bttc-0.0.73.7/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22454 2024-04-10 02:58:23.000000 bttc-0.0.73.7/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.7/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.046225 bttc-0.0.73.7/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.046225 bttc-0.0.73.7/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.046225 bttc-0.0.73.7/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.050225 bttc-0.0.73.7/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.050225 bttc-0.0.73.7/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.050225 bttc-0.0.73.7/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.050225 bttc-0.0.73.7/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.7/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.7/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 05:55:08.046225 bttc-0.0.73.7/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 05:55:08.000000 bttc-0.0.73.7/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 05:55:08.000000 bttc-0.0.73.7/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 05:55:08.000000 bttc-0.0.73.7/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 05:55:08.000000 bttc-0.0.73.7/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 05:55:08.000000 bttc-0.0.73.7/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 05:55:08.050225 bttc-0.0.73.7/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.7/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.634044 bttc-0.0.73.8/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.8/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 06:02:37.634044 bttc-0.0.73.8/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.8/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-10 06:02:27.000000 bttc-0.0.73.8/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.8/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.8/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-10 05:57:16.000000 bttc-0.0.73.8/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.73.8/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22454 2024-04-10 02:58:23.000000 bttc-0.0.73.8/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.8/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.626044 bttc-0.0.73.8/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.634044 bttc-0.0.73.8/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.634044 bttc-0.0.73.8/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.8/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 06:02:37.634044 bttc-0.0.73.8/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.8/setup.py
```

### Comparing `bttc-0.0.73.7/LICENSE` & `bttc-0.0.73.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/PKG-INFO` & `bttc-0.0.73.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.7
+Version: 0.0.73.8
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.7/README.md` & `bttc-0.0.73.8/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/__init__.py` & `bttc-0.0.73.8/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.73.7'
+__version__ = '0.0.73.8'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.73.7/bttc/apk_utils.py` & `bttc-0.0.73.8/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/ble_data.py` & `bttc-0.0.73.8/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/ble_utils.py` & `bttc-0.0.73.8/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/bt_data.py` & `bttc-0.0.73.8/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/bt_utils.py` & `bttc-0.0.73.8/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/cli/__init__.py` & `bttc-0.0.73.8/bttc/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Entry point of BTTC Cli."""
 
 from bttc.cli import constants
-from bttc.cli import main
 import cmd2
 from typing import (
     Callable,
     Type,
 )
 
 
-BttcCmdApp = main.BttcCmdApp
 CommandSet = cmd2.CommandSet
 Color = constants.Color
 
 
 def with_default_category(
     category: str, *, heritable: bool = True) -> Callable[
         [Type['CommandSet']], Type['CommandSet']]:
```

### Comparing `bttc-0.0.73.7/bttc/cli/constants.py` & `bttc-0.0.73.8/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/cli/main.py` & `bttc-0.0.73.8/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/common_data.py` & `bttc-0.0.73.8/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/constants.py` & `bttc-0.0.73.8/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/core.py` & `bttc-0.0.73.8/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/errors.py` & `bttc-0.0.73.8/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/general_utils.py` & `bttc-0.0.73.8/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.73.8/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.73.8/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.73.8/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/avrcp/errors.py` & `bttc-0.0.73.8/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/hfp/__init__.py` & `bttc-0.0.73.8/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/hfp/constants.py` & `bttc-0.0.73.8/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/hfp/errors.py` & `bttc-0.0.73.8/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.73.8/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.73.8/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.73.8/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.73.8/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/strategy.py` & `bttc-0.0.73.8/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/ad_checker.py` & `bttc-0.0.73.8/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/device_factory.py` & `bttc-0.0.73.8/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/iperf/__init__.py` & `bttc-0.0.73.8/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/iperf/errors.py` & `bttc-0.0.73.8/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/key_events_handler.py` & `bttc-0.0.73.8/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/log_parser.py` & `bttc-0.0.73.8/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/logcat.py` & `bttc-0.0.73.8/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/retry.py` & `bttc-0.0.73.8/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils/typing_utils.py` & `bttc-0.0.73.8/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/utils_loader.py` & `bttc-0.0.73.8/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc/wifi_utils.py` & `bttc-0.0.73.8/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/bttc.egg-info/PKG-INFO` & `bttc-0.0.73.8/bttc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.7
+Version: 0.0.73.8
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.7/bttc.egg-info/SOURCES.txt` & `bttc-0.0.73.8/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.7/setup.py` & `bttc-0.0.73.8/setup.py`

 * *Files identical despite different names*

