# Comparing `tmp/ansible-dev-tools-24.2.0.tar.gz` & `tmp/ansible-dev-tools-24.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-dev-tools-24.2.0.tar", last modified: Fri Feb  9 15:01:38 2024, max compression
+gzip compressed data, was "ansible-dev-tools-24.2.1.tar", last modified: Wed Apr 10 14:24:22 2024, max compression
```

## Comparing `ansible-dev-tools-24.2.0.tar` & `ansible-dev-tools-24.2.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.524065 ansible-dev-tools-24.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.512065 ansible-dev-tools-24.2.0/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.516065 ansible-dev-tools-24.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.516065 ansible-dev-tools-24.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.516065 ansible-dev-tools-24.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-02-09 15:01:38.524065 ansible-dev-tools-24.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.516065 ansible-dev-tools-24.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/contributor-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.516065 ansible-dev-tools-24.2.0/docs/media/
--rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/media/ansible-lint.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/media/ansible-navigator-run.mp4
--rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/media/compress.sh
--rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/media/create-collection.mp4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.520065 ansible-dev-tools-24.2.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/building-collection.md
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/ci-setup.md
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/content-best-practices.md
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/content-release.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.520065 ansible-dev-tools-24.2.0/docs/user-guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/images/ci.png
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/images/release.png
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/docs/user-guide/testing.md
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 15:01:38.524065 ansible-dev-tools-24.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.508065 ansible-dev-tools-24.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.520065 ansible-dev-tools-24.2.0/src/ansible_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-09 15:01:38.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools/version_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.524065 ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-02-09 15:01:38.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-09 15:01:38.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 15:01:38.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-09 15:01:38.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-09 15:01:38.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 15:01:38.000000 ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.524065 ansible-dev-tools-24.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.524065 ansible-dev-tools-24.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/tests/integration/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:01:38.524065 ansible-dev-tools-24.2.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/tools/update-readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-09 15:01:23.000000 ansible-dev-tools-24.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.965574 ansible-dev-tools-24.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.953574 ansible-dev-tools-24.2.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.953574 ansible-dev-tools-24.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.953574 ansible-dev-tools-24.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.953574 ansible-dev-tools-24.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-10 14:24:22.965574 ansible-dev-tools-24.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.957574 ansible-dev-tools-24.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/contributor-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.957574 ansible-dev-tools-24.2.1/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/media/ansible-lint.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/media/ansible-navigator-run.mp4
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/media/compress.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/media/create-collection.mp4
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.957574 ansible-dev-tools-24.2.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/building-collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/ci-setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/content-best-practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/content-release.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.961574 ansible-dev-tools-24.2.1/docs/user-guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/images/ci.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/images/release.png
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/docs/user-guide/testing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:24:22.965574 ansible-dev-tools-24.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.949574 ansible-dev-tools-24.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.961574 ansible-dev-tools-24.2.1/src/ansible_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-10 14:24:22.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools/version_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.961574 ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-10 14:24:22.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-10 14:24:22.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:24:22.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 14:24:22.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-10 14:24:22.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 14:24:22.000000 ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.961574 ansible-dev-tools-24.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.961574 ansible-dev-tools-24.2.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/tests/integration/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:24:22.961574 ansible-dev-tools-24.2.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/tools/update-readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-10 14:24:10.000000 ansible-dev-tools-24.2.1/tox.ini
```

### Comparing `ansible-dev-tools-24.2.0/.config/constraints.txt` & `ansible-dev-tools-24.2.1/.config/constraints.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,144 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --all-extras --no-annotate --output-file=.config/constraints.txt --strip-extras pyproject.toml
 #
-ansible-builder==3.0.0
+ansible-builder==3.0.1
 ansible-compat==4.1.11
-ansible-core==2.16.3
-ansible-creator==24.2.0
+ansible-core==2.16.5
+ansible-creator==24.4.1
 ansible-dev-environment==24.1.0
-ansible-lint==24.2.0
+ansible-lint==24.2.1
 ansible-navigator==24.2.0
-ansible-runner==2.3.4
+ansible-runner==2.3.6
 ansible-sign==0.1.1
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
 bindep==2.11.0
-black==24.1.1
+black==24.3.0
 bracex==2.4
-build==1.0.3
-cachetools==5.3.2
+build==1.2.1
+cachetools==5.3.3
 cairocffi==1.6.1
 cairosvg==2.7.1
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 click-help-colors==0.9.4
 colorama==0.4.6
