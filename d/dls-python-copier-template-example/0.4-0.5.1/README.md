# Comparing `tmp/dls-python-copier-template-example-0.4.tar.gz` & `tmp/dls-python-copier-template-example-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-python-copier-template-example-0.4.tar", last modified: Wed Mar 20 16:52:55 2024, max compression
+gzip compressed data, was "dls-python-copier-template-example-0.5.1.tar", last modified: Wed Apr 10 09:55:04 2024, max compression
```

## Comparing `dls-python-copier-template-example-0.4.tar` & `dls-python-copier-template-example-0.5.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.381237 dls-python-copier-template-example-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.373237 dls-python-copier-template-example-0.4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.373237 dls-python-copier-template-example-0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.369238 dls-python-copier-template-example-0.4/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.373237 dls-python-copier-template-example-0.4/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.373237 dls-python-copier-template-example-0.4/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.373237 dls-python-copier-template-example-0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_container.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.373237 dls-python-copier-template-example-0.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-03-20 16:52:55.381237 dls-python-copier-template-example-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/genindex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/how-to/run-container.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 16:52:55.381237 dls-python-copier-template-example-0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.369238 dls-python-copier-template-example-0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.381237 dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-03-20 16:52:55.000000 dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-20 16:52:55.000000 dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 16:52:55.000000 dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-20 16:52:55.000000 dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-20 16:52:55.000000 dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-20 16:52:55.000000 dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/src/python_copier_template_example/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/src/python_copier_template_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/src/python_copier_template_example/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-20 16:52:55.000000 dls-python-copier-template-example-0.4/src/python_copier_template_example/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:52:55.377237 dls-python-copier-template-example-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-20 16:52:46.000000 dls-python-copier-template-example-0.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.225790 dls-python-copier-template-example-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.213791 dls-python-copier-template-example-0.5.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.213791 dls-python-copier-template-example-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.209791 dls-python-copier-template-example-0.5.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.213791 dls-python-copier-template-example-0.5.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.213791 dls-python-copier-template-example-0.5.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_container.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16444 2024-04-10 09:55:04.221790 dls-python-copier-template-example-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/how-to/run-container.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.217790 dls-python-copier-template-example-0.5.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:55:04.225790 dls-python-copier-template-example-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.209791 dls-python-copier-template-example-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.221790 dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16444 2024-04-10 09:55:04.000000 dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-10 09:55:04.000000 dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:55:04.000000 dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 09:55:04.000000 dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-10 09:55:04.000000 dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 09:55:04.000000 dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.221790 dls-python-copier-template-example-0.5.1/src/python_copier_template_example/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/src/python_copier_template_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/src/python_copier_template_example/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 09:55:04.000000 dls-python-copier-template-example-0.5.1/src/python_copier_template_example/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:55:04.221790 dls-python-copier-template-example-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-10 09:54:59.000000 dls-python-copier-template-example-0.5.1/tests/test_cli.py
```

### Comparing `dls-python-copier-template-example-0.4/.copier-answers.yml` & `dls-python-copier-template-example-0.5.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.devcontainer/devcontainer.json` & `dls-python-copier-template-example-0.5.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/CONTRIBUTING.md` & `dls-python-copier-template-example-0.5.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/actions/install_requirements/action.yml` & `dls-python-copier-template-example-0.5.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/dependabot.yml` & `dls-python-copier-template-example-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/pages/make_switcher.py` & `dls-python-copier-template-example-0.5.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/workflows/_check.yml` & `dls-python-copier-template-example-0.5.1/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/workflows/_container.yml` & `dls-python-copier-template-example-0.5.1/.github/workflows/_container.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/workflows/_dist.yml` & `dls-python-copier-template-example-0.5.1/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/workflows/_docs.yml` & `dls-python-copier-template-example-0.5.1/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/workflows/_release.yml` & `dls-python-copier-template-example-0.5.1/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/workflows/_test.yml` & `dls-python-copier-template-example-0.5.1/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.github/workflows/ci.yml` & `dls-python-copier-template-example-0.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.gitignore` & `dls-python-copier-template-example-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.pre-commit-config.yaml` & `dls-python-copier-template-example-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/.vscode/launch.json` & `dls-python-copier-template-example-0.5.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/Dockerfile` & `dls-python-copier-template-example-0.5.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/LICENSE` & `dls-python-copier-template-example-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/PKG-INFO` & `dls-python-copier-template-example-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-python-copier-template-example
-Version: 0.4
+Version: 0.5.1
 Summary: An expanded https://github.com/DiamondLightSource/python-copier-template to illustrate how it looks with all the options enabled.
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -257,14 +257,15 @@
 
 ```python
 from python_copier_template_example import __version__
 
 print(f"Hello python_copier_template_example {__version__}")
 ```
 
+
 Or if it is a commandline tool then you might put some example commands here:
 
 ```
 python -m python_copier_template_example --version
 ```
 
 <!-- README only content. Anything below this line won't be included in index.md -->
```

### Comparing `dls-python-copier-template-example-0.4/README.md` & `dls-python-copier-template-example-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 ```python
 from python_copier_template_example import __version__
 
 print(f"Hello python_copier_template_example {__version__}")
 ```
 
+
 Or if it is a commandline tool then you might put some example commands here:
 
 ```
 python -m python_copier_template_example --version
 ```
 
 <!-- README only content. Anything below this line won't be included in index.md -->
```

### Comparing `dls-python-copier-template-example-0.4/docs/conf.py` & `dls-python-copier-template-example-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `dls-python-copier-template-example-0.5.1/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/docs/images/dls-logo.svg` & `dls-python-copier-template-example-0.5.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/docs/index.md` & `dls-python-copier-template-example-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/docs/tutorials/installation.md` & `dls-python-copier-template-example-0.5.1/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/pyproject.toml` & `dls-python-copier-template-example-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/PKG-INFO` & `dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-python-copier-template-example
-Version: 0.4
+Version: 0.5.1
 Summary: An expanded https://github.com/DiamondLightSource/python-copier-template to illustrate how it looks with all the options enabled.
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -257,14 +257,15 @@
 
 ```python
 from python_copier_template_example import __version__
 
 print(f"Hello python_copier_template_example {__version__}")
 ```
 
+
 Or if it is a commandline tool then you might put some example commands here:
 
 ```
 python -m python_copier_template_example --version
 ```
 
 <!-- README only content. Anything below this line won't be included in index.md -->
```

### Comparing `dls-python-copier-template-example-0.4/src/dls_python_copier_template_example.egg-info/SOURCES.txt` & `dls-python-copier-template-example-0.5.1/src/dls_python_copier_template_example.egg-info/SOURCES.txt`

 * *Files identical despite different names*

