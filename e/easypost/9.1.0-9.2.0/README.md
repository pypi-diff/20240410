# Comparing `tmp/easypost-9.1.0.tar.gz` & `tmp/easypost-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypost-9.1.0.tar", last modified: Mon Jan  8 22:55:28 2024, max compression
+gzip compressed data, was "easypost-9.2.0.tar", last modified: Wed Apr 10 21:19:41 2024, max compression
```

## Comparing `easypost-9.1.0.tar` & `easypost-9.2.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.278814 easypost-9.1.0/
--rw-r--r--   0 jhammond   (502) staff       (20)    13635 2024-01-08 22:55:01.000000 easypost-9.1.0/CHANGELOG.md
--rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-9.1.0/LICENSE
--rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-9.1.0/MANIFEST.in
--rw-r--r--   0 jhammond   (502) staff       (20)     8816 2024-01-08 22:55:28.278495 easypost-9.1.0/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     6962 2023-10-30 20:37:03.000000 easypost-9.1.0/README.md
--rw-r--r--   0 jhammond   (502) staff       (20)     8348 2023-12-05 18:36:55.000000 easypost-9.1.0/UPGRADE_GUIDE.md
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.249186 easypost-9.1.0/easypost/
--rw-r--r--   0 jhammond   (502) staff       (20)      373 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2052 2024-01-08 22:55:01.000000 easypost-9.1.0/easypost/constant.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4510 2023-12-05 17:36:38.000000 easypost-9.1.0/easypost/easypost_client.py
--rw-r--r--   0 jhammond   (502) staff       (20)     6705 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/easypost_object.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.250789 easypost-9.1.0/easypost/errors/
--rw-r--r--   0 jhammond   (502) staff       (20)       87 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/__init__.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.255345 easypost-9.1.0/easypost/errors/api/
--rw-r--r--   0 jhammond   (502) staff       (20)     1253 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2327 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/api_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/bad_request_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/encoding_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/external_api_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/forbidden_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/gateway_timeout_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/http_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/internal_server_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/invalid_request_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/json_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/method_not_allowed_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/not_found_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/payment_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/rate_limit_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/redirect_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      103 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/service_unavailable_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/timeout_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/unauthorized_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/api/unknown_api_error.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.257272 easypost-9.1.0/easypost/errors/general/
--rw-r--r--   0 jhammond   (502) staff       (20)      560 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)      206 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/easypost_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      119 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/end_of_pagination_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      113 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/filtering_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      117 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/invalid_object_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/invalid_parameter_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/missing_parameter_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      125 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/errors/general/signature_verification_error.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.258100 easypost-9.1.0/easypost/hooks/
--rw-r--r--   0 jhammond   (502) staff       (20)      169 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/hooks/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)      475 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/hooks/event_hook.py
--rw-r--r--   0 jhammond   (502) staff       (20)      147 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/hooks/request_hook.py
--rw-r--r--   0 jhammond   (502) staff       (20)      154 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/hooks/response_hook.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.263370 easypost-9.1.0/easypost/models/
--rw-r--r--   0 jhammond   (502) staff       (20)     1145 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/address.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/api_key.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/batch.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/billing.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/brand.py
--rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/carrier_account.py
--rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/customs_info.py
--rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/customs_item.py
--rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/end_shipper.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/event.py
--rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/insurance.py
--rw-r--r--   0 jhammond   (502) staff       (20)      477 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/order.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/parcel.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/payload.py
--rw-r--r--   0 jhammond   (502) staff       (20)      495 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/pickup.py
--rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/pickup_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/postage_label.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/refund.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/report.py
--rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/scan_form.py
--rw-r--r--   0 jhammond   (502) staff       (20)      483 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/shipment.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/tracker.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/user.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/models/webhook.py
--rw-r--r--   0 jhammond   (502) staff       (20)        0 2023-06-26 19:26:52.000000 easypost-9.1.0/easypost/py.typed
--rw-r--r--   0 jhammond   (502) staff       (20)    12807 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/requestor.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.269092 easypost-9.1.0/easypost/services/
--rw-r--r--   0 jhammond   (502) staff       (20)     1623 2023-12-05 17:36:38.000000 easypost-9.1.0/easypost/services/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2723 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/address_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1381 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/api_key_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3560 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/base_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3364 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/batch_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      898 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/beta_rate_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2339 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/beta_referral_customer_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2805 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/billing_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2470 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/carrier_account_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1013 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/carrier_metadata_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/customs_info_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/customs_item_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1665 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/end_shipper_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2217 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/event_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1359 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/insurance_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1243 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/order_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      511 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/parcel_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2071 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/pickup_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      361 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/rate_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5736 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/referral_customer_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1342 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/refund_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2556 2023-12-12 18:11:05.000000 easypost-9.1.0/easypost/services/report_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1348 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/scan_form_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5732 2023-12-20 21:43:24.000000 easypost-9.1.0/easypost/services/shipment_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2148 2023-12-04 19:27:14.000000 easypost-9.1.0/easypost/services/tracker_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4480 2024-01-08 22:55:01.000000 easypost-9.1.0/easypost/services/user_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      996 2023-10-30 20:37:03.000000 easypost-9.1.0/easypost/services/webhook_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4660 2023-12-20 21:43:24.000000 easypost-9.1.0/easypost/util.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.277433 easypost-9.1.0/easypost.egg-info/
--rw-r--r--   0 jhammond   (502) staff       (20)     8816 2024-01-08 22:55:28.000000 easypost-9.1.0/easypost.egg-info/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     4157 2024-01-08 22:55:28.000000 easypost-9.1.0/easypost.egg-info/SOURCES.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        1 2024-01-08 22:55:28.000000 easypost-9.1.0/easypost.egg-info/dependency_links.txt
--rw-r--r--   0 jhammond   (502) staff       (20)      247 2024-01-08 22:55:28.000000 easypost-9.1.0/easypost.egg-info/requires.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        9 2024-01-08 22:55:28.000000 easypost-9.1.0/easypost.egg-info/top_level.txt
--rw-r--r--   0 jhammond   (502) staff       (20)       38 2024-01-08 22:55:28.278866 easypost-9.1.0/setup.cfg
--rw-r--r--   0 jhammond   (502) staff       (20)     2315 2024-01-08 22:55:01.000000 easypost-9.1.0/setup.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-01-08 22:55:28.276927 easypost-9.1.0/tests/
--rw-r--r--   0 jhammond   (502) staff       (20)     4806 2024-01-08 22:55:01.000000 easypost-9.1.0/tests/test_address.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1184 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_api_key.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2731 2023-10-30 20:37:05.000000 easypost-9.1.0/tests/test_base_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4075 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_batch.py
--rw-r--r--   0 jhammond   (502) staff       (20)      791 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_beta_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1853 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_beta_referral_customer.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4083 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_billing.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3343 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_carrier_account.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1108 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_carrier_metadata.py
--rw-r--r--   0 jhammond   (502) staff       (20)      718 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_customs_info.py
--rw-r--r--   0 jhammond   (502) staff       (20)      707 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_customs_item.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1817 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_easypost_client.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1738 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_end_shipper.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2284 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3726 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_event.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2238 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_hook.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2333 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_insurance.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2322 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_order.py
--rw-r--r--   0 jhammond   (502) staff       (20)      573 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_parcel.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4359 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_pickup.py
--rw-r--r--   0 jhammond   (502) staff       (20)      321 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4797 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_referral_customer.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2062 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_refund.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3212 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_report.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1945 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_scan_form.py
--rw-r--r--   0 jhammond   (502) staff       (20)    11810 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_shipment.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2300 2023-12-04 19:27:14.000000 easypost-9.1.0/tests/test_tracker.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3214 2024-01-08 22:55:01.000000 easypost-9.1.0/tests/test_user.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3262 2023-10-30 20:37:03.000000 easypost-9.1.0/tests/test_webhook.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.330761 easypost-9.2.0/
+-rw-r--r--   0 jhammond   (502) staff       (20)    13848 2024-04-10 21:19:00.000000 easypost-9.2.0/CHANGELOG.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-9.2.0/LICENSE
+-rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-9.2.0/MANIFEST.in
+-rw-r--r--   0 jhammond   (502) staff       (20)     8816 2024-04-10 21:19:41.330382 easypost-9.2.0/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     6962 2024-01-09 20:57:59.000000 easypost-9.2.0/README.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     8348 2024-01-09 20:57:59.000000 easypost-9.2.0/UPGRADE_GUIDE.md
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.310955 easypost-9.2.0/easypost/
+-rw-r--r--   0 jhammond   (502) staff       (20)      373 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2052 2024-04-10 21:19:00.000000 easypost-9.2.0/easypost/constant.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4510 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/easypost_client.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     6705 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/easypost_object.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.311860 easypost-9.2.0/easypost/errors/
+-rw-r--r--   0 jhammond   (502) staff       (20)       87 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/__init__.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.314410 easypost-9.2.0/easypost/errors/api/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1253 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/errors/api/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2327 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/api_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/errors/api/bad_request_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/encoding_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       96 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/external_api_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/forbidden_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/gateway_timeout_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       89 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/http_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/internal_server_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/invalid_request_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       89 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/json_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      101 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/method_not_allowed_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/not_found_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/payment_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/rate_limit_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/redirect_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      103 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/service_unavailable_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/timeout_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/unauthorized_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/api/unknown_api_error.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.315440 easypost-9.2.0/easypost/errors/general/
+-rw-r--r--   0 jhammond   (502) staff       (20)      560 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      206 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/easypost_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      119 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/end_of_pagination_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      113 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/filtering_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      117 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/invalid_object_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      120 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/invalid_parameter_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      120 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/missing_parameter_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      125 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/errors/general/signature_verification_error.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.315924 easypost-9.2.0/easypost/hooks/
+-rw-r--r--   0 jhammond   (502) staff       (20)      169 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/hooks/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      475 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/hooks/event_hook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      147 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/hooks/request_hook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      154 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/hooks/response_hook.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.319347 easypost-9.2.0/easypost/models/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1145 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/address.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/api_key.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/batch.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/billing.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/brand.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      101 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/carrier_account.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       98 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/customs_info.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       98 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/customs_item.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/end_shipper.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/event.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       96 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/insurance.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      477 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/order.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/parcel.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/payload.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      495 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/pickup.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/pickup_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/postage_label.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/refund.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/report.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/scan_form.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      483 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/shipment.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/tracker.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/user.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/models/webhook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)        0 2023-06-26 19:26:52.000000 easypost-9.2.0/easypost/py.typed
+-rw-r--r--   0 jhammond   (502) staff       (20)    12807 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/requestor.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.322994 easypost-9.2.0/easypost/services/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1623 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2723 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/address_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1381 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/api_key_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3560 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/base_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3364 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/batch_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      898 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/beta_rate_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2339 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/beta_referral_customer_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2916 2024-04-10 21:19:00.000000 easypost-9.2.0/easypost/services/billing_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2470 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/carrier_account_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1013 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/carrier_metadata_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      546 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/customs_info_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      546 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/customs_item_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1665 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/end_shipper_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2217 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/event_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1762 2024-04-10 21:19:00.000000 easypost-9.2.0/easypost/services/insurance_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1243 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/order_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      511 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/parcel_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2071 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/pickup_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      361 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/rate_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5736 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/referral_customer_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1342 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/refund_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2556 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/report_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1348 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/scan_form_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5732 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/shipment_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2148 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/tracker_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4480 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/services/user_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      996 2024-01-09 19:36:56.000000 easypost-9.2.0/easypost/services/webhook_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4660 2024-01-09 20:57:59.000000 easypost-9.2.0/easypost/util.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.328850 easypost-9.2.0/easypost.egg-info/
+-rw-r--r--   0 jhammond   (502) staff       (20)     8816 2024-04-10 21:19:41.000000 easypost-9.2.0/easypost.egg-info/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     4157 2024-04-10 21:19:41.000000 easypost-9.2.0/easypost.egg-info/SOURCES.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        1 2024-04-10 21:19:41.000000 easypost-9.2.0/easypost.egg-info/dependency_links.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)      247 2024-04-10 21:19:41.000000 easypost-9.2.0/easypost.egg-info/requires.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        9 2024-04-10 21:19:41.000000 easypost-9.2.0/easypost.egg-info/top_level.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       38 2024-04-10 21:19:41.330811 easypost-9.2.0/setup.cfg
+-rw-r--r--   0 jhammond   (502) staff       (20)     2315 2024-04-10 21:19:00.000000 easypost-9.2.0/setup.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2024-04-10 21:19:41.328291 easypost-9.2.0/tests/
+-rw-r--r--   0 jhammond   (502) staff       (20)     4806 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_address.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1184 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_api_key.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2731 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_base_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4075 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_batch.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      791 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_beta_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1853 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_beta_referral_customer.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4929 2024-04-10 21:19:00.000000 easypost-9.2.0/tests/test_billing.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3343 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_carrier_account.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1108 2024-01-09 19:36:57.000000 easypost-9.2.0/tests/test_carrier_metadata.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      718 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_customs_info.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      707 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_customs_item.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1817 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_easypost_client.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1738 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_end_shipper.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2284 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3726 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_event.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2238 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_hook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2888 2024-04-10 21:19:00.000000 easypost-9.2.0/tests/test_insurance.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2322 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_order.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      573 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_parcel.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4359 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_pickup.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      321 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4797 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_referral_customer.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2062 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_refund.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3212 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_report.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1945 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_scan_form.py
+-rw-r--r--   0 jhammond   (502) staff       (20)    11810 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_shipment.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2300 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_tracker.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3214 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_user.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3262 2024-01-09 20:58:00.000000 easypost-9.2.0/tests/test_webhook.py
```

### Comparing `easypost-9.1.0/CHANGELOG.md` & `easypost-9.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## v9.2.0 (2024-04-10)
+
+- Fix payment method funding and deletion failures due to undetermined payment method type
+- Adds `refund` function in Insurance service for requesting a refund for a standalone insurance
+
 ## v9.1.0 (2024-01-08)
 
 - Adds `all_children` function to the User service for retrieving paginated lists of children
 - Adds `get_next_page_of_children` function to User service to get next paginated list of children
 
 ## v9.0.1 (2023-12-20)
