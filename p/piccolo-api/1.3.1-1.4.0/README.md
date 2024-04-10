# Comparing `tmp/piccolo_api-1.3.1.tar.gz` & `tmp/piccolo_api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piccolo_api-1.3.1.tar", last modified: Sat Mar 30 12:03:43 2024, max compression
+gzip compressed data, was "piccolo_api-1.4.0.tar", last modified: Wed Apr 10 20:29:38 2024, max compression
```

## Comparing `piccolo_api-1.3.1.tar` & `piccolo_api-1.4.0.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.856213 piccolo_api-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-30 12:03:43.856213 piccolo_api-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.844213 piccolo_api-1.3.1/piccolo_api/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.844213 piccolo_api-1.3.1/piccolo_api/change_password/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/change_password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/change_password/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.844213 piccolo_api-1.3.1/piccolo_api/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44411 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/crud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/crud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/crud/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/crud/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/crud/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.844213 piccolo_api-1.3.1/piccolo_api/csp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/csp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/csp/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/csrf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/csrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/csrf/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20182 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/fastapi/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/jwt_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/jwt_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/jwt_auth/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/jwt_auth/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/media/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/media/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/media/content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/media/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/media/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/openapi/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/openapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/openapi/templates/swagger_ui.html.jinja
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/rate_limiting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/rate_limiting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/rate_limiting/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.848213 piccolo_api-1.3.1/piccolo_api/register/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/register/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/session_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/session_auth/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/piccolo_migrations/2019-11-12T20-47-17.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/session_auth/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/shared/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/auth/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/auth/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/auth/junction.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/auth/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/shared/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/shared/middleware/junction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/templates/change_password.html
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/templates/register.html
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/templates/session_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/templates/session_logout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/token_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/token_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/token_auth/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/token_auth/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/token_auth/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.852213 piccolo_api-1.3.1/piccolo_api/token_auth/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/token_auth/piccolo_migrations/2019-11-18T22-24-41.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/token_auth/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/token_auth/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.856213 piccolo_api-1.3.1/piccolo_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/piccolo_api/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:03:43.856213 piccolo_api-1.3.1/piccolo_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-30 12:03:43.000000 piccolo_api-1.3.1/piccolo_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-30 12:03:43.000000 piccolo_api-1.3.1/piccolo_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:03:43.000000 piccolo_api-1.3.1/piccolo_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-30 12:03:43.000000 piccolo_api-1.3.1/piccolo_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-30 12:03:43.000000 piccolo_api-1.3.1/piccolo_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 12:03:43.856213 piccolo_api-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-30 12:03:27.000000 piccolo_api-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.779898 piccolo_api-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-10 20:29:38.779898 piccolo_api-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.767898 piccolo_api-1.4.0/piccolo_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.767898 piccolo_api-1.4.0/piccolo_api/change_password/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/change_password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/change_password/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.767898 piccolo_api-1.4.0/piccolo_api/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44411 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/crud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/crud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/crud/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/crud/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/crud/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.767898 piccolo_api-1.4.0/piccolo_api/csp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/csp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/csp/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.767898 piccolo_api-1.4.0/piccolo_api/csrf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/csrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/csrf/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20182 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/fastapi/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/jwt_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/jwt_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/jwt_auth/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/jwt_auth/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/media/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/media/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/media/content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/media/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/media/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/openapi/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/openapi/templates/swagger_ui.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/rate_limiting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/rate_limiting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/rate_limiting/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/register/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/register/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.771898 piccolo_api-1.4.0/piccolo_api/session_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/session_auth/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/piccolo_migrations/2019-11-12T20-47-17.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/session_auth/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/shared/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/auth/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/auth/excluded_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/auth/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/auth/junction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/auth/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/shared/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/shared/middleware/junction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/templates/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/templates/register.html
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/templates/session_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/templates/session_logout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/token_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/token_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/token_auth/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/token_auth/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/token_auth/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/token_auth/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/token_auth/piccolo_migrations/2019-11-18T22-24-41.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/token_auth/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/token_auth/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.775898 piccolo_api-1.4.0/piccolo_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/piccolo_api/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:29:38.779898 piccolo_api-1.4.0/piccolo_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-10 20:29:38.000000 piccolo_api-1.4.0/piccolo_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-10 20:29:38.000000 piccolo_api-1.4.0/piccolo_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:29:38.000000 piccolo_api-1.4.0/piccolo_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 20:29:38.000000 piccolo_api-1.4.0/piccolo_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 20:29:38.000000 piccolo_api-1.4.0/piccolo_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:29:38.779898 piccolo_api-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 20:29:24.000000 piccolo_api-1.4.0/setup.py
```

### Comparing `piccolo_api-1.3.1/LICENSE` & `piccolo_api-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/PKG-INFO` & `piccolo_api-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo_api
-Version: 1.3.1
+Version: 1.4.0
 Summary: Utilities for using the Piccolo ORM in ASGI apps, plus essential ASGI middleware such as authentication and rate limiting.
 Home-page: https://github.com/piccolo-orm/piccolo_api
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `piccolo_api-1.3.1/README.md` & `piccolo_api-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/change_password/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/change_password/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/crud/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/crud/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/crud/exceptions.py` & `piccolo_api-1.4.0/piccolo_api/crud/exceptions.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/crud/hooks.py` & `piccolo_api-1.4.0/piccolo_api/crud/hooks.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/crud/validators.py` & `piccolo_api-1.4.0/piccolo_api/crud/validators.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/csp/middleware.py` & `piccolo_api-1.4.0/piccolo_api/csp/middleware.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/csrf/middleware.py` & `piccolo_api-1.4.0/piccolo_api/csrf/middleware.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/fastapi/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/fastapi/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/jwt_auth/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/jwt_auth/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/jwt_auth/middleware.py` & `piccolo_api-1.4.0/piccolo_api/jwt_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/media/base.py` & `piccolo_api-1.4.0/piccolo_api/media/base.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/media/content_type.py` & `piccolo_api-1.4.0/piccolo_api/media/content_type.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/media/local.py` & `piccolo_api-1.4.0/piccolo_api/media/local.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/media/s3.py` & `piccolo_api-1.4.0/piccolo_api/media/s3.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/openapi/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/openapi/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/openapi/templates/swagger_ui.html.jinja` & `piccolo_api-1.4.0/piccolo_api/openapi/templates/swagger_ui.html.jinja`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/rate_limiting/middleware.py` & `piccolo_api-1.4.0/piccolo_api/rate_limiting/middleware.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/register/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/register/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/session_auth/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/session_auth/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/session_auth/middleware.py` & `piccolo_api-1.4.0/piccolo_api/session_auth/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     AuthenticationError,
     BaseUser,
 )
 from starlette.requests import HTTPConnection
 
 from piccolo_api.session_auth.tables import SessionsBase
 from piccolo_api.shared.auth import UnauthenticatedUser, User
