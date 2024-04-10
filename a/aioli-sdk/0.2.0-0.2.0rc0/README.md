# Comparing `tmp/aioli-sdk-0.2.0.tar.gz` & `tmp/aioli-sdk-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli-sdk-0.2.0.tar", last modified: Wed Apr 10 16:38:06 2024, max compression
+gzip compressed data, was "aioli-sdk-0.2.0rc0.tar", last modified: Wed Apr 10 15:34:40 2024, max compression
```

## Comparing `aioli-sdk-0.2.0.tar` & `aioli-sdk-0.2.0rc0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.204885 aioli-sdk-0.2.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2024-04-10 16:38:06.204885 aioli-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.192885 aioli-sdk-0.2.0/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.196885 aioli-sdk-0.2.0/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10169 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13963 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8252 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.196885 aioli-sdk-0.2.0/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24720 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.196885 aioli-sdk-0.2.0/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.196885 aioli-sdk-0.2.0/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3591 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.204885 aioli-sdk-0.2.0/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2024-04-10 16:38:06.000000 aioli-sdk-0.2.0/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2447 2024-04-10 16:38:06.000000 aioli-sdk-0.2.0/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 16:38:06.000000 aioli-sdk-0.2.0/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-10 16:38:06.000000 aioli-sdk-0.2.0/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 16:38:03.000000 aioli-sdk-0.2.0/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-10 16:38:06.000000 aioli-sdk-0.2.0/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-10 16:38:06.000000 aioli-sdk-0.2.0/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.200885 aioli-sdk-0.2.0/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3155 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.200885 aioli-sdk-0.2.0/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22808 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84654 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10510 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91188 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54366 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43077 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105939 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61880 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25045 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14916 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5592 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:06.204885 aioli-sdk-0.2.0/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2217 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4282 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3657 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7721 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4304 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5063 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5245 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2783 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3770 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3256 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2531 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2965 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6378 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5800 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2935 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3361 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2742 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3089 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3291 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2900 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5174 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4992 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3927 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3692 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8435 2024-04-10 16:38:01.000000 aioli-sdk-0.2.0/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-10 16:38:06.204885 aioli-sdk-0.2.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2024-04-10 16:31:23.000000 aioli-sdk-0.2.0/setup.py
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

### Comparing `aioli-sdk-0.2.0/PKG-INFO` & `aioli-sdk-0.2.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.0
+Version: 0.2.0rc0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli-sdk-0.2.0/aioli/cli/_util.py` & `aioli-sdk-0.2.0rc0/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/cli.py` & `aioli-sdk-0.2.0rc0/aioli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/deployment.py` & `aioli-sdk-0.2.0rc0/aioli/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/errors.py` & `aioli-sdk-0.2.0rc0/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/model.py` & `aioli-sdk-0.2.0rc0/aioli/cli/model.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/registry.py` & `aioli-sdk-0.2.0rc0/aioli/cli/registry.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/render.py` & `aioli-sdk-0.2.0rc0/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/role.py` & `aioli-sdk-0.2.0rc0/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/sso.py` & `aioli-sdk-0.2.0rc0/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/test/conftest.py` & `aioli-sdk-0.2.0rc0/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/test/test_cli.py` & `aioli-sdk-0.2.0rc0/aioli/cli/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/user.py` & `aioli-sdk-0.2.0rc0/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/cli/version.py` & `aioli-sdk-0.2.0rc0/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/api/authentication.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/api/certs.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/api/errors.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/api/request.py` & `aioli-sdk-0.2.0rc0/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/check.py` & `aioli-sdk-0.2.0rc0/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/constants.py` & `aioli-sdk-0.2.0rc0/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/declarative_argparse.py` & `aioli-sdk-0.2.0rc0/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/requests.py` & `aioli-sdk-0.2.0rc0/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/common/util.py` & `aioli-sdk-0.2.0rc0/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli/util.py` & `aioli-sdk-0.2.0rc0/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aioli_sdk.egg-info/PKG-INFO` & `aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.0
+Version: 0.2.0rc0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli-sdk-0.2.0/aioli_sdk.egg-info/SOURCES.txt` & `aioli-sdk-0.2.0rc0/aioli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aiolirest/__init__.py` & `aioli-sdk-0.2.0rc0/aiolirest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/authentication_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/deployments_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/deployments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/information_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/packaged_models_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/packaged_models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/registries_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/registries_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/roles_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/templates_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api/users_api.py` & `aioli-sdk-0.2.0rc0/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api_client.py` & `aioli-sdk-0.2.0rc0/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/api_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli-sdk-0.2.0/aiolirest/configuration.py` & `aioli-sdk-0.2.0rc0/aiolirest/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
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
-               "Version of the API: 0.2.0\n"\
+               "Version of the API: 0.2.0-rc0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli-sdk-0.2.0/aiolirest/exceptions.py` & `aioli-sdk-0.2.0rc0/aiolirest/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/__init__.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/auto_scaling_template.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/auto_scaling_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/autoscaling.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/autoscaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/configuration_resources.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/configuration_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/deployment.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/deployment_model_version.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/deployment_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/deployment_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/deployment_state.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/deployment_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/error_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/event_info.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/event_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/failure_info.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/failure_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/login_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/login_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/login_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/model_auth_token.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/model_auth_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/observability.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/observability.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/packaged_model.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/packaged_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/packaged_model_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/packaged_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/resource_profile.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/resource_profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/resources_template.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/resources_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/role.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/role_assignment.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/role_assignments.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/role_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/security.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/success_response.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/success_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/trained_model_registry.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/trained_model_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/trained_model_registry_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/trained_model_registry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/user.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/user_patch_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/user_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/models/user_request.py` & `aioli-sdk-0.2.0rc0/aiolirest/models/user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/aiolirest/rest.py` & `aioli-sdk-0.2.0rc0/aiolirest/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.0
+    The version of the OpenAPI document: 0.2.0-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli-sdk-0.2.0/setup.py` & `aioli-sdk-0.2.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.0",
+    version="0.2.0-rc0",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