```

### Comparing `easypost-9.1.0/LICENSE` & `easypost-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/PKG-INFO` & `easypost-9.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 9.1.0
+Version: 9.2.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
```

### Comparing `easypost-9.1.0/README.md` & `easypost-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/UPGRADE_GUIDE.md` & `easypost-9.2.0/UPGRADE_GUIDE.md`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/constant.py` & `easypost-9.2.0/easypost/constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 # Library version
-VERSION = "9.1.0"
+VERSION = "9.2.0"
 VERSION_INFO = [str(number) for number in VERSION.split(".")]
 
 # Client defaults
 API_BASE = "https://api.easypost.com"
 API_VERSION = "v2"
 AUTHOR = "EasyPost <oss@easypost.com>"
 SUPPORT_EMAIL = "support@easypost.com"
```

### Comparing `easypost-9.1.0/easypost/easypost_client.py` & `easypost-9.2.0/easypost/easypost_client.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/easypost_object.py` & `easypost-9.2.0/easypost/easypost_object.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/errors/api/__init__.py` & `easypost-9.2.0/easypost/errors/api/__init__.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/errors/api/api_error.py` & `easypost-9.2.0/easypost/errors/api/api_error.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/errors/general/__init__.py` & `easypost-9.2.0/easypost/errors/general/__init__.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/models/__init__.py` & `easypost-9.2.0/easypost/models/__init__.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/requestor.py` & `easypost-9.2.0/easypost/requestor.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/__init__.py` & `easypost-9.2.0/easypost/services/__init__.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/address_service.py` & `easypost-9.2.0/easypost/services/address_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/api_key_service.py` & `easypost-9.2.0/easypost/services/api_key_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/base_service.py` & `easypost-9.2.0/easypost/services/base_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/batch_service.py` & `easypost-9.2.0/easypost/services/batch_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/beta_rate_service.py` & `easypost-9.2.0/easypost/services/beta_rate_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/beta_referral_customer_service.py` & `easypost-9.2.0/easypost/services/beta_referral_customer_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/billing_service.py` & `easypost-9.2.0/easypost/services/billing_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,17 +62,18 @@
             "secondary": "secondary_payment_method",
         }
 
         payment_method_to_use = payment_method_map.get(priority)
 
         if payment_method_to_use and payment_methods[payment_method_to_use]:
             payment_method_id = payment_methods[payment_method_to_use]["id"]
