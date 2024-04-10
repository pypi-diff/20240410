# Comparing `tmp/celitech-sdk-1.0.0.tar.gz` & `tmp/celitech-sdk-1.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech-sdk-1.0.0.tar", last modified: Wed Apr 10 10:52:49 2024, max compression
+gzip compressed data, was "celitech-sdk-1.1.46.tar", last modified: Wed Apr 10 11:33:12 2024, max compression
```

## Comparing `celitech-sdk-1.0.0.tar` & `celitech-sdk-1.1.46.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.240018 celitech-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-04-10 10:52:49.240018 celitech-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:52:49.240018 celitech-sdk-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.224018 celitech-sdk-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.228018 celitech-sdk-1.0.0/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.228018 celitech-sdk-1.0.0/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.232018 celitech-sdk-1.0.0/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.232018 celitech-sdk-1.0.0/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.232018 celitech-sdk-1.0.0/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.232018 celitech-sdk-1.0.0/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.232018 celitech-sdk-1.0.0/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.232018 celitech-sdk-1.0.0/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.232018 celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.236018 celitech-sdk-1.0.0/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.236018 celitech-sdk-1.0.0/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.236018 celitech-sdk-1.0.0/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-10 10:52:37.000000 celitech-sdk-1.0.0/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:52:49.236018 celitech-sdk-1.0.0/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-04-10 10:52:49.000000 celitech-sdk-1.0.0/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-10 10:52:49.000000 celitech-sdk-1.0.0/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:52:49.000000 celitech-sdk-1.0.0/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 10:52:49.000000 celitech-sdk-1.0.0/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 10:52:49.000000 celitech-sdk-1.0.0/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.943633 celitech-sdk-1.1.46/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.943633 celitech-sdk-1.1.46/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.943633 celitech-sdk-1.1.46/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.947633 celitech-sdk-1.1.46/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.951633 celitech-sdk-1.1.46/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-10 11:33:00.000000 celitech-sdk-1.1.46/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:33:12.955633 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 11:33:12.000000 celitech-sdk-1.1.46/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech-sdk-1.0.0/LICENSE` & `celitech-sdk-1.1.46/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/PKG-INFO` & `celitech-sdk-1.1.46/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: celitech-sdk
-Version: 1.0.0
-Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Celitech Python SDK 1.0.0
+# Celitech Python SDK 1.1.46
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.0.0
+- SDK version: 1.1.46
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -103,20 +93,20 @@
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | destination | str | ❌ | List of available packages |
-| startDate | str | ❌ | List of available packages |
-| endDate | str | ❌ | List of available packages |
-| afterCursor | str | ❌ | List of available packages |
+| start_date | str | ❌ | List of available packages |
+| end_date | str | ❌ | List of available packages |
+| after_cursor | str | ❌ | List of available packages |
 | limit | float | ❌ | List of available packages |
-| startTime | int | ❌ | List of available packages |
-| endTime | int | ❌ | List of available packages |
+| start_time | int | ❌ | List of available packages |
+| end_time | int | ❌ | List of available packages |
 | duration | float | ❌ | List of available packages |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
@@ -130,17 +120,17 @@
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    start_time=8,
-    end_time=2,
-    duration=8.44
+    start_time=3,
+    end_time=10,
+    duration=6.67
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -161,17 +151,17 @@
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | iccid | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| afterDate | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| beforeDate | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| afterCursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_cursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | limit | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | after | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | before | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
@@ -187,16 +177,16 @@
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    after=2.38,
-    before=3.34
+    after=8.42,
+    before=3.39
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -227,16 +217,16 @@
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
     "network_brand": "CELITECH",