+from piccolo_api.shared.auth.excluded_paths import check_excluded_paths
 
 
 class SessionsAuthBackend(AuthenticationBackend):
     """
     Authenticaion middleware which uses session cookies.
     """
 
@@ -27,53 +28,60 @@
         session_table: t.Type[SessionsBase] = SessionsBase,
         cookie_name: str = "id",
         admin_only: bool = True,
         superuser_only: bool = False,
         active_only: bool = True,
         increase_expiry: t.Optional[timedelta] = None,
         allow_unauthenticated: bool = False,
+        excluded_paths: t.Optional[t.Sequence[str]] = None,
     ):
         """
         :param auth_table:
             The Piccolo table used for authenticating users. It defaults to
             :class:`BaseUser <piccolo.apps.user.tables.BaseUser>`.
         :param session_table:
             The Piccolo table used for storing sessions. If defaults to
             :class:`SessionsBase <piccolo_api.session_auth.tables.SessionsBase>`.
         :param cookie_name:
             The name of the session cookie. Override this if it clashes with
             other cookies in your application.
         :param admin_only:
-            If True, users which aren't admins will be rejected.
+            If ``True``, users which aren't admins will be rejected.
         :param superuser_only:
-            If True, users which aren't superusers will be rejected.
+            If ``True``, users which aren't superusers will be rejected.
         :param active_only:
-            If True, users which aren't active will be rejected.
+            If ``True``, users which aren't active will be rejected.
         :param increase_expiry:
             If set, the session expiry will be increased by this amount on each
             request, if it's close to expiry. This allows sessions to have a
             short expiry date, whilst also providing a good user experience.
         :param allow_unauthenticated:
-            If True, when a matching user session can't be found, the request
+            If ``True``, when a matching user session can't be found, the request
             still continues, but an unauthenticated user is added to the scope.
             It's then up to the application's endpoints to check if a user is
             authenticated or not using ``request.user.is_authenticated``. If
-            False, the request is automatically rejected if a user session
+            ``False``, the request is automatically rejected if a user session
             can't be found.
+        :param excluded_paths:
+            These paths don't require a session cookie - useful if you want to
+            exclude a few URLs, such as docs.
+
         """  # noqa: E501
         super().__init__()
         self.auth_table = auth_table
         self.session_table = session_table
         self.cookie_name = cookie_name
         self.admin_only = admin_only
         self.superuser_only = superuser_only
         self.active_only = active_only
         self.increase_expiry = increase_expiry
         self.allow_unauthenticated = allow_unauthenticated
