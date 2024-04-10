# Comparing `tmp/qbraid-core-0.1.0.dev4.tar.gz` & `tmp/qbraid-core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-core-0.1.0.dev4.tar", last modified: Thu Apr  4 23:09:23 2024, max compression
+gzip compressed data, was "qbraid-core-0.1.1.tar", last modified: Wed Apr 10 00:15:27 2024, max compression
```

## Comparing `qbraid-core-0.1.0.dev4.tar` & `qbraid-core-0.1.1.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.714338 qbraid-core-0.1.0.dev4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-04 23:09:23.714338 qbraid-core-0.1.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.706338 qbraid-core-0.1.0.dev4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.706338 qbraid-core-0.1.0.dev4/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.706338 qbraid-core-0.1.0.dev4/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:09:23.714338 qbraid-core-0.1.0.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.918968 qbraid-core-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-10 00:15:27.918968 qbraid-core-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:15:27.918968 qbraid-core-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/.github/workflows/docs.yml` & `qbraid-core-0.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/.github/workflows/format.yml` & `qbraid-core-0.1.1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/.github/workflows/main.yml` & `qbraid-core-0.1.1/.github/workflows/main.yml`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           path: dist/*.whl
 
   test:
     needs: build
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11', '3.12']
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `qbraid-core-0.1.0.dev4/.github/workflows/publish.yml` & `qbraid-core-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/.github/workflows/test-publish.yml` & `qbraid-core-0.1.1/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/.gitignore` & `qbraid-core-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/LICENSE` & `qbraid-core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/PKG-INFO` & `qbraid-core-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.0.dev4
+Version: 0.1.1
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -12,20 +12,19 @@
 Keywords: qbraid,quantum,cloud
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `qbraid-core-0.1.0.dev4/README.md` & `qbraid-core-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/Makefile` & `qbraid-core-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/_static/cards/jupyter.png` & `qbraid-core-0.1.1/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/_static/cards/python.png` & `qbraid-core-0.1.1/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/_static/cards/terminal.png` & `qbraid-core-0.1.1/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/_static/css/custom.css` & `qbraid-core-0.1.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/_static/css/s4defs-roles.css` & `qbraid-core-0.1.1/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/_static/favicon.ico` & `qbraid-core-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/_static/logo.png` & `qbraid-core-0.1.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/conf.py` & `qbraid-core-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/index.rst` & `qbraid-core-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/docs/make.bat` & `qbraid-core-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/pyproject.toml` & `qbraid-core-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.0.dev4"
+version = "0.1.1"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
 license = {text = "Proprietary"}
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["requests", "urllib3"]
```

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/__init__.py` & `qbraid-core-0.1.1/qbraid_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Classes
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
+   Session
    QbraidClient
    QbraidSession
    PostForcelistRetry
 
 
 Functions
 ----------
@@ -46,15 +47,15 @@
     ConfigError,
     QbraidException,
     RequestsApiError,
     ResourceNotFoundError,
     UserNotFoundError,
 )
 from .retry import PostForcelistRetry
-from .session import QbraidSession
+from .sessions import QbraidSession, Session
 
 try:
     # Injected in _version.py during the build process.
     from ._version import __version__
 except ImportError:
     __version__ = ""
 