-    "start_time": 2.37,
-    "end_time": 8.12
+    "start_time": 1.92,
+    "end_time": 1.94
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -268,16 +258,16 @@
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "start_time": 8.12,
-    "end_time": 4.35
+    "start_time": 6.98,
+    "end_time": 7.77
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -307,16 +297,16 @@
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "start_time": 8.76,
-    "end_time": 4.68
+    "start_time": 8.42,
+    "end_time": 5.43
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -326,15 +316,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| purchaseId | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+| purchase_id | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech-sdk-1.0.0/README.md` & `celitech-sdk-1.1.46/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# Celitech Python SDK 1.0.0
+Metadata-Version: 2.1
+Name: celitech-sdk
+Version: 1.1.46
+Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Celitech Python SDK 1.1.46
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.0.0
+- SDK version: 1.1.46
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -93,20 +103,20 @@
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | destination | str | ❌ | List of available packages |
-| startDate | str | ❌ | List of available packages |
-| endDate | str | ❌ | List of available packages |
-| afterCursor | str | ❌ | List of available packages |
+| start_date | str | ❌ | List of available packages |
+| end_date | str | ❌ | List of available packages |
+| after_cursor | str | ❌ | List of available packages |
 | limit | float | ❌ | List of available packages |
-| startTime | int | ❌ | List of available packages |
-| endTime | int | ❌ | List of available packages |
+| start_time | int | ❌ | List of available packages |
+| end_time | int | ❌ | List of available packages |
 | duration | float | ❌ | List of available packages |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
@@ -120,17 +130,17 @@
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    start_time=8,
-    end_time=2,
-    duration=8.44
+    start_time=3,
+    end_time=10,
+    duration=6.67
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -151,17 +161,17 @@
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | iccid | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| afterDate | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| beforeDate | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| afterCursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_cursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | limit | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | after | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | before | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
@@ -177,16 +187,16 @@
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    after=2.38,
-    before=3.34
+    after=8.42,
+    before=3.39
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -217,16 +227,16 @@
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
     "network_brand": "CELITECH",
-    "start_time": 2.37,
-    "end_time": 8.12
+    "start_time": 1.92,
+    "end_time": 1.94
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -258,16 +268,16 @@
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "start_time": 8.12,
-    "end_time": 4.35
+    "start_time": 6.98,
+    "end_time": 7.77
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -297,16 +307,16 @@
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "start_time": 8.76,
-    "end_time": 4.68
+    "start_time": 8.42,
+    "end_time": 5.43
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -316,15 +326,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| purchaseId | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+| purchase_id | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech-sdk-1.0.0/src/celitech/hooks/hook.py` & `celitech-sdk-1.1.46/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/__init__.py` & `celitech-sdk-1.1.46/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/base.py` & `celitech-sdk-1.1.46/src/celitech/models/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         """
         if value is None:
             return None
 
         if re.match(r"{}".format(pattern), value):
             return value
         else:
-            raise ValueError(f"Invalid value for {variable_name}: must match {pattern}")
+            raise ValueError(
+                f"Invalid value for {variable_name}: must match {pattern}, received {value}"
+            )
 
     def _enum_matching(
         self, value: Union[str, Enum], enum_values: List[str], variable_name: str
     ):
         """
         Checks if a value (str or enum) matches the required enum values and returns the value if there's a match.
 
@@ -53,15 +55,15 @@
             return None
 
         str_value = value.value if isinstance(value, Enum) else value
         if str_value in enum_values:
             return value
         else:
             raise ValueError(
-                f"Invalid value for {variable_name}: must match one of {enum_values}"
+                f"Invalid value for {variable_name}: must match one of {enum_values}, received {value}"
             )
 
     def _define_object(self, input_data, input_class):
         """
         Check if the input data is an instance of the input class and return the input data if it is.
         Otherwise, return an instance of the input class.
 
@@ -181,14 +183,15 @@
         if input_data is None:
             return None
 
         if isinstance(input_data, (str, float, int, bool)):
             return input_data
 
         for class_constructor in cls.class_list.values():
+            exception_list = []
             try:
                 # Check if the class is a only a TypeHint
                 origin = get_origin(class_constructor)
                 if origin is not None and isinstance(input_data, list):
                     list_instance = cls._get_list_instance(
                         input_data, class_constructor, origin
                     )
@@ -202,20 +205,18 @@
                     return input_data
 
                 # Check if the input_data is a dictionary that can be used to initialize the class
                 elif isinstance(input_data, dict):
                     instance = class_constructor._unmap(input_data)
                     if cls._check_params(input_data, instance):
                         return instance
-            except Exception:
-                pass
+            except Exception as e:
+                exception_list.append({"class": class_constructor, "exception": e})
 
-        raise ValueError(
-            f"Input data must match one of the models: {list(cls.class_list.keys())}"
-        )
+        cls._raise_one_of_error(exception_list)
 
     @classmethod
     def _get_list_instance(cls, input_data, class_constructor, origin):
         """
         Return the list of elements for a given class constructor and origin type.
 
         :param input_data: The input data to check.
