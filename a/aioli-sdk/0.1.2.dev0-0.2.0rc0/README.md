# Comparing `tmp/aioli-sdk-0.1.2.dev0.tar.gz` & `tmp/aioli-sdk-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli-sdk-0.1.2.dev0.tar", last modified: Thu Mar  7 06:16:29 2024, max compression
+gzip compressed data, was "aioli-sdk-0.2.0rc0.tar", last modified: Wed Apr 10 15:34:40 2024, max compression
```

## Comparing `aioli-sdk-0.1.2.dev0.tar` & `aioli-sdk-0.2.0rc0.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.508707 aioli-sdk-0.1.2.dev0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1420 2024-03-07 06:16:29.508707 aioli-sdk-0.1.2.dev0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.500707 aioli-sdk-0.1.2.dev0/aioli/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      109 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/__version__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.504707 aioli-sdk-0.1.2.dev0/aioli/cli/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1644 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8376 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6928 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6127 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6262 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6424 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/render.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3558 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/role.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13378 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/service.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.504707 aioli-sdk-0.1.2.dev0/aioli/cli/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      728 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19300 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6629 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/user.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3103 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.504707 aioli-sdk-0.1.2.dev0/aioli/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.504707 aioli-sdk-0.1.2.dev0/aioli/common/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      336 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18000 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8098 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3671 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10969 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/api/request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8655 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/check.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      650 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8480 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1724 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/requests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3591 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/common/util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2272 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/aioli/util.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.508707 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1420 2024-03-07 06:16:29.000000 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2373 2024-03-07 06:16:29.000000 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-07 06:16:29.000000 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2024-03-07 06:16:29.000000 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-07 06:16:29.000000 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2024-03-07 06:16:29.000000 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2024-03-07 06:16:29.000000 aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.504707 aioli-sdk-0.1.2.dev0/aiolirest/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2939 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.508707 aioli-sdk-0.1.2.dev0/aiolirest/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      468 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22756 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    53091 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10458 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    54871 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/models_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    54092 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    43025 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    74358 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/services_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    61828 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24993 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/api_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14862 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/configuration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5540 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:29.508707 aioli-sdk-0.1.2.dev0/aiolirest/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2020 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4230 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3399 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5900 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3363 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5119 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2731 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3079 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2479 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2690 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/role.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3239 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2848 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/security.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5094 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/service.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2769 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/service_auth_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4009 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/service_model_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4659 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/service_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2592 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4610 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4159 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3706 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3947 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3875 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/user.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2606 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3640 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/py.typed
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8383 2024-03-07 06:16:27.000000 aioli-sdk-0.1.2.dev0/aiolirest/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      113 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-03-07 06:16:29.508707 aioli-sdk-0.1.2.dev0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2404 2024-03-07 06:11:49.000000 aioli-sdk-0.1.2.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.196040 aioli-sdk-0.2.0rc0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-04-10 15:34:40.196040 aioli-sdk-0.2.0rc0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.184040 aioli-sdk-0.2.0rc0/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.188040 aioli-sdk-0.2.0rc0/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10169 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13963 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8252 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.188040 aioli-sdk-0.2.0rc0/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24720 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.188040 aioli-sdk-0.2.0rc0/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.188040 aioli-sdk-0.2.0rc0/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3591 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.196040 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-04-10 15:34:40.000000 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2447 2024-04-10 15:34:40.000000 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 15:34:40.000000 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-10 15:34:40.000000 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 15:34:37.000000 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-10 15:34:40.000000 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-10 15:34:40.000000 aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.192040 aioli-sdk-0.2.0rc0/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.192040 aioli-sdk-0.2.0rc0/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22812 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    84658 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10514 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91192 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54370 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43081 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105943 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61884 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25049 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14924 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5596 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:40.196040 aioli-sdk-0.2.0rc0/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2221 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3383 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3661 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7725 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5067 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5249 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2787 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3774 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2641 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2535 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6382 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5804 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2939 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3365 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3093 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3295 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2648 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5178 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4996 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3931 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3696 2024-04-10 15:34:34.000000 aioli-sdk-0.2.0rc0/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8439 2024-04-10 15:34:35.000000 aioli-sdk-0.2.0rc0/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-10 15:34:40.196040 aioli-sdk-0.2.0rc0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-04-10 15:27:27.000000 aioli-sdk-0.2.0rc0/setup.py
```

### Comparing `aioli-sdk-0.1.2.dev0/PKG-INFO` & `aioli-sdk-0.2.0rc0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.1.2.dev0
+Version: 0.2.0rc0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/_util.py` & `aioli-sdk-0.2.0rc0/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/cli.py` & `aioli-sdk-0.2.0rc0/aioli/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 import aioli
 from aioli.cli import render
 from aioli.cli.deployment import args_description as deployment_args_description
 from aioli.cli.model import args_description as model_args_description
 from aioli.cli.registry import args_description as registry_args_description
 from aioli.cli.role import args_description as role_args_description
-from aioli.cli.service import args_description as service_args_description
 from aioli.cli.sso import args_description as sso_args_description
 from aioli.cli.user import args_description as user_args_description
 from aioli.cli.version import args_description as version_args_description
 from aioli.cli.version import check_version
 from aioli.common import api
 from aioli.common.api import certs
 from aioli.common.check import check_not_none
@@ -51,15 +50,14 @@
         version="%(prog)s {}".format(aioli.__version__),
     ),
 ]
 all_args_description: ArgsDescription = (
     args_description
     + registry_args_description
     + model_args_description
-    + service_args_description
     + deployment_args_description
     + version_args_description
     + user_args_description
     + role_args_description
     + sso_args_description
 )
```

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/errors.py` & `aioli-sdk-0.2.0rc0/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/render.py` & `aioli-sdk-0.2.0rc0/aioli/cli/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 For example, the following two lines of pseudocode return similar objects:
 * bindings.v1Model.to_json()
 * _render.model_to_json(model.Model)
 """
 
 import csv
 import inspect
+import json
 import os
 import pathlib
 import sys
 from datetime import timezone
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
 import dateutil.parser
 import tabulate
 import termcolor
 from ruamel.yaml import YAML
 from ruamel.yaml.compat import StringIO
 
+from aioli import util as aioli_util
 from aioli.common import util
 
 # Avoid reporting BrokenPipeError when piping `tabulate` output through
 # a filter like `head`.
 _FORMAT = "presto"
 _DEFAULT_VALUE = "N/A"
 OMITTED_VALUE = "***"
@@ -168,16 +170,21 @@
     headers: Union[Dict[str, str], Sequence[str]],
     values: Sequence[Iterable[Any]],
     as_csv: bool,
     outfile: Optional[pathlib.Path] = None,
 ) -> None:
     out = outfile.open("w") if outfile else sys.stdout
     if as_csv or outfile:
+        # Construct a list of headers where any newlines are replaced by a space character
+        # otherwise our header will occupy >1 rows.
+        new_headers: List[str] = []
+        for header in headers:
+            new_headers.append(header.replace("\n", " "))
         writer = csv.writer(out)
-        writer.writerow(headers)
+        writer.writerow(new_headers)
         writer.writerows(values)
     else:
         # Tabulate needs to accept dict[str, str], but mypy thinks it cannot, so
         # we suppress that error.
         print(
             tabulate.tabulate(values, headers, tablefmt="presto"),
             file=out,
@@ -214,7 +221,22 @@
         "true",
     )
 
 
 def report_job_launched(_type: str, _id: str) -> None:
     msg = f"Launched {_type} (id: {_id})."
     print(termcolor.colored(msg, "green"))
+
+
+def print_json(data: Union[str, Any]) -> None:
+    """
+    Print JSON data in a human-readable format.
+    """
+    DEFAULT_INDENT = "  "
+    try:
+        if isinstance(data, str):
+            data = json.loads(data)
+        formatted_json = aioli_util.json_encode(data, sort_keys=True, indent=DEFAULT_INDENT)
+        print(formatted_json)
+    except json.decoder.JSONDecodeError:
+        print("Unable to generate JSON format. Printing default format.")
+        print(data)
```

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/role.py` & `aioli-sdk-0.2.0rc0/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/sso.py` & `aioli-sdk-0.2.0rc0/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/test/conftest.py` & `aioli-sdk-0.2.0rc0/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/user.py` & `aioli-sdk-0.2.0rc0/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/cli/version.py` & `aioli-sdk-0.2.0rc0/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/api/authentication.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/api/certs.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/api/errors.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/api/request.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/check.py` & `aioli-sdk-0.2.0rc0/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/constants.py` & `aioli-sdk-0.2.0rc0/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/declarative_argparse.py` & `aioli-sdk-0.2.0rc0/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/requests.py` & `aioli-sdk-0.2.0rc0/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/common/util.py` & `aioli-sdk-0.2.0rc0/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli/util.py` & `aioli-sdk-0.2.0rc0/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/PKG-INFO` & `aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.1.2.dev0
+Version: 0.2.0rc0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli-sdk-0.1.2.dev0/aioli_sdk.egg-info/SOURCES.txt` & `aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 aioli/cli/cli.py
 aioli/cli/deployment.py
 aioli/cli/errors.py
 aioli/cli/model.py
 aioli/cli/registry.py
 aioli/cli/render.py
 aioli/cli/role.py
-aioli/cli/service.py
 aioli/cli/sso.py
 aioli/cli/user.py
 aioli/cli/version.py
 aioli/cli/test/conftest.py
 aioli/cli/test/test_cli.py
 aioli/common/__init__.py
 aioli/common/check.py
@@ -46,39 +45,41 @@
 aiolirest/exceptions.py
 aiolirest/py.typed
 aiolirest/rest.py
 aiolirest/api/__init__.py
 aiolirest/api/authentication_api.py
 aiolirest/api/deployments_api.py
 aiolirest/api/information_api.py
-aiolirest/api/models_api.py
+aiolirest/api/packaged_models_api.py
 aiolirest/api/registries_api.py
 aiolirest/api/roles_api.py
-aiolirest/api/services_api.py
+aiolirest/api/templates_api.py
 aiolirest/api/users_api.py
 aiolirest/models/__init__.py
+aiolirest/models/auto_scaling_template.py
 aiolirest/models/autoscaling.py
 aiolirest/models/configuration_resources.py
 aiolirest/models/deployment.py
+aiolirest/models/deployment_model_version.py
 aiolirest/models/deployment_request.py
 aiolirest/models/deployment_state.py
 aiolirest/models/error_response.py
+aiolirest/models/event_info.py
 aiolirest/models/failure_info.py
 aiolirest/models/login_request.py
 aiolirest/models/login_response.py
+aiolirest/models/model_auth_token.py
+aiolirest/models/observability.py
+aiolirest/models/packaged_model.py
+aiolirest/models/packaged_model_request.py
 aiolirest/models/resource_profile.py
+aiolirest/models/resources_template.py
 aiolirest/models/role.py
 aiolirest/models/role_assignment.py
 aiolirest/models/role_assignments.py
 aiolirest/models/security.py
-aiolirest/models/service.py
-aiolirest/models/service_auth_token.py
-aiolirest/models/service_model_version.py
-aiolirest/models/service_request.py
 aiolirest/models/success_response.py
-aiolirest/models/trained_model.py
 aiolirest/models/trained_model_registry.py
 aiolirest/models/trained_model_registry_request.py
-aiolirest/models/trained_model_request.py
 aiolirest/models/user.py
 aiolirest/models/user_patch_request.py
 aiolirest/models/user_request.py
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/__init__.py` & `aioli-sdk-0.2.0rc0/aiolirest/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
 
 # import apis into sdk package
 from aiolirest.api.authentication_api import AuthenticationApi
 from aiolirest.api.deployments_api import DeploymentsApi
 from aiolirest.api.information_api import InformationApi
-from aiolirest.api.models_api import ModelsApi
+from aiolirest.api.packaged_models_api import PackagedModelsApi
 from aiolirest.api.registries_api import RegistriesApi
 from aiolirest.api.roles_api import RolesApi
-from aiolirest.api.services_api import ServicesApi
+from aiolirest.api.templates_api import TemplatesApi
 from aiolirest.api.users_api import UsersApi
 
 # import ApiClient
 from aiolirest.api_response import ApiResponse
 from aiolirest.api_client import ApiClient
 from aiolirest.configuration import Configuration
 from aiolirest.exceptions import OpenApiException
 from aiolirest.exceptions import ApiTypeError
 from aiolirest.exceptions import ApiValueError
 from aiolirest.exceptions import ApiKeyError
 from aiolirest.exceptions import ApiAttributeError
 from aiolirest.exceptions import ApiException
 
 # import models into sdk package
+from aiolirest.models.auto_scaling_template import AutoScalingTemplate
 from aiolirest.models.autoscaling import Autoscaling
 from aiolirest.models.configuration_resources import ConfigurationResources
 from aiolirest.models.deployment import Deployment
+from aiolirest.models.deployment_model_version import DeploymentModelVersion
 from aiolirest.models.deployment_request import DeploymentRequest
 from aiolirest.models.deployment_state import DeploymentState
 from aiolirest.models.error_response import ErrorResponse
+from aiolirest.models.event_info import EventInfo
 from aiolirest.models.failure_info import FailureInfo
 from aiolirest.models.login_request import LoginRequest
 from aiolirest.models.login_response import LoginResponse
+from aiolirest.models.model_auth_token import ModelAuthToken
+from aiolirest.models.observability import Observability
+from aiolirest.models.packaged_model import PackagedModel
+from aiolirest.models.packaged_model_request import PackagedModelRequest
 from aiolirest.models.resource_profile import ResourceProfile
+from aiolirest.models.resources_template import ResourcesTemplate
 from aiolirest.models.role import Role
 from aiolirest.models.role_assignment import RoleAssignment
 from aiolirest.models.role_assignments import RoleAssignments
 from aiolirest.models.security import Security
-from aiolirest.models.service import Service
-from aiolirest.models.service_auth_token import ServiceAuthToken
-from aiolirest.models.service_model_version import ServiceModelVersion
-from aiolirest.models.service_request import ServiceRequest
 from aiolirest.models.success_response import SuccessResponse
-from aiolirest.models.trained_model import TrainedModel
 from aiolirest.models.trained_model_registry import TrainedModelRegistry
 from aiolirest.models.trained_model_registry_request import TrainedModelRegistryRequest
-from aiolirest.models.trained_model_request import TrainedModelRequest
 from aiolirest.models.user import User
 from aiolirest.models.user_patch_request import UserPatchRequest
 from aiolirest.models.user_request import UserRequest
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api/authentication_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/authentication_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api/deployments_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/roles_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,58 +24,62 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictStr
 
-from typing import List
+from typing import List, Optional
 
-from aiolirest.models.deployment import Deployment
-from aiolirest.models.deployment_request import DeploymentRequest
+from aiolirest.models.role import Role
+from aiolirest.models.role_assignment import RoleAssignment
+from aiolirest.models.role_assignments import RoleAssignments
 from aiolirest.models.success_response import SuccessResponse
 
 from aiolirest.api_client import ApiClient
 from aiolirest.api_response import ApiResponse
 from aiolirest.rest import RESTResponseType
 
 