@@ -104,20 +105,19 @@
         service_name (str): The name of the service for which to create the client.
         **kwargs: Keyword arguments for session customization, used only if creating
                   a new default session.
 
     Returns:
         A service client instance.
     """
-    session = _get_default_session()
-    _ = session.get_available_services()  # Ensure the session is initialized
-    return session.client(*args, **kwargs)
+    return _get_default_session().client(*args, **kwargs)
 
 
 __all__ = [
+    "Session",
     "QbraidClient",
     "QbraidSession",
     "PostForcelistRetry",
     "client",
     "setup_default_session",
     "QbraidException",
     "AuthError",
```

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/_compat.py` & `qbraid-core-0.1.1/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/client.py` & `qbraid-core-0.1.1/qbraid_core/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,41 +8,51 @@
 import datetime
 import os
 import re
 from typing import Optional
 
 from ._compat import check_version
 from .exceptions import AuthError, RequestsApiError, ResourceNotFoundError, UserNotFoundError
-from .session import QbraidSession
+from .sessions import QbraidSession
 
 
 class QbraidClient:
     """Base class for qBraid micro-service clients."""
 
     def __init__(self, session: Optional[QbraidSession] = None):
-        self.session = session or QbraidSession()
+        self.session = session
+        self._user_metadata = None
         check_version("qbraid-core")
 
     @property
     def session(self) -> QbraidSession:
         """The QbraidSession used to make requests."""
         return self._session
 
     @session.setter
     def session(self, value: Optional[QbraidSession]) -> None:
         """Set the QbraidSession.
 
         Raises:
             AuthError: If the provided session is not valid.
         """
+        if value is not None and not isinstance(value, QbraidSession):
+            raise TypeError("session must be a QbraidSession instance or None")
+
         qbraid_session = value or QbraidSession()
         try:
-            _ = qbraid_session.get_user()
+            user = qbraid_session.get_user()
         except UserNotFoundError as err:
             raise AuthError("Access denied due to missing or invalid credentials") from err
+
+        metadata = user.get("personalInformation", {})
+        self._user_metadata = {
+            "organization": metadata.get("organization", "qbraid"),
+            "role": metadata.get("role", "guest"),
+        }
         self._session = qbraid_session
 
     @staticmethod
     def _is_valid_object_id(candidate_id: str) -> bool:
         """
         Check if the provided string is a valid MongoDB ObjectId format.
```

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/exceptions.py` & `qbraid-core-0.1.1/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/registry.py` & `qbraid-core-0.1.1/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/retry.py` & `qbraid-core-0.1.1/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/__init__.py` & `qbraid-core-0.1.1/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/client.py` & `qbraid-core-0.1.1/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/create.py` & `qbraid-core-0.1.1/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/paths.py` & `qbraid-core-0.1.1/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/state.py` & `qbraid-core-0.1.1/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/validate.py` & `qbraid-core-0.1.1/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/__init__.py` & `qbraid-core-0.1.1/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/adapter.py` & `qbraid-core-0.1.1/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/client.py` & `qbraid-core-0.1.1/qbraid_core/services/quantum/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,16 +50,23 @@
         except RequestsApiError as err:
             raise QuantumServiceRequestError("Failed to retrieve device data") from err
 
     def search_jobs(self, query: Optional[Dict[str, Any]] = None) -> List[Dict[str, Any]]:
         """Returns a list of quantum jobs run by the user that match the given query filters."""
         query = query or {}
 
+        max_results = query.pop("maxResults", None)
+        if max_results is not None:
+            query["resultsPerPage"] = max_results
+
         try:
-            return self.session.get("/quantum-jobs", params=query).json()
+            jobs_data = self.session.get("/quantum-jobs", params=query).json()
+            if "jobsArray" in jobs_data:
+                return jobs_data["jobsArray"]
+            return jobs_data
         except RequestsApiError as err:
             raise QuantumServiceRequestError("Failed to retrieve job data") from err
 
     def get_device(
         self,
         qbraid_id: Optional[str] = None,
         vendor_id: Optional[str] = None,
```

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/proxy.py` & `qbraid-core-0.1.1/qbraid_core/services/quantum/proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/session.py` & `qbraid-core-0.1.1/qbraid_core/sessions.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,161 +5,241 @@
 Module for making requests to the qBraid API.
 
 """
 import configparser
 import logging
 import os
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from urllib.parse import urljoin
 
+import requests
 import urllib3
-from requests import RequestException, Response, Session
 from requests.adapters import HTTPAdapter
 
+from .config import DEFAULT_CONFIG_SECTION, DEFAULT_ENDPOINT_URL, load_config, save_config
 from .exceptions import AuthError, ConfigError, RequestsApiError, UserNotFoundError
 from .registry import client_registry, discover_services
 from .retry import STATUS_FORCELIST, PostForcelistRetry
 
 if TYPE_CHECKING:
     import qbraid_core
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_ENDPOINT_URL = "https://api.qbraid.com/api"
-DEFAULT_CONFIG_PATH = os.path.join(os.path.expanduser("~"), ".qbraid", "qbraidrc")
-DEFAULT_CONFIG_SECTION = "default"
 
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-
-
-class QbraidSession(Session):  # pylint: disable=too-many-instance-attributes
+class Session(requests.Session):
     """Custom session with handling of request urls and authentication.
 