-            if payment_method_id.startswith("card_"):
+            payment_method_object_type = payment_methods[payment_method_to_use].get("object", None)
+            if payment_method_object_type == "CreditCard":
                 endpoint = "/credit_cards"
-            elif payment_method_id.startswith("bank_"):
+            elif payment_method_object_type == "BankAccount":
                 endpoint = "/bank_accounts"
             else:
                 raise InvalidObjectError(message=INVALID_PAYMENT_METHOD_ERROR)
         else:
             raise InvalidObjectError(message=INVALID_PAYMENT_METHOD_ERROR)
 
         return [endpoint, payment_method_id]
```

### Comparing `easypost-9.1.0/easypost/services/carrier_account_service.py` & `easypost-9.2.0/easypost/services/carrier_account_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/carrier_metadata_service.py` & `easypost-9.2.0/easypost/services/carrier_metadata_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/customs_info_service.py` & `easypost-9.2.0/easypost/services/customs_info_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/customs_item_service.py` & `easypost-9.2.0/easypost/services/customs_item_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/end_shipper_service.py` & `easypost-9.2.0/easypost/services/end_shipper_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/event_service.py` & `easypost-9.2.0/easypost/services/event_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/insurance_service.py` & `easypost-9.2.0/easypost/services/insurance_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import (
     Any,
     Dict,
     Optional,
 )
 