-class DeploymentsApi:
+class RolesApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def deployments_get(
+    def roles_add_assignments_post(
         self,
+        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Deployment]:
-        """Get all deployments.
+    ) -> RoleAssignments:
+        """Add user and role assignments
 
-        Return the properties of all configured deployments.
+        Authorize the specified users to perform actions associated with the specified roles.
 
+        :param role_assignments: User and Role Assignment Data (required)
+        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -90,23 +94,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_get_serialize(
+        _param = self._roles_add_assignments_post_serialize(
+            role_assignments=role_assignments,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Deployment]",
+            '201': "RoleAssignments",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -114,33 +120,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def deployments_get_with_http_info(
+    def roles_add_assignments_post_with_http_info(
         self,
+        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Deployment]]:
-        """Get all deployments.
+    ) -> ApiResponse[RoleAssignments]:
+        """Add user and role assignments
 
-        Return the properties of all configured deployments.
+        Authorize the specified users to perform actions associated with the specified roles.
 
+        :param role_assignments: User and Role Assignment Data (required)
+        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -155,23 +164,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_get_serialize(
+        _param = self._roles_add_assignments_post_serialize(
+            role_assignments=role_assignments,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Deployment]",
+            '201': "RoleAssignments",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -179,33 +190,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def deployments_get_without_preload_content(
+    def roles_add_assignments_post_without_preload_content(
         self,
+        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get all deployments.
+        """Add user and role assignments
 
-        Return the properties of all configured deployments.
+        Authorize the specified users to perform actions associated with the specified roles.
 
+        :param role_assignments: User and Role Assignment Data (required)
+        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -220,35 +234,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_get_serialize(
+        _param = self._roles_add_assignments_post_serialize(
+            role_assignments=role_assignments,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Deployment]",
+            '201': "RoleAssignments",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _deployments_get_serialize(
+    def _roles_add_assignments_post_serialize(
         self,
+        role_assignments,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -265,32 +282,47 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if role_assignments is not None:
+            _body_params = role_assignments
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/deployments',
+            method='POST',
+            resource_path='/roles/add-assignments',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -299,36 +331,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def deployments_id_delete(
+    def roles_assignments_get(
         self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        username: Annotated[Optional[StrictStr], Field(description="search by username")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> SuccessResponse:
-        """Delete a deployment.
+    ) -> List[RoleAssignment]:
+        """List user and role assignments
 
-        Delete a deployment by ID.  Deleting a deployment stops any service instances and removes the service from the cluster.
+        List users authorized to perform actions associated with a role.
 
-        :param id: Deployment ID (required)
-        :type id: str
+        :param username: search by username
+        :type username: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -343,25 +375,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_id_delete_serialize(
-            id=id,
+        _param = self._roles_assignments_get_serialize(
+            username=username,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SuccessResponse",
-            '404': "ErrorResponse",
+            '200': "List[RoleAssignment]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -369,36 +400,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def deployments_id_delete_with_http_info(
+    def roles_assignments_get_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        username: Annotated[Optional[StrictStr], Field(description="search by username")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[SuccessResponse]:
-        """Delete a deployment.
+    ) -> ApiResponse[List[RoleAssignment]]:
+        """List user and role assignments
 
-        Delete a deployment by ID.  Deleting a deployment stops any service instances and removes the service from the cluster.
+        List users authorized to perform actions associated with a role.
 
-        :param id: Deployment ID (required)
-        :type id: str
+        :param username: search by username
+        :type username: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -413,25 +444,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_id_delete_serialize(
-            id=id,
+        _param = self._roles_assignments_get_serialize(
+            username=username,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SuccessResponse",
-            '404': "ErrorResponse",
+            '200': "List[RoleAssignment]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -439,36 +469,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def deployments_id_delete_without_preload_content(
+    def roles_assignments_get_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        username: Annotated[Optional[StrictStr], Field(description="search by username")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a deployment.
+        """List user and role assignments
 
-        Delete a deployment by ID.  Deleting a deployment stops any service instances and removes the service from the cluster.
+        List users authorized to perform actions associated with a role.
 
-        :param id: Deployment ID (required)
-        :type id: str
+        :param username: search by username
+        :type username: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -483,38 +513,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_id_delete_serialize(
-            id=id,
+        _param = self._roles_assignments_get_serialize(
+            username=username,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SuccessResponse",
-            '404': "ErrorResponse",
+            '200': "List[RoleAssignment]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _deployments_id_delete_serialize(
+    def _roles_assignments_get_serialize(
         self,
-        id,
+        username,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -527,285 +556,19 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
         # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                '*/*'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'ApiKeyAuth'
-        ]
-
-        return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/deployments/{id}',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def deployments_id_get(
-        self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Deployment:
-        """Gets a deployment.
-
-        Return the properties of the deployment by ID.
-
-        :param id: Deployment ID (required)
-        :type id: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._deployments_id_get_serialize(
-            id=id,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Deployment",
-            '404': "ErrorResponse",
-            '500': "ErrorResponse"
-            
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def deployments_id_get_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Deployment]:
-        """Gets a deployment.
-
-        Return the properties of the deployment by ID.
-
-        :param id: Deployment ID (required)
-        :type id: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._deployments_id_get_serialize(
-            id=id,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Deployment",
-            '404': "ErrorResponse",
-            '500': "ErrorResponse"
+        if username is not None:
             
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def deployments_id_get_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Gets a deployment.
-
-        Return the properties of the deployment by ID.
-
-        :param id: Deployment ID (required)
-        :type id: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._deployments_id_get_serialize(
-            id=id,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Deployment",
-            '404': "ErrorResponse",
-            '500': "ErrorResponse"
+            _query_params.append(('username', username))
             
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _deployments_id_get_serialize(
-        self,
-        id,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> Tuple:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-            
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -818,15 +581,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/deployments/{id}',
+            resource_path='/roles/assignments',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -835,39 +598,33 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def deployments_id_put(
+    def roles_get(
         self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
-        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Deployment:
-        """Update deployment.
+    ) -> List[Role]:
+        """List all roles.
 
-        Update a deployment by providing an updated Deployment object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned
+        List all roles.
 
-        :param id: Deployment ID (required)
-        :type id: str
-        :param deployment: Deployment Data (required)
-        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -882,27 +639,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_id_put_serialize(
-            id=id,
-            deployment=deployment,
+        _param = self._roles_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Deployment",
-            '400': "ErrorResponse",
-            '404': "ErrorResponse",
+            '200': "List[Role]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -910,39 +663,33 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def deployments_id_put_with_http_info(
+    def roles_get_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
-        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Deployment]:
-        """Update deployment.
+    ) -> ApiResponse[List[Role]]:
+        """List all roles.
 
-        Update a deployment by providing an updated Deployment object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned
+        List all roles.
 
-        :param id: Deployment ID (required)
-        :type id: str
-        :param deployment: Deployment Data (required)
-        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -957,27 +704,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_id_put_serialize(
-            id=id,
-            deployment=deployment,
+        _param = self._roles_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Deployment",
-            '400': "ErrorResponse",
-            '404': "ErrorResponse",
+            '200': "List[Role]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -985,39 +728,33 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def deployments_id_put_without_preload_content(
+    def roles_get_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Deployment ID")],
-        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Update deployment.
+        """List all roles.
 
-        Update a deployment by providing an updated Deployment object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned
+        List all roles.
 
-        :param id: Deployment ID (required)
-        :type id: str
-        :param deployment: Deployment Data (required)
-        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1032,41 +769,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_id_put_serialize(
-            id=id,
-            deployment=deployment,
+        _param = self._roles_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Deployment",
-            '400': "ErrorResponse",
-            '404': "ErrorResponse",
+            '200': "List[Role]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _deployments_id_put_serialize(
+    def _roles_get_serialize(
         self,
-        id,
-        deployment,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1079,22 +810,18 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if deployment is not None:
-            _body_params = deployment
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1103,16 +830,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/deployments/{id}',
+            method='GET',
+            resource_path='/roles',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1121,36 +848,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def deployments_post(
+    def roles_remove_assignments_post(
         self,
-        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
+        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Deployment:
-        """Create a new deployment.
+    ) -> SuccessResponse:
+        """Remove user and role assignments
 
-        Create a deployment of a service onto a cluster. This object controls the deployment and encapsulates the status of that deployment.
+        Remove the specified users from performing actions associated with the specified roles.
 
-        :param deployment: Deployment Data (required)
-        :type deployment: DeploymentRequest
+        :param role_assignments: User and Role Assignment Data (required)
+        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1165,24 +892,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_post_serialize(
-            deployment=deployment,
+        _param = self._roles_remove_assignments_post_serialize(
+            role_assignments=role_assignments,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Deployment",
+            '201': "SuccessResponse",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1191,36 +918,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def deployments_post_with_http_info(
+    def roles_remove_assignments_post_with_http_info(
         self,
-        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
+        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Deployment]:
-        """Create a new deployment.
+    ) -> ApiResponse[SuccessResponse]:
+        """Remove user and role assignments
 
-        Create a deployment of a service onto a cluster. This object controls the deployment and encapsulates the status of that deployment.
+        Remove the specified users from performing actions associated with the specified roles.
 
-        :param deployment: Deployment Data (required)
-        :type deployment: DeploymentRequest
+        :param role_assignments: User and Role Assignment Data (required)
+        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1235,24 +962,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_post_serialize(
-            deployment=deployment,
+        _param = self._roles_remove_assignments_post_serialize(
+            role_assignments=role_assignments,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Deployment",
+            '201': "SuccessResponse",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1261,36 +988,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def deployments_post_without_preload_content(
+    def roles_remove_assignments_post_without_preload_content(
         self,
-        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
+        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create a new deployment.
+        """Remove user and role assignments
 
-        Create a deployment of a service onto a cluster. This object controls the deployment and encapsulates the status of that deployment.
+        Remove the specified users from performing actions associated with the specified roles.
 
-        :param deployment: Deployment Data (required)
-        :type deployment: DeploymentRequest
+        :param role_assignments: User and Role Assignment Data (required)
+        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1305,38 +1032,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._deployments_post_serialize(
-            deployment=deployment,
+        _param = self._roles_remove_assignments_post_serialize(
+            role_assignments=role_assignments,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Deployment",
+            '201': "SuccessResponse",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _deployments_post_serialize(
+    def _roles_remove_assignments_post_serialize(
         self,
-        deployment,
+        role_assignments,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1353,16 +1080,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if deployment is not None:
-            _body_params = deployment
+        if role_assignments is not None:
+            _body_params = role_assignments
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1385,15 +1112,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/deployments',
+            resource_path='/roles/remove-assignments',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api/information_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/information_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api/models_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/registries_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -27,54 +27,54 @@
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictStr
 
 from typing import List
 
 from aiolirest.models.success_response import SuccessResponse
-from aiolirest.models.trained_model import TrainedModel
-from aiolirest.models.trained_model_request import TrainedModelRequest
+from aiolirest.models.trained_model_registry import TrainedModelRegistry
+from aiolirest.models.trained_model_registry_request import TrainedModelRegistryRequest
 
 from aiolirest.api_client import ApiClient
 from aiolirest.api_response import ApiResponse
 from aiolirest.rest import RESTResponseType
 
 
-class ModelsApi:
+class RegistriesApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def models_get(
+    def registries_get(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[TrainedModel]:
-        """Get all models.
+    ) -> List[TrainedModelRegistry]:
+        """Get all model registries.
 
-        Return the properties of all configured models.
+        Return the properties of all configured model registries.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -90,23 +90,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_get_serialize(
+        _param = self._registries_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[TrainedModel]",
+            '200': "List[TrainedModelRegistry]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -114,32 +114,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def models_get_with_http_info(
+    def registries_get_with_http_info(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[TrainedModel]]:
-        """Get all models.
+    ) -> ApiResponse[List[TrainedModelRegistry]]:
+        """Get all model registries.
 
-        Return the properties of all configured models.
+        Return the properties of all configured model registries.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -155,23 +155,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_get_serialize(
+        _param = self._registries_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[TrainedModel]",
+            '200': "List[TrainedModelRegistry]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -179,32 +179,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def models_get_without_preload_content(
+    def registries_get_without_preload_content(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get all models.
+        """Get all model registries.
 
-        Return the properties of all configured models.
+        Return the properties of all configured model registries.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -220,34 +220,34 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_get_serialize(
+        _param = self._registries_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[TrainedModel]",
+            '200': "List[TrainedModelRegistry]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _models_get_serialize(
+    def _registries_get_serialize(
         self,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
@@ -282,15 +282,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/models',
+            resource_path='/registries',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -299,35 +299,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def models_id_delete(
+    def registries_id_delete(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> SuccessResponse:
-        """Delete a model.
+        """Delete a model registry.
 
-        Delete a model version by ID.  To successfully delete a model version it can no longer be referenced by any services. Each model version must be deleted separately.
+        Delete a model registry by ID.  To successfully delete a model registry it can no longer be referenced by any models.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -343,15 +343,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_delete_serialize(
+        _param = self._registries_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -369,35 +369,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def models_id_delete_with_http_info(
+    def registries_id_delete_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[SuccessResponse]:
-        """Delete a model.
+        """Delete a model registry.
 
-        Delete a model version by ID.  To successfully delete a model version it can no longer be referenced by any services. Each model version must be deleted separately.
+        Delete a model registry by ID.  To successfully delete a model registry it can no longer be referenced by any models.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -413,15 +413,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_delete_serialize(
+        _param = self._registries_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -439,35 +439,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def models_id_delete_without_preload_content(
+    def registries_id_delete_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a model.
+        """Delete a model registry.
 
-        Delete a model version by ID.  To successfully delete a model version it can no longer be referenced by any services. Each model version must be deleted separately.
+        Delete a model registry by ID.  To successfully delete a model registry it can no longer be referenced by any models.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -483,15 +483,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_delete_serialize(
+        _param = self._registries_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -504,15 +504,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _models_id_delete_serialize(
+    def _registries_id_delete_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -550,15 +550,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/models/{id}',
+            resource_path='/registries/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -567,35 +567,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def models_id_get(
+    def registries_id_get(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> TrainedModel:
-        """Get a model.
+    ) -> TrainedModelRegistry:
+        """Get a model registry by ID.
 
-        Return the properties of the model by ID.
+        Return the properties of the model registry by ID.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -611,24 +611,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_get_serialize(
+        _param = self._registries_id_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TrainedModel",
+            '200': "TrainedModelRegistry",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -637,35 +637,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def models_id_get_with_http_info(
+    def registries_id_get_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[TrainedModel]:
-        """Get a model.
+    ) -> ApiResponse[TrainedModelRegistry]:
+        """Get a model registry by ID.
 
-        Return the properties of the model by ID.
+        Return the properties of the model registry by ID.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -681,24 +681,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_get_serialize(
+        _param = self._registries_id_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TrainedModel",
+            '200': "TrainedModelRegistry",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -707,35 +707,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def models_id_get_without_preload_content(
+    def registries_id_get_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get a model.
+        """Get a model registry by ID.
 
-        Return the properties of the model by ID.
+        Return the properties of the model registry by ID.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -751,36 +751,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_get_serialize(
+        _param = self._registries_id_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TrainedModel",
+            '200': "TrainedModelRegistry",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _models_id_get_serialize(
+    def _registries_id_get_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -818,15 +818,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/models/{id}',
+            resource_path='/registries/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -835,39 +835,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def models_id_put(
+    def registries_id_put(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
-        trained_model: Annotated[TrainedModelRequest, Field(description="Model Data")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        trained_model_registry: Annotated[TrainedModelRegistryRequest, Field(description="Model Registry Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> TrainedModel:
-        """Update a model.
+    ) -> TrainedModelRegistry:
+        """Update a model registry.
 
-        Update a model by providing an updated TrainedModel object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned TrainedModel. You may change the name or description of a deployed model.  Changing the model image or URI will create a new version of the model which will be returned. Alternatively, you can create a new version of the model using the create method.
+        Update a model registry by providing an updated TrainedModelRegistry object.  This is normally obtained by a prior get operation, and then selectively modifying the returned TrainedModelRegistry.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
-        :param trained_model: Model Data (required)
-        :type trained_model: TrainedModelRequest
+        :param trained_model_registry: Model Registry Data (required)
+        :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -882,27 +882,26 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_put_serialize(
+        _param = self._registries_id_put_serialize(
             id=id,
-            trained_model=trained_model,
+            trained_model_registry=trained_model_registry,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TrainedModel",
+            '200': "TrainedModelRegistry",
             '400': "ErrorResponse",
-            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -910,39 +909,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def models_id_put_with_http_info(
+    def registries_id_put_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
-        trained_model: Annotated[TrainedModelRequest, Field(description="Model Data")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        trained_model_registry: Annotated[TrainedModelRegistryRequest, Field(description="Model Registry Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[TrainedModel]:
-        """Update a model.
+    ) -> ApiResponse[TrainedModelRegistry]:
+        """Update a model registry.
 
-        Update a model by providing an updated TrainedModel object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned TrainedModel. You may change the name or description of a deployed model.  Changing the model image or URI will create a new version of the model which will be returned. Alternatively, you can create a new version of the model using the create method.
+        Update a model registry by providing an updated TrainedModelRegistry object.  This is normally obtained by a prior get operation, and then selectively modifying the returned TrainedModelRegistry.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
-        :param trained_model: Model Data (required)
-        :type trained_model: TrainedModelRequest
+        :param trained_model_registry: Model Registry Data (required)
+        :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -957,27 +956,26 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_put_serialize(
+        _param = self._registries_id_put_serialize(
             id=id,
-            trained_model=trained_model,
+            trained_model_registry=trained_model_registry,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TrainedModel",
+            '200': "TrainedModelRegistry",
             '400': "ErrorResponse",
-            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -985,39 +983,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def models_id_put_without_preload_content(
+    def registries_id_put_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Model ID")],
-        trained_model: Annotated[TrainedModelRequest, Field(description="Model Data")],
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        trained_model_registry: Annotated[TrainedModelRegistryRequest, Field(description="Model Registry Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Update a model.
+        """Update a model registry.
 
-        Update a model by providing an updated TrainedModel object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned TrainedModel. You may change the name or description of a deployed model.  Changing the model image or URI will create a new version of the model which will be returned. Alternatively, you can create a new version of the model using the create method.
+        Update a model registry by providing an updated TrainedModelRegistry object.  This is normally obtained by a prior get operation, and then selectively modifying the returned TrainedModelRegistry.
 
-        :param id: Model ID (required)
+        :param id: Model Registry ID (required)
         :type id: str
-        :param trained_model: Model Data (required)
-        :type trained_model: TrainedModelRequest
+        :param trained_model_registry: Model Registry Data (required)
+        :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1032,41 +1030,40 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_id_put_serialize(
+        _param = self._registries_id_put_serialize(
             id=id,
-            trained_model=trained_model,
+            trained_model_registry=trained_model_registry,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TrainedModel",
+            '200': "TrainedModelRegistry",
             '400': "ErrorResponse",
-            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _models_id_put_serialize(
+    def _registries_id_put_serialize(
         self,
         id,
-        trained_model,
+        trained_model_registry,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1085,16 +1082,16 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if trained_model is not None:
-            _body_params = trained_model
+        if trained_model_registry is not None:
+            _body_params = trained_model_registry
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1104,15 +1101,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
-            resource_path='/models/{id}',
+            resource_path='/registries/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1121,36 +1118,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def models_post(
+    def registries_post(
         self,
-        trained_model: Annotated[TrainedModelRequest, Field(description="Model Data")],
+        trained_model_registry: Annotated[TrainedModelRegistryRequest, Field(description="Model Registry Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> TrainedModel:
-        """Create a new trained model description.
+    ) -> TrainedModelRegistry:
+        """Create a new model registry.
 
-        Provide the details of a model to be deployed.   It requires a containerized Bento, and optionally a reference to an S3 registry hosting the model (unless it is built into the Bento container). Multiple versions of the same model name are expected.   When created, a new version is assigned to the model.  Once deployed, models should be treated as immutable.   To update a model, create a new instance of the same model name with updated image and/or url.   This will create a new version of the model.
+        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from Nvidia NGC: AI Development Catalog.
 
-        :param trained_model: Model Data (required)
-        :type trained_model: TrainedModelRequest
+        :param trained_model_registry: Model Registry Data (required)
+        :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1165,24 +1162,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_post_serialize(
-            trained_model=trained_model,
+        _param = self._registries_post_serialize(
+            trained_model_registry=trained_model_registry,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "TrainedModel",
+            '201': "TrainedModelRegistry",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1191,36 +1188,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def models_post_with_http_info(
+    def registries_post_with_http_info(
         self,
-        trained_model: Annotated[TrainedModelRequest, Field(description="Model Data")],
+        trained_model_registry: Annotated[TrainedModelRegistryRequest, Field(description="Model Registry Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[TrainedModel]:
-        """Create a new trained model description.
+    ) -> ApiResponse[TrainedModelRegistry]:
+        """Create a new model registry.
 
-        Provide the details of a model to be deployed.   It requires a containerized Bento, and optionally a reference to an S3 registry hosting the model (unless it is built into the Bento container). Multiple versions of the same model name are expected.   When created, a new version is assigned to the model.  Once deployed, models should be treated as immutable.   To update a model, create a new instance of the same model name with updated image and/or url.   This will create a new version of the model.
+        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from Nvidia NGC: AI Development Catalog.
 
-        :param trained_model: Model Data (required)
-        :type trained_model: TrainedModelRequest
+        :param trained_model_registry: Model Registry Data (required)
+        :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1235,24 +1232,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_post_serialize(
-            trained_model=trained_model,
+        _param = self._registries_post_serialize(
+            trained_model_registry=trained_model_registry,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "TrainedModel",
+            '201': "TrainedModelRegistry",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1261,36 +1258,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def models_post_without_preload_content(
+    def registries_post_without_preload_content(
         self,
-        trained_model: Annotated[TrainedModelRequest, Field(description="Model Data")],
+        trained_model_registry: Annotated[TrainedModelRegistryRequest, Field(description="Model Registry Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create a new trained model description.
+        """Create a new model registry.
 
-        Provide the details of a model to be deployed.   It requires a containerized Bento, and optionally a reference to an S3 registry hosting the model (unless it is built into the Bento container). Multiple versions of the same model name are expected.   When created, a new version is assigned to the model.  Once deployed, models should be treated as immutable.   To update a model, create a new instance of the same model name with updated image and/or url.   This will create a new version of the model.
+        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from Nvidia NGC: AI Development Catalog.
 
-        :param trained_model: Model Data (required)
-        :type trained_model: TrainedModelRequest
+        :param trained_model_registry: Model Registry Data (required)
+        :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1305,38 +1302,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._models_post_serialize(
-            trained_model=trained_model,
+        _param = self._registries_post_serialize(
+            trained_model_registry=trained_model_registry,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "TrainedModel",
+            '201': "TrainedModelRegistry",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _models_post_serialize(
+    def _registries_post_serialize(
         self,
-        trained_model,
+        trained_model_registry,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1353,16 +1350,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if trained_model is not None:
-            _body_params = trained_model
+        if trained_model_registry is not None:
+            _body_params = trained_model_registry
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1385,15 +1382,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/models',
+            resource_path='/registries',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api/roles_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/users_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -22,64 +22,61 @@
 try:
     from typing import Annotated
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
-from pydantic import StrictStr
+from pydantic import StrictInt, StrictStr
 
-from typing import List, Optional
+from typing import List
 
-from aiolirest.models.role import Role
-from aiolirest.models.role_assignment import RoleAssignment
-from aiolirest.models.role_assignments import RoleAssignments
 from aiolirest.models.success_response import SuccessResponse
+from aiolirest.models.user import User
+from aiolirest.models.user_patch_request import UserPatchRequest
+from aiolirest.models.user_request import UserRequest
 
 from aiolirest.api_client import ApiClient
 from aiolirest.api_response import ApiResponse
 from aiolirest.rest import RESTResponseType
 
 
-class RolesApi:
+class UsersApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def roles_add_assignments_post(
+    def users_get(
         self,
-        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RoleAssignments:
-        """Add user and role assignments
+    ) -> List[User]:
+        """Get configured users.
 
-        Authorize the specified users to perform actions associated with the specified roles.
+        Get the properties of all configured users.
 
-        :param role_assignments: User and Role Assignment Data (required)
-        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -94,24 +91,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_add_assignments_post_serialize(
-            role_assignments=role_assignments,
+        _param = self._users_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "RoleAssignments",
+            '200': "List[User]",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -120,36 +116,33 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def roles_add_assignments_post_with_http_info(
+    def users_get_with_http_info(
         self,
-        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[RoleAssignments]:
-        """Add user and role assignments
+    ) -> ApiResponse[List[User]]:
+        """Get configured users.
 
-        Authorize the specified users to perform actions associated with the specified roles.
+        Get the properties of all configured users.
 
-        :param role_assignments: User and Role Assignment Data (required)
-        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -164,24 +157,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_add_assignments_post_serialize(
-            role_assignments=role_assignments,
+        _param = self._users_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "RoleAssignments",
+            '200': "List[User]",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -190,36 +182,33 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def roles_add_assignments_post_without_preload_content(
+    def users_get_without_preload_content(
         self,
-        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Add user and role assignments
+        """Get configured users.
 
-        Authorize the specified users to perform actions associated with the specified roles.
+        Get the properties of all configured users.
 
-        :param role_assignments: User and Role Assignment Data (required)
-        :type role_assignments: RoleAssignments
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -234,38 +223,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_add_assignments_post_serialize(
-            role_assignments=role_assignments,
+        _param = self._users_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "RoleAssignments",
+            '200': "List[User]",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _roles_add_assignments_post_serialize(
+    def _users_get_serialize(
         self,
-        role_assignments,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -282,47 +269,32 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if role_assignments is not None:
-            _body_params = role_assignments
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/roles/add-assignments',
+            method='GET',
+            resource_path='/users',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -331,36 +303,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def roles_assignments_get(
+    def users_id_delete(
         self,
-        username: Annotated[Optional[StrictStr], Field(description="search by username")] = None,
+        id: Annotated[StrictInt, Field(description="User ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[RoleAssignment]:
-        """List user and role assignments
+    ) -> SuccessResponse:
+        """Delete a user.
 
-        List users authorized to perform actions associated with a role.
+        Delete a user specified by ID.
 
-        :param username: search by username
-        :type username: str
+        :param id: User ID (required)
+        :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -375,24 +347,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_assignments_get_serialize(
-            username=username,
+        _param = self._users_id_delete_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RoleAssignment]",
+            '200': "SuccessResponse",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -400,36 +373,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def roles_assignments_get_with_http_info(
+    def users_id_delete_with_http_info(
         self,
-        username: Annotated[Optional[StrictStr], Field(description="search by username")] = None,
+        id: Annotated[StrictInt, Field(description="User ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[RoleAssignment]]:
-        """List user and role assignments
+    ) -> ApiResponse[SuccessResponse]:
+        """Delete a user.
 
-        List users authorized to perform actions associated with a role.
+        Delete a user specified by ID.
 
-        :param username: search by username
-        :type username: str
+        :param id: User ID (required)
+        :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -444,24 +417,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_assignments_get_serialize(
-            username=username,
+        _param = self._users_id_delete_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RoleAssignment]",
+            '200': "SuccessResponse",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -469,36 +443,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def roles_assignments_get_without_preload_content(
+    def users_id_delete_without_preload_content(
         self,
-        username: Annotated[Optional[StrictStr], Field(description="search by username")] = None,
+        id: Annotated[StrictInt, Field(description="User ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """List user and role assignments
+        """Delete a user.
 
-        List users authorized to perform actions associated with a role.
+        Delete a user specified by ID.
 
-        :param username: search by username
-        :type username: str
+        :param id: User ID (required)
+        :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -513,37 +487,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_assignments_get_serialize(
-            username=username,
+        _param = self._users_id_delete_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RoleAssignment]",
+            '200': "SuccessResponse",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _roles_assignments_get_serialize(
+    def _users_id_delete_serialize(
         self,
-        username,
+        id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -556,19 +531,285 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
-        if username is not None:
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                '*/*'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='DELETE',
+            resource_path='/users/{id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def users_id_get(
+        self,
+        id: Annotated[StrictInt, Field(description="User ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[User]:
+        """Gets a user.
+
+        Get the properties of the user specified by ID.
+
+        :param id: User ID (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._users_id_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[User]",
+            '400': "ErrorResponse",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def users_id_get_with_http_info(
+        self,
+        id: Annotated[StrictInt, Field(description="User ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[User]]:
+        """Gets a user.
+
+        Get the properties of the user specified by ID.
+
+        :param id: User ID (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._users_id_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[User]",
+            '400': "ErrorResponse",
+            '500': "ErrorResponse"
             
-            _query_params.append(('username', username))
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def users_id_get_without_preload_content(
+        self,
+        id: Annotated[StrictInt, Field(description="User ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Gets a user.
+
+        Get the properties of the user specified by ID.
+
+        :param id: User ID (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._users_id_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[User]",
+            '400': "ErrorResponse",
+            '500': "ErrorResponse"
             
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _users_id_get_serialize(
+        self,
+        id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -581,15 +822,311 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/roles/assignments',
+            resource_path='/users/{id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def users_id_patch(
+        self,
+        id: Annotated[StrictStr, Field(description="User ID")],
+        user_patch_request: Annotated[UserPatchRequest, Field(description="yes")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> User:
+        """Update user properties.
+
+        Update a user's properties. Provide a body that contains one or more of the properties: - `password` - `admin` - `active`
+
+        :param id: User ID (required)
+        :type id: str
+        :param user_patch_request: yes (required)
+        :type user_patch_request: UserPatchRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._users_id_patch_serialize(
+            id=id,
+            user_patch_request=user_patch_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "User",
+            '400': "ErrorResponse",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def users_id_patch_with_http_info(
+        self,
+        id: Annotated[StrictStr, Field(description="User ID")],
+        user_patch_request: Annotated[UserPatchRequest, Field(description="yes")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[User]:
+        """Update user properties.
+
+        Update a user's properties. Provide a body that contains one or more of the properties: - `password` - `admin` - `active`
+
+        :param id: User ID (required)
+        :type id: str
+        :param user_patch_request: yes (required)
+        :type user_patch_request: UserPatchRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._users_id_patch_serialize(
+            id=id,
+            user_patch_request=user_patch_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "User",
+            '400': "ErrorResponse",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def users_id_patch_without_preload_content(
+        self,
+        id: Annotated[StrictStr, Field(description="User ID")],
+        user_patch_request: Annotated[UserPatchRequest, Field(description="yes")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Update user properties.
+
+        Update a user's properties. Provide a body that contains one or more of the properties: - `password` - `admin` - `active`
+
+        :param id: User ID (required)
+        :type id: str
+        :param user_patch_request: yes (required)
+        :type user_patch_request: UserPatchRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._users_id_patch_serialize(
+            id=id,
+            user_patch_request=user_patch_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "User",
+            '400': "ErrorResponse",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _users_id_patch_serialize(
+        self,
+        id,
+        user_patch_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if user_patch_request is not None:
+            _body_params = user_patch_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                '*/*'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='PATCH',
+            resource_path='/users/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -598,32 +1135,32 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def roles_get(
+    def users_me_get(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Role]:
-        """List all roles.
+    ) -> User:
+        """Get current authenticated user.
 
-        List all roles.
+        Get the properties of the current user.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -639,23 +1176,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_get_serialize(
+        _param = self._users_me_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Role]",
+            '200': "User",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -663,32 +1201,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def roles_get_with_http_info(
+    def users_me_get_with_http_info(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Role]]:
-        """List all roles.
+    ) -> ApiResponse[User]:
+        """Get current authenticated user.
 
-        List all roles.
+        Get the properties of the current user.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -704,23 +1242,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_get_serialize(
+        _param = self._users_me_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Role]",
+            '200': "User",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -728,32 +1267,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def roles_get_without_preload_content(
+    def users_me_get_without_preload_content(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """List all roles.
+        """Get current authenticated user.
 
-        List all roles.
+        Get the properties of the current user.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -769,34 +1308,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_get_serialize(
+        _param = self._users_me_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Role]",
+            '200': "User",
+            '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _roles_get_serialize(
+    def _users_me_get_serialize(
         self,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
@@ -831,15 +1371,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/roles',
+            resource_path='/users/me',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -848,36 +1388,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def roles_remove_assignments_post(
+    def users_post(
         self,
-        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
+        user: Annotated[UserRequest, Field(description="User Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> SuccessResponse:
-        """Remove user and role assignments
+        """Create a new user.
 
-        Remove the specified users from performing actions associated with the specified roles.
+        Create a new user.  This method is enabled only for administrator users.
 
-        :param role_assignments: User and Role Assignment Data (required)
-        :type role_assignments: RoleAssignments
+        :param user: User Data (required)
+        :type user: UserRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -892,16 +1432,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_remove_assignments_post_serialize(
-            role_assignments=role_assignments,
+        _param = self._users_post_serialize(
+            user=user,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -918,36 +1458,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def roles_remove_assignments_post_with_http_info(
+    def users_post_with_http_info(
         self,
-        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
+        user: Annotated[UserRequest, Field(description="User Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[SuccessResponse]:
-        """Remove user and role assignments
+        """Create a new user.
 
-        Remove the specified users from performing actions associated with the specified roles.
+        Create a new user.  This method is enabled only for administrator users.
 
-        :param role_assignments: User and Role Assignment Data (required)
-        :type role_assignments: RoleAssignments
+        :param user: User Data (required)
+        :type user: UserRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -962,16 +1502,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_remove_assignments_post_serialize(
-            role_assignments=role_assignments,
+        _param = self._users_post_serialize(
+            user=user,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -988,36 +1528,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def roles_remove_assignments_post_without_preload_content(
+    def users_post_without_preload_content(
         self,
-        role_assignments: Annotated[RoleAssignments, Field(description="User and Role Assignment Data")],
+        user: Annotated[UserRequest, Field(description="User Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Remove user and role assignments
+        """Create a new user.
 
-        Remove the specified users from performing actions associated with the specified roles.
+        Create a new user.  This method is enabled only for administrator users.
 
-        :param role_assignments: User and Role Assignment Data (required)
-        :type role_assignments: RoleAssignments
+        :param user: User Data (required)
+        :type user: UserRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1032,16 +1572,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._roles_remove_assignments_post_serialize(
-            role_assignments=role_assignments,
+        _param = self._users_post_serialize(
+            user=user,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1053,17 +1593,17 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _roles_remove_assignments_post_serialize(
+    def _users_post_serialize(
         self,
-        role_assignments,
+        user,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1080,16 +1620,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if role_assignments is not None:
-            _body_params = role_assignments
+        if user is not None:
+            _body_params = user
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1112,15 +1652,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/roles/remove-assignments',
+            resource_path='/users',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api/services_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/deployments_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,59 +24,59 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictStr
 
-from typing import List
+from typing import List, Optional
 
-from aiolirest.models.service import Service
-from aiolirest.models.service_auth_token import ServiceAuthToken
-from aiolirest.models.service_model_version import ServiceModelVersion
-from aiolirest.models.service_request import ServiceRequest
+from aiolirest.models.deployment import Deployment
+from aiolirest.models.deployment_request import DeploymentRequest
+from aiolirest.models.event_info import EventInfo
+from aiolirest.models.observability import Observability
 from aiolirest.models.success_response import SuccessResponse
 
 from aiolirest.api_client import ApiClient
 from aiolirest.api_response import ApiResponse
 from aiolirest.rest import RESTResponseType
 
 
-class ServicesApi:
+class DeploymentsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def services_get(
+    def deployments_get(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Service]:
-        """Get all services.
+    ) -> List[Deployment]:
+        """Get all deployments.
 
-        Return the properties of all configured services.
+        Return the properties of all configured deployments.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -92,23 +92,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_get_serialize(
+        _param = self._deployments_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Service]",
+            '200': "List[Deployment]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -116,32 +116,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def services_get_with_http_info(
+    def deployments_get_with_http_info(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Service]]:
-        """Get all services.
+    ) -> ApiResponse[List[Deployment]]:
+        """Get all deployments.
 
-        Return the properties of all configured services.
+        Return the properties of all configured deployments.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -157,23 +157,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_get_serialize(
+        _param = self._deployments_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Service]",
+            '200': "List[Deployment]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -181,32 +181,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def services_get_without_preload_content(
+    def deployments_get_without_preload_content(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get all services.
+        """Get all deployments.
 
-        Return the properties of all configured services.
+        Return the properties of all configured deployments.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -222,34 +222,34 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_get_serialize(
+        _param = self._deployments_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Service]",
+            '200': "List[Deployment]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _services_get_serialize(
+    def _deployments_get_serialize(
         self,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
@@ -284,15 +284,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/services',
+            resource_path='/deployments',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -301,35 +301,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def services_id_delete(
+    def deployments_id_delete(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> SuccessResponse:
-        """Delete a service.
+        """Delete a deployment.
 
-        Delete a service by ID.  To successfully delete a service it can no longer be referenced by any deployment.
+        Delete a deployment by ID.  Deleting a deployment stops any service instances and removes the service from the cluster.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -345,15 +345,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_delete_serialize(
+        _param = self._deployments_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -371,35 +371,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def services_id_delete_with_http_info(
+    def deployments_id_delete_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[SuccessResponse]:
-        """Delete a service.
+        """Delete a deployment.
 
-        Delete a service by ID.  To successfully delete a service it can no longer be referenced by any deployment.
+        Delete a deployment by ID.  Deleting a deployment stops any service instances and removes the service from the cluster.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -415,15 +415,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_delete_serialize(
+        _param = self._deployments_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -441,35 +441,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def services_id_delete_without_preload_content(
+    def deployments_id_delete_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a service.
+        """Delete a deployment.
 
-        Delete a service by ID.  To successfully delete a service it can no longer be referenced by any deployment.
+        Delete a deployment by ID.  Deleting a deployment stops any service instances and removes the service from the cluster.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -485,15 +485,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_delete_serialize(
+        _param = self._deployments_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -506,15 +506,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _services_id_delete_serialize(
+    def _deployments_id_delete_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -552,15 +552,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/services/{id}',
+            resource_path='/deployments/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -569,35 +569,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def services_id_get(
+    def deployments_id_events_get(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Service:
-        """Gets a service.
+    ) -> List[EventInfo]:
+        """Get recent, significant events related to the service progressing towards the next status.
 
-        Gets a service by ID.
+        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most-recent to oldest.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -613,24 +613,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_get_serialize(
+        _param = self._deployments_id_events_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Service",
+            '200': "List[EventInfo]",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -639,35 +639,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def services_id_get_with_http_info(
+    def deployments_id_events_get_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Service]:
-        """Gets a service.
+    ) -> ApiResponse[List[EventInfo]]:
+        """Get recent, significant events related to the service progressing towards the next status.
 
-        Gets a service by ID.
+        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most-recent to oldest.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -683,24 +683,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_get_serialize(
+        _param = self._deployments_id_events_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Service",
+            '200': "List[EventInfo]",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -709,35 +709,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def services_id_get_without_preload_content(
+    def deployments_id_events_get_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Gets a service.
+        """Get recent, significant events related to the service progressing towards the next status.
 
-        Gets a service by ID.
+        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most-recent to oldest.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -753,36 +753,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_get_serialize(
+        _param = self._deployments_id_events_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Service",
+            '200': "List[EventInfo]",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _services_id_get_serialize(
+    def _deployments_id_events_get_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -820,15 +820,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/services/{id}',
+            resource_path='/deployments/{id}/events',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -837,39 +837,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def services_id_put(
+    def deployments_id_get(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
-        service: Annotated[ServiceRequest, Field(description="Service Data")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Service:
-        """Update service.
+    ) -> Deployment:
+        """Gets a deployment.
 
-        Update a service by providing an updated Service object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the Service. You may rollout or rollback a new model version by updating the model referenced by the service. Specifying a model name in the update, will roll-out the latest version of the model. Specifying a model ID will rollout/rollback to a specific model version.
+        Return the properties of the deployment by ID.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
-        :param service: Service Data (required)
-        :type service: ServiceRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -884,26 +881,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_put_serialize(
+        _param = self._deployments_id_get_serialize(
             id=id,
-            service=service,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Service",
-            '400': "ErrorResponse",
+            '200': "Deployment",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -912,39 +907,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def services_id_put_with_http_info(
+    def deployments_id_get_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
-        service: Annotated[ServiceRequest, Field(description="Service Data")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Service]:
-        """Update service.
+    ) -> ApiResponse[Deployment]:
+        """Gets a deployment.
 
-        Update a service by providing an updated Service object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the Service. You may rollout or rollback a new model version by updating the model referenced by the service. Specifying a model name in the update, will roll-out the latest version of the model. Specifying a model ID will rollout/rollback to a specific model version.
+        Return the properties of the deployment by ID.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
-        :param service: Service Data (required)
-        :type service: ServiceRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -959,26 +951,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_put_serialize(
+        _param = self._deployments_id_get_serialize(
             id=id,
-            service=service,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Service",
-            '400': "ErrorResponse",
+            '200': "Deployment",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -987,39 +977,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def services_id_put_without_preload_content(
+    def deployments_id_get_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
-        service: Annotated[ServiceRequest, Field(description="Service Data")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Update service.
+        """Gets a deployment.
 
-        Update a service by providing an updated Service object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the Service. You may rollout or rollback a new model version by updating the model referenced by the service. Specifying a model name in the update, will roll-out the latest version of the model. Specifying a model ID will rollout/rollback to a specific model version.
+        Return the properties of the deployment by ID.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
-        :param service: Service Data (required)
-        :type service: ServiceRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1034,41 +1021,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_put_serialize(
+        _param = self._deployments_id_get_serialize(
             id=id,
-            service=service,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Service",
-            '400': "ErrorResponse",
+            '200': "Deployment",
             '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _services_id_put_serialize(
+    def _deployments_id_get_serialize(
         self,
         id,
-        service,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1087,16 +1071,14 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if service is not None:
-            _body_params = service
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1105,16 +1087,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/services/{id}',
+            method='GET',
+            resource_path='/deployments/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1123,36 +1105,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def services_id_token_get(
+    def deployments_id_observability_get(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        version: Annotated[Optional[StrictStr], Field(description="Information about a specific version as identified by nativeAppName.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ServiceAuthToken:
-        """Generate and return an auth token for the service.
+    ) -> Observability:
+        """Deployment observability information.
 
-        When the service is deployed with `authorizationRequired=true`, the returned token enables authenticated access to the deployed inference service API.
+        Returns configuration data that enables launching a dashboard URL that describes logs and metrics for the deployment.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
+        :param version: Information about a specific version as identified by nativeAppName.
+        :type version: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1167,24 +1152,26 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_token_get_serialize(
+        _param = self._deployments_id_observability_get_serialize(
             id=id,
+            version=version,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ServiceAuthToken",
+            '200': "Observability",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1192,36 +1179,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def services_id_token_get_with_http_info(
+    def deployments_id_observability_get_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        version: Annotated[Optional[StrictStr], Field(description="Information about a specific version as identified by nativeAppName.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ServiceAuthToken]:
-        """Generate and return an auth token for the service.
+    ) -> ApiResponse[Observability]:
+        """Deployment observability information.
 
-        When the service is deployed with `authorizationRequired=true`, the returned token enables authenticated access to the deployed inference service API.
+        Returns configuration data that enables launching a dashboard URL that describes logs and metrics for the deployment.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
+        :param version: Information about a specific version as identified by nativeAppName.
+        :type version: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1236,24 +1226,26 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_token_get_serialize(
+        _param = self._deployments_id_observability_get_serialize(
             id=id,
+            version=version,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ServiceAuthToken",
+            '200': "Observability",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1261,36 +1253,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def services_id_token_get_without_preload_content(
+    def deployments_id_observability_get_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        version: Annotated[Optional[StrictStr], Field(description="Information about a specific version as identified by nativeAppName.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Generate and return an auth token for the service.
+        """Deployment observability information.
 
-        When the service is deployed with `authorizationRequired=true`, the returned token enables authenticated access to the deployed inference service API.
+        Returns configuration data that enables launching a dashboard URL that describes logs and metrics for the deployment.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
+        :param version: Information about a specific version as identified by nativeAppName.
+        :type version: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1305,37 +1300,40 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_token_get_serialize(
+        _param = self._deployments_id_observability_get_serialize(
             id=id,
+            version=version,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ServiceAuthToken",
+            '200': "Observability",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _services_id_token_get_serialize(
+    def _deployments_id_observability_get_serialize(
         self,
         id,
+        version,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1351,14 +1349,18 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
+        if version is not None:
+            
+            _query_params.append(('version', version))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1371,15 +1373,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/services/{id}/token',
+            resource_path='/deployments/{id}/observability',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1388,36 +1390,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def services_id_versions_get(
+    def deployments_id_put(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[ServiceModelVersion]:
-        """Get all ServiceModelVersion records for a service
+    ) -> Deployment:
+        """Update deployment.
 
-        Return all version records
+        Update a deployment by providing an updated Deployment object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned deployment.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
+        :param deployment: Deployment Data (required)
+        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1432,24 +1437,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_versions_get_serialize(
+        _param = self._deployments_id_put_serialize(
             id=id,
+            deployment=deployment,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ServiceModelVersion]",
+            '200': "Deployment",
+            '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1457,36 +1465,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def services_id_versions_get_with_http_info(
+    def deployments_id_put_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[ServiceModelVersion]]:
-        """Get all ServiceModelVersion records for a service
+    ) -> ApiResponse[Deployment]:
+        """Update deployment.
 
-        Return all version records
+        Update a deployment by providing an updated Deployment object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned deployment.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
+        :param deployment: Deployment Data (required)
+        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1501,24 +1512,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_versions_get_serialize(
+        _param = self._deployments_id_put_serialize(
             id=id,
+            deployment=deployment,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ServiceModelVersion]",
+            '200': "Deployment",
+            '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1526,36 +1540,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def services_id_versions_get_without_preload_content(
+    def deployments_id_put_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="Service ID")],
+        id: Annotated[StrictStr, Field(description="Deployment ID")],
+        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get all ServiceModelVersion records for a service
+        """Update deployment.
 
-        Return all version records
+        Update a deployment by providing an updated Deployment object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned deployment.
 
-        :param id: Service ID (required)
+        :param id: Deployment ID (required)
         :type id: str
+        :param deployment: Deployment Data (required)
+        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1570,37 +1587,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_id_versions_get_serialize(
+        _param = self._deployments_id_put_serialize(
             id=id,
+            deployment=deployment,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ServiceModelVersion]",
+            '200': "Deployment",
+            '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _services_id_versions_get_serialize(
+    def _deployments_id_put_serialize(
         self,
         id,
+        deployment,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1619,14 +1640,266 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if deployment is not None:
+            _body_params = deployment
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                '*/*'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='PUT',
+            resource_path='/deployments/{id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def deployments_namespaces_get(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[str]:
+        """Get all namespaces that can be selected for deployemnts.
+
+        List of namespace names.
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._deployments_namespaces_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[str]",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def deployments_namespaces_get_with_http_info(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[str]]:
+        """Get all namespaces that can be selected for deployemnts.
+
+        List of namespace names.
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._deployments_namespaces_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[str]",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def deployments_namespaces_get_without_preload_content(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Get all namespaces that can be selected for deployemnts.
+
+        List of namespace names.
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._deployments_namespaces_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[str]",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _deployments_namespaces_get_serialize(
+        self,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1636,15 +1909,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/services/{id}/versions',
+            resource_path='/deployments/namespaces',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1653,36 +1926,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def services_post(
+    def deployments_post(
         self,
-        service: Annotated[ServiceRequest, Field(description="Service Data")],
+        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Service:
-        """Create a new service description.
+    ) -> Deployment:
+        """Create a new deployment.
 
-        Provide the details of a service to be deployed.   The Service identifies the model and the resource requirements to deploy the service.   If the model is reference by name, it will automatically be translated to the ID of the latest model version.   To reference a version of the model other than the latest, specify the ID of a specific model version.
+        Create a deployment of a service onto a cluster. This object controls the deployment and encapsulates the status of that deployment.
 
-        :param service: Service Data (required)
-        :type service: ServiceRequest
+        :param deployment: Deployment Data (required)
+        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1697,24 +1970,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_post_serialize(
-            service=service,
+        _param = self._deployments_post_serialize(
+            deployment=deployment,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Service",
+            '201': "Deployment",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1723,36 +1996,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def services_post_with_http_info(
+    def deployments_post_with_http_info(
         self,
-        service: Annotated[ServiceRequest, Field(description="Service Data")],
+        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Service]:
-        """Create a new service description.
+    ) -> ApiResponse[Deployment]:
+        """Create a new deployment.
 
-        Provide the details of a service to be deployed.   The Service identifies the model and the resource requirements to deploy the service.   If the model is reference by name, it will automatically be translated to the ID of the latest model version.   To reference a version of the model other than the latest, specify the ID of a specific model version.
+        Create a deployment of a service onto a cluster. This object controls the deployment and encapsulates the status of that deployment.
 
-        :param service: Service Data (required)
-        :type service: ServiceRequest
+        :param deployment: Deployment Data (required)
+        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1767,24 +2040,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_post_serialize(
-            service=service,
+        _param = self._deployments_post_serialize(
+            deployment=deployment,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Service",
+            '201': "Deployment",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1793,36 +2066,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def services_post_without_preload_content(
+    def deployments_post_without_preload_content(
         self,
-        service: Annotated[ServiceRequest, Field(description="Service Data")],
+        deployment: Annotated[DeploymentRequest, Field(description="Deployment Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create a new service description.
+        """Create a new deployment.
 
-        Provide the details of a service to be deployed.   The Service identifies the model and the resource requirements to deploy the service.   If the model is reference by name, it will automatically be translated to the ID of the latest model version.   To reference a version of the model other than the latest, specify the ID of a specific model version.
+        Create a deployment of a service onto a cluster. This object controls the deployment and encapsulates the status of that deployment.
 
-        :param service: Service Data (required)
-        :type service: ServiceRequest
+        :param deployment: Deployment Data (required)
+        :type deployment: DeploymentRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1837,38 +2110,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._services_post_serialize(
-            service=service,
+        _param = self._deployments_post_serialize(
+            deployment=deployment,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Service",
+            '201': "Deployment",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _services_post_serialize(
+    def _deployments_post_serialize(
         self,
-        service,
+        deployment,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1885,16 +2158,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if service is not None:
-            _body_params = service
+        if deployment is not None:
+            _body_params = deployment
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1917,15 +2190,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/services',
+            resource_path='/deployments',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api/users_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/packaged_models_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -22,60 +22,62 @@
 try:
     from typing import Annotated
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictStr
 
-from typing import List
+from typing import List, Optional
 
+from aiolirest.models.deployment_model_version import DeploymentModelVersion
+from aiolirest.models.model_auth_token import ModelAuthToken
+from aiolirest.models.observability import Observability
+from aiolirest.models.packaged_model import PackagedModel
+from aiolirest.models.packaged_model_request import PackagedModelRequest
 from aiolirest.models.success_response import SuccessResponse
-from aiolirest.models.user import User
-from aiolirest.models.user_patch_request import UserPatchRequest
-from aiolirest.models.user_request import UserRequest
 
 from aiolirest.api_client import ApiClient
 from aiolirest.api_response import ApiResponse
 from aiolirest.rest import RESTResponseType
 
 
-class UsersApi:
+class PackagedModelsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def users_get(
+    def models_get(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[User]:
-        """Get configured users.
+    ) -> List[PackagedModel]:
+        """Get all models.
 
-        Get the properties of all configured users.
+        Return the properties of all configured models.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -91,24 +93,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_get_serialize(
+        _param = self._models_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[User]",
-            '400': "ErrorResponse",
+            '200': "List[PackagedModel]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -116,32 +117,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def users_get_with_http_info(
+    def models_get_with_http_info(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[User]]:
-        """Get configured users.
+    ) -> ApiResponse[List[PackagedModel]]:
+        """Get all models.
 
-        Get the properties of all configured users.
+        Return the properties of all configured models.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -157,24 +158,23 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_get_serialize(
+        _param = self._models_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[User]",
-            '400': "ErrorResponse",
+            '200': "List[PackagedModel]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -182,32 +182,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def users_get_without_preload_content(
+    def models_get_without_preload_content(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get configured users.
+        """Get all models.
 
-        Get the properties of all configured users.
+        Return the properties of all configured models.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -223,35 +223,34 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_get_serialize(
+        _param = self._models_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[User]",
-            '400': "ErrorResponse",
+            '200': "List[PackagedModel]",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _users_get_serialize(
+    def _models_get_serialize(
         self,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
@@ -286,15 +285,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/users',
+            resource_path='/models',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -303,36 +302,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def users_id_delete(
+    def models_id_delete(
         self,
-        id: Annotated[StrictInt, Field(description="User ID")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> SuccessResponse:
-        """Delete a user.
+        """Delete a model.
 
-        Delete a user specified by ID.
+        Delete a model version by ID.  To successfully delete a model version it can no longer be referenced by any services. Each model version must be deleted separately.
 
-        :param id: User ID (required)
-        :type id: int
+        :param id: PackagedModel ID (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -347,25 +346,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_delete_serialize(
+        _param = self._models_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "SuccessResponse",
-            '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -373,36 +372,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def users_id_delete_with_http_info(
+    def models_id_delete_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="User ID")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[SuccessResponse]:
-        """Delete a user.
+        """Delete a model.
 
-        Delete a user specified by ID.
+        Delete a model version by ID.  To successfully delete a model version it can no longer be referenced by any services. Each model version must be deleted separately.
 
-        :param id: User ID (required)
-        :type id: int
+        :param id: PackagedModel ID (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -417,25 +416,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_delete_serialize(
+        _param = self._models_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "SuccessResponse",
-            '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -443,36 +442,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def users_id_delete_without_preload_content(
+    def models_id_delete_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="User ID")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a user.
+        """Delete a model.
 
-        Delete a user specified by ID.
+        Delete a model version by ID.  To successfully delete a model version it can no longer be referenced by any services. Each model version must be deleted separately.
 
-        :param id: User ID (required)
-        :type id: int
+        :param id: PackagedModel ID (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -487,36 +486,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_delete_serialize(
+        _param = self._models_id_delete_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "SuccessResponse",
-            '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _users_id_delete_serialize(
+    def _models_id_delete_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -554,15 +553,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/users/{id}',
+            resource_path='/models/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -571,36 +570,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def users_id_get(
+    def models_id_get(
         self,
-        id: Annotated[StrictInt, Field(description="User ID")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[User]:
-        """Gets a user.
+    ) -> PackagedModel:
+        """Get a model.
 
-        Get the properties of the user specified by ID.
+        Return the properties of the model by ID.
 
-        :param id: User ID (required)
-        :type id: int
+        :param id: PackagedModel ID (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -615,25 +614,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_get_serialize(
+        _param = self._models_id_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[User]",
-            '400': "ErrorResponse",
+            '200': "PackagedModel",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -641,36 +640,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def users_id_get_with_http_info(
+    def models_id_get_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="User ID")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[User]]:
-        """Gets a user.
+    ) -> ApiResponse[PackagedModel]:
+        """Get a model.
 
-        Get the properties of the user specified by ID.
+        Return the properties of the model by ID.
 
-        :param id: User ID (required)
-        :type id: int
+        :param id: PackagedModel ID (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -685,25 +684,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_get_serialize(
+        _param = self._models_id_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[User]",
-            '400': "ErrorResponse",
+            '200': "PackagedModel",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -711,36 +710,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def users_id_get_without_preload_content(
+    def models_id_get_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="User ID")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Gets a user.
+        """Get a model.
 
-        Get the properties of the user specified by ID.
+        Return the properties of the model by ID.
 
-        :param id: User ID (required)
-        :type id: int
+        :param id: PackagedModel ID (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -755,36 +754,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_get_serialize(
+        _param = self._models_id_get_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[User]",
-            '400': "ErrorResponse",
+            '200': "PackagedModel",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _users_id_get_serialize(
+    def _models_id_get_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -822,15 +821,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/users/{id}',
+            resource_path='/models/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -839,39 +838,42 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def users_id_patch(
+    def models_id_observability_get(
         self,
-        id: Annotated[StrictStr, Field(description="User ID")],
-        user_patch_request: Annotated[UserPatchRequest, Field(description="yes")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        deployment: Annotated[Optional[StrictStr], Field(description="The deployment name or id to select.")] = None,
+        revision: Annotated[Optional[StrictStr], Field(description="Information about a specific nativeAppName revision of the deployment.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> User:
-        """Update user properties.
+    ) -> Observability:
+        """Packaged model observability information.
 
-        Update a user's properties. Provide a body that contains one or more of the properties: - `password` - `admin` - `active`
+        Returns configuration data that enables launching a dashboard URL that describes logs and metrics for the deployments of the packaged model. Without qualification, the most recent deployment is selected. You can limit the search to a specific deployment by specifying a deployment name or ID in the deployment query parameter.   You can limit the search to specific revision as specified by a nativeAppName value in the revision query parameter.
 
-        :param id: User ID (required)
+        :param id: PackagedModel ID (required)
         :type id: str
-        :param user_patch_request: yes (required)
-        :type user_patch_request: UserPatchRequest
+        :param deployment: The deployment name or id to select.
+        :type deployment: str
+        :param revision: Information about a specific nativeAppName revision of the deployment.
+        :type revision: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -886,26 +888,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_patch_serialize(
+        _param = self._models_id_observability_get_serialize(
             id=id,
-            user_patch_request=user_patch_request,
+            deployment=deployment,
+            revision=revision,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
-            '400': "ErrorResponse",
+            '200': "Observability",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -913,39 +916,42 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def users_id_patch_with_http_info(
+    def models_id_observability_get_with_http_info(
         self,
-        id: Annotated[StrictStr, Field(description="User ID")],
-        user_patch_request: Annotated[UserPatchRequest, Field(description="yes")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        deployment: Annotated[Optional[StrictStr], Field(description="The deployment name or id to select.")] = None,
+        revision: Annotated[Optional[StrictStr], Field(description="Information about a specific nativeAppName revision of the deployment.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[User]:
-        """Update user properties.
+    ) -> ApiResponse[Observability]:
+        """Packaged model observability information.
 
-        Update a user's properties. Provide a body that contains one or more of the properties: - `password` - `admin` - `active`
+        Returns configuration data that enables launching a dashboard URL that describes logs and metrics for the deployments of the packaged model. Without qualification, the most recent deployment is selected. You can limit the search to a specific deployment by specifying a deployment name or ID in the deployment query parameter.   You can limit the search to specific revision as specified by a nativeAppName value in the revision query parameter.
 
-        :param id: User ID (required)
+        :param id: PackagedModel ID (required)
         :type id: str
-        :param user_patch_request: yes (required)
-        :type user_patch_request: UserPatchRequest
+        :param deployment: The deployment name or id to select.
+        :type deployment: str
+        :param revision: Information about a specific nativeAppName revision of the deployment.
+        :type revision: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -960,26 +966,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_patch_serialize(
+        _param = self._models_id_observability_get_serialize(
             id=id,
-            user_patch_request=user_patch_request,
+            deployment=deployment,
+            revision=revision,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
-            '400': "ErrorResponse",
+            '200': "Observability",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -987,39 +994,42 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def users_id_patch_without_preload_content(
+    def models_id_observability_get_without_preload_content(
         self,
-        id: Annotated[StrictStr, Field(description="User ID")],
-        user_patch_request: Annotated[UserPatchRequest, Field(description="yes")],
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        deployment: Annotated[Optional[StrictStr], Field(description="The deployment name or id to select.")] = None,
+        revision: Annotated[Optional[StrictStr], Field(description="Information about a specific nativeAppName revision of the deployment.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Update user properties.
+        """Packaged model observability information.
 
-        Update a user's properties. Provide a body that contains one or more of the properties: - `password` - `admin` - `active`
+        Returns configuration data that enables launching a dashboard URL that describes logs and metrics for the deployments of the packaged model. Without qualification, the most recent deployment is selected. You can limit the search to a specific deployment by specifying a deployment name or ID in the deployment query parameter.   You can limit the search to specific revision as specified by a nativeAppName value in the revision query parameter.
 
-        :param id: User ID (required)
+        :param id: PackagedModel ID (required)
         :type id: str
-        :param user_patch_request: yes (required)
-        :type user_patch_request: UserPatchRequest
+        :param deployment: The deployment name or id to select.
+        :type deployment: str
+        :param revision: Information about a specific nativeAppName revision of the deployment.
+        :type revision: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1034,40 +1044,42 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_id_patch_serialize(
+        _param = self._models_id_observability_get_serialize(
             id=id,
-            user_patch_request=user_patch_request,
+            deployment=deployment,
+            revision=revision,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
-            '400': "ErrorResponse",
+            '200': "Observability",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _users_id_patch_serialize(
+    def _models_id_observability_get_serialize(
         self,
         id,
-        user_patch_request,
+        deployment,
+        revision,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1083,50 +1095,43 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
+        if deployment is not None:
+            
+            _query_params.append(('deployment', deployment))
+            
+        if revision is not None:
+            
+            _query_params.append(('revision', revision))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if user_patch_request is not None:
-            _body_params = user_patch_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/users/{id}',
+            method='GET',
+            resource_path='/models/{id}/observability',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1135,33 +1140,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def users_me_get(
+    def models_id_put(
         self,
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        packaged_model: Annotated[PackagedModelRequest, Field(description="PackagedModel Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> User:
-        """Get current authenticated user.
+    ) -> PackagedModel:
+        """Update a model.
 
-        Get the properties of the current user.
+        Update a model by providing an updated PackagedModel object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned PackagedModel. You may change the name or description of a deployed model.  Changing the model image or URI will create a new version of the model which will be returned. Alternatively, you can create a new version of the model using the create method.
 
+        :param id: PackagedModel ID (required)
+        :type id: str
+        :param packaged_model: PackagedModel Data (required)
+        :type packaged_model: PackagedModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1176,24 +1187,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_me_get_serialize(
+        _param = self._models_id_put_serialize(
+            id=id,
+            packaged_model=packaged_model,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
+            '200': "PackagedModel",
             '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1201,33 +1215,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def users_me_get_with_http_info(
+    def models_id_put_with_http_info(
         self,
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        packaged_model: Annotated[PackagedModelRequest, Field(description="PackagedModel Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[User]:
-        """Get current authenticated user.
+    ) -> ApiResponse[PackagedModel]:
+        """Update a model.
 
-        Get the properties of the current user.
+        Update a model by providing an updated PackagedModel object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned PackagedModel. You may change the name or description of a deployed model.  Changing the model image or URI will create a new version of the model which will be returned. Alternatively, you can create a new version of the model using the create method.
 
+        :param id: PackagedModel ID (required)
+        :type id: str
+        :param packaged_model: PackagedModel Data (required)
+        :type packaged_model: PackagedModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1242,24 +1262,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_me_get_serialize(
+        _param = self._models_id_put_serialize(
+            id=id,
+            packaged_model=packaged_model,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
+            '200': "PackagedModel",
             '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1267,33 +1290,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def users_me_get_without_preload_content(
+    def models_id_put_without_preload_content(
         self,
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        packaged_model: Annotated[PackagedModelRequest, Field(description="PackagedModel Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get current authenticated user.
+        """Update a model.
 
-        Get the properties of the current user.
+        Update a model by providing an updated PackagedModel object.  This is normally obtained by a prior get operation, and then selectively modifying properties of the returned PackagedModel. You may change the name or description of a deployed model.  Changing the model image or URI will create a new version of the model which will be returned. Alternatively, you can create a new version of the model using the create method.
 
+        :param id: PackagedModel ID (required)
+        :type id: str
+        :param packaged_model: PackagedModel Data (required)
+        :type packaged_model: PackagedModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1308,36 +1337,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_me_get_serialize(
+        _param = self._models_id_put_serialize(
+            id=id,
+            packaged_model=packaged_model,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
+            '200': "PackagedModel",
             '400': "ErrorResponse",
+            '404': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _users_me_get_serialize(
+    def _models_id_put_serialize(
         self,
+        id,
+        packaged_model,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1350,14 +1384,283 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if packaged_model is not None:
+            _body_params = packaged_model
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                '*/*'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='PUT',
+            resource_path='/models/{id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def models_id_token_get(
+        self,
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ModelAuthToken:
+        """Generate and return an auth token for the packaged model.
+
+        When the model is deployed with `authorizationRequired=true`, the returned token enables authenticated access to the deployed inference service API.
+
+        :param id: PackagedModel ID (required)
+        :type id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._models_id_token_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ModelAuthToken",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def models_id_token_get_with_http_info(
+        self,
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ModelAuthToken]:
+        """Generate and return an auth token for the packaged model.
+
+        When the model is deployed with `authorizationRequired=true`, the returned token enables authenticated access to the deployed inference service API.
+
+        :param id: PackagedModel ID (required)
+        :type id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._models_id_token_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ModelAuthToken",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def models_id_token_get_without_preload_content(
+        self,
+        id: Annotated[StrictStr, Field(description="PackagedModel ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Generate and return an auth token for the packaged model.
+
+        When the model is deployed with `authorizationRequired=true`, the returned token enables authenticated access to the deployed inference service API.
+
+        :param id: PackagedModel ID (required)
+        :type id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._models_id_token_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ModelAuthToken",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _models_id_token_get_serialize(
+        self,
+        id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1371,15 +1674,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/users/me',
+            resource_path='/models/{id}/token',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1388,36 +1691,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def users_post(
+    def models_post(
         self,
-        user: Annotated[UserRequest, Field(description="User Data")],
+        packaged_model: Annotated[PackagedModelRequest, Field(description="PackagedModel Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> SuccessResponse:
-        """Create a new user.
+    ) -> PackagedModel:
+        """Create a new packaged model.
 
-        Create a new user.  This method is enabled only for administrator users.
+        Provide the details of the model and code to be deployed, and the resources required. A packaged model can be served in a number of formats: * A containerized Bento provided as an image * An openllm model directly downloaded * An s3 bucket hosting a bento, an openllm model, or nim model For models that are downloaded, an appropriate registry should be referenced to provide configuration and access information for the S3 or Huggingface.co,  Multiple versions of the same model name are expected.   When created, a new version/id is assigned to model.  Once deployed, the model/code referenced by the packaged model should be treated as immutable. Rolling out a new version of a packaged model should be accomplished using a new S3 path, or image. 
 
-        :param user: User Data (required)
-        :type user: UserRequest
+        :param packaged_model: PackagedModel Data (required)
+        :type packaged_model: PackagedModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1432,24 +1735,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_post_serialize(
-            user=user,
+        _param = self._models_post_serialize(
+            packaged_model=packaged_model,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "SuccessResponse",
+            '201': "PackagedModel",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1458,36 +1761,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def users_post_with_http_info(
+    def models_post_with_http_info(
         self,
-        user: Annotated[UserRequest, Field(description="User Data")],
+        packaged_model: Annotated[PackagedModelRequest, Field(description="PackagedModel Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[SuccessResponse]:
-        """Create a new user.
+    ) -> ApiResponse[PackagedModel]:
+        """Create a new packaged model.
 
-        Create a new user.  This method is enabled only for administrator users.
+        Provide the details of the model and code to be deployed, and the resources required. A packaged model can be served in a number of formats: * A containerized Bento provided as an image * An openllm model directly downloaded * An s3 bucket hosting a bento, an openllm model, or nim model For models that are downloaded, an appropriate registry should be referenced to provide configuration and access information for the S3 or Huggingface.co,  Multiple versions of the same model name are expected.   When created, a new version/id is assigned to model.  Once deployed, the model/code referenced by the packaged model should be treated as immutable. Rolling out a new version of a packaged model should be accomplished using a new S3 path, or image. 
 
-        :param user: User Data (required)
-        :type user: UserRequest
+        :param packaged_model: PackagedModel Data (required)
+        :type packaged_model: PackagedModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1502,24 +1805,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_post_serialize(
-            user=user,
+        _param = self._models_post_serialize(
+            packaged_model=packaged_model,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "SuccessResponse",
+            '201': "PackagedModel",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -1528,36 +1831,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def users_post_without_preload_content(
+    def models_post_without_preload_content(
         self,
-        user: Annotated[UserRequest, Field(description="User Data")],
+        packaged_model: Annotated[PackagedModelRequest, Field(description="PackagedModel Data")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create a new user.
+        """Create a new packaged model.
 
-        Create a new user.  This method is enabled only for administrator users.
+        Provide the details of the model and code to be deployed, and the resources required. A packaged model can be served in a number of formats: * A containerized Bento provided as an image * An openllm model directly downloaded * An s3 bucket hosting a bento, an openllm model, or nim model For models that are downloaded, an appropriate registry should be referenced to provide configuration and access information for the S3 or Huggingface.co,  Multiple versions of the same model name are expected.   When created, a new version/id is assigned to model.  Once deployed, the model/code referenced by the packaged model should be treated as immutable. Rolling out a new version of a packaged model should be accomplished using a new S3 path, or image. 
 
-        :param user: User Data (required)
-        :type user: UserRequest
+        :param packaged_model: PackagedModel Data (required)
+        :type packaged_model: PackagedModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1572,38 +1875,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._users_post_serialize(
-            user=user,
+        _param = self._models_post_serialize(
+            packaged_model=packaged_model,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "SuccessResponse",
+            '201': "PackagedModel",
             '400': "ErrorResponse",
             '500': "ErrorResponse"
             
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _users_post_serialize(
+    def _models_post_serialize(
         self,
-        user,
+        packaged_model,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1620,16 +1923,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if user is not None:
-            _body_params = user
+        if packaged_model is not None:
+            _body_params = packaged_model
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 '*/*'
             ]
@@ -1652,15 +1955,299 @@
         # authentication setting
         _auth_settings: List[str] = [
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/users',
+            resource_path='/models',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def models_versions_get(
+        self,
+        model: Annotated[Optional[StrictStr], Field(description="PackagedModel ID or Name")] = None,
+        version: Annotated[Optional[StrictStr], Field(description="Version number of the packaged model")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[DeploymentModelVersion]:
+        """Get all DeploymentModelVersion records for a packaged model.
+
+        Query all deployed version records based upon packaged model name or id, and version.   If a model name is specified, all versions of the name are returned regardless of id.
+
+        :param model: PackagedModel ID or Name
+        :type model: str
+        :param version: Version number of the packaged model
+        :type version: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._models_versions_get_serialize(
+            model=model,
+            version=version,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[DeploymentModelVersion]",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def models_versions_get_with_http_info(
+        self,
+        model: Annotated[Optional[StrictStr], Field(description="PackagedModel ID or Name")] = None,
+        version: Annotated[Optional[StrictStr], Field(description="Version number of the packaged model")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[DeploymentModelVersion]]:
+        """Get all DeploymentModelVersion records for a packaged model.
+
+        Query all deployed version records based upon packaged model name or id, and version.   If a model name is specified, all versions of the name are returned regardless of id.
+
+        :param model: PackagedModel ID or Name
+        :type model: str
+        :param version: Version number of the packaged model
+        :type version: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._models_versions_get_serialize(
+            model=model,
+            version=version,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[DeploymentModelVersion]",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def models_versions_get_without_preload_content(
+        self,
+        model: Annotated[Optional[StrictStr], Field(description="PackagedModel ID or Name")] = None,
+        version: Annotated[Optional[StrictStr], Field(description="Version number of the packaged model")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Get all DeploymentModelVersion records for a packaged model.
+
+        Query all deployed version records based upon packaged model name or id, and version.   If a model name is specified, all versions of the name are returned regardless of id.
+
+        :param model: PackagedModel ID or Name
+        :type model: str
+        :param version: Version number of the packaged model
+        :type version: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._models_versions_get_serialize(
+            model=model,
+            version=version,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[DeploymentModelVersion]",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _models_versions_get_serialize(
+        self,
+        model,
+        version,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if model is not None:
+            
+            _query_params.append(('model', model))
+            
+        if version is not None:
+            
+            _query_params.append(('version', version))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                '*/*'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/models/versions',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api_client.py` & `aioli-sdk-0.2.0rc0/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/api_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/configuration.py` & `aioli-sdk-0.2.0rc0/aiolirest/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1\n"\
+               "Version of the API: 0.2.0-rc0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/exceptions.py` & `aioli-sdk-0.2.0rc0/aiolirest/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/__init__.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 # coding: utf-8
 
 # flake8: noqa
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
+from aiolirest.models.auto_scaling_template import AutoScalingTemplate
 from aiolirest.models.autoscaling import Autoscaling
 from aiolirest.models.configuration_resources import ConfigurationResources
 from aiolirest.models.deployment import Deployment
+from aiolirest.models.deployment_model_version import DeploymentModelVersion
 from aiolirest.models.deployment_request import DeploymentRequest
 from aiolirest.models.deployment_state import DeploymentState
 from aiolirest.models.error_response import ErrorResponse
+from aiolirest.models.event_info import EventInfo
 from aiolirest.models.failure_info import FailureInfo
 from aiolirest.models.login_request import LoginRequest
 from aiolirest.models.login_response import LoginResponse
+from aiolirest.models.model_auth_token import ModelAuthToken
+from aiolirest.models.observability import Observability
+from aiolirest.models.packaged_model import PackagedModel
+from aiolirest.models.packaged_model_request import PackagedModelRequest
 from aiolirest.models.resource_profile import ResourceProfile
+from aiolirest.models.resources_template import ResourcesTemplate
 from aiolirest.models.role import Role
 from aiolirest.models.role_assignment import RoleAssignment
 from aiolirest.models.role_assignments import RoleAssignments
 from aiolirest.models.security import Security
-from aiolirest.models.service import Service
-from aiolirest.models.service_auth_token import ServiceAuthToken
-from aiolirest.models.service_model_version import ServiceModelVersion
-from aiolirest.models.service_request import ServiceRequest
 from aiolirest.models.success_response import SuccessResponse
-from aiolirest.models.trained_model import TrainedModel
 from aiolirest.models.trained_model_registry import TrainedModelRegistry
 from aiolirest.models.trained_model_registry_request import TrainedModelRegistryRequest
-from aiolirest.models.trained_model_request import TrainedModelRequest
 from aiolirest.models.user import User
 from aiolirest.models.user_patch_request import UserPatchRequest
 from aiolirest.models.user_request import UserRequest
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/autoscaling.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/autoscaling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/configuration_resources.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/configuration_resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 class ConfigurationResources(BaseModel):
     """
     ConfigurationResources models a configuration's resource requirements.
     """ # noqa: E501
-    gpu_type: Optional[StrictStr] = Field(default=None, description="GPU type required.", alias="gpuType")
+    gpu_type: Optional[StrictStr] = Field(default=None, description="An optional GPU type required by this service (e.g. nvidia-tesla-a100).  If unspecified, any GPU available will be used.  Your cluster administrator should provide the list of GPU types that can be specified on your cluster.", alias="gpuType")
     limits: Optional[ResourceProfile] = None
     requests: Optional[ResourceProfile] = None
     __properties: ClassVar[List[str]] = ["gpuType", "limits", "requests"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/deployment.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/deployment_state.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,56 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr, field_validator
+from pydantic import BaseModel, StrictInt, StrictStr, field_validator
 from pydantic import Field
-from aiolirest.models.deployment_state import DeploymentState
-from aiolirest.models.security import Security
+from aiolirest.models.failure_info import FailureInfo
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Deployment(BaseModel):
+class DeploymentState(BaseModel):
     """
-    Deployment describes the deployment of a service.
+    Describes the current state of the deployment as managed by KServe
     """ # noqa: E501
-    cluster_name: Optional[StrictStr] = Field(default=None, description="Name of the cluster.", alias="clusterName")
-    id: Optional[StrictStr] = Field(default=None, description="The ID of the deployment. This is a read-only property and is automatically assigned on creation.")
-    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the deployment. This is a read-only field and is automatically updated.", alias="modifiedAt")
-    name: StrictStr = Field(description="The deployment name.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
-    namespace: Optional[StrictStr] = Field(default=None, description="The Kubernetes namespace to be used for the deployment.")
-    secondary_state: Optional[DeploymentState] = Field(default=None, alias="secondaryState")
-    security: Optional[Security] = None
-    service: StrictStr = Field(description="Service name or ID to be deployed.")
-    state: Optional[DeploymentState] = None
-    status: Optional[StrictStr] = Field(default=None, description="Summary status of the deployed service. * Deploying - Service configuration is in progress. * Failed - The service configuration failed. * Ready - The service has been successfully configured and is serving. * Updating - A new service revision is being rolledout. * UpdateFailed - The current service revision failed to rollout due to an error.   The prior version is still serving requests. * Deleting - The deployed service is being removed. * Unknown - Unable to determined the status. This is a read-only property.")
-    __properties: ClassVar[List[str]] = ["clusterName", "id", "modifiedAt", "name", "namespace", "secondaryState", "security", "service", "state", "status"]
+    endpoint: Optional[StrictStr] = Field(default=None, description="Endpoint to access inference service.")
+    failure_info: Optional[List[FailureInfo]] = Field(default=None, description="List of any failures that have occurred.", alias="failureInfo")
+    native_app_name: Optional[StrictStr] = Field(default=None, description="The name of the Kubernetes application for the specific service version. Use this name to match the app value in Grafana/Prometheus to obtain logs and metrics for this deployed service version.", alias="nativeAppName")
+    status: Optional[StrictStr] = Field(default=None, description="Status of a particular service revision. * `Deploying` - Service configuration is in progress. * `Failed` - The service configuration failed. * `Ready` - The service has been successfully configured and is serving. * `Updating` - A new service revision is being rolledout. * `UpdateFailed` - The current service revision failed to rollout due to an error.   The prior version is still serving requests. * `Deleting` - The deployed service is being removed. * `Paused` - The deployed service has been stopped by the user or an external action. * `Unknown` - Unable to determined the status.  This is a read-only property.")
+    traffic_percentage: Optional[StrictInt] = Field(default=None, description="Target percentage of traffic intended for this service version when successfully deployed.", alias="trafficPercentage")
+    __properties: ClassVar[List[str]] = ["endpoint", "failureInfo", "nativeAppName", "status", "trafficPercentage"]
 
     @field_validator('status')
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('Deploying', 'Ready', 'Updating', 'UpdateFailed', 'Failed', 'Deleting', 'Unknown'):
-            raise ValueError("must be one of enum values ('Deploying', 'Ready', 'Updating', 'UpdateFailed', 'Failed', 'Deleting', 'Unknown')")
+        if value not in ('Deploying', 'Ready', 'Updating', 'UpdateFailed', 'Failed', 'Deleting', 'None', 'Unknown'):
+            raise ValueError("must be one of enum values ('Deploying', 'Ready', 'Updating', 'UpdateFailed', 'Failed', 'Deleting', 'None', 'Unknown')")
         return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
@@ -68,15 +62,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Deployment from a JSON string"""
+        """Create an instance of DeploymentState from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -87,42 +81,35 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of secondary_state
-        if self.secondary_state:
-            _dict['secondaryState'] = self.secondary_state.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of security
-        if self.security:
-            _dict['security'] = self.security.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of state
-        if self.state:
-            _dict['state'] = self.state.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in failure_info (list)
+        _items = []
+        if self.failure_info:
+            for _item in self.failure_info:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['failureInfo'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of Deployment from a dict"""
+        """Create an instance of DeploymentState from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "clusterName": obj.get("clusterName"),
-            "id": obj.get("id"),
-            "modifiedAt": obj.get("modifiedAt"),
-            "name": obj.get("name"),
-            "namespace": obj.get("namespace"),
-            "secondaryState": DeploymentState.from_dict(obj.get("secondaryState")) if obj.get("secondaryState") is not None else None,
-            "security": Security.from_dict(obj.get("security")) if obj.get("security") is not None else None,
-            "service": obj.get("service"),
-            "state": DeploymentState.from_dict(obj.get("state")) if obj.get("state") is not None else None,
-            "status": obj.get("status")
+            "endpoint": obj.get("endpoint"),
+            "failureInfo": [FailureInfo.from_dict(_item) for _item in obj.get("failureInfo")] if obj.get("failureInfo") is not None else None,
+            "nativeAppName": obj.get("nativeAppName"),
+            "status": obj.get("status"),
+            "trafficPercentage": obj.get("trafficPercentage")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/deployment_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/role.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
-from aiolirest.models.security import Security
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class DeploymentRequest(BaseModel):
+class Role(BaseModel):
     """
-    Deployment describes the deployment of a service.
+    Role describes defined role.
     """ # noqa: E501
-    name: StrictStr = Field(description="The deployment name.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
-    namespace: Optional[StrictStr] = Field(default=None, description="The Kubernetes namespace to be used for the deployment.")
-    security: Optional[Security] = None
-    service: StrictStr = Field(description="Service name or ID to be deployed.")
-    __properties: ClassVar[List[str]] = ["name", "namespace", "security", "service"]
+    id: Optional[StrictInt] = Field(default=None, description="Role ID.")
+    role_name: Optional[StrictStr] = Field(default=None, description="Role Name.", alias="roleName")
+    __properties: ClassVar[List[str]] = ["id", "roleName"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -51,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of DeploymentRequest from a JSON string"""
+        """Create an instance of Role from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,30 +67,25 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of security
-        if self.security:
-            _dict['security'] = self.security.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of DeploymentRequest from a dict"""
+        """Create an instance of Role from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "namespace": obj.get("namespace"),
-            "security": Security.from_dict(obj.get("security")) if obj.get("security") is not None else None,
-            "service": obj.get("service")
+            "id": obj.get("id"),
+            "roleName": obj.get("roleName")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/deployment_state.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/trained_model_registry_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, StrictStr, field_validator
 from pydantic import Field
-from aiolirest.models.failure_info import FailureInfo
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class DeploymentState(BaseModel):
+class TrainedModelRegistryRequest(BaseModel):
     """
-    Describes the current state of the deployment as managed by KServe
+    Provides the metadata that describes how to access a named model registry to enable download of a trained model for deployment.
     """ # noqa: E501
-    endpoint: Optional[StrictStr] = Field(default=None, description="Endpoint to access inference service.")
-    failure_info: Optional[List[FailureInfo]] = Field(default=None, description="List of any failures that have occurred.", alias="failureInfo")
-    native_app_name: Optional[StrictStr] = Field(default=None, description="The name of the Kubernetes application for the specific service version. Use this name to match the app value in Grafana/Prometheus to obtain logs and metrics for this deployed service version.", alias="nativeAppName")
-    status: Optional[StrictStr] = Field(default=None, description="Status of a particular service revision. * None - Nothing deployed. * Deploying - Service configuration is in progress. * Failed - The service configuration failed. * Ready - The service has been successfully configured and is serving. * Updating - A new service revision is being rolledout. * UpdateFailed - The current service revision failed to rollout due to an error.   The prior version is still serving requests. * Deleting - The deployed service is being removed. * Unknown - Unable to determined the status. This is a read-only property.")
-    traffic_percentage: Optional[StrictInt] = Field(default=None, description="Target percentage of traffic intended for this service version when successfully deployed.", alias="trafficPercentage")
-    __properties: ClassVar[List[str]] = ["endpoint", "failureInfo", "nativeAppName", "status", "trafficPercentage"]
+    access_key: Optional[StrictStr] = Field(default=None, description="For an `s3` registry, the value is the access key/username.", alias="accessKey")
+    bucket: Optional[StrictStr] = Field(default=None, description="For an `s3` registry, the value is the S3 bucket name.")
+    endpoint_url: Optional[StrictStr] = Field(default=None, description="For an `s3` registry, the S3 registry endpoint.", alias="endpointUrl")
+    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the registry. This is a read-only field and is automatically updated.", alias="modifiedAt")
+    name: StrictStr = Field(description="The name of the registry.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
+    secret_key: StrictStr = Field(description="The secret key is the password, secret key, or access token for the registry.  * For an `s3` registry, the `secretKey` provides a secret key for the S3 bucket. * For an `openllm` registry, the`secretKey` is the access token for huggingface.co and is supplied to the launched container via the `HF_TOKEN`  environment variable.bucket.", alias="secretKey")
+    type: StrictStr = Field(description="The type of this model registry. * `s3` - Configuration to enable access to an s3 bucket. * `openllm` - Configuration to enable direct download of openllm models from huggingface.co.   Provide your access token in the `secretKey` field. * `ngc` - Not yet supported. Configuration to enable direct download from the NGC: AI Development Catalog. * `http` - Not yet supported.  Configuration to enable model download from a protected http endpoint that requires login.")
+    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "modifiedAt", "name", "secretKey", "type"]
 
-    @field_validator('status')
-    def status_validate_enum(cls, value):
+    @field_validator('type')
+    def type_validate_enum(cls, value):
         """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('Deploying', 'Ready', 'Updating', 'UpdateFailed', 'Failed', 'Deleting', 'None', 'Unknown'):
-            raise ValueError("must be one of enum values ('Deploying', 'Ready', 'Updating', 'UpdateFailed', 'Failed', 'Deleting', 'None', 'Unknown')")
+        if value not in ('s3', 'openllm', 'ngc', 'http'):
+            raise ValueError("must be one of enum values ('s3', 'openllm', 'ngc', 'http')")
         return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
@@ -62,15 +60,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of DeploymentState from a JSON string"""
+        """Create an instance of TrainedModelRegistryRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -81,35 +79,30 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in failure_info (list)
-        _items = []
-        if self.failure_info:
-            for _item in self.failure_info:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['failureInfo'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of DeploymentState from a dict"""
+        """Create an instance of TrainedModelRegistryRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "endpoint": obj.get("endpoint"),
-            "failureInfo": [FailureInfo.from_dict(_item) for _item in obj.get("failureInfo")] if obj.get("failureInfo") is not None else None,
-            "nativeAppName": obj.get("nativeAppName"),
-            "status": obj.get("status"),
-            "trafficPercentage": obj.get("trafficPercentage")
+            "accessKey": obj.get("accessKey"),
+            "bucket": obj.get("bucket"),
+            "endpointUrl": obj.get("endpointUrl"),
+            "modifiedAt": obj.get("modifiedAt"),
+            "name": obj.get("name"),
+            "secretKey": obj.get("secretKey"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/error_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/error_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/failure_info.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/failure_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 class FailureInfo(BaseModel):
     """
     FailureInfo
     """ # noqa: E501
-    failure_type: Optional[StrictStr] = Field(default=None, description="And identifier of the type of the failure. * ModelLoadFailed - The model failed to load within a ServingRuntime container. * RevisionFailed - The newly deployed service revision failed.", alias="failureType")
+    failure_type: Optional[StrictStr] = Field(default=None, description="An identifier of the type of the failure.  Some example failure types: * `ModelLoadFailed` - The model failed to load within a ServingRuntime container. * `RevisionFailed` - The newly deployed service revision failed. * `ServiceMissing`- The created inference service was manually deleted by an external actor.", alias="failureType")
     message: Optional[StrictStr] = Field(default=None, description="The error messages describing the failure.")
     time: Optional[StrictStr] = Field(default=None, description="The time at which the failure occurred.")
     __properties: ClassVar[List[str]] = ["failureType", "message", "time"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/login_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/login_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/login_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/success_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,25 +17,26 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictStr
+from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class LoginResponse(BaseModel):
+class SuccessResponse(BaseModel):
     """
-    LoginResponse
+    A successful response with a message.
     """ # noqa: E501
-    token: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["token"]
+    message: Optional[StrictStr] = Field(default=None, description="Response message.")
+    __properties: ClassVar[List[str]] = ["message"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -46,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of LoginResponse from a JSON string"""
+        """Create an instance of SuccessResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,20 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of LoginResponse from a dict"""
+        """Create an instance of SuccessResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "token": obj.get("token")
+            "message": obj.get("message")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/resource_profile.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/resource_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/role.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/role_assignment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, StrictStr, field_validator
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Role(BaseModel):
+class RoleAssignment(BaseModel):
     """
-    Role describes defined role.
+    RoleAssignment describes a user-role assignment.
     """ # noqa: E501
-    id: Optional[StrictInt] = Field(default=None, description="Role ID.")
-    role_name: Optional[StrictStr] = Field(default=None, description="Role Name.", alias="roleName")
-    __properties: ClassVar[List[str]] = ["id", "roleName"]
+    role_name: StrictStr = Field(description="Role Name.", alias="roleName")
+    user_name: StrictStr = Field(description="User Name.", alias="userName")
+    __properties: ClassVar[List[str]] = ["roleName", "userName"]
+
+    @field_validator('role_name')
+    def role_name_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('Admin', 'Viewer', 'Maintainer', 'Robot'):
+            raise ValueError("must be one of enum values ('Admin', 'Viewer', 'Maintainer', 'Robot')")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -48,15 +55,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Role from a JSON string"""
+        """Create an instance of RoleAssignment from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +78,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of Role from a dict"""
+        """Create an instance of RoleAssignment from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "roleName": obj.get("roleName")
+            "roleName": obj.get("roleName"),
+            "userName": obj.get("userName")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/role_assignment.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/model_auth_token.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, StrictStr
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class RoleAssignment(BaseModel):
+class ModelAuthToken(BaseModel):
     """
-    RoleAssignment describes a user-role assignment.
+    An authenication token to access the service.
     """ # noqa: E501
-    role_name: StrictStr = Field(description="Role Name.", alias="roleName")
-    user_name: StrictStr = Field(description="User Name.", alias="userName")
-    __properties: ClassVar[List[str]] = ["roleName", "userName"]
-
-    @field_validator('role_name')
-    def role_name_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in ('Admin', 'Viewer', 'Maintainer', 'Robot'):
-            raise ValueError("must be one of enum values ('Admin', 'Viewer', 'Maintainer', 'Robot')")
-        return value
+    token: Optional[StrictStr] = Field(default=None, description="A JWT authentication token string required to access the deployed service. It is specified in an `Authentication` header with the prefix `Bearer ` when making calls to the inference endpoint.")
+    __properties: ClassVar[List[str]] = ["token"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -55,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of RoleAssignment from a JSON string"""
+        """Create an instance of ModelAuthToken from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,21 +70,20 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of RoleAssignment from a dict"""
+        """Create an instance of ModelAuthToken from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "roleName": obj.get("roleName"),
-            "userName": obj.get("userName")
+            "token": obj.get("token")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/role_assignments.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/role_assignments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/security.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/security.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/service.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/packaged_model_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictStr, field_validator
 from pydantic import Field
-from aiolirest.models.autoscaling import Autoscaling
 from aiolirest.models.configuration_resources import ConfigurationResources
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Service(BaseModel):
+class PackagedModelRequest(BaseModel):
     """
-    Describes the configuration of a service including model version to be deployed, the resources required by the model, and any auto-scaling parameters. It is deployed onto a Kubernetes cluster via a Deployment object.
+    The PackagedModel describes a specific model that can be loaded. It optionally references a model registry to provide authorization, and other details.
     """ # noqa: E501
     arguments: Optional[List[StrictStr]] = Field(default=None, description="Arguments to be added to the service command line")
-    auto_scaling: Optional[Autoscaling] = Field(default=None, alias="autoScaling")
-    canary_traffic_percent: Optional[StrictInt] = Field(default=None, description="Percent traffic to pass to new model version", alias="canaryTrafficPercent")
-    description: Optional[StrictStr] = Field(default=None, description="Description of the service.")
+    description: Optional[StrictStr] = Field(default=None, description="A description of the model.")
     environment: Optional[Dict[str, StrictStr]] = Field(default=None, description="Environment variables added to the service")
-    id: Optional[StrictStr] = Field(default=None, description="The ID of the service. This is a read-only field and is automatically assigned on creation.")
-    model: StrictStr = Field(description="Model (name or ID) to be deployed.")
-    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the service. This is a read-only field and is automatically updated.", alias="modifiedAt")
-    name: StrictStr = Field(description="The service name.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
+    image: Optional[StrictStr] = Field(default=None, description="Docker container image servicing the model.")
+    format: Optional[StrictStr] = Field(default='custom', description="Model format for downloaded models (e.g. from s3, http, etc.) * `custom` - The packaged model is provided in a container image. * `bento-archive` - The packaged model is a bento archive file (.bento).  It will be downloaded,  expanded, and then  will be served using the `bentolm serve` command in a provided bentoml serving container. * `openllm` - The packaged model will be served using the `openllm serve` command in a  provided openllm serving container. * `nim` - The packaged model will be servied using an Nvidia NIM microservices container.", alias="modelFormat")
+    name: StrictStr = Field(description="The name of the model. Must consist of alphanumeric characters, '-', or '.', and must start and end with an alphanumeric character. The length of the model name must be 63 characters or less.")
+    registry: Optional[StrictStr] = Field(default=None, description="The name or ID of the model registry.")
     resources: Optional[ConfigurationResources] = None
-    __properties: ClassVar[List[str]] = ["arguments", "autoScaling", "canaryTrafficPercent", "description", "environment", "id", "model", "modifiedAt", "name", "resources"]
+    url: Optional[StrictStr] = Field(default=None, description="Reference to the bento or model to be served.  Supported schemes are: * `openllm://` - An openllm model name from huggingface.co dynamically loaded and executed with a VLLM backend. * `s3://` - An openllm model path which will be dynamically downloaded from an associated s3  registry bucket and executed with a VLLM backend.")
+    __properties: ClassVar[List[str]] = ["arguments", "description", "environment", "image", "modelFormat", "name", "registry", "resources", "url"]
+
+    @field_validator('format')
+    def format_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('bento-archive', 'openllm', 'nim', 'custom'):
+            raise ValueError("must be one of enum values ('bento-archive', 'openllm', 'nim', 'custom')")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -58,15 +66,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Service from a JSON string"""
+        """Create an instance of PackagedModelRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,39 +85,35 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of auto_scaling
-        if self.auto_scaling:
-            _dict['autoScaling'] = self.auto_scaling.to_dict()
         # override the default output from pydantic by calling `to_dict()` of resources
         if self.resources:
             _dict['resources'] = self.resources.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of Service from a dict"""
+        """Create an instance of PackagedModelRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "arguments": obj.get("arguments"),
-            "autoScaling": Autoscaling.from_dict(obj.get("autoScaling")) if obj.get("autoScaling") is not None else None,
-            "canaryTrafficPercent": obj.get("canaryTrafficPercent"),
             "description": obj.get("description"),
             "environment": obj.get("environment"),
-            "id": obj.get("id"),
-            "model": obj.get("model"),
-            "modifiedAt": obj.get("modifiedAt"),
+            "image": obj.get("image"),
+            "modelFormat": obj.get("modelFormat") if obj.get("modelFormat") is not None else 'custom',
             "name": obj.get("name"),
-            "resources": ConfigurationResources.from_dict(obj.get("resources")) if obj.get("resources") is not None else None
+            "registry": obj.get("registry"),
+            "resources": ConfigurationResources.from_dict(obj.get("resources")) if obj.get("resources") is not None else None,
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/service_auth_token.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/login_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,25 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictStr
-from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ServiceAuthToken(BaseModel):
+class LoginResponse(BaseModel):
     """
-    An authenication token to access the service.
+    LoginResponse
     """ # noqa: E501
-    token: Optional[StrictStr] = Field(default=None, description="A JWT authentication token string required to access the deployed service. It is specified in an `Authentication` header with the prefix `Bearer ` when making calls to the inference endpoint.")
+    token: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["token"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
@@ -47,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ServiceAuthToken from a JSON string"""
+        """Create an instance of LoginResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +69,15 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ServiceAuthToken from a dict"""
+        """Create an instance of LoginResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/service_model_version.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/deployment_model_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -23,26 +23,27 @@
 from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ServiceModelVersion(BaseModel):
+class DeploymentModelVersion(BaseModel):
     """
-    The ServiceModelVersion provides the model evolution data that track model deployment changes over time.
+    The DeploymentModelVersion provides model evolution data that track model deployment changes over time.
     """ # noqa: E501
     canary_traffic_percent: Optional[StrictInt] = Field(default=None, description="Percent traffic to pass to the model.", alias="canaryTrafficPercent")
     deployed: Optional[StrictStr] = Field(default=None, description="The deployment time. This is a read-only field and is automatically assigned on creation.")
+    deployment_id: Optional[StrictStr] = Field(default=None, description="The deployment ID", alias="deploymentId")
+    deployment_name: Optional[StrictStr] = Field(default=None, description="The deployment name", alias="deploymentName")
     model: Optional[StrictStr] = Field(default=None, description="The name of the model.")
     mdl_id: Optional[StrictStr] = Field(default=None, description="The ID of the model.", alias="modelID")
     mdl_version: Optional[StrictStr] = Field(default=None, description="The version of the model.", alias="modelVersion")
     native_app_name: Optional[StrictStr] = Field(default=None, description="The name of the Kubernetes application for the specific service version. Use this name to match the app value in Grafana/Prometheus to obtain logs and metrics for this deployed service version.", alias="nativeAppName")
-    service: Optional[StrictStr] = Field(default=None, description="The ID of the service.")
-    __properties: ClassVar[List[str]] = ["canaryTrafficPercent", "deployed", "model", "modelID", "modelVersion", "nativeAppName", "service"]
+    __properties: ClassVar[List[str]] = ["canaryTrafficPercent", "deployed", "deploymentId", "deploymentName", "model", "modelID", "modelVersion", "nativeAppName"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ServiceModelVersion from a JSON string"""
+        """Create an instance of DeploymentModelVersion from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -76,26 +77,27 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ServiceModelVersion from a dict"""
+        """Create an instance of DeploymentModelVersion from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "canaryTrafficPercent": obj.get("canaryTrafficPercent"),
             "deployed": obj.get("deployed"),
+            "deploymentId": obj.get("deploymentId"),
+            "deploymentName": obj.get("deploymentName"),
             "model": obj.get("model"),
             "modelID": obj.get("modelID"),
             "modelVersion": obj.get("modelVersion"),
-            "nativeAppName": obj.get("nativeAppName"),
-            "service": obj.get("service")
+            "nativeAppName": obj.get("nativeAppName")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/service_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/deployment_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,33 +19,34 @@
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
 from aiolirest.models.autoscaling import Autoscaling
-from aiolirest.models.configuration_resources import ConfigurationResources
+from aiolirest.models.security import Security
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ServiceRequest(BaseModel):
+class DeploymentRequest(BaseModel):
     """
-    Describes the configuration of a service including model version to be deployed, the resources required by the model, and any auto-scaling parameters. It is deployed onto a Kubernetes cluster via a Deployment object.
+    Deployment describes the deployment of a service.
     """ # noqa: E501
     arguments: Optional[List[StrictStr]] = Field(default=None, description="Arguments to be added to the service command line")
     auto_scaling: Optional[Autoscaling] = Field(default=None, alias="autoScaling")
     canary_traffic_percent: Optional[StrictInt] = Field(default=None, description="Percent traffic to pass to new model version", alias="canaryTrafficPercent")
-    description: Optional[StrictStr] = Field(default=None, description="Description of the service.")
     environment: Optional[Dict[str, StrictStr]] = Field(default=None, description="Environment variables added to the service")
-    model: StrictStr = Field(description="Model (name or ID) to be deployed.")
-    name: StrictStr = Field(description="The service name.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
-    resources: Optional[ConfigurationResources] = None
-    __properties: ClassVar[List[str]] = ["arguments", "autoScaling", "canaryTrafficPercent", "description", "environment", "model", "name", "resources"]
+    goal_status: Optional[StrictStr] = Field(default='Ready', description="Specifies the intended status to be achieved by the deployment.  Supported values are: * `Ready` - The inference serivce will be deployed to enable inference calls. * `Paused` - The inference serivce will be stopped and no longer accept calls.  The default is `Ready`.", alias="goalStatus")
+    model: StrictStr = Field(description="PackagedModel name or ID to be deployed.")
+    name: StrictStr = Field(description="The deployment name.  It must be a valid subdomain name and consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character.")
+    namespace: Optional[StrictStr] = Field(default=None, description="The Kubernetes namespace to be used for the deployment.")
+    security: Optional[Security] = None
+    __properties: ClassVar[List[str]] = ["arguments", "autoScaling", "canaryTrafficPercent", "environment", "goalStatus", "model", "name", "namespace", "security"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -56,15 +57,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ServiceRequest from a JSON string"""
+        """Create an instance of DeploymentRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,34 +79,35 @@
             exclude={
             },
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of auto_scaling
         if self.auto_scaling:
             _dict['autoScaling'] = self.auto_scaling.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of resources
-        if self.resources:
-            _dict['resources'] = self.resources.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of security
+        if self.security:
+            _dict['security'] = self.security.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ServiceRequest from a dict"""
+        """Create an instance of DeploymentRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "arguments": obj.get("arguments"),
             "autoScaling": Autoscaling.from_dict(obj.get("autoScaling")) if obj.get("autoScaling") is not None else None,
             "canaryTrafficPercent": obj.get("canaryTrafficPercent"),
-            "description": obj.get("description"),
             "environment": obj.get("environment"),
+            "goalStatus": obj.get("goalStatus") if obj.get("goalStatus") is not None else 'Ready',
             "model": obj.get("model"),
             "name": obj.get("name"),
-            "resources": ConfigurationResources.from_dict(obj.get("resources")) if obj.get("resources") is not None else None
+            "namespace": obj.get("namespace"),
+            "security": Security.from_dict(obj.get("security")) if obj.get("security") is not None else None
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/success_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/auto_scaling_template.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,25 +18,28 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
+from aiolirest.models.autoscaling import Autoscaling
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class SuccessResponse(BaseModel):
+class AutoScalingTemplate(BaseModel):
     """
-    A successful response with a message.
+    Provides a named set of values to configure auto scaling parameters for a deployment.
     """ # noqa: E501
-    message: Optional[StrictStr] = Field(default=None, description="Response message.")
-    __properties: ClassVar[List[str]] = ["message"]
+    auto_scaling: Optional[Autoscaling] = Field(default=None, alias="autoScaling")
+    description: Optional[StrictStr] = Field(default=None, description="Description of the template.")
+    name: StrictStr = Field(description="The template name. Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
+    __properties: ClassVar[List[str]] = ["autoScaling", "description", "name"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -47,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of SuccessResponse from a JSON string"""
+        """Create an instance of AutoScalingTemplate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,24 +69,29 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of auto_scaling
+        if self.auto_scaling:
+            _dict['autoScaling'] = self.auto_scaling.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of SuccessResponse from a dict"""
+        """Create an instance of AutoScalingTemplate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "message": obj.get("message")
+            "autoScaling": Autoscaling.from_dict(obj.get("autoScaling")) if obj.get("autoScaling") is not None else None,
+            "description": obj.get("description"),
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/trained_model_registry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictStr, field_validator
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class TrainedModel(BaseModel):
+class TrainedModelRegistry(BaseModel):
     """
-    The TrainedModel describes a specific model that can be loaded. It optionally references a model registry to provide authorization, and other details.
+    Provides the metadata that describes how to access a named model registry to enable download of a trained model for deployment.
     """ # noqa: E501
-    description: Optional[StrictStr] = Field(default=None, description="A description of the model.")
-    id: Optional[StrictStr] = Field(default=None, description="The ID of the model.  This is a read-only field and is automatically assigned on creation.")
-    image: StrictStr = Field(description="Docker container image servicing the model.")
-    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the model. This is a read-only field and is automatically updated.", alias="modifiedAt")
-    name: StrictStr = Field(description="The name of the model.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
-    registry: Optional[StrictStr] = Field(default=None, description="The name or ID of the model registry.")
-    url: Optional[StrictStr] = Field(default=None, description="Reference to the bento or model to be served.  Supported schemes are: * openllm:// - An openllm model name from huggingface.co dynamically loaded and executed with a VLLM backend. * openllm-cpu:// - An openllm model from huggingface.co dynamically loaded and executed in a CPU-only container with pt backend. * s3:// - An openllm model path which will be dynamically downloaded from an associated s3 registry bucket and executed with a VLLM backend. * cpus3:// - An openllm model path which will be dynamically downloaded from an associated s3 registry bucket and executed in a CPU-only container.")
-    version: Optional[StrictInt] = Field(default=None, description="The version of the model.  This is a read-only field and is automatically assigned on creation.")
-    __properties: ClassVar[List[str]] = ["description", "id", "image", "modifiedAt", "name", "registry", "url", "version"]
+    access_key: Optional[StrictStr] = Field(default=None, description="For an `s3` registry, the value is the access key/username.", alias="accessKey")
+    bucket: Optional[StrictStr] = Field(default=None, description="For an `s3` registry, the value is the S3 bucket name.")
+    endpoint_url: Optional[StrictStr] = Field(default=None, description="For an `s3` registry, the S3 registry endpoint.", alias="endpointUrl")
+    id: Optional[StrictStr] = Field(default=None, description="The ID of the model registry. This is a read-only field and is automatically assigned on creation.")
+    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the registry. This is a read-only field and is automatically updated.", alias="modifiedAt")
+    name: StrictStr = Field(description="The name of the registry.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
+    secret_key: StrictStr = Field(description="The secret key is the password, secret key, or access token for the registry.  * For an `s3` registry, the `secretKey` provides a secret key for the S3 bucket. * For an `openllm` registry, the`secretKey` is the access token for huggingface.co and is supplied to the launched container via the `HF_TOKEN`  environment variable.bucket.", alias="secretKey")
+    type: StrictStr = Field(description="The type of this model registry. * `s3` - Configuration to enable access to an s3 bucket. * `openllm` - Configuration to enable direct download of openllm models from huggingface.co.   Provide your access token in the `secretKey` field. * `ngc` - Not yet supported. Configuration to enable direct download from the NGC: AI Development Catalog. * `http` - Not yet supported.  Configuration to enable model download from a protected http endpoint that requires login.")
+    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "id", "modifiedAt", "name", "secretKey", "type"]
+
+    @field_validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('s3', 'openllm', 'ngc', 'http'):
+            raise ValueError("must be one of enum values ('s3', 'openllm', 'ngc', 'http')")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -54,15 +61,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TrainedModel from a JSON string"""
+        """Create an instance of TrainedModelRegistry from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,27 +84,27 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of TrainedModel from a dict"""
+        """Create an instance of TrainedModelRegistry from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "description": obj.get("description"),
+            "accessKey": obj.get("accessKey"),
+            "bucket": obj.get("bucket"),
+            "endpointUrl": obj.get("endpointUrl"),
             "id": obj.get("id"),
-            "image": obj.get("image"),
             "modifiedAt": obj.get("modifiedAt"),
             "name": obj.get("name"),
-            "registry": obj.get("registry"),
-            "url": obj.get("url"),
-            "version": obj.get("version")
+            "secretKey": obj.get("secretKey"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model_registry.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr, field_validator
+from pydantic import BaseModel, StrictBool, StrictStr
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class TrainedModelRegistry(BaseModel):
+class User(BaseModel):
     """
-    The TrainedModelRegistry provides the metadata that describes how to access a named model registry.
+    Name and properties of a user.
     """ # noqa: E501
-    access_key: StrictStr = Field(description="S3 access key/username.", alias="accessKey")
-    bucket: StrictStr = Field(description="S3 Bucket name.")
-    endpoint_url: StrictStr = Field(description="S3 endpoint URL.", alias="endpointUrl")
-    id: Optional[StrictStr] = Field(default=None, description="The ID of the model registry. This is a read-only field and is automatically assigned on creation.")
-    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the registry. This is a read-only field and is automatically updated.", alias="modifiedAt")
-    name: StrictStr = Field(description="The name of the model registry.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
-    secret_key: StrictStr = Field(description="S3 secret key/password.", alias="secretKey")
-    type: StrictStr = Field(description="The type of this model registry.")
-    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "id", "modifiedAt", "name", "secretKey", "type"]
-
-    @field_validator('type')
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in ('s3', 'path', 'http'):
-            raise ValueError("must be one of enum values ('s3', 'path', 'http')")
-        return value
+    active: Optional[StrictBool] = Field(default=None, description="Allows for disabling a user without deleting them.   Only active users an login.")
+    display_name: StrictStr = Field(description="Display name of the user in the UI.", alias="displayName")
+    id: Optional[StrictStr] = Field(default=None, description="The ID of the user. This is a read-only field and is automatically assigned on creation.")
+    last_auth_at: Optional[StrictStr] = Field(default=None, description="Date-time of last use of this account. This is a read-only field and is automatically updated.", alias="lastAuthAt")
+    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the user configuration. This is a read-only field and is automatically updated.", alias="modifiedAt")
+    remote: Optional[StrictBool] = Field(default=None, description="User data comes from a external/remote provider. This is a read-only field and is automatically updated.")
+    username: StrictStr = Field(description="The user name used for login.")
+    __properties: ClassVar[List[str]] = ["active", "displayName", "id", "lastAuthAt", "modifiedAt", "remote", "username"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -61,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TrainedModelRegistry from a JSON string"""
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,27 +76,26 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of TrainedModelRegistry from a dict"""
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "accessKey": obj.get("accessKey"),
-            "bucket": obj.get("bucket"),
-            "endpointUrl": obj.get("endpointUrl"),
+            "active": obj.get("active"),
+            "displayName": obj.get("displayName"),
             "id": obj.get("id"),
+            "lastAuthAt": obj.get("lastAuthAt"),
             "modifiedAt": obj.get("modifiedAt"),
-            "name": obj.get("name"),
-            "secretKey": obj.get("secretKey"),
-            "type": obj.get("type")
+            "remote": obj.get("remote"),
+            "username": obj.get("username")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model_registry_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/user_patch_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,42 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr, field_validator
-from pydantic import Field
+from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, StrictBool, StrictStr
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class TrainedModelRegistryRequest(BaseModel):
+class UserPatchRequest(BaseModel):
     """
-    The TrainedModelRegistry provides the metadata that describes how to access a named model registry.
+    UserPatchRequest
     """ # noqa: E501
-    access_key: StrictStr = Field(description="S3 access key/username.", alias="accessKey")
-    bucket: StrictStr = Field(description="S3 Bucket name.")
-    endpoint_url: StrictStr = Field(description="S3 endpoint URL.", alias="endpointUrl")
-    name: StrictStr = Field(description="The name of the model registry.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
-    secret_key: StrictStr = Field(description="S3 secret key/password.", alias="secretKey")
-    type: StrictStr = Field(description="The type of this model registry.")
-    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "name", "secretKey", "type"]
-
-    @field_validator('type')
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in ('s3', 'path', 'http'):
-            raise ValueError("must be one of enum values ('s3', 'path', 'http')")
-        return value
+    active: Optional[StrictBool] = None
+    password: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["active", "password"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -59,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TrainedModelRegistryRequest from a JSON string"""
+        """Create an instance of UserPatchRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,25 +70,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of TrainedModelRegistryRequest from a dict"""
+        """Create an instance of UserPatchRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "accessKey": obj.get("accessKey"),
-            "bucket": obj.get("bucket"),
-            "endpointUrl": obj.get("endpointUrl"),
-            "name": obj.get("name"),
-            "secretKey": obj.get("secretKey"),
-            "type": obj.get("type")
+            "active": obj.get("active"),
+            "password": obj.get("password")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/trained_model_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/user_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool, StrictStr, field_validator
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class TrainedModelRequest(BaseModel):
+class UserRequest(BaseModel):
     """
-    The TrainedModel describes a specific model that can be loaded. It optionally references a model registry to provide authorization, and other details.
+    Name and properties of a user.
     """ # noqa: E501
-    description: Optional[StrictStr] = Field(default=None, description="A description of the model.")
-    image: StrictStr = Field(description="Docker container image servicing the model.")
-    name: StrictStr = Field(description="The name of the model.  Must begin with a letter, but may contain letters, numbers, underscore, and hyphen.")
-    registry: Optional[StrictStr] = Field(default=None, description="The name or ID of the model registry.")
-    url: Optional[StrictStr] = Field(default=None, description="Reference to the bento or model to be served.  Supported schemes are: * openllm:// - An openllm model name from huggingface.co dynamically loaded and executed with a VLLM backend. * openllm-cpu:// - An openllm model from huggingface.co dynamically loaded and executed in a CPU-only container with pt backend. * s3:// - An openllm model path which will be dynamically downloaded from an associated s3 registry bucket and executed with a VLLM backend. * cpus3:// - An openllm model path which will be dynamically downloaded from an associated s3 registry bucket and executed in a CPU-only container.")
-    __properties: ClassVar[List[str]] = ["description", "image", "name", "registry", "url"]
+    active: Optional[StrictBool] = Field(default=None, description="Allows for disabling a user without deleting them.   Only active users an login.")
+    display_name: StrictStr = Field(description="Display name of the user in the UI.", alias="displayName")
+    remote: Optional[StrictBool] = Field(default=None, description="The user is remotely authenticated")
+    role_name: Optional[StrictStr] = Field(default=None, description="Role name.", alias="roleName")
+    username: StrictStr = Field(description="The user name used for login.")
+    __properties: ClassVar[List[str]] = ["active", "displayName", "remote", "roleName", "username"]
+
+    @field_validator('role_name')
+    def role_name_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('Admin', 'Viewer', 'Maintainer', 'Robot'):
+            raise ValueError("must be one of enum values ('Admin', 'Viewer', 'Maintainer', 'Robot')")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -51,15 +61,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TrainedModelRequest from a JSON string"""
+        """Create an instance of UserRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,24 +84,24 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of TrainedModelRequest from a dict"""
+        """Create an instance of UserRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "description": obj.get("description"),
-            "image": obj.get("image"),
-            "name": obj.get("name"),
-            "registry": obj.get("registry"),
-            "url": obj.get("url")
+            "active": obj.get("active"),
+            "displayName": obj.get("displayName"),
+            "remote": obj.get("remote"),
+            "roleName": obj.get("roleName"),
+            "username": obj.get("username")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/user.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/event_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictBool, StrictStr
+from pydantic import BaseModel, StrictStr
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class User(BaseModel):
+class EventInfo(BaseModel):
     """
-    Name and properties of a user.
+    EventInfo
     """ # noqa: E501
-    active: Optional[StrictBool] = Field(default=None, description="Allows for disabling a user without deleting them.   Only active users an login.")
-    display_name: StrictStr = Field(description="Display name of the user in the UI.", alias="displayName")
-    id: Optional[StrictStr] = Field(default=None, description="The ID of the user. This is a read-only field and is automatically assigned on creation.")
-    last_auth_at: Optional[StrictStr] = Field(default=None, description="Date-time of last use of this account. This is a read-only field and is automatically updated.", alias="lastAuthAt")
-    modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the user configuration. This is a read-only field and is automatically updated.", alias="modifiedAt")
-    remote: Optional[StrictBool] = Field(default=None, description="User data comes from a external/remote provider. This is a read-only field and is automatically updated.")
-    username: StrictStr = Field(description="The user name used for login.")
-    __properties: ClassVar[List[str]] = ["active", "displayName", "id", "lastAuthAt", "modifiedAt", "remote", "username"]
+    event_type: Optional[StrictStr] = Field(default=None, description="Type of the event. * `Normal` - An informational event. * `Warning` - A condition that may require attention.", alias="eventType")
+    message: Optional[StrictStr] = Field(default=None, description="Message for the event.")
+    reason: Optional[StrictStr] = Field(default=None, description="Common reasons for the event. * `ScalingReplicaSet` - The number of deployed replicas is being increased or decreased. * `Pulling` - Indicates that the container image is being loaded from a registry. * `Pulled` - Container image already present on machine. * `RevisionReady` - Revision becomes ready upon all resources being ready.  Kubernetes official website does not provide a full list of values for Reason. Use the below link for the latest compilation of event Reasons. Ref: https://docs.appdynamics.com/observability/cisco-cloud-observability/en/kubernetes-and-app-service-monitoring/events-collection/events-reason-reference.")
+    time: Optional[StrictStr] = Field(default=None, description="The time at which the event occurred.")
+    __properties: ClassVar[List[str]] = ["eventType", "message", "reason", "time"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of User from a JSON string"""
+        """Create an instance of EventInfo from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -76,26 +73,23 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of User from a dict"""
+        """Create an instance of EventInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "active": obj.get("active"),
-            "displayName": obj.get("displayName"),
-            "id": obj.get("id"),
-            "lastAuthAt": obj.get("lastAuthAt"),
-            "modifiedAt": obj.get("modifiedAt"),
-            "remote": obj.get("remote"),
-            "username": obj.get("username")
+            "eventType": obj.get("eventType"),
+            "message": obj.get("message"),
+            "reason": obj.get("reason"),
+            "time": obj.get("time")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/models/user_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/observability.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,43 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, StrictStr
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class UserRequest(BaseModel):
+class Observability(BaseModel):
     """
-    Name and properties of a user.
+    Provides URLs to access a web interface (e.g. Grafana) for a requested deployment or version.
     """ # noqa: E501
-    active: Optional[StrictBool] = Field(default=None, description="Allows for disabling a user without deleting them.   Only active users an login.")
-    display_name: StrictStr = Field(description="Display name of the user in the UI.", alias="displayName")
-    remote: Optional[StrictBool] = Field(default=None, description="The user is remotely authenticated")
-    role_name: Optional[StrictStr] = Field(default=None, description="Role name.", alias="roleName")
-    username: StrictStr = Field(description="The user name used for login.")
-    __properties: ClassVar[List[str]] = ["active", "displayName", "remote", "roleName", "username"]
-
-    @field_validator('role_name')
-    def role_name_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('Admin', 'Viewer', 'Maintainer', 'Robot'):
-            raise ValueError("must be one of enum values ('Admin', 'Viewer', 'Maintainer', 'Robot')")
-        return value
+    auth: Optional[StrictStr] = Field(default=None, description="JWT autentication token to access the observability web interface.")
+    dashboard_url: Optional[StrictStr] = Field(default=None, description="URL to view metrics/logs associated with the requested deployment.", alias="dashboardUrl")
+    __properties: ClassVar[List[str]] = ["auth", "dashboardUrl"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -61,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UserRequest from a JSON string"""
+        """Create an instance of Observability from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,24 +71,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of UserRequest from a dict"""
+        """Create an instance of Observability from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "active": obj.get("active"),
-            "displayName": obj.get("displayName"),
-            "remote": obj.get("remote"),
-            "roleName": obj.get("roleName"),
-            "username": obj.get("username")
+            "auth": obj.get("auth"),
+            "dashboardUrl": obj.get("dashboardUrl")
         })
         return _obj
```

### Comparing `aioli-sdk-0.1.2.dev0/aiolirest/rest.py` & `aioli-sdk-0.2.0rc0/aiolirest/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Aioli API (MVP)
+    HPE Machine Learning Inference Software (MLIS/Aioli)
 
-    *Aioli* is the AI On-line Inference Platform that enables easy deployment, tracking, and serving of your trained models regardless of your preferred AI framework.
+    HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.1
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.1.2.dev0/setup.py` & `aioli-sdk-0.2.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.1.2-dev0",
+    version="0.2.0-rc0",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