-coverage==7.4.1
-cryptography==42.0.2
+coverage==7.4.4
+cryptography==42.0.5
 csscompressor==0.9.5
 cssselect2==0.7.0
 defusedxml==0.7.1
 distlib==0.3.8
 distro==1.9.0
-dnspython==2.5.0
+dnspython==2.6.1
 docstring-parser-fork==0.0.5
 docutils==0.20.1
 enrich==1.2.7
 exceptiongroup==1.2.0
-execnet==2.0.2
-filelock==3.13.1
+execnet==2.1.0
+filelock==3.13.3
 ghp-import==2.1.0
-griffe==0.40.1
+griffe==0.42.1
 htmlmin2==0.1.13
-identify==2.5.33
+identify==2.5.35
 idna==3.6
 iniconfig==2.0.0
 jinja2==3.1.3
 jsmin==3.0.1
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 linkchecker==10.4.0
 lockfile==0.12.2
-markdown==3.5.2
+markdown==3.6
 markdown-exec==1.8.0
 markdown-include==0.8.1
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdurl==0.1.2
 mergedeep==1.3.4
 mkdocs==1.5.3
-mkdocs-ansible==24.2.1
-mkdocs-autorefs==0.5.0
+mkdocs-ansible==24.3.0
+mkdocs-autorefs==1.0.1
 mkdocs-gen-files==0.5.0
-mkdocs-htmlproofer-plugin==1.0.0
-mkdocs-material==9.5.8
+mkdocs-htmlproofer-plugin==1.2.0
+mkdocs-material==9.5.17
 mkdocs-material-extensions==1.3.1
 mkdocs-minify-plugin==0.8.0
 mkdocs-monorepo-plugin==1.1.0
-mkdocstrings==0.24.0
-mkdocstrings-python==1.8.0
+mkdocstrings==0.24.3
+mkdocstrings-python==1.9.2
 molecule==24.2.0
-mypy==1.8.0
+mypy==1.9.0
 mypy-extensions==1.0.0
 nodeenv==1.8.0
 onigurumacffi==1.3.0
-packaging==23.2
+packaging==24.0
 paginate==0.5.6
 parsley==1.3
 pathspec==0.12.1
 pbr==6.0.0
 pexpect==4.9.0
-pillow==10.2.0
-pip-tools==7.3.0
-pipdeptree==2.13.2
+pillow==10.3.0
+pip-tools==7.4.1
+pipdeptree==2.17.0
 platformdirs==4.2.0
 pluggy==1.4.0
-pre-commit==3.6.0
+pre-commit==3.7.0
 ptyprocess==0.7.0
-pycparser==2.21
-pydoclint==0.4.0
+pycparser==2.22
+pydoclint==0.4.1
 pygments==2.17.2
-pymdown-extensions==10.7
+pymdown-extensions==10.7.1
 pyproject-api==1.6.1
 pyproject-hooks==1.0.0
-pytest==8.0.0
+pytest==8.1.1
 pytest-ansible==24.1.2
 pytest-xdist==3.5.0
 python-daemon==3.0.1
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
 python-gnupg==0.5.2
 python-slugify==8.0.4
 pyyaml==6.0.1
 pyyaml-env-tag==0.1
-referencing==0.33.0
+referencing==0.34.0
 regex==2023.12.25
 requests==2.31.0
-requirements-parser==0.5.0
+requirements-parser==0.9.0
 resolvelib==1.0.1
-rich==13.7.0
-rpds-py==0.17.1
+rich==13.7.1
+rpds-py==0.18.0
 ruamel-yaml==0.18.6
 ruamel-yaml-clib==0.2.8
-ruff==0.2.1
+ruff==0.3.5
 six==1.16.0
 soupsieve==2.5
 subprocess-tee==0.4.1
 text-unidecode==1.3
 tinycss2==1.2.1
 toml-sort==0.23.1
 tomli==2.0.1
-tomlkit==0.12.3
-tox==4.12.1
+tomlkit==0.12.4
+tox==4.14.2
 tox-ansible==24.2.0
-types-setuptools==69.0.0.20240125
-typing-extensions==4.9.0
-tzdata==2023.4
-urllib3==2.2.0
-virtualenv==20.25.0
+types-setuptools==69.2.0.20240317
+typing-extensions==4.11.0
+tzdata==2024.1
+urllib3==2.2.1
+virtualenv==20.25.1
 watchdog==4.0.0
