# Comparing `tmp/qbraid-cli-0.8.0.dev1.tar.gz` & `tmp/qbraid-cli-0.8.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-cli-0.8.0.dev1.tar", last modified: Thu Feb 29 14:52:50 2024, max compression
+gzip compressed data, was "qbraid-cli-0.8.0.dev3.tar", last modified: Wed Apr 10 17:23:03 2024, max compression
```

## Comparing `qbraid-cli-0.8.0.dev1.tar` & `qbraid-cli-0.8.0.dev3.tar`

### file list

```diff
@@ -1,97 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.env-example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.132495 qbraid-cli-0.8.0.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.132495 qbraid-cli-0.8.0.dev1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.132495 qbraid-cli-0.8.0.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/MANIFEST.IN
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.132495 qbraid-cli-0.8.0.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.136495 qbraid-cli-0.8.0.dev1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.136495 qbraid-cli-0.8.0.dev1/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.136495 qbraid-cli-0.8.0.dev1/docs/_static/style/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/style/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/_static/style/s4defs-roles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.140495 qbraid-cli-0.8.0.dev1/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/configure.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/devices-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/envs-activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/envs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/envs-uninstall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/envs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/jobs-add.rst
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/jobs-disable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/jobs-enable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/jobs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/cli/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.140495 qbraid-cli-0.8.0.dev1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.140495 qbraid-cli-0.8.0.dev1/qbraid_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-29 14:52:49.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.140495 qbraid-cli-0.8.0.dev1/qbraid_cli/configure/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/configure/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.140495 qbraid-cli-0.8.0.dev1/qbraid_cli/credits/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/credits/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.140495 qbraid-cli-0.8.0.dev1/qbraid_cli/devices/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/devices/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.140495 qbraid-cli-0.8.0.dev1/qbraid_cli/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/envs/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/envs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/envs/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/qbraid_cli/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/jobs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/jobs/toggle_braket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/qbraid_cli/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/kernels/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/qbraid_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-02-29 14:52:50.000000 qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-29 14:52:50.000000 qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 14:52:50.000000 qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-29 14:52:50.000000 qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-29 14:52:50.000000 qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-29 14:52:50.000000 qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/tests/test_envs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:52:50.144496 qbraid-cli-0.8.0.dev1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-02-29 14:52:36.000000 qbraid-cli-0.8.0.dev1/tools/split_rst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.453631 qbraid-cli-0.8.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.421630 qbraid-cli-0.8.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.421630 qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.425630 qbraid-cli-0.8.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/MANIFEST.IN
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 17:23:03.453631 qbraid-cli-0.8.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.425630 qbraid-cli-0.8.0.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.425630 qbraid-cli-0.8.0.dev3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.429630 qbraid-cli-0.8.0.dev3/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.429630 qbraid-cli-0.8.0.dev3/docs/_static/style/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/style/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/style/s4defs-roles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.433630 qbraid-cli-0.8.0.dev3/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/devices-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs-activate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs-uninstall.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-add.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-disable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-enable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.433630 qbraid-cli-0.8.0.dev3/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.433630 qbraid-cli-0.8.0.dev3/qbraid_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/credits/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/toggle_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/kernels/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:23:03.453631 qbraid-cli-0.8.0.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_configure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/test_configure_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/test_prompt_for_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/test_validate_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_credits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_credits/test_credits_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_devices/test_devices_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_devices/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_activate_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_find_shell_rc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_print_activate_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_create_qbraid_env_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_update_state_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_is_valid_env_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_request_delete_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_validate_env_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_aws_configure_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_disable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_enable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_get_package_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_handle_jobs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_run_progress_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_validate_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tests/test_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_kernels/test_kernels_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tools/split_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tools/verify_headers.py
```

### Comparing `qbraid-cli-0.8.0.dev1/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/.github/workflows/docs.yml` & `qbraid-cli-0.8.0.dev3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/.github/workflows/main.yml` & `qbraid-cli-0.8.0.dev3/.github/workflows/main.yml`

 * *Files 16% similar despite different names*

```diff
@@ -19,31 +19,32 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: pip
       - name: Upgrade pip and install build tools
         run: |
