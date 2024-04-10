# Comparing `tmp/ul-api-utils-7.8.4.tar.gz` & `tmp/ul-api-utils-7.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-api-utils-7.8.4.tar", last modified: Thu Mar 28 13:39:54 2024, max compression
+gzip compressed data, was "ul-api-utils-7.8.5.tar", last modified: Wed Apr 10 07:00:43 2024, max compression
```

## Comparing `ul-api-utils-7.8.4.tar` & `ul-api-utils-7.8.5.tar`

### file list

```diff
@@ -1,178 +1,179 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.380204 ul-api-utils-7.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2022-02-08 08:28:45.000000 ul-api-utils-7.8.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13527 2024-03-28 13:39:54.380204 ul-api-utils-7.8.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12938 2023-04-11 10:27:02.000000 ul-api-utils-7.8.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.204197 ul-api-utils-7.8.4/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/example/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-02-19 15:49:36.000000 ul-api-utils-7.8.4/example/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.208197 ul-api-utils-7.8.4/example/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/example/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-09-19 08:28:56.000000 ul-api-utils-7.8.4/example/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-15 22:48:45.000000 ul-api-utils-7.8.4/example/pure_flask_example.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-15 22:48:45.000000 ul-api-utils-7.8.4/example/rate_limit_load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.208197 ul-api-utils-7.8.4/example/routes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/example/routes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12719 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/example/routes/api_some.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.208197 ul-api-utils-7.8.4/example/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/example/workers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/example/workers/worker.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 13:39:54.380204 ul-api-utils-7.8.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.220198 ul-api-utils-7.8.4/ul_api_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.224198 ul-api-utils-7.8.4/ul_api_utils/access/
--rw-rw-rw-   0 root         (0) root         (0)     4526 2023-09-19 08:28:56.000000 ul-api-utils-7.8.4/ul_api_utils/access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.236199 ul-api-utils-7.8.4/ul_api_utils/api_resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_request.py
--rw-rw-rw-   0 root         (0) root         (0)    17766 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource_error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)    18224 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource_fn_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource_type.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_response_db.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/api_response_payload_alias.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-28 12:08:16.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/db_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/api_resource/signature_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.240198 ul-api-utils-7.8.4/ul_api_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8453 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/commands/cmd_enc_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-11-17 09:49:11.000000 ul-api-utils-7.8.4/ul_api_utils/commands/cmd_gen_api_user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/commands/cmd_gen_new_api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     8788 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/commands/cmd_generate_api_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     3441 2023-11-17 09:49:11.000000 ul-api-utils-7.8.4/ul_api_utils/commands/cmd_start.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/commands/cmd_worker_start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.244199 ul-api-utils-7.8.4/ul_api_utils/commands/start/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/commands/start/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/commands/start/gunicorn.conf.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/commands/start/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.276200 ul-api-utils-7.8.4/ul_api_utils/conf/
--rw-rw-rw-   0 root         (0) root         (0)   999747 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/conf/ul-debugger-main.js
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/conf/ul-debugger-ui.js
--rw-rw-rw-   0 root         (0) root         (0)     3232 2023-11-17 09:49:11.000000 ul-api-utils-7.8.4/ul_api_utils/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-12 08:21:41.000000 ul-api-utils-7.8.4/ul_api_utils/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.280200 ul-api-utils-7.8.4/ul_api_utils/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/debug/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/debug/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/debug/malloc.py
--rw-rw-rw-   0 root         (0) root         (0)    14591 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/debug/stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.280200 ul-api-utils-7.8.4/ul_api_utils/encrypt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/encrypt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.288200 ul-api-utils-7.8.4/ul_api_utils/internal_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.292201 ul-api-utils-7.8.4/ul_api_utils/internal_api/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/__tests__/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
--rw-rw-rw-   0 root         (0) root         (0)    14067 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/internal_api_check_context.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/internal_api_error.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/internal_api/internal_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-19 10:35:07.000000 ul-api-utils-7.8.4/ul_api_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.296201 ul-api-utils-7.8.4/ul_api_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.296201 ul-api-utils-7.8.4/ul_api_utils/modules/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/modules/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10719 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)    25154 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/modules/api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/modules/api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/modules/api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/modules/intermediate_state.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/modules/worker_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4620 2023-06-28 12:08:16.000000 ul-api-utils-7.8.4/ul_api_utils/modules/worker_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/modules/worker_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.300201 ul-api-utils-7.8.4/ul_api_utils/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7516 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2023-06-28 12:08:16.000000 ul-api-utils-7.8.4/ul_api_utils/resources/debugger_scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.308201 ul-api-utils-7.8.4/ul_api_utils/resources/health_check/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/health_check/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/resources/health_check/const.py
--rw-rw-rw-   0 root         (0) root         (0)    18449 2023-09-19 09:52:18.000000 ul-api-utils-7.8.4/ul_api_utils/resources/health_check/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/resources/health_check/health_check_template.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/resources/health_check/resource.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/resources/not_implemented.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/resources/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3358 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/resources/rate_limitter.py
--rw-rw-rw-   0 root         (0) root         (0)     5359 2024-02-19 10:35:07.000000 ul-api-utils-7.8.4/ul_api_utils/resources/swagger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.312202 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.312202 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_fields/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_fields/custom_checkbox_select.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.316202 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3777 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/uni_form.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.352203 ul-api-utils-7.8.4/ul_api_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.352203 ul-api-utils-7.8.4/ul_api_utils/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/__tests__/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/__tests__/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/api_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/api_format.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-02-12 08:21:41.000000 ul-api-utils-7.8.4/ul_api_utils/utils/api_method.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/api_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/api_request_info.py
--rw-rw-rw-   0 root         (0) root         (0)     5021 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/avro.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2023-11-17 09:49:11.000000 ul-api-utils-7.8.4/ul_api_utils/utils/broker_topics_message_count.py
--rw-rw-rw-   0 root         (0) root         (0)      670 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/cached_per_request.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/decode_base64.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/deprecated.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-09-19 08:28:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.352203 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.356203 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)    28944 2024-02-19 10:35:07.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.376204 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-15 07:34:58.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/imports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.376204 ul-api-utils-7.8.4/ul_api_utils/utils/jinja/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/utils/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/jinja/t_url_for.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/jinja/to_pretty_json.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-06-28 12:08:16.000000 ul-api-utils-7.8.4/ul_api_utils/utils/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/load_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-28 12:08:16.000000 ul-api-utils-7.8.4/ul_api_utils/utils/token_check.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/token_check_through_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/utils/uuid_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.380204 ul-api-utils-7.8.4/ul_api_utils/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/validators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.380204 ul-api-utils-7.8.4/ul_api_utils/validators/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:39:52.000000 ul-api-utils-7.8.4/ul_api_utils/validators/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/validators/__tests__/test_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4023 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/validators/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/validators/validate_empty_object.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-22 12:49:56.000000 ul-api-utils-7.8.4/ul_api_utils/validators/validate_uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:39:54.224198 ul-api-utils-7.8.4/ul_api_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13527 2024-03-28 13:39:54.000000 ul-api-utils-7.8.4/ul_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6016 2024-03-28 13:39:54.000000 ul-api-utils-7.8.4/ul_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 13:39:54.000000 ul-api-utils-7.8.4/ul_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-03-28 13:39:54.000000 ul-api-utils-7.8.4/ul_api_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      516 2024-03-28 13:39:54.000000 ul-api-utils-7.8.4/ul_api_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-28 13:39:54.000000 ul-api-utils-7.8.4/ul_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2022-01-13 12:55:17.000000 ul-api-utils-7.8.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13527 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2023-06-20 10:17:45.000000 ul-api-utils-7.8.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.987094 ul-api-utils-7.8.5/example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.999094 ul-api-utils-7.8.5/example/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-09-06 09:19:02.000000 ul-api-utils-7.8.5/example/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-16 17:17:46.000000 ul-api-utils-7.8.5/example/pure_flask_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-11 16:20:02.000000 ul-api-utils-7.8.5/example/rate_limit_load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.999094 ul-api-utils-7.8.5/example/routes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/routes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12856 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/routes/api_some.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:42.999094 ul-api-utils-7.8.5/example/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/example/workers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/example/workers/worker.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.019095 ul-api-utils-7.8.5/ul_api_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.027095 ul-api-utils-7.8.5/ul_api_utils/access/
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2023-09-06 09:19:02.000000 ul-api-utils-7.8.5/ul_api_utils/access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.051096 ul-api-utils-7.8.5/ul_api_utils/api_resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    17766 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_error_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)    18224 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_fn_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_db.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_payload_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/db_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/api_resource/signature_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.059096 ul-api-utils-7.8.5/ul_api_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8453 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_enc_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_api_user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_new_api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     8788 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_generate_api_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/cmd_worker_start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.063097 ul-api-utils-7.8.5/ul_api_utils/commands/start/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/start/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/commands/start/gunicorn.conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/commands/start/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.075097 ul-api-utils-7.8.5/ul_api_utils/conf/
+-rw-rw-rw-   0 root         (0) root         (0)   999747 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-main.js
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-ui.js
+-rw-rw-rw-   0 root         (0) root         (0)     3232 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.087098 ul-api-utils-7.8.5/ul_api_utils/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/debug/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/debug/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/debug/malloc.py
+-rw-rw-rw-   0 root         (0) root         (0)    14591 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/debug/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.091098 ul-api-utils-7.8.5/ul_api_utils/encrypt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/encrypt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.095098 ul-api-utils-7.8.5/ul_api_utils/internal_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.103098 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    14067 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_check_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.107098 ul-api-utils-7.8.5/ul_api_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.107098 ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25626 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15112 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/intermediate_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/worker_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4620 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/worker_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/modules/worker_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.119099 ul-api-utils-7.8.5/ul_api_utils/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7516 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/debugger_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.135099 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/const.py
+-rw-rw-rw-   0 root         (0) root         (0)    18449 2023-09-19 22:04:40.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/health_check/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/not_implemented.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3358 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/resources/rate_limitter.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/sockets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5359 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/swagger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.135099 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.135099 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_fields/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_fields/custom_checkbox_select.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.139099 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3777 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/uni_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.159100 ul-api-utils-7.8.5/ul_api_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.159100 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/api_request_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     5021 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/avro.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2024-02-12 08:16:10.000000 ul-api-utils-7.8.5/ul_api_utils/utils/broker_topics_message_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      670 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/cached_per_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/decode_base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/deprecated.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-09-06 09:19:02.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.163100 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.163100 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    28944 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.167101 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/imports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.167101 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/t_url_for.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/jinja/to_pretty_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/load_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/token_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/token_check_through_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/utils/uuid_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/ul_api_utils/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/validators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.175101 ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 07:00:41.000000 ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/test_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4023 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/validate_empty_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-08-10 09:58:03.000000 ul-api-utils-7.8.5/ul_api_utils/validators/validate_uuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:00:43.027095 ul-api-utils-7.8.5/ul_api_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13527 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6050 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      516 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 07:00:42.000000 ul-api-utils-7.8.5/ul_api_utils.egg-info/top_level.txt
```

### Comparing `ul-api-utils-7.8.4/LICENSE` & `ul-api-utils-7.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/PKG-INFO` & `ul-api-utils-7.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.8.4
+Version: 7.8.5
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.8.4/README.md` & `ul-api-utils-7.8.5/README.md`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/example/conf.py` & `ul-api-utils-7.8.5/example/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import os
 
 from ul_db_utils.modules.db import DbConfig
 
 from ul_api_utils.modules.api_sdk import ApiSdk
-from ul_api_utils.modules.api_sdk_config import ApiSdkConfig, ApiSdkIdentifyTypeEnum, ApiSdkFlaskDebuggingPluginsEnabled
+from ul_api_utils.modules.api_sdk_config import ApiSdkConfig, ApiSdkIdentifyTypeEnum, \
+    ApiSdkFlaskDebuggingPluginsEnabled, SocketIOConfig
 from example.permissions import permissions
 
 sdk = ApiSdk(ApiSdkConfig(
+    sockets_config=SocketIOConfig(
+        message_queue='redis://localhost:16379',
+    ),
     service_name='example_service',
     permissions=permissions,
     cache_storage_uri='redis://localhost:16379',
     cache_default_ttl=60,
     rate_limit_storage_uri='redis://localhost:16379',
     rate_limit_identify=ApiSdkIdentifyTypeEnum.JWT_USER_ID,
     flask_debugging_plugins=ApiSdkFlaskDebuggingPluginsEnabled(
```