-wcmatch==8.5
+wcmatch==8.5.1
 webencodings==0.5.1
-wheel==0.42.0
-yamllint==1.34.0
+wheel==0.43.0
+yamllint==1.35.1
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `ansible-dev-tools-24.2.0/.config/requirements-lock.txt` & `ansible-dev-tools-24.2.1/.config/requirements-lock.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --no-annotate --output-file=.config/requirements-lock.txt --strip-extras pyproject.toml
 #
-ansible-builder==3.0.0
+ansible-builder==3.0.1
 ansible-compat==4.1.11
-ansible-core==2.16.3
-ansible-creator==24.2.0
+ansible-core==2.16.5
+ansible-creator==24.4.1
 ansible-dev-environment==24.1.0
-ansible-lint==24.2.0
+ansible-lint==24.2.1
 ansible-navigator==24.2.0
-ansible-runner==2.3.4
+ansible-runner==2.3.6
 ansible-sign==0.1.1
 attrs==23.2.0
 bindep==2.11.0
-black==24.1.1
+black==24.3.0
 bracex==2.4
-cachetools==5.3.2
+cachetools==5.3.3
 cffi==1.16.0
 chardet==5.2.0
 click==8.1.7
 click-help-colors==0.9.4
 colorama==0.4.6
-cryptography==42.0.2
+cryptography==42.0.5
 distlib==0.3.8
 distro==1.9.0
 docutils==0.20.1
 enrich==1.2.7
 exceptiongroup==1.2.0
-execnet==2.0.2
-filelock==3.13.1
+execnet==2.1.0
+filelock==3.13.3
 iniconfig==2.0.0
 jinja2==3.1.3
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 lockfile==0.12.2
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdurl==0.1.2
 molecule==24.2.0
 mypy-extensions==1.0.0
 onigurumacffi==1.3.0
-packaging==23.2
+packaging==24.0
 parsley==1.3
 pathspec==0.12.1
 pbr==6.0.0
 pexpect==4.9.0
 platformdirs==4.2.0
 pluggy==1.4.0
 ptyprocess==0.7.0
-pycparser==2.21
+pycparser==2.22
 pygments==2.17.2
 pyproject-api==1.6.1
-pytest==8.0.0
+pytest==8.1.1
 pytest-ansible==24.1.2
 pytest-xdist==3.5.0
 python-daemon==3.0.1
 python-gnupg==0.5.2
 pyyaml==6.0.1
-referencing==0.33.0
-requirements-parser==0.5.0
+referencing==0.34.0
+requirements-parser==0.9.0
 resolvelib==1.0.1
-rich==13.7.0
-rpds-py==0.17.1
+rich==13.7.1
+rpds-py==0.18.0
 ruamel-yaml==0.18.6
 ruamel-yaml-clib==0.2.8
 six==1.16.0
 subprocess-tee==0.4.1
 tomli==2.0.1
-tox==4.12.1
+tox==4.14.2
 tox-ansible==24.2.0
-types-setuptools==69.0.0.20240125
-typing-extensions==4.9.0
-tzdata==2023.4
-virtualenv==20.25.0
-wcmatch==8.5
-yamllint==1.34.0
+types-setuptools==69.2.0.20240317
+typing-extensions==4.11.0
+tzdata==2024.1
+virtualenv==20.25.1
+wcmatch==8.5.1
+yamllint==1.35.1
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `ansible-dev-tools-24.2.0/.github/workflows/release.yml` & `ansible-dev-tools-24.2.1/.github/workflows/release.yml`

 * *Files 11% similar despite different names*

```diff
@@ -31,13 +31,13 @@
       - name: Check out src from Git
         uses: actions/checkout@v4
         with:
           fetch-depth: 0 # needed by setuptools-scm
           submodules: true
 
       - name: Build dists