+        self.excluded_paths = excluded_paths or []
 
+    @check_excluded_paths
     async def authenticate(
         self, conn: HTTPConnection
     ) -> t.Optional[t.Tuple[AuthCredentials, BaseUser]]:
         token = conn.cookies.get(self.cookie_name, None)
         if not token:
             if self.allow_unauthenticated:
                 return (AuthCredentials(scopes=[]), UnauthenticatedUser())
```

### Comparing `piccolo_api-1.3.1/piccolo_api/session_auth/piccolo_migrations/2019-11-12T20-47-17.py` & `piccolo_api-1.4.0/piccolo_api/session_auth/piccolo_migrations/2019-11-12T20-47-17.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/session_auth/tables.py` & `piccolo_api-1.4.0/piccolo_api/session_auth/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/shared/auth/captcha.py` & `piccolo_api-1.4.0/piccolo_api/shared/auth/captcha.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/shared/auth/hooks.py` & `piccolo_api-1.4.0/piccolo_api/shared/auth/hooks.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/shared/auth/junction.py` & `piccolo_api-1.4.0/piccolo_api/shared/auth/junction.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/shared/auth/styles.py` & `piccolo_api-1.4.0/piccolo_api/shared/auth/styles.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/shared/auth/user.py` & `piccolo_api-1.4.0/piccolo_api/shared/auth/user.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/shared/middleware/junction.py` & `piccolo_api-1.4.0/piccolo_api/shared/middleware/junction.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/templates/base.html` & `piccolo_api-1.4.0/piccolo_api/templates/base.html`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/templates/change_password.html` & `piccolo_api-1.4.0/piccolo_api/templates/change_password.html`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/templates/register.html` & `piccolo_api-1.4.0/piccolo_api/templates/register.html`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/templates/session_login.html` & `piccolo_api-1.4.0/piccolo_api/templates/session_login.html`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/token_auth/endpoints.py` & `piccolo_api-1.4.0/piccolo_api/token_auth/endpoints.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/token_auth/middleware.py` & `piccolo_api-1.4.0/piccolo_api/token_auth/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     AuthenticationBackend,
     AuthenticationError,
     BaseUser,
     SimpleUser,
 )
 from starlette.requests import HTTPConnection
 