-    This is a child class of :py:class:`requests.Session`. It handles qbraid
-    authentication with custom headers, has SSL verification disabled
-    for compatibility with lab, and returns all responses as jsons for
-    convenience in the sdk.
-
-    Args:
-        user_email: qBraid / JupyterHub User.
-        api_key: Authenticated qBraid API key.
-        refresh_token: Authenticated qBraid refresh-token.
-        id_token: Authenticated qBraid id-token.
-        base_url: Base URL for the session's requests.
-        retries_total: Number of total retries for the requests.
-        retries_connect: Number of connect retries for the requests.
-        backoff_factor: Backoff factor between retry attempts.
-
+    This is a child class of :py:class:`requests.Session`. It handles
+    authentication with custom headers,and retries on specific 5xx errors.
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        user_email: Optional[str] = None,
-        api_key: Optional[str] = None,
-        refresh_token: Optional[str] = None,
-        id_token: Optional[str] = None,
+        *args,
         base_url: Optional[str] = None,
+        headers: Optional[Dict[str, Any]] = None,
+        auth_headers: Optional[Dict[str, Any]] = None,
         retries_total: int = 2,
         retries_connect: int = 1,
         backoff_factor: float = 0.5,
-    ) -> None:
-        super().__init__()
+        **kwargs,
+    ):
+        """
+        Initialize custom session with default base_url and auth_headers.
 
-        self.user_email = user_email
-        self.api_key = api_key
-        self.refresh_token = refresh_token
-        self.id_token = id_token
+        Args:
+            base_url (optional, str): Base URL to prepend to all requests.
+            headers (optional, dict): Dictionary of headers to include in all requests.
+            auth_headers (optional, dict): Dictionary of authorization headers to include in all
+                                           requests. Values will be masked in error messages.
+            retries_total (int): Number of total retries for the requests. Default 2.
+            retries_connect (int): Number of connect retries for the requests. Default 1.
+            backoff_factor (float): Backoff factor (seconds) between retry attempts. Default 0.5.
+        """
+        super().__init__(*args, **kwargs)
         self.base_url = base_url
-        self.verify = False
-        self.headers.update({"domain": "qbraid"})
-
+        self.auth_headers = {}
+        if auth_headers:
+            self.auth_headers.update(auth_headers)
+        if headers:
+            self.headers.update(headers)
+        self.headers.update(self.auth_headers)
         self._initialize_retry(retries_total, retries_connect, backoff_factor)
-
-    def __del__(self) -> None:
-        """qbraid session destructor. Closes the session."""
-        self.close()
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     @property
     def base_url(self) -> Optional[str]:
-        """Return the qbraid api url."""
+        """Return the base URL."""
         return self._base_url
 
     @base_url.setter
     def base_url(self, value: Optional[str]) -> None:
-        """Set the qbraid api url."""
-        url = value or self.get_config_variable("url")
-        self._base_url = url or DEFAULT_ENDPOINT_URL
+        """Set the base URL."""
+        self._base_url = value
 