@@ -245,7 +246,27 @@
         """
         input_values = {k: v for k, v in raw_input.items() if v is not None}.values()
         instance_map = instance._map()
         instance_values = {
             k: v for k, v in instance_map.items() if v is not None
         }.values()
         return len(input_values) == len(instance_values)
+
+    @classmethod
+    def _raise_one_of_error(cls, exception_list):
+        """
+        Raises a ValueError with the appropriate error message for one of models.
+
+        :param exception_list: List of exceptions that occurred.
+        :type exception_list: list
+        :raises ValueError: If input data does not match any of the models.
+        """
+        if not exception_list:
+            return
+        exception_messages = "\n".join(
+            f"Class: {exception['class']}, Exception: {exception['exception']}"
+            for exception in exception_list
+        )
+        raise ValueError(
+            f"Input data must match one of the models: {list(cls.class_list.keys())}"
+            f"Errors occurred:\n{exception_messages}"
+        )
```

### Comparing `celitech-sdk-1.0.0/src/celitech/models/create_purchase_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/create_purchase_request.py` & `celitech-sdk-1.1.46/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/edit_purchase_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/edit_purchase_request.py` & `celitech-sdk-1.1.46/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/get_esim_device_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/get_esim_history_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/get_esim_mac_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/get_esim_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/list_destinations_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/list_packages_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/list_purchases_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/top_up_esim_ok_response.py` & `celitech-sdk-1.1.46/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/top_up_esim_request.py` & `celitech-sdk-1.1.46/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/utils/cast_models.py` & `celitech-sdk-1.1.46/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/models/utils/json_map.py` & `celitech-sdk-1.1.46/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech-sdk-1.1.46/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/request_chain/request_chain.py` & `celitech-sdk-1.1.46/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/transport/request.py` & `celitech-sdk-1.1.46/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/transport/request_error.py` & `celitech-sdk-1.1.46/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/transport/response.py` & `celitech-sdk-1.1.46/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/transport/serializer.py` & `celitech-sdk-1.1.46/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/net/transport/utils.py` & `celitech-sdk-1.1.46/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/sdk.py` & `celitech-sdk-1.1.46/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/services/destinations.py` & `celitech-sdk-1.1.46/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/services/e_sim.py` & `celitech-sdk-1.1.46/src/celitech/services/e_sim.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: GetEsimOkResponse
         """
 
-        Validator(str).validate(iccid)
+        Validator(str).min_length(18).max_length(22).validate(iccid)
 
         serialized_request = (
             Serializer(f"{self.base_url}/esim", self.get_default_headers())
             .add_query("iccid", iccid)
             .serialize()
             .set_method("GET")
         )
@@ -45,15 +45,15 @@
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: GetEsimDeviceOkResponse
         """
 
-        Validator(str).validate(iccid)
+        Validator(str).min_length(18).max_length(22).validate(iccid)
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/esim/{{iccid}}/device", self.get_default_headers()
             )
             .add_path("iccid", iccid)
             .serialize()
@@ -73,15 +73,15 @@
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: GetEsimHistoryOkResponse
         """
 
-        Validator(str).validate(iccid)
+        Validator(str).min_length(18).max_length(22).validate(iccid)
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/esim/{{iccid}}/history", self.get_default_headers()
             )
             .add_path("iccid", iccid)
             .serialize()