-        run: python -m tox
+        run: python3 -m tox
 
       - name: Publish to pypi.org
         if: >- # "create" workflows run separately from "push" & "pull_request"
           github.event_name == 'release'
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `ansible-dev-tools-24.2.0/.github/workflows/tox.yml` & `ansible-dev-tools-24.2.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/.gitignore` & `ansible-dev-tools-24.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/.pre-commit-config.yaml` & `ansible-dev-tools-24.2.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     rev: v3.1.0
     hooks:
       - id: add-trailing-comma
         args:
           - --py36-plus
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks.git
-    rev: v1.5.4
+    rev: v1.5.5
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
     rev: v4.0.0-alpha.8
     hooks:
@@ -43,72 +43,72 @@
         always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
 
   - repo: https://github.com/psf/black
-    rev: 24.1.1
+    rev: 24.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pappasam/toml-sort
     rev: v0.23.1
     hooks:
       - id: toml-sort-fix
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: 1.3.1
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.1
+    rev: v0.3.4
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v8.3.0
+    rev: v8.6.1
     hooks:
       - id: cspell
         name: Spell check with cspell
 
   - repo: https://github.com/jsh9/pydoclint
-    rev: 0.3.10
+    rev: 0.4.1
     hooks:
       - id: pydoclint
         args:
           - "--config=pyproject.toml"
 
   - repo: https://github.com/pycqa/pylint.git
-    rev: v3.0.3
+    rev: v3.1.0
     hooks:
       - id: pylint
         args:
           - --output-format=colorized
         additional_dependencies:
           - pytest
           - tox
 
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pytest
           - tox
           - types-setuptools
         args:
           - src
           - tests
         pass_filenames: false
 
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.3.0
+    rev: 7.4.1
     hooks:
       - id: pip-compile
         name: deps
         alias: deps
         always_run: true
         stages: [manual]
         entry: >
```

### Comparing `ansible-dev-tools-24.2.0/LICENSE` & `ansible-dev-tools-24.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/PKG-INFO` & `ansible-dev-tools-24.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.2.0
+Version: 24.2.1
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ansible-builder
-Requires-Dist: ansible-creator
+Requires-Dist: ansible-creator>=24.4.1
 Requires-Dist: ansible-dev-environment
 Requires-Dist: ansible-lint
 Requires-Dist: ansible-navigator
 Requires-Dist: ansible-sign
 Requires-Dist: molecule
 Requires-Dist: pytest-ansible
 Requires-Dist: setuptools
@@ -45,14 +45,16 @@
 Requires-Dist: pip-tools; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pydoclint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: toml-sort; extra == "test"
 