### Comparing `ul-api-utils-7.8.4/example/pure_flask_example.py` & `ul-api-utils-7.8.5/example/pure_flask_example.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/example/routes/api_some.py` & `ul-api-utils-7.8.5/example/routes/api_some.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from time import sleep
 from datetime import datetime, timedelta
-from typing import List, Optional, Tuple
-
+from typing import List, Optional, Tuple, Any
+from ul_api_utils.resources.sockets import socket_io
 from flask import jsonify
 from pydantic import BaseModel
 from ul_db_utils.modules.db import db
 from werkzeug import Response as BaseResponse
 
 from example.conf import sdk
 from example.permissions import SOME_PERMISSION, SOME_PERMISSION2
@@ -310,7 +310,12 @@
 
     return api_resource.response_file_ok(
         path_or_file=fn,
         mimetype='text/plain',
         as_attachment=True,
         attachment_filename='import_devices_log.txt',
     )
+
+
+@socket_io.on('message')
+def handle(data: Any, message: Any) -> None:
+    ...
```

### Comparing `ul-api-utils-7.8.4/example/workers/worker.py` & `ul-api-utils-7.8.5/example/workers/worker.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/setup.py` & `ul-api-utils-7.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-api-utils',
-    version='7.8.4',
+    version='7.8.5',
     description='Python api utils',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='',
     packages=find_packages(),
     package_data={
```

### Comparing `ul-api-utils-7.8.4/ul_api_utils/access/__init__.py` & `ul-api-utils-7.8.5/ul_api_utils/access/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_request.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource_config.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource_error_handling.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_error_handling.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_resource_fn_typing.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_resource_fn_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_response.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_response_db.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_db.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/api_response_payload_alias.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/api_response_payload_alias.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/api_resource/signature_check.py` & `ul-api-utils-7.8.5/ul_api_utils/api_resource/signature_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/commands/cmd_enc_keys.py` & `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_enc_keys.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/commands/cmd_gen_api_user_token.py` & `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_api_user_token.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/commands/cmd_gen_new_api_user.py` & `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_gen_new_api_user.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/commands/cmd_generate_api_docs.py` & `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_generate_api_docs.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/commands/cmd_start.py` & `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_start.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     app_file_name: str = 'main.py'
     app_name: str = 'flask_app'
     env: str
     port: int
     debug: bool
     max_requests: int
     max_requests_jitter: int
+    worker_class: str
 
     @property
     def app_rel_dir(self) -> str:
         return os.path.relpath(self.app_dir, os.getcwd())
 
     @property
     def app_file_path(self) -> str:
@@ -45,14 +46,15 @@
     def add_parser_args(parser: argparse.ArgumentParser) -> None:
         parser.add_argument('--app-dir', dest='app_dir', type=str, required=True, help="dir to import ")
         parser.add_argument('--env', dest='env', type=str, required=True)
         parser.add_argument('--port', dest='port', type=int, required=False, default=30000)
         parser.add_argument('--debug', dest='debug', type=arg_str2bool, default=False, required=False)
         parser.add_argument('--max-requests', dest='max_requests', type=int, default=1000, required=False)
         parser.add_argument('--max-requests-jitter', dest='max_requests_jitter', type=int, default=50, required=False)
+        parser.add_argument('--worker-class', dest='worker_class', type=str, default='sync', required=False)
 
     def run(self) -> None:
         env = os.environ.copy()
         name = re.sub(r'[^0-9a-z]+', '-', f'gncrn-{os.path.relpath(self.app_dir, os.getcwd()).lower().strip("/").strip()}')
         env['PYTHONUNBUFFERED'] = os.environ.get('PYTHONUNBUFFERED', '0')
         env['PYTHONPATH'] = os.getcwd()
         env['APPLICATION_START_DT'] = datetime.now().isoformat()
@@ -65,14 +67,15 @@
 
         conf = os.path.abspath(os.path.normpath(os.path.join(THIS_LIB_CWD, "commands", "start", "gunicorn.conf.py")))
         debug = (self.debug and self.env == ENV_LOCAL)
 
         args = [
             f'-n={name}',
             f'-w={APPLICATION_GUNICORN_WORKERS}',
+            f'--worker-class={self.worker_class}',
             f'-b=0.0.0.0:{self.port}',
             f'--config={conf}',
             '--log-level=INFO',
             f'--max-requests={self.max_requests}',
             f'--max-requests-jitter={self.max_requests_jitter}',
             '--timeout=60',
             '--access-logfile=-',
```

### Comparing `ul-api-utils-7.8.4/ul_api_utils/commands/cmd_worker_start.py` & `ul-api-utils-7.8.5/ul_api_utils/commands/cmd_worker_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/commands/start/wsgi.py` & `ul-api-utils-7.8.5/ul_api_utils/commands/start/wsgi.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/conf/ul-debugger-main.js` & `ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-main.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/conf/ul-debugger-ui.js` & `ul-api-utils-7.8.5/ul_api_utils/conf/ul-debugger-ui.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/conf.py` & `ul-api-utils-7.8.5/ul_api_utils/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/const.py` & `ul-api-utils-7.8.5/ul_api_utils/const.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/debug/debugger.py` & `ul-api-utils-7.8.5/ul_api_utils/debug/debugger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/debug/malloc.py` & `ul-api-utils-7.8.5/ul_api_utils/debug/malloc.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/debug/stat.py` & `ul-api-utils-7.8.5/ul_api_utils/debug/stat.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py` & `ul-api-utils-7.8.5/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/errors.py` & `ul-api-utils-7.8.5/ul_api_utils/errors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/internal_api/__tests__/internal_api.py` & `ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/internal_api/__tests__/internal_api_content_type.py` & `ul-api-utils-7.8.5/ul_api_utils/internal_api/__tests__/internal_api_content_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/internal_api/internal_api.py` & `ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/internal_api/internal_api_check_context.py` & `ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_check_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/internal_api/internal_api_response.py` & `ul-api-utils-7.8.5/ul_api_utils/internal_api/internal_api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/main.py` & `ul-api-utils-7.8.5/ul_api_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py` & `ul-api-utils-7.8.5/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/modules/api_sdk.py` & `ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 import os
 import time
 import traceback
 from base64 import b64decode
 from datetime import datetime
 from functools import wraps
 from typing import List, Union, Callable, Tuple, Any, Optional, TypeVar, cast, Set, TYPE_CHECKING
-
+from ul_api_utils.resources.sockets import socket_io
 from flask import Response, request, Flask, url_for as flask_url_for, _app_ctx_stack
 from pydantic import BaseModel
 from redis.connection import parse_url
 from ul_py_tool.utils.arg_files_glob import arg_files_print
 from werkzeug import Response as BaseResponse
-
 from ul_api_utils.access import PermissionDefinition, GLOBAL_PERMISSION__PRIVATE, GLOBAL_PERMISSION__PRIVATE_RT, \
     GLOBAL_PERMISSION__PUBLIC, PermissionRegistry
 from ul_api_utils.api_resource.api_resource import ApiResource
 from ul_api_utils.api_resource.api_resource_config import ApiResourceConfig
 from ul_api_utils.api_resource.api_resource_fn_typing import ApiResourceFnTyping
 from ul_api_utils.api_resource.api_resource_type import ApiResourceType
 from ul_api_utils.api_resource.api_response import ApiResponse, JsonApiResponse, RootJsonApiResponse, ProxyJsonApiResponse, AnyJsonApiResponse
 from ul_api_utils.conf import APPLICATION_DEBUGGER_PIN, APPLICATION_DEBUG, APPLICATION_DIR, APPLICATION_ENV_IS_LOCAL, APPLICATION_START_DT, APPLICATION_DEBUG_LOGGING
 from ul_api_utils.const import REQUEST_HEADER__DEBUGGER, REQUEST_HEADER__INTERNAL
 from ul_api_utils.debug import stat
 from ul_api_utils.debug.debugger import Debugger
 from ul_api_utils.errors import UserAbstractApiError, ResourceRuntimeApiError, ResponseTypeRuntimeApiError
 from ul_api_utils.internal_api.internal_api_check_context import internal_api_check_context
-from ul_api_utils.modules.api_sdk_config import ApiSdkConfig
+from ul_api_utils.modules.api_sdk_config import ApiSdkConfig, SocketAsyncModesEnum
 from ul_api_utils.modules.intermediate_state import try_init, try_configure
 from ul_api_utils.resources.caching import ULCache, TCacheMode, ULCacheMode, ULCacheConfig
 from ul_api_utils.resources.debugger_scripts import load_debugger_static_scripts
 from ul_api_utils.resources.health_check.health_check import HealthCheckContext
 from ul_api_utils.resources.health_check.resource import init_health_check_resource
 from ul_api_utils.resources.not_implemented import not_implemented_handler
 from ul_api_utils.resources.permissions import load_permissions
@@ -196,14 +195,23 @@
 
         load_permissions(self, self._initialized_flask_name, self._config.permissions)
 
         load_debugger_static_scripts(self)
 
         load_swagger(self, self._fn_registry, self._config.api_route_path_prefix)
 
+        if self.config.sockets_config:
+            socket_io.init_app(
+                self._flask_app,
+                message_queue=self.config.sockets_config.message_queue,
+                async_mode=SocketAsyncModesEnum.GEVENT.value,
+                channel=self.config.sockets_config.channel,
+                cors_allowed_origins=self.config.sockets_config.cors_allowed_origins,
+            )
+
         return self._flask_app
 
     @property
     def _flask_app(self) -> Flask:
         if self._flask_app_cache is not None:
             return self._flask_app_cache
```

### Comparing `ul-api-utils-7.8.4/ul_api_utils/modules/api_sdk_config.py` & `ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 from ul_api_utils.modules.api_sdk_jwt import ApiSdkJwt
 
 
 def join_route_paths(prev_sect: str, next_sect: str) -> str:
     return prev_sect.rstrip('/') + '/' + next_sect.lstrip('/')
 
 
+class SocketAsyncModesEnum(Enum):
+    THREADING = 'threading'
+    GEVENT = 'gevent'
+    EVENTLET = 'eventlet'
+    GEVENT_UWSGI = 'gevent_uwsgi'
+
+
 class ApiSdkIdentifyTypeEnum(Enum):
     DISABLED = 'DISABLED'
     CLIENT_IP = 'IP'
     JWT_USER_ID = 'JWT_USER_ID'
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}.{self.name}'
@@ -25,27 +32,33 @@
     scheme: str = 'Basic'
 
 
 class ApiSdkFlaskDebuggingPluginsEnabled(BaseModel):
     flask_monitoring_dashboard: bool = False
 
 
+class SocketIOConfig(BaseModel):
+    message_queue: str
+    channel: Optional[str] = "flask-socketio"
+    cors_allowed_origins: Optional[str] = "*"
+
+
 class ApiSdkConfig(BaseModel):
     service_name: str
     permissions: Optional[Union[Callable[[], PermissionRegistry], PermissionRegistry]] = None
     permissions_check_enabled: bool = True  # GLOBAL CHECK OF ACCESS AND PERMISSIONS ENABLE
     permissions_validator: Optional[Callable[[ApiSdkJwt, PermissionDefinition], bool]] = None
 
     jwt_validator: Optional[Callable[[ApiSdkJwt], bool]] = None
     jwt_environment_check_enabled: bool = True
 
     http_auth: Optional[ApiSdkHttpAuth] = None
 
     static_url_path: Optional[str] = None
-
+    sockets_config: Optional[SocketIOConfig] = None
     web_error_template: Optional[str] = None
 
     rate_limit: Union[str, List[str]] = '100/minute'  # [count (int)] [per|/] [second|minute|hour|day|month|year][s]
     rate_limit_storage_uri: str = ''  # supports url of redis, memcached, mongodb
     rate_limit_identify: Union[ApiSdkIdentifyTypeEnum, Callable[[], str]] = ApiSdkIdentifyTypeEnum.DISABLED  # must be None if disabled
 
     cache_storage_uri: str = ''  # supports only redis
```

### Comparing `ul-api-utils-7.8.4/ul_api_utils/modules/api_sdk_jwt.py` & `ul-api-utils-7.8.5/ul_api_utils/modules/api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/modules/intermediate_state.py` & `ul-api-utils-7.8.5/ul_api_utils/modules/intermediate_state.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/modules/worker_context.py` & `ul-api-utils-7.8.5/ul_api_utils/modules/worker_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/modules/worker_sdk.py` & `ul-api-utils-7.8.5/ul_api_utils/modules/worker_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/caching.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/caching.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/debugger_scripts.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/debugger_scripts.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/health_check/health_check.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/health_check/health_check_template.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/health_check/health_check_template.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/health_check/resource.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/health_check/resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/not_implemented.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/not_implemented.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/permissions.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/rate_limitter.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/rate_limitter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/swagger.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/swagger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_select_widget.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/custom_widgets/custom_text_input_widget.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/resources/web_forms/uni_form.py` & `ul-api-utils-7.8.5/ul_api_utils/resources/web_forms/uni_form.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/sentry.py` & `ul-api-utils-7.8.5/ul_api_utils/sentry.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/__tests__/api_path_version.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/__tests__/unwrap_typing.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/__tests__/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/api_encoding.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/api_encoding.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/api_format.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/api_format.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/api_method.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/api_method.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/api_pagination.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/api_pagination.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/api_path_version.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/avro.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/avro.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/broker_topics_message_count.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/broker_topics_message_count.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/cached_per_request.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/cached_per_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/colors.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/deprecated.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flags.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flags.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/json_encoder.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/load_modules.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/load_modules.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/token_check_through_request.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/token_check_through_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/unwrap_typing.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/utils/uuid_converter.py` & `ul-api-utils-7.8.5/ul_api_utils/utils/uuid_converter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/validators/__tests__/test_custom_fields.py` & `ul-api-utils-7.8.5/ul_api_utils/validators/__tests__/test_custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils/validators/custom_fields.py` & `ul-api-utils-7.8.5/ul_api_utils/validators/custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.8.4/ul_api_utils.egg-info/PKG-INFO` & `ul-api-utils-7.8.5/ul_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.8.4
+Version: 7.8.5
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.8.4/ul_api_utils.egg-info/SOURCES.txt` & `ul-api-utils-7.8.5/ul_api_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
 ul_api_utils/resources/__init__.py
 ul_api_utils/resources/caching.py
 ul_api_utils/resources/debugger_scripts.py
 ul_api_utils/resources/not_implemented.py
 ul_api_utils/resources/permissions.py
 ul_api_utils/resources/rate_limitter.py
+ul_api_utils/resources/sockets.py
 ul_api_utils/resources/swagger.py
 ul_api_utils/resources/health_check/__init__.py
 ul_api_utils/resources/health_check/const.py
 ul_api_utils/resources/health_check/health_check.py
 ul_api_utils/resources/health_check/health_check_template.py
 ul_api_utils/resources/health_check/resource.py
 ul_api_utils/resources/web_forms/__init__.py
```

### Comparing `ul-api-utils-7.8.4/ul_api_utils.egg-info/requires.txt` & `ul-api-utils-7.8.5/ul_api_utils.egg-info/requires.txt`

 * *Files identical despite different names*