-          python -m pip install --upgrade pip
+          pip install --upgrade pip
           pip install setuptools wheel build
       - name: Build the package
         run: |
           python -m build
       - name: Upload built package
         uses: actions/upload-artifact@v3
         with:
           name: built-package
           path: dist/*.whl
 
   test:
     needs: build
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.9', '3.10', '3.11']
+        os: [ubuntu-latest, windows-latest]
+        python-version: ['3.9', '3.10', '3.11', '3.12']
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
@@ -51,14 +52,21 @@
       - name: Download built package
         uses: actions/download-artifact@v3
         with:
           name: built-package
           path: dist
       - name: Install package
         run: |
-          pip install dist/*.whl
+          if ($env:RUNNER_OS -eq "Windows") {
+            Get-ChildItem dist/*.whl | ForEach-Object { pip install $_.FullName }
+          } else {
+            pip install dist/*.whl
+          }
+        shell: pwsh
       - name: Install testing dependencies
         run: |
           pip install pytest
       - name: Run tests with pytest
         run: |
-          pytest
+          pytest
+        env:
+          QBRAID_API_KEY: ${{ secrets.QBRAID_API_KEY }}
```

### Comparing `qbraid-cli-0.8.0.dev1/.github/workflows/publish.yml` & `qbraid-cli-0.8.0.dev3/.github/workflows/test-publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-name: Publish to PyPI
+name: Publish to TestPyPI
 
 on:
-  release:
-    types: [published]
   workflow_dispatch:
 
 jobs:
   pypi-publish:
-    name: Build dist & upload to PyPI
+    name: Build dist & upload to TestPyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 1
 
       - name: Set up Python
@@ -19,13 +17,13 @@
         with:
           python-version: '3.10'
 
       - name: Build binary wheel + source tarball
         run: |
           python3 -m pip install --upgrade pip build
           python3 -m build
-
-      - name: Publish package to PyPI
+      - name: Publish package to TestPyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `qbraid-cli-0.8.0.dev1/.gitignore` & `qbraid-cli-0.8.0.dev3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -157,8 +157,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
```

### Comparing `qbraid-cli-0.8.0.dev1/.readthedocs.yml` & `qbraid-cli-0.8.0.dev3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/CONTRIBUTING.md` & `qbraid-cli-0.8.0.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/Makefile` & `qbraid-cli-0.8.0.dev3/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/PKG-INFO` & `qbraid-cli-0.8.0.dev3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev1
+Version: 0.8.0.dev3
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
-Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html
+Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
 Project-URL: Launch on Lab, https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git
 Keywords: qbraid,cli,quantum,cloud
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
+Classifier: License :: Other/Proprietary License
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: typer[all]
-Requires-Dist: rich
-Requires-Dist: requests
-Requires-Dist: jupyter_client
-Requires-Dist: qbraid==0.5.1
+Requires-Dist: typer>=0.12.1
+Requires-Dist: rich>=10.11.0
+Requires-Dist: jupyter_client<9.0.0,>=7.0.0
+Requires-Dist: qbraid-core>=0.1.1
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -42,14 +44,16 @@
 Requires-Dist: toml; extra == "docs"
 Requires-Dist: build; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
+[![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
+[![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
 [![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/KugF6Cnncm)
 
 Command Line Interface for interacting with all parts of the qBraid platform.
 
 The **qBraid CLI** is a specialized command-line interface tool designed *exclusively* for use within the [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) platform. It is not intended for local installations or use outside the qBraid Lab environment. This tool ensures seamless integration and optimized performance specifically tailored for qBraid Lab's unique cloud-based quantum computing ecosystem.
 
@@ -78,15 +82,15 @@
      |_|                         
 
 
 - Use 'qbraid --help' to see available commands.
 
 - Use 'qbraid --version' to see the current version.
 
-Reference Docs: https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html
+Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 ```
 
 A qBraid CLI command has the following structure:
 
 ```shell
 $ qbraid <command> <subcommand> [options and parameters]
 ```
```

### Comparing `qbraid-cli-0.8.0.dev1/README.md` & `qbraid-cli-0.8.0.dev3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
+[![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
+[![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
 [![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/KugF6Cnncm)
 
 Command Line Interface for interacting with all parts of the qBraid platform.
 
 The **qBraid CLI** is a specialized command-line interface tool designed *exclusively* for use within the [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) platform. It is not intended for local installations or use outside the qBraid Lab environment. This tool ensures seamless integration and optimized performance specifically tailored for qBraid Lab's unique cloud-based quantum computing ecosystem.
 
@@ -34,15 +36,15 @@
      |_|                         
 
 
 - Use 'qbraid --help' to see available commands.
 
 - Use 'qbraid --version' to see the current version.
 
-Reference Docs: https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html
+Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 ```
 
 A qBraid CLI command has the following structure:
 
 ```shell
 $ qbraid <command> <subcommand> [options and parameters]
 ```
```

### Comparing `qbraid-cli-0.8.0.dev1/docs/Makefile` & `qbraid-cli-0.8.0.dev3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/api-key.png` & `qbraid-cli-0.8.0.dev3/docs/_static/api-key.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/cards/jupyter.png` & `qbraid-cli-0.8.0.dev3/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/cards/python.png` & `qbraid-cli-0.8.0.dev3/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/cards/terminal.png` & `qbraid-cli-0.8.0.dev3/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/favicon.ico` & `qbraid-cli-0.8.0.dev3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/logo.png` & `qbraid-cli-0.8.0.dev3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/style/custom.css` & `qbraid-cli-0.8.0.dev3/docs/_static/style/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/_static/style/s4defs-roles.css` & `qbraid-cli-0.8.0.dev3/docs/_static/style/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/configure.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/configure.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/devices-list.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/devices-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/envs-activate.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/envs-activate.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/envs-list.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/envs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/envs-uninstall.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/envs-uninstall.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/envs.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/envs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/jobs-add.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/jobs-add.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/jobs-disable.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/jobs-disable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/jobs-enable.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/jobs-enable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/jobs-list.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/jobs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/jobs.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/kernels.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/kernels.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/cli/qbraid.rst` & `qbraid-cli-0.8.0.dev3/docs/cli/qbraid.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/conf.py` & `qbraid-cli-0.8.0.dev3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/guide/overview.rst` & `qbraid-cli-0.8.0.dev3/docs/guide/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
        |_|                     
 
 
    - Use `qbraid --help` to see available commands.
 
    - Use `qbraid --version` to display the current version.
 
-   Reference Docs: https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html
+   Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 
 
 **List environments** installed in your qBraid Lab instance using:
 
 .. code-block:: console
    
    $ qbraid envs list
```

### Comparing `qbraid-cli-0.8.0.dev1/docs/index.rst` & `qbraid-cli-0.8.0.dev3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/docs/make.bat` & `qbraid-cli-0.8.0.dev3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev1/pyproject.toml` & `qbraid-cli-0.8.0.dev3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-cli"
-version = "0.8.0.dev1"
+version = "0.8.0.dev3"
 description = "Command Line Interface for interacting with all parts of the qBraid platform."
 readme = "README.md"
 authors = [{ name = "qBraid Development Team", email = "contact@qbraid.com" }]
 license = { text = "Proprietary" }
 keywords = ["qbraid", "cli", "quantum", "cloud"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
-    "Intended Audience :: System Administrators",
     "Natural Language :: English",
+    "License :: Other/Proprietary License",
+    "Intended Audience :: System Administrators",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "typer[all]",
-    "rich",
-    "requests",
-    "jupyter_client",
-    "qbraid==0.5.1"
+    "typer>=0.12.1",
+    "rich>=10.11.0",
+    "jupyter_client>=7.0.0,<9.0.0",
+    "qbraid-core>=0.1.1",
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
-Documentation = "https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html"
+Documentation = "https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html"
 "Bug Tracker" = "https://github.com/qBraid/qBraid-Lab/issues"
 Discord = "https://discord.gg/KugF6Cnncm"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git"
 
 [project.optional-dependencies]
 jobs = ["amazon-braket-sdk>=1.48.1"]
 dev = ["black", "isort", "pylint", "pytest"]
@@ -48,14 +50,15 @@
 qbraid = "qbraid_cli.main:app"
 
 [tool.setuptools_scm]
 write_to = "qbraid_cli/_version.py"
 
 [tool.black]
 line-length = 100
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
@@ -68,8 +71,8 @@
 [tool.pylint.MASTER]
 ignore-paths = [
   "^.*\\_version.py$",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-ra"
-testpaths = ["tests"]
+testpaths = ["tests"]
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/envs/activate.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/envs/activate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Module supporting 'qbraid envs activate' command.
 
 """
 
 import os
 from pathlib import Path
@@ -27,36 +30,36 @@
 def print_activate_command(venv_path: Path) -> None:
     """Prints the command to activate the virtual environment with improved formatting."""
     typer.echo("To activate this environment, use command:\n")
     if os.name == "nt":
         # Windows operating system
         activate_script = venv_path / "Scripts" / "activate"
         activate_script_ps = venv_path / "Scripts" / "Activate.ps1"
-        typer.echo("    " + str(activate_script))
+        typer.echo("\t$ " + str(activate_script))
         typer.echo("\nOr for PowerShell, use:\n")
-        typer.echo("    " + f"& {activate_script_ps}")
+        typer.echo("\t$ " + f"& {activate_script_ps}")
     else:
         # Unix-like operating systems (Linux/macOS)
         activate_script = venv_path / "bin" / "activate"
-        typer.echo("    " + f"source {activate_script}")
+        typer.echo("\t$ " + f"source {activate_script}")
     typer.echo("")
     raise typer.Exit()
 
 
 def activate_pyvenv(venv_path: Path):
     """Activate the virtual environment."""
     shell_path = os.environ.get("SHELL")
 
     if shell_path is None:
         print_activate_command(venv_path)
-
+        return  # Return early since we can't proceed without a shell
     try:
         shell_rc = find_shell_rc(shell_path)
     except (FileNotFoundError, ValueError):
         print_activate_command(venv_path)
-
+        return  # Return early since no suitable shell rc file was found
     bin_path = str(venv_path / "bin")
 
     os.system(
         f"cat {shell_rc} {bin_path}/activate > {bin_path}/activate2 && "
         f"{shell_path} --rcfile {bin_path}/activate2"
     )
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/envs/app.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/envs/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,48 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Module defining commands in the 'qbraid envs' namespace.
 
 """
 
-import json
-import keyword
-import re
 import shutil
 import subprocess
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 import typer
 from rich.console import Console
 
+from qbraid_cli.envs.data_handling import installed_envs_data, request_delete_env, validate_env_name
 from qbraid_cli.handlers import QbraidException, run_progress_task
 
-app = typer.Typer(help="Manage qBraid environments.")
-
-
-def is_valid_env_name(env_name: str) -> bool:  # pylint: disable=too-many-return-statements
-    """
-    Validates a Python virtual environment name against best practices.
-
-    This function checks if the given environment name is valid based on certain
-    criteria, including length, use of special characters, reserved names, and
-    operating system-specific restrictions.
-
-    Args:
-        env_name (str): The name of the Python virtual environment to validate.
-
-    Returns:
-        bool: True if the name is valid, False otherwise.
-
-    Raises:
-        ValueError: If the environment name is not a string or is empty.
-    """
-    # Basic checks for empty names or purely whitespace names
-    if not env_name or env_name.isspace():
-        return False
-
-    # Check for invalid characters, including shell metacharacters and spaces
-    if re.search(r'[<>:"/\\|?*\s&;()$[\]#~!{}]', env_name):
-        return False
-
-    if env_name.startswith("tmp"):
-        return False
-
-    # Reserved names for Windows (example list, can be expanded)
-    reserved_names = [
-        "CON",
-        "PRN",
-        "AUX",
-        "NUL",
-        "COM1",
-        "COM2",
-        "COM3",
-        "COM4",
-        "COM5",
-        "COM6",
-        "COM7",
-        "COM8",
-        "COM9",
-        "LPT1",
-        "LPT2",
-        "LPT3",
-        "LPT4",
-        "LPT5",
-        "LPT6",
-        "LPT7",
-        "LPT8",
-        "LPT9",
-    ]
-    if env_name.upper() in reserved_names:
-        return False
-
-    if len(env_name) > 20:
-        return False
-
-    # Check against Python reserved words
-    if keyword.iskeyword(env_name):
-        return False
-
-    # Check if it starts with a number, which is not a good practice
-    if env_name[0].isdigit():
-        return False
-
-    return True
-
-
-def validate_env_name(value: str) -> str:
-    """Validate environment name."""
-    if not is_valid_env_name(value):
-        raise typer.BadParameter(
-            f"Invalid environment name '{value}'. " "Please use a valid Python environment name."
-        )
-    return value
-
-
-def installed_envs_data() -> Tuple[Dict[str, Path], Dict[str, str]]:
-    """Gather paths and aliases for all installed qBraid environments."""
-    from qbraid.api.system import get_qbraid_envs_paths, is_valid_slug
-
-    installed = {}
-    aliases = {}
-
-    qbraid_env_paths: List[Path] = get_qbraid_envs_paths()
-
-    for env_path in qbraid_env_paths:
-        for entry in env_path.iterdir():
-            if entry.is_dir() and is_valid_slug(entry.name):
-                installed[entry.name] = entry
+envs_app = typer.Typer(help="Manage qBraid environments.")
 
-                if entry.name == "qbraid_000000":
-                    aliases["default"] = entry.name
-                    continue
 
-                state_json_path = entry / "state.json"
-                if state_json_path.exists():
-                    try:
-                        with open(state_json_path, "r", encoding="utf-8") as f:
-                            data = json.load(f)
-                        aliases[data.get("name", entry.name[:-7])] = entry.name
-                    # pylint: disable-next=broad-exception-caught
-                    except (json.JSONDecodeError, Exception):
-                        aliases[entry.name[:-7]] = entry.name
-                else:
-                    aliases[entry.name[:-7]] = entry.name
-
-    return installed, aliases
-
-
-def request_delete_env(slug: str) -> str:
-    """Send request to delete environment given slug."""
-    from qbraid.api import QbraidSession, RequestsApiError
-
-    session = QbraidSession()
-
-    try:
-        session.delete(f"/environments/{slug}")
-    except RequestsApiError as err:
-        raise QbraidException("Delete environment request failed") from err
-
-
-@app.command(name="create")
+@envs_app.command(name="create")
 def envs_create(  # pylint: disable=too-many-statements
     name: str = typer.Option(
         ..., "--name", "-n", help="Name of the environment to create", callback=validate_env_name
     ),
     description: Optional[str] = typer.Option(
         None, "--description", "-d", help="Short description of the environment"
     ),
+    auto_confirm: bool = typer.Option(
+        False, "--yes", "-y", help="Automatically answer 'yes' to all prompts"
+    ),
 ) -> None:
     """Create a new qBraid environment."""
     from .create import create_qbraid_env_assets, create_venv
 
     def request_new_env(req_body: Dict[str, str]) -> Dict[str, Any]:
         """Send request to create new environment and return the slug."""
-        from qbraid.api import QbraidSession, RequestsApiError
+        from qbraid_core import QbraidSession, RequestsApiError
 
         session = QbraidSession()
 
         try:
             env_data = session.post("/environments/create", json=req_body).json()
         except RequestsApiError as err:
             raise QbraidException("Create environment request failed") from err
@@ -172,17 +52,17 @@
                 "Create environment request responsed with invalid environment data"
             )
 
         return env_data
 
     def gather_local_data() -> Tuple[Path, str]:
         """Gather environment data and return the slug."""
-        from qbraid.api.system import get_qbraid_envs_paths
+        from qbraid_core.services.environments import get_default_envs_paths
 
-        env_path = get_qbraid_envs_paths()[0]
+        env_path = get_default_envs_paths()[0]
 
         result = subprocess.run(
             [sys.executable, "--version"],
             capture_output=True,
             text=True,
             check=True,
         )
@@ -233,15 +113,15 @@
     typer.echo(f"  shellPrompt: {prompt}")
     typer.echo(f"  kernelName: {kernel_name}")
 
     typer.echo("\n\n## Environment Plan ##\n")
     typer.echo(f"  location: {slug_path}")
     typer.echo(f"  version: {python_version}\n")
 
-    user_confirmation = typer.confirm("Proceed", default=True)
+    user_confirmation = auto_confirm or typer.confirm("Proceed", default=True)
     typer.echo("")
     if not user_confirmation:
         request_delete_env(slug)
         typer.echo("qBraidSystemExit: Exiting.")
         raise typer.Exit()
 
     run_progress_task(
@@ -272,17 +152,20 @@
     typer.echo(f"#     $ qbraid envs activate {name}")
     typer.echo("#")
     typer.echo("# To deactivate an active environment, use")
     typer.echo("#")
     typer.echo("#     $ deactivate")
 
 
-@app.command(name="remove")
+@envs_app.command(name="remove")
 def envs_remove(
-    name: str = typer.Option(..., "-n", "--name", help="Name of the environment to remove")
+    name: str = typer.Option(..., "-n", "--name", help="Name of the environment to remove"),
+    auto_confirm: bool = typer.Option(
+        False, "--yes", "-y", help="Automatically answer 'yes' to all prompts"
+    ),
 ) -> None:
     """Delete a qBraid environment."""
 
     def gather_local_data(env_name: str) -> Tuple[Path, str]:
         """Get environment path and slug from name (alias)."""
         installed, aliases = installed_envs_data()
         for alias, slug in aliases.items():
@@ -300,16 +183,15 @@
         f"located at '{slug_path}'.\n"
         "This will remove all local packages and permanently delete all "
         "of its associated qBraid environment metadata.\n"
         "This operation CANNOT be undone.\n\n"
         "Are you sure you want to continue?"
     )
 
-    # Ask for user confirmation
-    if typer.confirm(confirmation_message, abort=True):
+    if auto_confirm or typer.confirm(confirmation_message, abort=True):
         typer.echo("")
         run_progress_task(
             request_delete_env,
             slug,
             description="Deleting remote environment data...",
             error_message="Failed to delete qBraid environment",
         )
@@ -317,56 +199,57 @@
         run_progress_task(
             shutil.rmtree,
             slug_path,
             description="Deleting local environment...",
             error_message="Failed to delete qBraid environment",
         )
         typer.echo(f"\nEnvironment '{name}' successfully removed.")
-        # console = Console()
-        # console.print(
-        #     f"\n[bold green]Successfully deleted qBraid environment: "
-        #     f"[/bold green][bold magenta]{name}[/bold magenta]\n"
-        # )
 
 
-@app.command(name="list")
+@envs_app.command(name="list")
 def envs_list():
     """List installed qBraid environments."""
     installed, aliases = installed_envs_data()
 
+    console = Console()
+
     if len(installed) == 0:
-        print("No qBraid environments installed.")
-        print("\nUse 'qbraid envs create' to create a new environment.")
+        console.print(
+            "No qBraid environments installed.\n\n"
+            + "Use 'qbraid envs create' to create a new environment.",
+            style="yellow",
+        )
         return
 
     alias_path_pairs = [(alias, installed[slug_name]) for alias, slug_name in aliases.items()]
-
     sorted_alias_path_pairs = sorted(
         alias_path_pairs,
         key=lambda x: (x[0] != "default", str(x[1]).startswith(str(Path.home())), x[0]),
     )
 
     current_env_path = Path(sys.executable).parent.parent.parent
 
     max_alias_length = (
-        max(len(alias) for alias, _ in sorted_alias_path_pairs) if sorted_alias_path_pairs else 0
-    )
-    max_path_length = (
-        max(len(str(path)) for _, path in sorted_alias_path_pairs) if sorted_alias_path_pairs else 0
+        max(len(str(alias)) for alias, envpath in sorted_alias_path_pairs)
+        if sorted_alias_path_pairs
+        else 0
     )
 
     print("# qbraid environments:")
     print("#")
     print("")
+
     for alias, path in sorted_alias_path_pairs:
-        mark = "*  " if path == current_env_path else "   "
-        print(f"{alias.ljust(max_alias_length + 7)}{mark}{str(path).ljust(max_path_length)}")
+        mark = "*" if path == current_env_path else " "
+        # Format each line with spacing based on the longest alias for alignment
+        line = f"{alias.ljust(max_alias_length+3)}{mark} {path}"  # fix the most optimal spacing
+        console.print(line)
 
 
-@app.command(name="activate")
+@envs_app.command(name="activate")
 def envs_activate(
     name: str = typer.Argument(..., help="Name of the environment. Values from 'qbraid envs list'.")
 ):
     """Activate qBraid environment.
 
     NOTE: Currently only works on qBraid Lab platform, and select few other OS types.
     """
@@ -380,8 +263,8 @@
 
     from .activate import activate_pyvenv
 
     activate_pyvenv(venv_path)
 
 
 if __name__ == "__main__":
-    app()
+    envs_app()
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/envs/create.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/envs/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Module supporting 'qbraid envs create' command.
 
 """
 
 import json
 import os
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/exceptions.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Module defining custom exceptions for the qBraid CLI.
 
 """
 
 from typing import Optional
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/handlers.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Module providing application support utilities, including abstractions for error handling
 and executing operations with progress tracking within the qBraid CLI.
 
 """
 
 import traceback
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/jobs/app.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,69 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Module defining commands in the 'qbraid jobs' namespace.
 
 """
 
 import sys
-from typing import Callable, Dict, Optional, Tuple
+from typing import Any, Callable, Dict, Tuple
 
 import typer
 from rich.console import Console
 
-from qbraid_cli.handlers import handle_error, run_progress_task, validate_item
-
-app = typer.Typer(help="Manage qBraid quantum jobs.")
-
-QJOB_LIBS = ["braket"]
-
-
-def validate_library(value: str) -> str:
-    """Validate quantum jobs library."""
-    return validate_item(value, QJOB_LIBS, "Library")
-
-
-def get_state(library: Optional[str] = None) -> Dict[str, Tuple[bool, bool]]:
-    """Get the state of qBraid Quantum Jobs for the specified library."""
-    from qbraid.api.system import qbraid_jobs_state
-
-    state_values = {}
-
-    if library:
-        libraries_to_check = [library]
-    else:
-        libraries_to_check = QJOB_LIBS
-
-    for lib in libraries_to_check:
-        state_values[lib] = qbraid_jobs_state(lib)
-
-    return state_values
-
-
-def run_progress_get_state(library: Optional[str] = None) -> Dict[str, Tuple[bool, bool]]:
-    """Run get state function with rich progress UI."""
-    return run_progress_task(
-        get_state,
-        library,
-        description="Collecting package metadata...",
-        error_message=f"Failed to collect {library} package metadata.",
-    )
-
+from qbraid_cli.handlers import handle_error, run_progress_task
+from qbraid_cli.jobs.toggle_braket import disable_braket, enable_braket
+from qbraid_cli.jobs.validation import handle_jobs_state, run_progress_get_state, validate_library
 
-def handle_jobs_state(
-    library: str,
-    action: str,  # 'enable' or 'disable'
-    action_callback: Callable[[], None],
-) -> None:
-    """Handle the common logic for enabling or disabling qBraid Quantum Jobs."""
-    state_values: Dict[str, Tuple[bool, bool]] = run_progress_get_state(library)
-    installed, enabled = state_values[library]
-
-    if not installed:
-        handle_error(message=f"{library} not installed.")
-    if (enabled and action == "enable") or (not enabled and action == "disable"):
-        action_color = "green" if enabled else "red"
-        console = Console()
-        console.print(
-            f"\nqBraid quantum jobs already [bold {action_color}]{action}d[/bold {action_color}] "
-            f"for [magenta]{library}[/magenta]."
-        )
-        console.print(
-            "To check the state of all quantum jobs libraries in this environment, "
-            "use: `[bold]qbraid jobs state[/bold]`"
-        )
-        raise typer.Exit()
+jobs_app = typer.Typer(help="Manage qBraid quantum jobs.")
 
-    action_callback()  # Perform the specific enable/disable action
 
-
-@app.command(name="enable")
+@jobs_app.command(name="enable")
 def jobs_enable(
     library: str = typer.Argument(
         ..., help="Software library with quantum jobs support.", callback=validate_library
-    )
+    ),
+    auto_confirm: bool = typer.Option(
+        False, "--yes", "-y", help="Automatically answer 'yes' to all prompts"
+    ),
 ) -> None:
     """Enable qBraid Quantum Jobs."""
 
     def enable_action():
         if library == "braket":
-            from .toggle_braket import enable_braket
-
-            enable_braket()
+            enable_braket(auto_confirm=auto_confirm)
         else:
             raise RuntimeError(f"Unsupported device library: '{library}'.")
 
     handle_jobs_state(library, "enable", enable_action)
 
 
-@app.command(name="disable")
+@jobs_app.command(name="disable")
 def jobs_disable(
     library: str = typer.Argument(
         ..., help="Software library with quantum jobs support.", callback=validate_library
-    )
+    ),
+    auto_confirm: bool = typer.Option(
+        False, "--yes", "-y", help="Automatically answer 'yes' to all prompts"
+    ),
 ) -> None:
     """Disable qBraid Quantum Jobs."""
 
     def disable_action():
         if library == "braket":
-            from .toggle_braket import disable_braket
-
-            disable_braket()
+            disable_braket(auto_confirm=auto_confirm)
         else:
             raise RuntimeError(f"Unsupported device library: '{library}'.")
 
     handle_jobs_state(library, "disable", disable_action)
 
 
-@app.command(name="state")
+@jobs_app.command(name="state")
 def jobs_state(
     library: str = typer.Argument(
         default=None,
         help="Optional: Specify a software library with quantum jobs support to check its status.",
         callback=validate_library,
     )
 ) -> None:
@@ -138,32 +84,67 @@
             "[green]enabled"
             if enabled and installed
             else "[red]disabled" if installed else "[grey70]unavailable"
         )
         console.print(f"{lib:<{padding-1}}", state_str, end="\n")
 
 
-@app.command(name="list")
+@jobs_app.command(name="list")
 def jobs_list(
     limit: int = typer.Option(
         10, "--limit", "-l", help="Limit the maximum number of results returned"
     )
 ) -> None:
     """List qBraid Quantum Jobs."""
 
-    def import_jobs() -> Tuple[Callable, Exception]:
-        from qbraid import get_jobs
-        from qbraid.exceptions import QbraidError
+    def import_jobs() -> Tuple[Any, Callable]:
+        from qbraid_core.services.quantum import QuantumClient, process_job_data
+
+        client = QuantumClient()
 
-        return get_jobs, QbraidError
+        return client, process_job_data
 
-    result: Tuple[Callable, Exception] = run_progress_task(import_jobs)
-    get_jobs, QbraidError = result
+    result: Tuple[Any, Callable] = run_progress_task(import_jobs)
+    client, process_job_data = result
+    # https://github.com/qBraid/api/issues/644
+    # raw_data = client.search_jobs(query={"numResults": limit})
+    raw_data = client.search_jobs(query={})
+    job_data, msg = process_job_data(raw_data)
+    job_data = job_data[:limit]
 
+    longest_job_id = max(len(item[0]) for item in job_data)
+    spacing = longest_job_id + 5
     try:
-        get_jobs(filters={"numResults": limit})
-    except QbraidError:
+        console = Console()
+        header_1 = "Job ID"
+        header_2 = "Submitted"
+        header_3 = "Status"
+        console.print(f"\n[bold]{header_1.ljust(spacing)}{header_2.ljust(36)}{header_3}[/bold]")
+        for job_id, submitted, status in job_data:
+            if status == "COMPLETED":
+                status_color = "green"
+            elif status in ["FAILED", "CANCELLED"]:
+                status_color = "red"
+            elif status in [
+                "INITIALIZING",
+                "INITIALIZED",
+                "CREATED",
+                "QUEUED",
+                "VALIDATING",
+                "RUNNING",
+            ]:
+                status_color = "blue"
+            else:
+                status_color = "grey"
+            console.print(
+                f"{job_id.ljust(spacing)}{submitted.ljust(35)}",
+                f"[{status_color}]{status}[/{status_color}]",
+            )
+
+        console.print(f"\n{msg}", style="italic", justify="left")
+
+    except Exception:  # pylint: disable=broad-exception-caught
         handle_error(message="Failed to fetch quantum jobs.")
 
 
 if __name__ == "__main__":
-    app()
+    jobs_app()
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/jobs/toggle_braket.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/toggle_braket.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Module supporting 'qbraid jobs enable/disable braket' and commands.
 
 """
 
 import logging
 import os
 import subprocess
 import sys
 from pathlib import Path
 from typing import Optional, Tuple
 
 import typer
+from qbraid_core.system import (
+    QbraidSystemError,
+    get_active_site_packages_path,
+    get_latest_package_version,
+    get_local_package_version,
+)
 
 from qbraid_cli.exceptions import QbraidException
 from qbraid_cli.handlers import handle_error, handle_filesystem_operation, run_progress_task
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
@@ -29,30 +38,24 @@
         Tuple[str, str, str]: The installed and latest versions of the package, and the
                               local site-packages path where it is / would be installed.
 
     Raises:
         QbraidException: If package version or location data cannot be retrieved.
 
     """
-    from qbraid.api.system import (
-        get_active_site_packages_path,
-        get_latest_package_version,
-        get_local_package_version,
-    )
-    from qbraid.exceptions import QbraidError
 
     try:
         installed_version = get_local_package_version(package)
         latest_version = get_latest_package_version(package)
-    except QbraidError as err:
+    except QbraidSystemError as err:
         raise QbraidException("Failed to retrieve package version information") from err
 
     try:
         site_packages_path = get_active_site_packages_path()
-    except QbraidError as err:
+    except QbraidSystemError as err:
         raise QbraidException("Failed to retrieve site-package location") from err
 
     return installed_version, latest_version, site_packages_path
 
 
 def confirm_updates(
     mode: str,
@@ -66,17 +69,14 @@
     Args:
         mode (str): The mode of operation, either "enable" or "disable".
         site_packages_path (str): The location of the site-packages directory where
                                   target package(s) will be updated.
         installed_version (optional, str): The installed version of the target package.
         latest_version (optional, str): The latest version of the target package available on PyPI.
 
-    Returns:
-        None
-
     Raises:
         ValueError: If an invalid mode is provided.
         typer.Exit: If the user declines to proceed with enabling or disabling qBraid Quantum Jobs.
 
     """
     core_package = "botocore"
     versioned_package = "boto3"
@@ -150,47 +150,49 @@
 
     try:
         handle_filesystem_operation(configure_aws, aws_dir)
     except QbraidException:
         handle_error(message="Failed to configure qBraid quantum jobs.")
 
 
-def enable_braket():
+def enable_braket(auto_confirm: bool = False):
     """Enable qBraid quantum jobs for Amazon Braket."""
-    installed_version, latest_version, site_packages_path = run_progress_task(
+    installed, latest, path = run_progress_task(
         get_package_data, "boto3", description="Solving environment..."
     )
-    confirm_updates("enable", site_packages_path, installed_version, latest_version)
-    aws_configure_dummy()  # TODO: possibly add another confirmation for writing aws config files
 
+    if not auto_confirm:
+        confirm_updates("enable", path, installed_version=installed, latest_version=latest)
+
+    aws_configure_dummy()  # TODO: possibly add another confirmation for writing aws config files
     try:
         subprocess.check_call([sys.executable, "-m", "pip", "install", "--upgrade", "boto3"])
         subprocess.check_call(
             [sys.executable, "-m", "pip", "uninstall", "botocore", "-y", "--quiet"]
         )
         subprocess.check_call(
             [sys.executable, "-m", "pip", "install", "git+https://github.com/qBraid/botocore.git"]
         )
     except subprocess.CalledProcessError:
         handle_error(message="Failed to enable qBraid quantum jobs.")
 
     typer.secho("\nSuccessfully enabled qBraid quantum jobs.", fg=typer.colors.GREEN, bold=True)
-    typer.secho(
-        "\nTo disable, run: `qbraid jobs disable braket`\n", fg=typer.colors.GREEN, bold=True
-    )
+    typer.secho("\nTo disable, run: \n\n\t$ qbraid jobs disable braket\n")
 
 
-def disable_braket():
+def disable_braket(auto_confirm: bool = False):
     """Disable qBraid quantum jobs for Amazon Braket."""
     package = "botocore"
-    installed_version, latest_version, site_packages_path = run_progress_task(
+    installed, latest, path = run_progress_task(
         get_package_data, package, description="Solving environment..."
     )
-    package = f"{package}~={installed_version}" if installed_version < latest_version else package
-    confirm_updates("disable", site_packages_path)
+    package = f"{package}~={installed}" if installed < latest else package
+
+    if not auto_confirm:
+        confirm_updates("disable", path)
 
     try:
         subprocess.check_call(
             [
                 sys.executable,
                 "-m",
                 "pip",
@@ -200,8 +202,8 @@
             ],
             stderr=subprocess.DEVNULL,
         )
     except subprocess.CalledProcessError:
         handle_error(message="Failed to disable qBraid quantum jobs.")
 
     typer.secho("\nSuccessfully disabled qBraid quantum jobs.", fg=typer.colors.GREEN, bold=True)
-    typer.secho("\nTo enable, run: `qbraid jobs enable braket`\n", fg=typer.colors.GREEN, bold=True)
+    typer.secho("\nTo enable, run: \n\n\t$ qbraid jobs enable braket\n")
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli/main.py` & `qbraid-cli-0.8.0.dev3/qbraid_cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Entrypoint for the qBraid CLI.
 
 """
 
 import typer
+import urllib3
 
-from .configure import app as configure_app
-from .credits import app as credits_app
-from .devices import app as devices_app
-from .envs import app as envs_app
-from .jobs import app as jobs_app
-from .kernels import app as kernels_app
+from qbraid_cli.configure.app import configure_app
+from qbraid_cli.credits.app import credits_app
+from qbraid_cli.devices.app import devices_app
+from qbraid_cli.envs.app import envs_app
+from qbraid_cli.jobs.app import jobs_app
+from qbraid_cli.kernels.app import kernels_app
 
-app = typer.Typer()
+app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 app.add_typer(configure_app, name="configure")
 app.add_typer(envs_app, name="envs")
 app.add_typer(jobs_app, name="jobs")
 app.add_typer(devices_app, name="devices")
 app.add_typer(kernels_app, name="kernels")
 app.add_typer(credits_app, name="credits")
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
 
 def version_callback(value: bool):
     """Show the version and exit."""
     if value:
         from ._version import __version__
 
         typer.echo(f"qbraid-cli/{__version__}")
@@ -46,23 +52,24 @@
     typer.echo("     |_|                         ")
     typer.echo("")
     typer.echo("")
     typer.echo("- Use 'qbraid --help' to see available commands.")
     typer.echo("")
     typer.echo("- Use 'qbraid --version' to see the current version.")
     typer.echo("")
-    typer.echo("Reference Docs: https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html")
+    typer.echo("Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html")
 
 
 @app.callback(invoke_without_command=True)
 def main(
     ctx: typer.Context,
     version: bool = typer.Option(
         None,
         "--version",
+        "-v",
         callback=version_callback,
         is_eager=True,
         help="Show the version and exit.",
     ),
 ):
     """The qBraid CLI."""
     if ctx.invoked_subcommand is None and not version:
```

### Comparing `qbraid-cli-0.8.0.dev1/qbraid_cli.egg-info/PKG-INFO` & `qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev1
+Version: 0.8.0.dev3
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
-Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html
+Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
 Project-URL: Launch on Lab, https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git
 Keywords: qbraid,cli,quantum,cloud
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
+Classifier: License :: Other/Proprietary License
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: typer[all]
-Requires-Dist: rich
-Requires-Dist: requests
-Requires-Dist: jupyter_client
-Requires-Dist: qbraid==0.5.1
+Requires-Dist: typer>=0.12.1
+Requires-Dist: rich>=10.11.0
+Requires-Dist: jupyter_client<9.0.0,>=7.0.0
+Requires-Dist: qbraid-core>=0.1.1
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -42,14 +44,16 @@
 Requires-Dist: toml; extra == "docs"
 Requires-Dist: build; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
+[![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
+[![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
 [![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/KugF6Cnncm)
 
 Command Line Interface for interacting with all parts of the qBraid platform.
 
 The **qBraid CLI** is a specialized command-line interface tool designed *exclusively* for use within the [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) platform. It is not intended for local installations or use outside the qBraid Lab environment. This tool ensures seamless integration and optimized performance specifically tailored for qBraid Lab's unique cloud-based quantum computing ecosystem.
 
@@ -78,15 +82,15 @@
      |_|                         
 
 
 - Use 'qbraid --help' to see available commands.
 
 - Use 'qbraid --version' to see the current version.
 
-Reference Docs: https://docs.qbraid.com/projects/cli/en/latest/cli/qbraid.html
+Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 ```
 
 A qBraid CLI command has the following structure:
 
 ```shell
 $ qbraid <command> <subcommand> [options and parameters]
 ```
```

### Comparing `qbraid-cli-0.8.0.dev1/tests/test_envs.py` & `qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_is_valid_env_name.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
-Tests for commands and helper functions in the 'qbraid envs' namespace.
+Unit tests for commands and helper functions in the 'qbraid envs' namespace.
 
 """
 
 import pytest
 
-from qbraid_cli.envs.app import is_valid_env_name
+from qbraid_cli.envs.data_handling import is_valid_env_name
 
 
 @pytest.mark.parametrize(
     "env_name, expected",
     [
         # Valid names
         ("valid_env", True),
```

### Comparing `qbraid-cli-0.8.0.dev1/tools/split_rst.py` & `qbraid-cli-0.8.0.dev3/tools/split_rst.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2024, qBraid Development Team
+# All rights reserved.
+
 """
 Script for splitting a reStructuredText (rst) file into
 multiple files based on sections.
 
 """
 
 import os
```