-    @property
-    def user_email(self) -> Optional[str]:
-        """Return the session user email."""
-        return self._user_email
+    def _initialize_retry(
+        self, retries_total: int, retries_connect: int, backoff_factor: float
+    ) -> None:
+        """Set the session retry policy.
 
-    @user_email.setter
-    def user_email(self, value: Optional[str]) -> None:
-        """Set the session user email."""
-        user_email = value or self.get_config_variable("email")
-        self._user_email = user_email or os.getenv("JUPYTERHUB_USER")
-        if user_email:
-            self.headers.update({"email": user_email})  # type: ignore[attr-defined]
+        Args:
+            retries_total (int): Number of total retries for the requests.
+            retries_connect (int): Number of connect retries for the requests.
+            backoff_factor (float): Backoff factor between retry attempts.
+        """
+        retry = PostForcelistRetry(
+            total=retries_total,
+            connect=retries_connect,
+            backoff_factor=backoff_factor,
+            status_forcelist=STATUS_FORCELIST,
+        )
+
+        retry_adapter = HTTPAdapter(max_retries=retry)
+        self.mount("http://", retry_adapter)
+        self.mount("https://", retry_adapter)
+
+    def request(self, method: str, url: str, *args, **kwargs) -> requests.Response:
+        """Construct, prepare, and send a ``Request``.
+        Override the request method to prepend base_url to the URL and include additional headers.
+
+        Args:
+            method (str): HTTP method (e.g., 'get', 'post').
+            url (str): URL for the request. Prepend base_url if url is a relative URL.
+            **kwargs: Additional arguments for the request
+
+        Returns:
+            Response object.
+
+        Raises:
+            RequestsApiError: If the request failed.
+        """
+        # Prepend the base_url if it is provided and the url is relative
+        if self.base_url and not url.startswith(("http://", "https://")):
+            base_url = self.base_url.rstrip("/") + "/"
+            url = url.lstrip("/")
+            url = urljoin(base_url, url)
+
+        try:
+            response = super().request(method, url, *args, **kwargs)
+            response.raise_for_status()
+        except requests.RequestException as err:
+            # Wrap requests exceptions for compatibility.
+            message = str(err)
+            if err.response is not None:
+                try:
+                    error_json = err.response.json()["error"]
+                    msg = error_json["message"]
+                    code = error_json["code"]
+                    message += f". {msg}, Error code: {code}."
+                    logger.debug(
+                        "Response uber-trace-id: %s", err.response.headers["uber-trace-id"]
+                    )
+                except Exception:  # pylint: disable=broad-except
+                    # the response did not contain the expected json.
+                    message += f". {err.response.text}"
+
+            for _, value in self.auth_headers.items():
+                message = message.replace(value, "...")
+
+            raise RequestsApiError(message) from err
+
+        return response
+
+
+class QbraidSession(Session):  # pylint: disable=too-many-instance-attributes
+    """Custom session with handling of request urls and authentication.
+
+    This is a child class of :py:class:`qbraid_core.sessions.Session`.
+    It handles qbraid authentication with custom headers and has SSL
+    verification disabled for compatibility with qBraid Lab.
+    """
+
+    def __init__(self, *args, api_key: Optional[str] = None, **kwargs) -> None:
+        """Initialize custom session with default base_url and auth_headers.
+
+        Args:
+            api_key (optional, str): Authenticated qBraid API key.
+        """
+        self.api_key = api_key
+        self.user_email = kwargs.pop("user_email", None)
+        self.refresh_token = kwargs.pop("refresh_token", None)
+        self.verify = False
+
+        if "headers" not in kwargs:
+            kwargs["headers"] = {}
+        if "domain" not in kwargs["headers"]:
+            kwargs["headers"]["domain"] = kwargs.pop("pool", "qbraid")
+
+        if "auth_headers" not in kwargs:
+            kwargs["auth_headers"] = {}
+        if self.api_key:
+            kwargs["auth_headers"]["api-key"] = self.api_key
+        if self.refresh_token:
+            kwargs["auth_headers"]["refresh-token"] = self.refresh_token
+        if self.user_email:
+            kwargs["auth_headers"]["email"] = self.user_email
+        super().__init__(*args, **kwargs)
+
+    @Session.base_url.setter
+    def base_url(self, value: Optional[str]) -> None:
+        """Set the qbraid api url."""
+        url = value or self.get_config("url")
+        value = url or DEFAULT_ENDPOINT_URL
+        value = value.rstrip("/") + "/"
+        super(QbraidSession, QbraidSession).base_url.fset(self, value)
 
     @property
     def api_key(self) -> Optional[str]:
         """Return the api key."""
         return self._api_key
 
     @api_key.setter
     def api_key(self, value: Optional[str]) -> None:
         """Set the api key."""
-        api_key = value or self.get_config_variable("api-key")
+        api_key = value or self.get_config("api-key")
         self._api_key = api_key or os.getenv("QBRAID_API_KEY")
-        if api_key:
-            self.headers.update({"api-key": api_key})  # type: ignore[attr-defined]
+
+    @property
+    def user_email(self) -> Optional[str]:
+        """Return the session user email."""
+        return self._user_email
+
+    @user_email.setter
+    def user_email(self, value: Optional[str]) -> None:
+        """Set the session user email."""
+        user_email = value or self.get_config("email")
+        self._user_email = user_email or os.getenv("JUPYTERHUB_USER")
 
     @property
     def refresh_token(self) -> Optional[str]:
         """Return the session refresh token."""
         return self._refresh_token
 
     @refresh_token.setter
     def refresh_token(self, value: Optional[str]) -> None:
         """Set the session refresh token."""