@@ -101,15 +101,15 @@
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: GetEsimMacOkResponse
         """
 
-        Validator(str).validate(iccid)
+        Validator(str).min_length(18).max_length(22).validate(iccid)
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/esim/{{iccid}}/mac", self.get_default_headers()
             )
             .add_path("iccid", iccid)
             .serialize()
```

### Comparing `celitech-sdk-1.0.0/src/celitech/services/packages.py` & `celitech-sdk-1.1.46/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/services/purchases.py` & `celitech-sdk-1.1.46/src/celitech/services/purchases.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: ListPurchasesOkResponse
         """
 
-        Validator(str).is_optional().validate(iccid)
+        Validator(str).is_optional().min_length(18).max_length(22).validate(iccid)
         Validator(str).is_optional().validate(after_date)
         Validator(str).is_optional().validate(before_date)
         Validator(str).is_optional().validate(after_cursor)
         Validator(float).is_optional().validate(limit)
         Validator(float).is_optional().validate(after)
         Validator(float).is_optional().validate(before)
```

### Comparing `celitech-sdk-1.0.0/src/celitech/services/utils/base_service.py` & `celitech-sdk-1.1.46/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/services/utils/default_headers.py` & `celitech-sdk-1.1.46/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.0.0/src/celitech/services/utils/validator.py` & `celitech-sdk-1.1.46/src/celitech/services/utils/validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import operator
 from typing import Union, Any, Type, Pattern, get_args
 from ...models.base import OneOfBaseModel
 
 
 class Validator:
     """
     A simple validator class for validating the type and pattern of a value.
@@ -21,16 +22,20 @@
 
         :param Type[Any] _type: The expected type for the value. Defaults to None.
         """
         self._type: Type[Any] = _type
         self._is_optional: bool = False
         self._is_array: bool = False
         self._pattern: Pattern[str] = None
+        self._min_length: int = None
+        self._max_length: int = None
         self._min: int = None
+        self._min_exclusive: bool = False
         self._max: int = None
+        self._max_exclusive: bool = False
 
     def is_array(self) -> "Validator":
         """
         Marks the value as an array.
 
         :return: The Validator instance for method chaining.
         :rtype: Validator
@@ -55,34 +60,60 @@
         :param str pattern: The regular expression pattern.
         :return: The Validator instance for method chaining.
         :rtype: Validator
         """
         self._pattern = re.compile(pattern)
         return self
 
-    def min(self, min: int) -> "Validator":
+    def min(self, min: int, exclusive=False) -> "Validator":
         """
         Specifies a minimum value for validating the value.
 
-        :param int min: The minimum value.
+        :param int min: The minimum value to be validated against.
+        :param bool exclusive: (optional) If set to True, the minimum value is not inclusive.
         :return: The Validator instance for method chaining.
         :rtype: Validator
         """
         self._min = min
+        self._min_exclusive = exclusive
         return self
 
-    def max(self, max: int) -> "Validator":
+    def max(self, max: int, exclusive=False) -> "Validator":
         """
         Specifies a maximum value for validating the value.
 
         :param int max: The maximum value.
+        :param bool exclusive: (optional) If set to True, the maximum value is not inclusive.
         :return: The Validator instance for method chaining.
         :rtype: Validator
         """
         self._max = max