+from easypost.easypost_object import convert_to_easypost_object
 from easypost.models import Insurance
+from easypost.requestor import (
+    RequestMethod,
+    Requestor,
+)
 from easypost.services.base_service import BaseService
 
 
 class InsuranceService(BaseService):
     def __init__(self, client):
         self._client = client
         self._model_class = Insurance.__name__
@@ -43,7 +48,16 @@
             "page_size": page_size,
         }
 
         if optional_params:
             params.update(optional_params)
 
         return self.all(**params)
+
+    def refund(self, id: str) -> Insurance:
+        url = f"/insurances/{id}/refund"
+        response = Requestor(self._client).request(
+            method=RequestMethod.POST,
+            url=url,
+        )
+
+        return convert_to_easypost_object(response=response)
```

### Comparing `easypost-9.1.0/easypost/services/order_service.py` & `easypost-9.2.0/easypost/services/order_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/pickup_service.py` & `easypost-9.2.0/easypost/services/pickup_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/referral_customer_service.py` & `easypost-9.2.0/easypost/services/referral_customer_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/refund_service.py` & `easypost-9.2.0/easypost/services/refund_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/report_service.py` & `easypost-9.2.0/easypost/services/report_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/scan_form_service.py` & `easypost-9.2.0/easypost/services/scan_form_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/shipment_service.py` & `easypost-9.2.0/easypost/services/shipment_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/tracker_service.py` & `easypost-9.2.0/easypost/services/tracker_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/user_service.py` & `easypost-9.2.0/easypost/services/user_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/services/webhook_service.py` & `easypost-9.2.0/easypost/services/webhook_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost/util.py` & `easypost-9.2.0/easypost/util.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/easypost.egg-info/PKG-INFO` & `easypost-9.2.0/easypost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 9.1.0
+Version: 9.2.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
```

### Comparing `easypost-9.1.0/easypost.egg-info/SOURCES.txt` & `easypost-9.2.0/easypost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/setup.py` & `easypost-9.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ]
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="easypost",
-    version="9.1.0",
+    version="9.2.0",
     description="EasyPost Shipping API Client Library for Python",
     author="EasyPost",
     author_email="support@easypost.com",
     url="https://easypost.com/",
     packages=find_packages(
         exclude=[
             "docs",
```

### Comparing `easypost-9.1.0/tests/test_address.py` & `easypost-9.2.0/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_api_key.py` & `easypost-9.2.0/tests/test_api_key.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_base_service.py` & `easypost-9.2.0/tests/test_base_service.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_batch.py` & `easypost-9.2.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_beta_rate.py` & `easypost-9.2.0/tests/test_beta_rate.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_beta_referral_customer.py` & `easypost-9.2.0/tests/test_beta_referral_customer.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_billing.py` & `easypost-9.2.0/tests/test_billing.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,34 +20,34 @@
         url="/endpoint/card_123/charges",
         params={"amount": "2000"},
     )
 
 
 @patch(
     "easypost.services.billing_service.BillingService.retrieve_payment_methods",
-    return_value={"primary_payment_method": {"id": "card_123"}},
+    return_value={"primary_payment_method": {"id": "pm_123", "object": "CreditCard"}},
 )
 @patch("easypost.services.billing_service.Requestor.request", return_value={"mock": "response"})
 def test_billing_payment_method_delete_credit_card(mock_request, mock_payment_methods, prod_client):
     """Tests we make a valid call to delete a credit card."""
     prod_client.billing.delete_payment_method(priority="primary")
 
-    mock_request.assert_called_once_with(method=easypost.requestor.RequestMethod.DELETE, url="/credit_cards/card_123")
+    mock_request.assert_called_once_with(method=easypost.requestor.RequestMethod.DELETE, url="/credit_cards/pm_123")
 
 
 @patch(
     "easypost.services.billing_service.BillingService.retrieve_payment_methods",
-    return_value={"primary_payment_method": {"id": "bank_123"}},
+    return_value={"primary_payment_method": {"id": "pm_123", "object": "BankAccount"}},
 )
 @patch("easypost.services.billing_service.Requestor.request", return_value={"mock": "response"})
 def test_billing_payment_method_delete_bank_account(mock_request, mock_payment_methods, prod_client):
     """Tests we make a valid call to delete a bank account."""
     prod_client.billing.delete_payment_method(priority="primary")
 
-    mock_request.assert_called_once_with(method=easypost.requestor.RequestMethod.DELETE, url="/bank_accounts/bank_123")
+    mock_request.assert_called_once_with(method=easypost.requestor.RequestMethod.DELETE, url="/bank_accounts/pm_123")
 
 
 @patch(
     "easypost.services.billing_service.BillingService.retrieve_payment_methods",
     return_value={"primary_payment_method": {"id": "bad_id"}},
 )
 @patch("easypost.services.billing_service.Requestor.request", return_value={"mock": "response"})
@@ -81,7 +81,27 @@
 def test_billing_retrieve_payment_methods_no_billing_setup(mock_request, prod_client):
     """Tests that we throw an error when we cannot retrieve payment methods due to no billing being setup."""
     with pytest.raises(InvalidObjectError) as error:
         _ = prod_client.billing.retrieve_payment_methods()
 
     mock_request.assert_called_once()
     assert str(error.value) == "Billing has not been setup for this user. Please add a payment method."
+
+
+@patch(
+    "easypost.services.billing_service.BillingService.retrieve_payment_methods",
+    return_value={
+        "primary_payment_method": {"id": "pm_123", "object": "CreditCard"},
+        "secondary_payment_method": {"id": "pm_456", "object": "BankAccount"},
+    },
+)
+def test_billing__get_payment_method_info_by_object_type(mock_request, prod_client):
+    """Tests we can determine the payment method type/endpoint by object type."""
+    endpoint, payment_method_id = prod_client.billing._get_payment_method_info(priority="primary")
+
+    assert endpoint == "/credit_cards"
+    assert payment_method_id == "pm_123"
+
+    endpoint, payment_method_id = prod_client.billing._get_payment_method_info(priority="secondary")
+
+    assert endpoint == "/bank_accounts"
+    assert payment_method_id == "pm_456"
```

### Comparing `easypost-9.1.0/tests/test_carrier_account.py` & `easypost-9.2.0/tests/test_carrier_account.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_carrier_metadata.py` & `easypost-9.2.0/tests/test_carrier_metadata.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_customs_info.py` & `easypost-9.2.0/tests/test_customs_info.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_customs_item.py` & `easypost-9.2.0/tests/test_customs_item.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_easypost_client.py` & `easypost-9.2.0/tests/test_easypost_client.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_end_shipper.py` & `easypost-9.2.0/tests/test_end_shipper.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_error.py` & `easypost-9.2.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_event.py` & `easypost-9.2.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_hook.py` & `easypost-9.2.0/tests/test_hook.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_insurance.py` & `easypost-9.2.0/tests/test_insurance.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,7 +60,21 @@
         assert first_id_of_first_page != first_id_of_second_page
 
         # Verify that the filters are being passed along for behind-the-scenes reference
         assert first_page[_FILTERS_KEY] == next_page[_FILTERS_KEY]
     except Exception as e:
         if e.message != NO_MORE_PAGES_ERROR:
             raise Exception(_TEST_FAILED_INTENTIONALLY_ERROR)
+
+
+@pytest.mark.vcr()
+def test_insurance_refund(test_client, basic_insurance):
+    insurance_data = basic_insurance
+    insurance_data["tracking_code"] = "EZ1000000001"
+
+    insurance = test_client.insurance.create(**insurance_data)
+    cancelled_insurance = test_client.insurance.refund(id=insurance.id)
+
+    assert isinstance(cancelled_insurance, Insurance)
+    assert str.startswith(cancelled_insurance.id, "ins_")
+    assert cancelled_insurance.status == "cancelled"
+    assert cancelled_insurance.messages[0] == "Insurance was cancelled by the user."
```

### Comparing `easypost-9.1.0/tests/test_order.py` & `easypost-9.2.0/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_parcel.py` & `easypost-9.2.0/tests/test_parcel.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_pickup.py` & `easypost-9.2.0/tests/test_pickup.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_referral_customer.py` & `easypost-9.2.0/tests/test_referral_customer.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_refund.py` & `easypost-9.2.0/tests/test_refund.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_report.py` & `easypost-9.2.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_scan_form.py` & `easypost-9.2.0/tests/test_scan_form.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_shipment.py` & `easypost-9.2.0/tests/test_shipment.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_tracker.py` & `easypost-9.2.0/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_user.py` & `easypost-9.2.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `easypost-9.1.0/tests/test_webhook.py` & `easypost-9.2.0/tests/test_webhook.py`

 * *Files identical despite different names*