-        refresh_token = value or self.get_config_variable("refresh-token")
-        self._refresh_token = refresh_token or os.getenv(
-            "QBRAID_REFRESH_TOKEN", os.getenv("REFRESH")
-        )  # keep REFRESH for backwards compatibility
-        if refresh_token:
-            self.headers.update({"refresh-token": refresh_token})  # type: ignore[attr-defined]
-
-    @property
-    def id_token(self) -> Optional[str]:
-        """Return the session id token."""
-        return self._id_token
-
-    @id_token.setter
-    def id_token(self, value: Optional[str]) -> None:
-        """Set the session id token."""
-        id_token = value or self.get_config_variable("id-token")
-        self._id_token = id_token or os.getenv("QBRAID_ID_TOKEN")
-        if id_token and "refresh-token" not in self.headers:
-            self.headers.update({"id-token": id_token})  # type: ignore[attr-defined]
+        refresh_token = value or self.get_config("refresh-token")
+        self._refresh_token = refresh_token or os.getenv("REFRESH")
 
-    def get_config_variable(self, config_name: str) -> Optional[str]:
+    def get_config(self, config_name: str) -> Optional[str]:
         """Returns the config value of specified config.
 
         Args:
             config_name: The name of the config
         """
-        filepath = DEFAULT_CONFIG_PATH
-        if os.path.isfile(filepath):
-            config = configparser.ConfigParser()
-            config.read(filepath)
-            section = DEFAULT_CONFIG_SECTION
-            if section in config.sections():
-                if config_name in config[section]:
-                    return config[section][config_name]
+        try:
+            config = load_config()
+        except ConfigError:
+            return None
+
+        section = DEFAULT_CONFIG_SECTION
+        if section in config.sections():
+            if config_name in config[section]:
+                return config[section][config_name]
         return None
 
     def get_user(self) -> Dict[str, Any]:
         """Get user metadata.
 
         Returns:
             Dictionary containing user metadata.
@@ -173,75 +253,56 @@
             raise UserNotFoundError from err
 
         if not metadata:
             raise UserNotFoundError("User metadata invalid or not found.")
 
         return metadata
 
-    def save_config(  # pylint: disable=too-many-arguments,too-many-branches
-        self,
-        user_email: Optional[str] = None,
-        api_key: Optional[str] = None,
-        refresh_token: Optional[str] = None,
-        id_token: Optional[str] = None,
-        base_url: Optional[str] = None,
+    def save_config(
+        self, api_key: Optional[str] = None, base_url: Optional[str] = None, **kwargs
     ) -> None:
         """Create qbraidrc file. In qBraid Lab, qbraidrc is automatically present in filesystem.
 
-        Args:
-            user_email:  JupyterHub User.
-            api_key: Authenticated qBraid api-key.
-            refresh_token: Authenticated qBraid refresh-token.
-            id_token: Authenticated qBraid id-token.
-            base_url: Base URL for the session's requests.
-
         Raises:
             UserNotFoundError: If user metadata is invalid or not found.
             AuthError: If there is a credential mismatch.
             ConfigError: If there is an error saving the config.
         """
-        self.user_email = user_email or self.user_email
         self.api_key = api_key or self.api_key
-        self.refresh_token = refresh_token or self.refresh_token
-        self.id_token = id_token or self.id_token
         self.base_url = base_url or self.base_url
+        self.user_email = kwargs.get("user_email", self.user_email)
+        self.refresh_token = kwargs.get("refresh_token", self.refresh_token)
 
         res_json = self.get_user()
         res_email = res_json.get("email")
 
         if self.user_email and self.user_email != res_email:
             raise AuthError(
                 f"Credential mismatch: Session initialized for '{self.user_email}', \
                     but API key corresponds to '{res_email}'."
             )
 
         try:
-            filepath = DEFAULT_CONFIG_PATH
-
-            if not os.path.isfile(filepath):
-                os.makedirs(os.path.dirname(filepath), exist_ok=True)
             config = configparser.ConfigParser()
             section = DEFAULT_CONFIG_SECTION
             if section not in config.sections():
                 config.add_section(section)
             if self.user_email:
                 config.set(section, "email", self.user_email)
             if self.api_key:
                 config.set(section, "api-key", self.api_key)
             if self.refresh_token:
                 config.set(section, "refresh-token", self.refresh_token)
-            if self.id_token:
-                config.set(section, "id-token", self.id_token)
             if self.base_url:
                 config.set(section, "url", self.base_url)
-            with open(filepath, "w", encoding="utf-8") as cfgfile:
-                config.write(cfgfile)
         except Exception as err:
             raise ConfigError from err
 
+        save_config(config)
+
     def get_available_services(self) -> List[str]:
         """
         Get a list of available services that can be loaded as low-level
         clients via :py:meth:`Session.client`.
 
         Returns:
             List: List of service names.