-from piccolo_api.shared.auth import UnauthenticatedUser, User
+from piccolo_api.shared.auth import User
+from piccolo_api.shared.auth.excluded_paths import check_excluded_paths
 from piccolo_api.token_auth.tables import TokenAuth
 
 
 class TokenAuthProvider(metaclass=ABCMeta):
     """
     Subclass to create your own token provider.
     """
@@ -86,51 +87,35 @@
         token_auth_provider: TokenAuthProvider = DEFAULT_PROVIDER,
         excluded_paths: t.Optional[t.Sequence[str]] = None,
     ):
         """
         :param token_auth_provider:
             Used to verify that a token is correct.
         :param excluded_paths:
-            These paths don't require a token.
+            These paths don't require a token - useful if you want to
+            exclude a few URLs, such as docs.
+
         """
         super().__init__()
         self.token_auth_provider = token_auth_provider
         self.excluded_paths = excluded_paths or []
 
     def extract_token(self, header: str) -> str:
         try:
             token = header.split("Bearer ")[1]
         except IndexError:
             raise AuthenticationError("The header is in the wrong format.")
 
         return token
 
+    @check_excluded_paths
     async def authenticate(
         self, conn: HTTPConnection
     ) -> t.Optional[t.Tuple[AuthCredentials, BaseUser]]:
         auth_header = conn.headers.get("Authorization", None)
-        conn_path = dict(conn)
-
-        for excluded_path in self.excluded_paths:
-            if excluded_path.endswith("*"):
-                if (
-                    conn_path["raw_path"]
-                    .decode("utf-8")
-                    .startswith(excluded_path.rstrip("*"))
-                ):
-                    return (
-                        AuthCredentials(scopes=[]),
-                        UnauthenticatedUser(),
-                    )
-            else:
-                if conn_path["path"] == excluded_path:
-                    return (
-                        AuthCredentials(scopes=[]),
-                        UnauthenticatedUser(),
-                    )
 
         if not auth_header:
             raise AuthenticationError("The Authorization header is missing.")
 
         token = self.extract_token(auth_header)
 
         user = await self.token_auth_provider.get_user(token=token)
```

### Comparing `piccolo_api-1.3.1/piccolo_api/token_auth/piccolo_migrations/2019-11-18T22-24-41.py` & `piccolo_api-1.4.0/piccolo_api/token_auth/piccolo_migrations/2019-11-18T22-24-41.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/token_auth/tables.py` & `piccolo_api-1.4.0/piccolo_api/token_auth/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api/utils/types.py` & `piccolo_api-1.4.0/piccolo_api/utils/types.py`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/piccolo_api.egg-info/PKG-INFO` & `piccolo_api-1.4.0/piccolo_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo_api
-Version: 1.3.1
+Version: 1.4.0
 Summary: Utilities for using the Piccolo ORM in ASGI apps, plus essential ASGI middleware such as authentication and rate limiting.
 Home-page: https://github.com/piccolo-orm/piccolo_api
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `piccolo_api-1.3.1/piccolo_api.egg-info/SOURCES.txt` & `piccolo_api-1.4.0/piccolo_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 piccolo_api/session_auth/piccolo_app.py
 piccolo_api/session_auth/tables.py
 piccolo_api/session_auth/piccolo_migrations/2019-11-12T20-47-17.py
 piccolo_api/session_auth/piccolo_migrations/__init__.py
 piccolo_api/shared/__init__.py
 piccolo_api/shared/auth/__init__.py
 piccolo_api/shared/auth/captcha.py
+piccolo_api/shared/auth/excluded_paths.py
 piccolo_api/shared/auth/hooks.py
 piccolo_api/shared/auth/junction.py
 piccolo_api/shared/auth/styles.py
 piccolo_api/shared/auth/user.py
 piccolo_api/shared/middleware/__init__.py
 piccolo_api/shared/middleware/junction.py
 piccolo_api/templates/base.html
```

### Comparing `piccolo_api-1.3.1/pyproject.toml` & `piccolo_api-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piccolo_api-1.3.1/setup.py` & `piccolo_api-1.4.0/setup.py`

 * *Files identical despite different names*

