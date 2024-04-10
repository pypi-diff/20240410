# Comparing `tmp/celitech-sdk-1.1.46.tar.gz` & `tmp/celitech-sdk-1.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech-sdk-1.1.46.tar", last modified: Wed Apr 10 11:33:12 2024, max compression
+gzip compressed data, was "celitech-sdk-1.1.47.tar", last modified: Wed Apr 10 11:55:27 2024, max compression
```

## Comparing `celitech-sdk-1.1.46.tar` & `celitech-sdk-1.1.47.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.943633 celitech-sdk-1.1.46/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.943633 celitech-sdk-1.1.46/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.943633 celitech-sdk-1.1.46/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.779032 celitech-sdk-1.1.47/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-04-10 11:55:27.779032 celitech-sdk-1.1.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:55:27.779032 celitech-sdk-1.1.47/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.767032 celitech-sdk-1.1.47/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.767032 celitech-sdk-1.1.47/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.767032 celitech-sdk-1.1.47/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.771032 celitech-sdk-1.1.47/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.771032 celitech-sdk-1.1.47/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.771032 celitech-sdk-1.1.47/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.771032 celitech-sdk-1.1.47/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.775032 celitech-sdk-1.1.47/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.775032 celitech-sdk-1.1.47/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.775032 celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.775032 celitech-sdk-1.1.47/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.775032 celitech-sdk-1.1.47/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.779032 celitech-sdk-1.1.47/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-10 11:55:16.000000 celitech-sdk-1.1.47/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:55:27.779032 celitech-sdk-1.1.47/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-04-10 11:55:27.000000 celitech-sdk-1.1.47/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-10 11:55:27.000000 celitech-sdk-1.1.47/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:55:27.000000 celitech-sdk-1.1.47/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 11:55:27.000000 celitech-sdk-1.1.47/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 11:55:27.000000 celitech-sdk-1.1.47/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech-sdk-1.1.46/LICENSE` & `celitech-sdk-1.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/PKG-INFO` & `celitech-sdk-1.1.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.46
+Version: 1.1.47
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.46
+# Celitech Python SDK 1.1.47
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.46
+- SDK version: 1.1.47
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -130,17 +130,17 @@
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    start_time=3,
-    end_time=10,
-    duration=6.67
+    start_time=8,
+    end_time=2,
+    duration=8.44
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -187,16 +187,16 @@
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    after=8.42,
-    before=3.39
+    after=2.38,
+    before=3.34
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -227,16 +227,16 @@
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
     "network_brand": "CELITECH",
-    "start_time": 1.92,
-    "end_time": 1.94
+    "start_time": 2.37,
+    "end_time": 8.12
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -268,16 +268,16 @@
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "start_time": 6.98,
-    "end_time": 7.77
+    "start_time": 8.12,
+    "end_time": 4.35
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -307,16 +307,16 @@
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "start_time": 8.42,
-    "end_time": 5.43
+    "start_time": 8.76,
+    "end_time": 4.68
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
```

### Comparing `celitech-sdk-1.1.46/README.md` & `celitech-sdk-1.1.47/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Celitech Python SDK 1.1.46
+# Celitech Python SDK 1.1.47
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.46
+- SDK version: 1.1.47
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -120,17 +120,17 @@
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    start_time=3,
-    end_time=10,
-    duration=6.67
+    start_time=8,
+    end_time=2,
+    duration=8.44
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -177,16 +177,16 @@
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    after=8.42,
-    before=3.39
+    after=2.38,
+    before=3.34
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -217,16 +217,16 @@
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
     "network_brand": "CELITECH",
-    "start_time": 1.92,
-    "end_time": 1.94
+    "start_time": 2.37,
+    "end_time": 8.12
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -258,16 +258,16 @@
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "start_time": 6.98,
-    "end_time": 7.77
+    "start_time": 8.12,
+    "end_time": 4.35
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -297,16 +297,16 @@
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "start_time": 8.42,
-    "end_time": 5.43
+    "start_time": 8.76,
+    "end_time": 4.68
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
```

### Comparing `celitech-sdk-1.1.46/src/celitech/hooks/hook.py` & `celitech-sdk-1.1.47/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/__init__.py` & `celitech-sdk-1.1.47/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/base.py` & `celitech-sdk-1.1.47/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/create_purchase_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/create_purchase_request.py` & `celitech-sdk-1.1.47/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/edit_purchase_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/edit_purchase_request.py` & `celitech-sdk-1.1.47/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/get_esim_device_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/get_esim_history_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/get_esim_mac_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/get_esim_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/list_destinations_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/list_packages_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/list_purchases_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/top_up_esim_ok_response.py` & `celitech-sdk-1.1.47/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/top_up_esim_request.py` & `celitech-sdk-1.1.47/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/utils/cast_models.py` & `celitech-sdk-1.1.47/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/models/utils/json_map.py` & `celitech-sdk-1.1.47/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech-sdk-1.1.47/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/request_chain/request_chain.py` & `celitech-sdk-1.1.47/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/transport/request.py` & `celitech-sdk-1.1.47/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/transport/request_error.py` & `celitech-sdk-1.1.47/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/transport/response.py` & `celitech-sdk-1.1.47/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/transport/serializer.py` & `celitech-sdk-1.1.47/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/net/transport/utils.py` & `celitech-sdk-1.1.47/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/sdk.py` & `celitech-sdk-1.1.47/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/services/destinations.py` & `celitech-sdk-1.1.47/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/services/e_sim.py` & `celitech-sdk-1.1.47/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/services/packages.py` & `celitech-sdk-1.1.47/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/services/purchases.py` & `celitech-sdk-1.1.47/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/services/utils/base_service.py` & `celitech-sdk-1.1.47/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/services/utils/default_headers.py` & `celitech-sdk-1.1.47/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech/services/utils/validator.py` & `celitech-sdk-1.1.47/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.46/src/celitech_sdk.egg-info/PKG-INFO` & `celitech-sdk-1.1.47/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.46
+Version: 1.1.47
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.46
+# Celitech Python SDK 1.1.47
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.46
+- SDK version: 1.1.47
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -130,17 +130,17 @@
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    start_time=3,
-    end_time=10,
-    duration=6.67
+    start_time=8,
+    end_time=2,
+    duration=8.44
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -187,16 +187,16 @@
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    after=8.42,
-    before=3.39
+    after=2.38,
+    before=3.34
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -227,16 +227,16 @@
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
     "network_brand": "CELITECH",
-    "start_time": 1.92,
-    "end_time": 1.94
+    "start_time": 2.37,
+    "end_time": 8.12
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -268,16 +268,16 @@
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "start_time": 6.98,
-    "end_time": 7.77
+    "start_time": 8.12,
+    "end_time": 4.35
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -307,16 +307,16 @@
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "start_time": 8.42,
-    "end_time": 5.43
+    "start_time": 8.76,
+    "end_time": 4.68
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
```

### Comparing `celitech-sdk-1.1.46/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech-sdk-1.1.47/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*