@@ -254,74 +315,13 @@
 
         Args:
             service_name: Name of the service.
 
         Returns:
             qbraid_core.QbraidClient: Client for the specified service.
         """
+        if len(client_registry) == 0:
+            self.get_available_services()
         client_class = client_registry.get(service_name)
         if not client_class:
             raise ValueError(f"Service '{service_name}' not registered")
         return client_class(session=self)
-
-    def _initialize_retry(
-        self, retries_total: int, retries_connect: int, backoff_factor: float
-    ) -> None:
-        """Set the session retry policy.
-
-        Args:
-            retries_total: Number of total retries for the requests.
-            retries_connect: Number of connect retries for the requests.
-            backoff_factor: Backoff factor between retry attempts.
-        """
-        retry = PostForcelistRetry(
-            total=retries_total,
-            connect=retries_connect,
-            backoff_factor=backoff_factor,
-            status_forcelist=STATUS_FORCELIST,
-        )
-
-        retry_adapter = HTTPAdapter(max_retries=retry)
-        self.mount("http://", retry_adapter)
-        self.mount("https://", retry_adapter)
-
-    def request(self, method: str, url: str, **kwargs: Any) -> Response:  # type: ignore[override]
-        """Construct, prepare, and send a ``Request``.
-
-        Args:
-            method: Method for the new request (e.g. ``POST``).
-            url: URL for the new request.
-            **kwargs: Additional arguments for the request.
-        Returns:
-            Response object.
-        Raises:
-            RequestsApiError: If the request failed.
-        """
-        # pylint: disable=arguments-differ
-        final_url = self.base_url + url
-
-        headers = self.headers.copy()
-        headers.update(kwargs.pop("headers", {}))
-
-        try:
-            response = super().request(method, final_url, headers=headers, **kwargs)
-            response.raise_for_status()
-        except RequestException as ex:
-            # Wrap requests exceptions for compatibility.
-            message = str(ex)
-            if ex.response is not None:
-                try:
-                    error_json = ex.response.json()["error"]
-                    msg = error_json["message"]
-                    code = error_json["code"]
-                    message += f". {msg}, Error code: {code}."
-                    logger.debug("Response uber-trace-id: %s", ex.response.headers["uber-trace-id"])
-                except Exception:  # pylint: disable=broad-except
-                    # the response did not contain the expected json.
-                    message += f". {ex.response.text}"
-
-            if self.refresh_token:
-                message = message.replace(self.refresh_token, "...")
-
-            raise RequestsApiError(message) from ex
-
-        return response
```

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/system/__init__.py` & `qbraid-core-0.1.1/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/system/executables.py` & `qbraid-core-0.1.1/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/system/generic.py` & `qbraid-core-0.1.1/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/system/packages.py` & `qbraid-core-0.1.1/qbraid_core/system/packages.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core/system/threader.py` & `qbraid-core-0.1.1/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core.egg-info/PKG-INFO` & `qbraid-core-0.1.1/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.0.dev4
+Version: 0.1.1
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -12,20 +12,19 @@
 Keywords: qbraid,quantum,cloud
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `qbraid-core-0.1.0.dev4/qbraid_core.egg-info/SOURCES.txt` & `qbraid-core-0.1.1/qbraid_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 docs/api/qbraid_core.rst
 docs/api/qbraid_core.services.rst
 docs/api/qbraid_core.system.rst
 qbraid_core/__init__.py
 qbraid_core/_compat.py
 qbraid_core/_version.py
 qbraid_core/client.py
+qbraid_core/config.py
 qbraid_core/exceptions.py
 qbraid_core/registry.py
 qbraid_core/retry.py
-qbraid_core/session.py
+qbraid_core/sessions.py
 qbraid_core.egg-info/PKG-INFO
 qbraid_core.egg-info/SOURCES.txt
 qbraid_core.egg-info/dependency_links.txt
 qbraid_core.egg-info/requires.txt
 qbraid_core.egg-info/top_level.txt
 qbraid_core/services/__init__.py
 qbraid_core/services/environments/__init__.py
@@ -58,13 +59,14 @@
 qbraid_core/system/generic.py
 qbraid_core/system/packages.py
 qbraid_core/system/threader.py
 tests/__init__.py
 tests/conftest.py
 tests/test_client.py
 tests/test_compat.py
+tests/test_config.py
 tests/test_environments.py
 tests/test_session.py
 tests/test_system.py
 tests/fixtures/__init__.py
 tests/fixtures/environments.py
 tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.0.dev4/tests/fixtures/environments.py` & `qbraid-core-0.1.1/tests/fixtures/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Module containing environment fixtures for unit tests.
 
 """
 import os
 
 import pytest
 