+<!-- cspell:disable-next-line -->
+
 # Ansible Development Tools (ADT)
 
 The `ansible-dev-tools` python package provides an easy way to install and discover the best tools available to create and test ansible content.
 
 The curated list of tools installed as part of the Ansible automation developer tools package includes:
 
 [ansible-core](https://github.com/ansible/ansible): Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy and maintain. Automate everything from code deployment to network configuration to cloud management, in a language that approaches plain English, using SSH, with no agents to install on remote systems.
@@ -73,30 +75,30 @@
 
 [tox-ansible](https://github.com/ansible/tox-ansible): The tox-ansible plugin dynamically creates a full matrix of python interpreter and ansible-core version environments for running integration, sanity, and unit for an ansible collection both locally and in a Github action. tox virtual environments are leveraged for collection building, collection installation, dependency installation, and testing.
 
 [ansible-dev-environment](https://github.com/ansible/ansible-dev-environment): A pip-like install for Ansible collections.
 
 ## Installation
 
-`python -m pip install ansible-dev-tools`
+`python3 -m pip install ansible-dev-tools`
 
 ## Usage
 
 In addition to installing each of the above tools, `ansible-dev-tools` provides an easy way to show the versions of the content creation tools that make up the current development environment.
 
 <!-- START -->
 
 ```
 $ adt --version
-ansible-builder                          3.0.0
-ansible-core                             2.16.3
-ansible-creator                          24.2.0
+ansible-builder                          3.0.1
+ansible-core                             2.16.5
+ansible-creator                          24.4.1
 ansible-dev-environment                  24.1.0
-ansible-dev-tools                        0.2.0a0
-ansible-lint                             24.2.0
+ansible-dev-tools                        24.2.0
+ansible-lint                             24.2.1
 ansible-navigator                        24.2.0
 ansible-sign                             0.1.1
 molecule                                 24.2.0
 pytest-ansible                           24.1.2
 tox-ansible                              24.2.0
 ```
```

### Comparing `ansible-dev-tools-24.2.0/README.md` & `ansible-dev-tools-24.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<!-- cspell:disable-next-line -->
+
 # Ansible Development Tools (ADT)
 
 The `ansible-dev-tools` python package provides an easy way to install and discover the best tools available to create and test ansible content.
 
 The curated list of tools installed as part of the Ansible automation developer tools package includes:
 
 [ansible-core](https://github.com/ansible/ansible): Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy and maintain. Automate everything from code deployment to network configuration to cloud management, in a language that approaches plain English, using SSH, with no agents to install on remote systems.
@@ -22,30 +24,30 @@
 
 [tox-ansible](https://github.com/ansible/tox-ansible): The tox-ansible plugin dynamically creates a full matrix of python interpreter and ansible-core version environments for running integration, sanity, and unit for an ansible collection both locally and in a Github action. tox virtual environments are leveraged for collection building, collection installation, dependency installation, and testing.
 
 [ansible-dev-environment](https://github.com/ansible/ansible-dev-environment): A pip-like install for Ansible collections.
 
 ## Installation
 
-`python -m pip install ansible-dev-tools`
+`python3 -m pip install ansible-dev-tools`
 
 ## Usage
 
 In addition to installing each of the above tools, `ansible-dev-tools` provides an easy way to show the versions of the content creation tools that make up the current development environment.
 
 <!-- START -->
 
 ```
 $ adt --version
-ansible-builder                          3.0.0
-ansible-core                             2.16.3
-ansible-creator                          24.2.0
+ansible-builder                          3.0.1
+ansible-core                             2.16.5
+ansible-creator                          24.4.1
 ansible-dev-environment                  24.1.0
-ansible-dev-tools                        0.2.0a0
-ansible-lint                             24.2.0
+ansible-dev-tools                        24.2.0
+ansible-lint                             24.2.1
 ansible-navigator                        24.2.0
 ansible-sign                             0.1.1
 molecule                                 24.2.0
 pytest-ansible                           24.1.2
 tox-ansible                              24.2.0
 ```
```

### Comparing `ansible-dev-tools-24.2.0/cspell.config.yaml` & `ansible-dev-tools-24.2.1/cspell.config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,16 @@
   - networking-terms
   - python
   - words
   - "!aws"
   - "!backwards-compatibility"
   - "!cryptocurrencies"
   - "!cpp"
+flagWords:
+  - ADT
 ignorePaths:
   # All dot files in the root
   - \.*
   # This file
   - cspell.config.yaml
   # The mypy configuration file
   - mypy.ini
```

### Comparing `ansible-dev-tools-24.2.0/docs/contributor-guide.md` & `ansible-dev-tools-24.2.1/docs/contributor-guide.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/index.md` & `ansible-dev-tools-24.2.1/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 ---
 hide:
   - navigation
   - toc
 ---
 
+<!-- cspell:disable-next-line -->
+
 # Ansible Development Tools (ADT)
 
 ## Introduction
 
-Ansible Development Tools or ADT for short, aims to streamline the setup and usage of several tools needed in order to create [Ansible](https://www.ansible.com/) content.
-When it comes to creating automation content using Ansible, there are several packages available that can help users in different parts of the content creating journey. From bootstrapping new projects, all the way to ensuring content follows best practices and verifying it behaves as intended via well established test frameworks.
+<!-- cspell:disable-next-line -->
+
+Ansible Development Tools or ADT for short, aims to streamline the setup and usage of several tools needed to create [Ansible](https://www.ansible.com/) content.
+When it comes to creating automation content using Ansible, there are several packages available that can help users in different parts of the content-creating journey. From bootstrapping new projects, all the way to ensuring content follows best practices and verifying it behaves as intended via well-established test frameworks.
 
 ## Key Features
 
-- All-in-One Ansible Toolkit: ADT combines critical Ansible development packages into a unified Python package.
+- All-in-One Ansible Toolkit: ansible-dev-tools combines critical Ansible development packages into a unified Python package called [ansible-dev-tools](https://pypi.org/project/ansible-dev-tools/).
 
-- Simplified Ansible Automation: ADT focuses on crafting your automation scenarios and workflows with speed by reducing boilerplate code without
+- Simplified Ansible Automation: ansible-dev-tools focuses on crafting your automation scenarios and workflows with speed by reducing boilerplate code without
   dealing with the intricacies of managing and integrating different Ansible libraries.
 
-For those looking for an IDE based experience, we also recommend you get familiar with the [Ansible extension for VSCode](https://marketplace.visualstudio.com/items?itemName=redhat.ansible).
+For those looking for an IDE-based experience, we also recommend you get familiar with the [Ansible extension for VSCode](https://marketplace.visualstudio.com/items?itemName=redhat.ansible).
 
 ## Included Packages
 
 The curated list of tools installed as part of the Ansible Development Tools includes:
 
 - [ansible-builder](https://github.com/ansible/ansible-builder): Ansible Builder automates the process of building execution environments using the schemas and tooling defined in various Ansible Collections and by the user.
 - [ansible-core](https://github.com/ansible/ansible): Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy and maintain. Automate everything from code deployment to network configuration to cloud management, in a language that approaches plain English, using SSH, with no agents to install on remote systems.
@@ -33,12 +37,12 @@
 - [ansible-sign](https://github.com/ansible/ansible-sign): Utility for signing and verifying Ansible project directory contents.
 - [molecule](https://github.com/ansible/molecule): Molecule aids in the development and testing of Ansible content: collections, playbooks and roles
 - [pytest-ansible](https://github.com/ansible/pytest-ansible): A pytest plugin that enables the use of ansible in tests, enables the use of pytest as a collection unit test runner, and exposes molecule scenarios using a pytest fixture.
 - [tox-ansible](https://github.com/ansible/tox-ansible): The tox-ansible plugin dynamically creates a full matrix of python interpreter and ansible-core version environments for running integration, sanity, and unit for an ansible collection both locally and in a Github action. tox virtual environments are leveraged for collection building, collection installation, dependency installation, and testing.
 
 ## Getting started
 
-To get started, follow the [installation](installation.md) steps to get ADT setup and check [User Guide](user-guide/index.md) for more details.
+To get started, follow the [installation](installation.md) steps to get ansible-dev-tools setup and check [User Guide](user-guide/index.md) for more details.
 
 ## Community
 
 Questions, feedback, or contributions? Join the Ansible community on [Matrix](https://matrix.to/#/#devtools:ansible.com) or [open an issue](https://github.com/ansible/ansible-dev-tools/issues/new). We're dedicated to supporting your Ansible automation journey! For more details on how to interact with our community, please visit the [Ansible Communication](https://docs.ansible.com/ansible/latest/community/communication.html) page.
```

### Comparing `ansible-dev-tools-24.2.0/docs/media/ansible-lint.mp4` & `ansible-dev-tools-24.2.1/docs/media/ansible-lint.mp4`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/media/ansible-navigator-run.mp4` & `ansible-dev-tools-24.2.1/docs/media/ansible-navigator-run.mp4`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/media/create-collection.mp4` & `ansible-dev-tools-24.2.1/docs/media/create-collection.mp4`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/building-collection.md` & `ansible-dev-tools-24.2.1/docs/user-guide/building-collection.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/ci-setup.md` & `ansible-dev-tools-24.2.1/docs/user-guide/ci-setup.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/content-best-practices.md` & `ansible-dev-tools-24.2.1/docs/user-guide/content-best-practices.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/content-release.md` & `ansible-dev-tools-24.2.1/docs/user-guide/content-release.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/images/ci.png` & `ansible-dev-tools-24.2.1/docs/user-guide/images/ci.png`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/images/release.png` & `ansible-dev-tools-24.2.1/docs/user-guide/images/release.png`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/index.md` & `ansible-dev-tools-24.2.1/docs/user-guide/index.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/docs/user-guide/testing.md` & `ansible-dev-tools-24.2.1/docs/user-guide/testing.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/mkdocs.yml` & `ansible-dev-tools-24.2.1/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 site_name: Ansible Development Tools Documentation
 site_url: https://ansible.readthedocs.io/projects/dev-tools/
 repo_url: https://github.com/ansible/ansible-dev-tools
 edit_uri: blob/main/docs/
-copyright: Copyright © 2023 Red Hat, Inc.
+copyright: Copyright © Red Hat, Inc.
 docs_dir: docs
 strict: true
 
 theme:
   name: ansible
   features:
     - announce.dismiss
@@ -98,15 +98,16 @@
   - Contributor Guide: contributor-guide.md
 
 plugins:
   - autorefs
   - markdown-exec
   - material/search:
       separator: '[\s\-,:!=\[\]()"`/]+|\.(?!\d)|&[lg]t;|(?!\b)(?=[A-Z][a-z])'
-  - material/social
+  # https://github.com/squidfunk/mkdocs-material/issues/6983
+  # - material/social
   - material/tags
   - mkdocstrings:
       handlers:
         python:
           paths: [src]
           options:
             # Sphinx is for historical reasons, but we could consider switching if needed
```

### Comparing `ansible-dev-tools-24.2.0/pyproject.toml` & `ansible-dev-tools-24.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/src/ansible_dev_tools/arg_parser.py` & `ansible-dev-tools-24.2.1/src/ansible_dev_tools/arg_parser.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/src/ansible_dev_tools/cli.py` & `ansible-dev-tools-24.2.1/src/ansible_dev_tools/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/src/ansible_dev_tools/version_builder.py` & `ansible-dev-tools-24.2.1/src/ansible_dev_tools/version_builder.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/PKG-INFO` & `ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.2.0
+Version: 24.2.1
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ansible-builder
-Requires-Dist: ansible-creator
+Requires-Dist: ansible-creator>=24.4.1
 Requires-Dist: ansible-dev-environment
 Requires-Dist: ansible-lint
 Requires-Dist: ansible-navigator
 Requires-Dist: ansible-sign
 Requires-Dist: molecule
 Requires-Dist: pytest-ansible
 Requires-Dist: setuptools
@@ -45,14 +45,16 @@
 Requires-Dist: pip-tools; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pydoclint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: toml-sort; extra == "test"
 
+<!-- cspell:disable-next-line -->
+
 # Ansible Development Tools (ADT)
 
 The `ansible-dev-tools` python package provides an easy way to install and discover the best tools available to create and test ansible content.
 
 The curated list of tools installed as part of the Ansible automation developer tools package includes:
 
 [ansible-core](https://github.com/ansible/ansible): Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy and maintain. Automate everything from code deployment to network configuration to cloud management, in a language that approaches plain English, using SSH, with no agents to install on remote systems.
@@ -73,30 +75,30 @@
 
 [tox-ansible](https://github.com/ansible/tox-ansible): The tox-ansible plugin dynamically creates a full matrix of python interpreter and ansible-core version environments for running integration, sanity, and unit for an ansible collection both locally and in a Github action. tox virtual environments are leveraged for collection building, collection installation, dependency installation, and testing.
 
 [ansible-dev-environment](https://github.com/ansible/ansible-dev-environment): A pip-like install for Ansible collections.
 
 ## Installation
 
-`python -m pip install ansible-dev-tools`
+`python3 -m pip install ansible-dev-tools`
 
 ## Usage
 
 In addition to installing each of the above tools, `ansible-dev-tools` provides an easy way to show the versions of the content creation tools that make up the current development environment.
 
 <!-- START -->
 
 ```
 $ adt --version
-ansible-builder                          3.0.0
-ansible-core                             2.16.3
-ansible-creator                          24.2.0
+ansible-builder                          3.0.1
+ansible-core                             2.16.5
+ansible-creator                          24.4.1
 ansible-dev-environment                  24.1.0
-ansible-dev-tools                        0.2.0a0
-ansible-lint                             24.2.0
+ansible-dev-tools                        24.2.0
+ansible-lint                             24.2.1
 ansible-navigator                        24.2.0
 ansible-sign                             0.1.1
 molecule                                 24.2.0
 pytest-ansible                           24.1.2
 tox-ansible                              24.2.0
 ```
```

### Comparing `ansible-dev-tools-24.2.0/src/ansible_dev_tools.egg-info/SOURCES.txt` & `ansible-dev-tools-24.2.1/src/ansible_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/tools/update-readme.py` & `ansible-dev-tools-24.2.1/tools/update-readme.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-tools-24.2.0/tox.ini` & `ansible-dev-tools-24.2.1/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -60,18 +60,18 @@
 deps =
     build>=0.9
     twine>=4.0.2  # pyup: ignore
 extras =
 set_env =
 commands =
     rm -rfv {toxinidir}/dist/
-    python -m build \
+    python3 -m build \
       --outdir {toxinidir}/dist/ \
       {toxinidir}
-    sh -c "python -m twine check --strict {toxinidir}/dist/*"
+    sh -c "python3 -m twine check --strict {toxinidir}/dist/*"
     pip install '.[test,docs]'
     adt --version
 
 [testenv:docs]
 description = Builds docs
 skip_install = true
 set_env =
```