+        self._max_exclusive = exclusive
+        return self
+
+    def min_length(self, min_length: int) -> "Validator":
+        """
+        Specifies a minimum length for validating the value.
+
+        :param int min_length: The minimum length to be validated against.
+        :return: The Validator instance for method chaining.
+        :rtype: Validator
+        """
+        self._min_length = min_length
+        return self
+
+    def max_length(self, max_length: int) -> "Validator":
+        """
+        Specifies a maximum length for validating the value.
+
+        :param int max_length: The maximum length.
+        :return: The Validator instance for method chaining.
+        :rtype: Validator
+        """
+        self._max_length = max_length
         return self
 
     def validate(self, value: Any) -> None:
         """
         Validates the provided value based on the specified criteria.
 
         :param Any value: The input that needs to be checked
@@ -146,18 +177,33 @@
     def _validate_rules(self, value: Any) -> None:
         """
         Validate the rules specified for the value.
 
         :param Any value: The input that needs to be validated
         :raises ValueError: If the value does not meet the specified validation criteria.
         """
-        if self._min is not None and value < self._min:
-            raise ValueError(f"Invalid value: {value} is less than {self._min}")
-        if self._max is not None and value > self._max:
-            raise ValueError(f"Invalid value: {value} is greater than {self._max}")
+        min_operator = operator.lt if self._min_exclusive else operator.le
+        max_operator = operator.gt if self._max_exclusive else operator.ge
+
+        if self._min is not None and not min_operator(self._min, value):
+            raise ValueError(
+                f"Invalid value: {value} is {'less than or equal to' if self._min_exclusive else 'less than'} {self._min}"
+            )
+        if self._max is not None and not max_operator(self._max, value):
+            raise ValueError(
+                f"Invalid value: {value} is {'greater than or equal to' if self._max_exclusive else 'greater than'} {self._max}"
+            )
+        if self._min_length is not None and len(value) < self._min_length:
+            raise ValueError(
+                f"Invalid value: the length of {value} is less than {self._min_length}"
+            )
+        if self._max_length is not None and len(value) > self._max_length:
+            raise ValueError(
+                f"Invalid value: the length of {value} is greater than {self._max_length}"
+            )
         if self._pattern and not self._pattern.match(str(value)):
             raise ValueError(
                 f"Invalid value: {value} does not match pattern {self._pattern}"
             )
 
     def _is_one_of_type(self, cls_type):
         """
```

### Comparing `celitech-sdk-1.0.0/src/celitech_sdk.egg-info/PKG-INFO` & `celitech-sdk-1.1.46/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.0.0
+Version: 1.1.46
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.0.0
+# Celitech Python SDK 1.1.46
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.0.0
+- SDK version: 1.1.46
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -103,20 +103,20 @@
 - HTTP Method: `GET`
 - Endpoint: `/packages`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | destination | str | ❌ | List of available packages |
-| startDate | str | ❌ | List of available packages |
-| endDate | str | ❌ | List of available packages |
-| afterCursor | str | ❌ | List of available packages |
+| start_date | str | ❌ | List of available packages |
+| end_date | str | ❌ | List of available packages |
+| after_cursor | str | ❌ | List of available packages |
 | limit | float | ❌ | List of available packages |
-| startTime | int | ❌ | List of available packages |
-| endTime | int | ❌ | List of available packages |
+| start_time | int | ❌ | List of available packages |
+| end_time | int | ❌ | List of available packages |
 | duration | float | ❌ | List of available packages |
 
 **Return Type**
 
 `ListPackagesOkResponse`
 
 **Example Usage Code Snippet**
@@ -130,17 +130,17 @@
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    start_time=8,
-    end_time=2,
-    duration=8.44
+    start_time=3,
+    end_time=10,
+    duration=6.67
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -161,17 +161,17 @@
 - HTTP Method: `GET`
 - Endpoint: `/purchases`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | iccid | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| afterDate | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| beforeDate | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
-| afterCursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| before_date | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
+| after_cursor | str | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | limit | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | after | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 | before | float | ❌ | This endpoint can be used to list all the successful purchases made between a given interval. |
 
 **Return Type**
 
 `ListPurchasesOkResponse`
@@ -187,16 +187,16 @@
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
     limit=20,
-    after=2.38,
-    before=3.34
+    after=8.42,
+    before=3.39
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
-    "start_time": 2.37,
-    "end_time": 8.12
+    "start_time": 1.92,
+    "end_time": 1.94
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
-    "start_time": 8.12,
-    "end_time": 4.35
+    "start_time": 6.98,
+    "end_time": 7.77
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
-    "start_time": 8.76,
-    "end_time": 4.68
+    "start_time": 8.42,
+    "end_time": 5.43
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -326,15 +326,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/purchases/{purchaseId}/consumption`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| purchaseId | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
+| purchase_id | str | ✅ | This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages. |
 
 **Return Type**
 
 `GetPurchaseConsumptionOkResponse`
 
 **Example Usage Code Snippet**
```

### Comparing `celitech-sdk-1.0.0/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech-sdk-1.1.46/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