-from qbraid_core.session import QbraidSession
+from qbraid_core.sessions import QbraidSession
 
 qbraid_refresh_token = os.getenv("REFRESH")
 qbraid_api_key = os.getenv("QBRAID_API_KEY")
 qbraid_user = os.getenv("JUPYTERHUB_USER")
 
 
 @pytest.fixture
```

### Comparing `qbraid-core-0.1.0.dev4/tests/test_client.py` & `qbraid-core-0.1.1/tests/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import os
 
 import pytest
 
 from qbraid_core.client import QbraidClient
-from qbraid_core.session import QbraidSession
+from qbraid_core.sessions import QbraidSession
 
 skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS", "False").lower() != "true"
 REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of qBraid storage)"
 
 
 @pytest.mark.parametrize(
     "test_case",
@@ -25,15 +25,17 @@
         ("", False),
         ("507f1f77bcf86cd79943901Z", False),
     ],
 )
 def test_is_valid_object_id(test_case):
     """Test that the is_valid_mongo_id function works as expected."""
     mongo_id, is_valid = test_case
-    assert QbraidClient._is_valid_object_id(mongo_id) == is_valid
+    # pylint: disable-next=protected-access
+    test_is_valid = QbraidClient._is_valid_object_id(mongo_id)
+    assert test_is_valid == is_valid
 
 
 def test_convert_email_symbols():
     """Test function that converts email to username."""
     email_input = "test-format.company_org@qbraid.com"
     expected_output = "test-2dformat-2ecompany-5forg-40qbraid-2ecom"
     # pylint: disable-next=protected-access
```

### Comparing `qbraid-core-0.1.0.dev4/tests/test_compat.py` & `qbraid-core-0.1.1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/tests/test_environments.py` & `qbraid-core-0.1.1/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/tests/test_session.py` & `qbraid-core-0.1.1/tests/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,45 +6,35 @@
 custom user configurations and required run-command pre-sets.
 
 """
 import os
 
 import pytest
 
+from qbraid_core.config import DEFAULT_CONFIG_PATH
 from qbraid_core.exceptions import AuthError, RequestsApiError, UserNotFoundError
-from qbraid_core.session import (
-    DEFAULT_CONFIG_PATH,
-    STATUS_FORCELIST,
-    PostForcelistRetry,
-    QbraidSession,
-)
+from qbraid_core.sessions import STATUS_FORCELIST, PostForcelistRetry, QbraidSession
 
-qbraidrc_path = os.path.join(os.path.expanduser("~"), ".qbraid", "qbraidrc")
-
-# These environment variables don't actually exist in qBraid Lab, but instead
-# are set and used for convenience for local development and testing.
 qbraid_refresh_token = os.getenv("REFRESH")
 qbraid_api_key = os.getenv("QBRAID_API_KEY")
-
-# This is the only environment variable that actually exists in qBraid Lab
 qbraid_user = os.getenv("JUPYTERHUB_USER")
 
 skip_remote_tests: bool = os.getenv("QBRAID_RUN_REMOTE_TESTS", "False").lower() != "true"
 REASON = "QBRAID_RUN_REMOTE_TESTS not set (requires configuration of qBraid storage)"
 
 
-def _remove_id_token_qbraidrc():
+def _remove_line_qbraidrc(key):
     """Remove id-token from qbraidrc file."""
     try:
         with open(DEFAULT_CONFIG_PATH, "r", encoding="utf-8") as file:
             lines = file.readlines()
 
         with open(DEFAULT_CONFIG_PATH, "w", encoding="utf-8") as file:
             for line in lines:
-                if not line.startswith("id-token"):
+                if not line.startswith(key):
                     file.write(line)
     except FileNotFoundError:
         pass
 
 
 def test_api_error():
     """Test raising error when making invalid API request."""
@@ -60,40 +50,40 @@
     assert session.refresh_token == refresh_token
     del session
 
 
 @pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_qbraid_config_overwrite_with_id_token():
     """Test setting/saving id-token and then test overwritting config value"""
-    dummy_id_token = "alice123"
-    dummy_id_token_overwrite = "bob456"
-    session = QbraidSession(id_token=dummy_id_token)
-    assert session.id_token == dummy_id_token
+    dummy_api_key = "alice123"
+    dummy_api_key_overwrite = "bob456"
+    session = QbraidSession(refresh_token=dummy_api_key)
+    assert session.refresh_token == dummy_api_key
     session.save_config()
-    assert session.get_config_variable("id-token") == dummy_id_token
-    session.save_config(id_token=dummy_id_token_overwrite)
-    assert session.get_config_variable("id-token") == dummy_id_token_overwrite
-    _remove_id_token_qbraidrc()
+    assert session.get_config("refresh-token") == dummy_api_key
+    session.save_config(refresh_token=dummy_api_key_overwrite)
+    assert session.get_config("refresh-token") == dummy_api_key_overwrite
+    _remove_line_qbraidrc("refresh-token")
 
 
 @pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_qbraid_session_api_key():
     """Test initializing QbraidSession without args and then saving config."""
     session = QbraidSession()
     session.save_config(api_key=qbraid_api_key, user_email=qbraid_user)
-    assert session.get_config_variable("api-key") == qbraid_api_key
+    assert session.get_config("api-key") == qbraid_api_key
 
 
 @pytest.mark.skipif(skip_remote_tests, reason=REASON)
 def test_qbraid_session_save_config():
     """Test initializing QbraidSession without args and then saving config."""
     session = QbraidSession()
     session.save_config(user_email=qbraid_user, refresh_token=qbraid_refresh_token)
-    assert session.get_config_variable("email") == qbraid_user
-    assert session.get_config_variable("refresh-token") == qbraid_refresh_token
+    assert session.get_config("email") == qbraid_user
+    assert session.get_config("refresh-token") == qbraid_refresh_token
 
 
 def test_qbraid_session_credential_mismatch_error():
     """Test initializing QbraidSession with mismatched email and apiKey."""
     session = QbraidSession(api_key=qbraid_api_key, user_email="fakeuser@email.com")
     with pytest.raises(AuthError):
         session.save_config()
```

### Comparing `qbraid-core-0.1.0.dev4/tests/test_system.py` & `qbraid-core-0.1.1/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev4/tools/verify_headers.py` & `qbraid-core-0.1.1/tools/verify_headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,14 +169,11 @@
 
     # Check if at least two arguments are provided and the first argument is not a flag
     if len(sys.argv) < 2 or sys.argv[1].startswith("--"):
         print("Usage: python verify_headers.py SRC [OPTIONS] ...")
         sys.exit(1)
 
     skip_files = ["qbraid_core/_version.py"]
-    script_directory = os.path.dirname(os.path.abspath(__file__))
-    project_directory = os.path.abspath(os.path.join(script_directory, ".."))
-    skip_files = [os.path.join(project_directory, file_path) for file_path in skip_files]
 
     fix = "--fix" in sys.argv
     files_and_dirs = [arg for arg in sys.argv[1:] if arg != "--fix"]
     verify_headers(files_and_dirs, fix=fix, skip_files=skip_files)
```

