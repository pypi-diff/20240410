# Comparing `tmp/circup-1.6.2.tar.gz` & `tmp/circup-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circup-1.6.2.tar", last modified: Sat Mar  9 16:08:40 2024, max compression
+gzip compressed data, was "circup-1.7.0.tar", last modified: Tue Apr  9 22:59:22 2024, max compression
```

## Comparing `circup-1.6.2.tar` & `circup-1.7.0.tar`

### file list

```diff
@@ -1,83 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.457984 circup-1.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.445984 circup-1.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-09 16:08:21.000000 circup-1.6.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-09 16:08:21.000000 circup-1.6.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.445984 circup-1.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-09 16:08:21.000000 circup-1.6.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-09 16:08:21.000000 circup-1.6.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-09 16:08:21.000000 circup-1.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-09 16:08:21.000000 circup-1.6.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-09 16:08:21.000000 circup-1.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-03-09 16:08:21.000000 circup-1.6.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-09 16:08:21.000000 circup-1.6.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/CODE_OF_CONDUCT.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-03-09 16:08:21.000000 circup-1.6.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/CONTRIBUTING.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-09 16:08:21.000000 circup-1.6.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.445984 circup-1.6.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-09 16:08:21.000000 circup-1.6.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-09 16:08:21.000000 circup-1.6.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-09 16:08:21.000000 circup-1.6.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-03-09 16:08:40.457984 circup-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-03-09 16:08:21.000000 circup-1.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.445984 circup-1.6.2/circup/
--rw-r--r--   0 runner    (1001) docker     (127)    57126 2024-03-09 16:08:21.000000 circup-1.6.2/circup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31649 2024-03-09 16:08:21.000000 circup-1.6.2/circup/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.449984 circup-1.6.2/circup/config/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-09 16:08:21.000000 circup-1.6.2/circup/config/bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-09 16:08:21.000000 circup-1.6.2/circup/config/bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-03-09 16:08:21.000000 circup-1.6.2/circup/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.453984 circup-1.6.2/circup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-03-09 16:08:40.000000 circup-1.6.2/circup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-09 16:08:40.000000 circup-1.6.2/circup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 16:08:40.000000 circup-1.6.2/circup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-09 16:08:40.000000 circup-1.6.2/circup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-09 16:08:40.000000 circup-1.6.2/circup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-09 16:08:40.000000 circup-1.6.2/circup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.449984 circup-1.6.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.449984 circup-1.6.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-09 16:08:21.000000 circup-1.6.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-09 16:08:21.000000 circup-1.6.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-03-09 16:08:21.000000 circup-1.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-09 16:08:21.000000 circup-1.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)    36437 2024-03-09 16:08:21.000000 circup-1.6.2/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/docs/logo.png.license
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-09 16:08:21.000000 circup-1.6.2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-09 16:08:21.000000 circup-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-09 16:08:21.000000 circup-1.6.2/requirements.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 16:08:40.457984 circup-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-09 16:08:21.000000 circup-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.453984 circup-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:21.000000 circup-1.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.453984 circup-1.6.2/tests/bad_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:21.000000 circup-1.6.2/tests/bad_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-09 16:08:21.000000 circup-1.6.2/tests/bad_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-09 16:08:21.000000 circup-1.6.2/tests/bad_python.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-09 16:08:21.000000 circup-1.6.2/tests/bundle.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/tests/bundle.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-09 16:08:21.000000 circup-1.6.2/tests/device.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/tests/device.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.453984 circup-1.6.2/tests/dir_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:21.000000 circup-1.6.2/tests/dir_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-09 16:08:21.000000 circup-1.6.2/tests/dir_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-09 16:08:21.000000 circup-1.6.2/tests/import_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-09 16:08:21.000000 circup-1.6.2/tests/local_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-09 16:08:21.000000 circup-1.6.2/tests/local_module_cp7.mpy
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/tests/local_module_cp7.mpy.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 16:08:40.453984 circup-1.6.2/tests/mock_device/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-09 16:08:21.000000 circup-1.6.2/tests/mock_device/boot_out.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-09 16:08:21.000000 circup-1.6.2/tests/mock_device/boot_out.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-09 16:08:21.000000 circup-1.6.2/tests/mount_exists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/tests/mount_exists.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-09 16:08:21.000000 circup-1.6.2/tests/mount_missing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/tests/mount_missing.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-09 16:08:21.000000 circup-1.6.2/tests/remote_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-09 16:08:21.000000 circup-1.6.2/tests/test_bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-09 16:08:21.000000 circup-1.6.2/tests/test_bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-09 16:08:21.000000 circup-1.6.2/tests/test_bundle_config_local.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-09 16:08:21.000000 circup-1.6.2/tests/test_bundle_config_local.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    43012 2024-03-09 16:08:21.000000 circup-1.6.2/tests/test_circup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-09 16:08:21.000000 circup-1.6.2/tests/test_module.mpy
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-09 16:08:21.000000 circup-1.6.2/tests/test_module.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.586066 circup-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.570066 circup-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-09 22:59:11.000000 circup-1.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-09 22:59:11.000000 circup-1.7.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-09 22:59:11.000000 circup-1.7.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-09 22:59:11.000000 circup-1.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 22:59:11.000000 circup-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 22:59:11.000000 circup-1.7.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-09 22:59:11.000000 circup-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-09 22:59:11.000000 circup-1.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-09 22:59:11.000000 circup-1.7.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/CODE_OF_CONDUCT.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-09 22:59:11.000000 circup-1.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/CONTRIBUTING.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-04-09 22:59:22.582066 circup-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-09 22:59:11.000000 circup-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/circup/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 22:59:11.000000 circup-1.7.0/circup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31649 2024-04-09 22:59:11.000000 circup-1.7.0/circup/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-09 22:59:11.000000 circup-1.7.0/circup/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19934 2024-04-09 22:59:11.000000 circup-1.7.0/circup/command_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-09 22:59:11.000000 circup-1.7.0/circup/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/circup/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 22:59:11.000000 circup-1.7.0/circup/config/bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 22:59:11.000000 circup-1.7.0/circup/config/bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 22:59:11.000000 circup-1.7.0/circup/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-09 22:59:11.000000 circup-1.7.0/circup/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-09 22:59:11.000000 circup-1.7.0/circup/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/circup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-09 22:59:11.000000 circup-1.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 22:59:11.000000 circup-1.7.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-09 22:59:11.000000 circup-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 22:59:11.000000 circup-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)    36437 2024-04-09 22:59:11.000000 circup-1.7.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/docs/logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 22:59:11.000000 circup-1.7.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:59:11.000000 circup-1.7.0/optional_requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 22:59:11.000000 circup-1.7.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 22:59:11.000000 circup-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:59:11.000000 circup-1.7.0/requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:59:22.586066 circup-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-09 22:59:11.000000 circup-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/tests/bad_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bad_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bad_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bad_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bundle.json
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bundle.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 22:59:11.000000 circup-1.7.0/tests/device.json
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/device.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/tests/dir_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/dir_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-09 22:59:11.000000 circup-1.7.0/tests/dir_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 22:59:11.000000 circup-1.7.0/tests/import_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 22:59:11.000000 circup-1.7.0/tests/local_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 22:59:11.000000 circup-1.7.0/tests/local_module_cp7.mpy
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/local_module_cp7.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/tests/mock_device/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mock_device/boot_out.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mock_device/boot_out.txt.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.570066 circup-1.7.0/tests/mock_device/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/tests/mock_device/lib/adafruit_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mock_device/lib/adafruit_waveform/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_exists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_exists.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_missing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_missing.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 22:59:11.000000 circup-1.7.0/tests/remote_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config_local.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config_local.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_circup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_module.mpy
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_module.mpy.license
```

### Comparing `circup-1.6.2/.github/ISSUE_TEMPLATE.md` & `circup-1.7.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/.github/PULL_REQUEST_TEMPLATE.md` & `circup-1.7.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/.github/workflows/build.yml` & `circup-1.7.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/.github/workflows/release.yml` & `circup-1.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/.gitignore` & `circup-1.7.0/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
+!tests/mock_device/lib/
 lib64/
 parts/
 sdist/
 var/
 wheels/
 *.egg-info/
 .installed.cfg
@@ -89,14 +90,15 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+*_venv/
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
```

### Comparing `circup-1.6.2/.pre-commit-config.yaml` & `circup-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/.pylintrc` & `circup-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/CODE_OF_CONDUCT.rst` & `circup-1.7.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/CONTRIBUTING.rst` & `circup-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/LICENSE` & `circup-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/LICENSES/CC-BY-4.0.txt` & `circup-1.7.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/LICENSES/MIT.txt` & `circup-1.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/LICENSES/Unlicense.txt` & `circup-1.7.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/PKG-INFO` & `circup-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.6.2
+Version: 1.7.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
@@ -53,24 +53,24 @@
 Requires-Dist: pytest-faulthandler; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: all
-Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: coverage; extra == "all"
-Requires-Dist: twine; extra == "all"
 Requires-Dist: wheel; extra == "all"
 Requires-Dist: pytest-faulthandler; extra == "all"
-Requires-Dist: pytest; extra == "all"
+Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
 Requires-Dist: pylint; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: coverage; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: sphinx; extra == "all"
 
 
 CircUp
 ======
 
 .. image:: https://readthedocs.org/projects/circup/badge/?version=latest
     :target: https://circuitpython.readthedocs.io/projects/circup/en/latest/
```

### Comparing `circup-1.6.2/README.rst` & `circup-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/circup/backends.py` & `circup-1.7.0/circup/backends.py`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/circup/shared.py` & `circup-1.7.0/circup/shared.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,56 @@
 """
 Utilities that are shared and used by both click CLI command functions
 and Backend class functions.
 """
 import glob
 import os
 import re
-
+import json
 import appdirs
+import pkg_resources
+import requests
 
 #: Version identifier for a bad MPY file format
 BAD_FILE_FORMAT = "Invalid"
 
 #: The location of data files used by circup (following OS conventions).
 DATA_DIR = appdirs.user_data_dir(appname="circup", appauthor="adafruit")
 
+#: Module formats list (and the other form used in github files)
+PLATFORMS = {"py": "py", "8mpy": "8.x-mpy", "9mpy": "9.x-mpy"}
+
+#: Timeout for requests calls like get()
+REQUESTS_TIMEOUT = 30
+
+#: The path to the JSON file containing the metadata about the bundles.
+BUNDLE_CONFIG_FILE = pkg_resources.resource_filename(
+    "circup", "config/bundle_config.json"
+)
+#: Overwrite the bundles list with this file (only done manually)
+BUNDLE_CONFIG_OVERWRITE = os.path.join(DATA_DIR, "bundle_config.json")
+#: The path to the JSON file containing the local list of bundles.
+BUNDLE_CONFIG_LOCAL = os.path.join(DATA_DIR, "bundle_config_local.json")
+#: The path to the JSON file containing the metadata about the bundles.
+BUNDLE_DATA = os.path.join(DATA_DIR, "circup.json")
+
+#:  The libraries (and blank lines) which don't go on devices
+NOT_MCU_LIBRARIES = [
+    "",
+    "adafruit-blinka",
+    "adafruit-blinka-bleio",
+    "adafruit-blinka-displayio",
+    "adafruit-circuitpython-typing",
+    "circuitpython_typing",
+    "pyserial",
+]
+
+#: Commands that do not require an attached board
+BOARDLESS_COMMANDS = ["show", "bundle-add", "bundle-remove", "bundle-show"]
+
 
 def _get_modules_file(path, logger):
     """
     Get a dictionary containing metadata about all the Python modules found in
     the referenced file system path.
 
     :param str path: The directory in which to find modules.
@@ -138,7 +171,48 @@
                 offset += 1  # ...and again but backtrack by one.
         if compatibility:
             result["compatibility"] = compatibility
         else:
             # not a valid MPY file
             result["__version__"] = BAD_FILE_FORMAT
     return result
+
+
+def tags_data_load(logger):
+    """
+    Load the list of the version tags of the bundles on disk.
+
+    :return: a dict() of tags indexed by Bundle identifiers/keys.
+    """
+    tags_data = None
+    try:
+        with open(BUNDLE_DATA, encoding="utf-8") as data:
+            try:
+                tags_data = json.load(data)
+            except json.decoder.JSONDecodeError as ex:
+                # Sometimes (why?) the JSON file becomes corrupt. In which case
+                # log it and carry on as if setting up for first time.
+                logger.error("Could not parse %s", BUNDLE_DATA)
+                logger.exception(ex)
+    except FileNotFoundError:
+        pass
+    if not isinstance(tags_data, dict):
+        tags_data = {}
+    return tags_data
+
+
+def get_latest_release_from_url(url, logger):
+    """
+    Find the tag name of the latest release by using HTTP HEAD and decoding the redirect.
+
+    :param str url: URL to the latest release page on a git repository.
+    :return: The most recent tag value for the release.
+    """
+
+    logger.info("Requesting redirect information: %s", url)
+    response = requests.head(url, timeout=REQUESTS_TIMEOUT)
+    responseurl = response.url
+    if response.is_redirect:
+        responseurl = response.headers["Location"]
+    tag = responseurl.rsplit("/", 1)[-1]
+    logger.info("Tag: '%s'", tag)
+    return tag
```

### Comparing `circup-1.6.2/circup.egg-info/PKG-INFO` & `circup-1.7.0/circup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.6.2
+Version: 1.7.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
@@ -53,24 +53,24 @@
 Requires-Dist: pytest-faulthandler; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: all
-Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: coverage; extra == "all"
-Requires-Dist: twine; extra == "all"
 Requires-Dist: wheel; extra == "all"
 Requires-Dist: pytest-faulthandler; extra == "all"
-Requires-Dist: pytest; extra == "all"
+Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
 Requires-Dist: pylint; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: coverage; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: sphinx; extra == "all"
 
 
 CircUp
 ======
 
 .. image:: https://readthedocs.org/projects/circup/badge/?version=latest
     :target: https://circuitpython.readthedocs.io/projects/circup/en/latest/
```

### Comparing `circup-1.6.2/circup.egg-info/SOURCES.txt` & `circup-1.7.0/circup.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,34 @@
 CODE_OF_CONDUCT.rst
 CODE_OF_CONDUCT.rst.license
 CONTRIBUTING.rst
 CONTRIBUTING.rst.license
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
+optional_requirements.txt.license
 readthedocs.yml
 requirements.txt
 requirements.txt.license
 setup.py
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/build.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 circup/__init__.py
 circup/backends.py
+circup/bundle.py
+circup/command_utils.py
+circup/commands.py
+circup/logging.py
+circup/module.py
 circup/shared.py
 circup.egg-info/PKG-INFO
 circup.egg-info/SOURCES.txt
 circup.egg-info/dependency_links.txt
 circup.egg-info/entry_points.txt
 circup.egg-info/requires.txt
 circup.egg-info/top_level.txt
@@ -61,8 +68,9 @@
 tests/test_module.mpy
 tests/test_module.mpy.license
 tests/bad_module/__init__.py
 tests/bad_module/my_module.py
 tests/dir_module/__init__.py
 tests/dir_module/my_module.py
 tests/mock_device/boot_out.txt
-tests/mock_device/boot_out.txt.license
+tests/mock_device/boot_out.txt.license
+tests/mock_device/lib/adafruit_waveform/.gitkeep
```

### Comparing `circup-1.6.2/docs/_static/favicon.ico` & `circup-1.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/docs/conf.py` & `circup-1.7.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = [
     "_build",
     "Thumbs.db",
```

### Comparing `circup-1.6.2/docs/logo.png` & `circup-1.7.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/setup.py` & `circup-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/tests/bundle.json` & `circup-1.7.0/tests/bundle.json`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/tests/mount_exists.txt` & `circup-1.7.0/tests/mount_exists.txt`

 * *Files identical despite different names*

### Comparing `circup-1.6.2/tests/test_circup.py` & `circup-1.7.0/tests/test_circup.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,23 @@
 from unittest import mock
 from click.testing import CliRunner
 import pytest
 import requests
 
 import circup
 from circup import DiskBackend
+from circup.command_utils import (
+    find_device,
+    ensure_latest_bundle,
+    get_bundle,
+    get_bundles_dict,
+)
+from circup.shared import PLATFORMS
+from circup.module import Module
+from circup.logging import logger
 
 TEST_BUNDLE_CONFIG_JSON = "tests/test_bundle_config.json"
 with open(TEST_BUNDLE_CONFIG_JSON, "rb") as tbc:
     TEST_BUNDLE_DATA = json.load(tbc)
 TEST_BUNDLE_NAME = TEST_BUNDLE_DATA["test_bundle"]
 
 TEST_BUNDLE_CONFIG_LOCAL_JSON = "tests/test_bundle_config_local.json"
@@ -48,29 +57,24 @@
     TEST_BUNDLE_LOCAL_DATA = json.load(tbc)
 
 
 def test_Bundle_init():
     """
     Create a Bundle and check all the strings are set as expected.
     """
-    with mock.patch("circup.logger.info"), mock.patch(
-        "circup.os.path.isfile", return_value=True
-    ), mock.patch("circup.CPY_VERSION", "4.1.2"), mock.patch(
-        "circup.tags_data_load", return_value=dict()
-    ), mock.patch(
-        "circup.DATA_DIR", "DATA_DIR"
-    ):
-        bundle = circup.Bundle(TEST_BUNDLE_NAME)
+    bundle = circup.Bundle(TEST_BUNDLE_NAME)
     assert repr(bundle) == repr(
         {
             "key": TEST_BUNDLE_NAME,
             "url": "https://github.com/" + TEST_BUNDLE_NAME,
             "urlzip": "adafruit-circuitpython-bundle-{platform}-{tag}.zip",
-            "dir": "DATA_DIR/adafruit/adafruit-circuitpython-bundle-{platform}",
-            "zip": "DATA_DIR/adafruit-circuitpython-bundle-{platform}.zip",
+            "dir": circup.shared.DATA_DIR
+            + "/adafruit/adafruit-circuitpython-bundle-{platform}",
+            "zip": circup.shared.DATA_DIR
+            + "/adafruit-circuitpython-bundle-{platform}.zip",
             "url_format": "https://github.com/"
             + TEST_BUNDLE_NAME
             + "/releases/download/{tag}/"
             "adafruit-circuitpython-bundle-{platform}-{tag}.zip",
             "current": None,
             "latest": None,
         }
@@ -78,130 +82,128 @@
 
 
 def test_Bundle_lib_dir():
     """
     Check the return of Bundle.lib_dir with a test tag.
     """
     bundle_data = {TEST_BUNDLE_NAME: "TESTTAG"}
-    with mock.patch("circup.logger.info"), mock.patch(
-        "circup.os.path.isfile", return_value=True
-    ), mock.patch("circup.tags_data_load", return_value=bundle_data), mock.patch(
-        "circup.DATA_DIR", "DATA_DIR"
-    ):
+    with mock.patch("circup.bundle.tags_data_load", return_value=bundle_data):
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         assert bundle.current_tag == "TESTTAG"
         assert bundle.lib_dir("py") == (
-            "DATA_DIR/"
+            circup.shared.DATA_DIR + "/"
             "adafruit/adafruit-circuitpython-bundle-py/"
             "adafruit-circuitpython-bundle-py-TESTTAG/lib"
         )
         assert bundle.lib_dir("8mpy") == (
-            "DATA_DIR/"
+            circup.shared.DATA_DIR + "/"
             "adafruit/adafruit-circuitpython-bundle-8mpy/"
             "adafruit-circuitpython-bundle-8.x-mpy-TESTTAG/lib"
         )
 
 
 def test_Bundle_latest_tag():
     """
     Check the latest tag gets through Bundle.latest_tag.
     """
     bundle_data = {TEST_BUNDLE_NAME: "TESTTAG"}
-    with mock.patch("circup.logger.info"), mock.patch(
-        "circup.os.path.isfile", return_value=True
-    ), mock.patch(
-        "circup.get_latest_release_from_url", return_value="BESTESTTAG"
-    ), mock.patch(
-        "circup.tags_data_load", return_value=bundle_data
-    ), mock.patch(
-        "circup.DATA_DIR", "DATA_DIR"
-    ):
+    with mock.patch(
+        "circup.bundle.get_latest_release_from_url", return_value="BESTESTTAG"
+    ), mock.patch("circup.bundle.tags_data_load", return_value=bundle_data):
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         assert bundle.latest_tag == "BESTESTTAG"
 
 
 def test_get_bundles_dict():
     """
     Check we are getting the bundles list from BUNDLE_CONFIG_FILE.
     """
-    with mock.patch("circup.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON), mock.patch(
-        "circup.BUNDLE_CONFIG_LOCAL", ""
-    ):
-        bundles_dict = circup.get_bundles_dict()
+    with mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON
+    ), mock.patch("circup.shared.BUNDLE_CONFIG_LOCAL", ""):
+        bundles_dict = get_bundles_dict()
         assert bundles_dict == TEST_BUNDLE_DATA
 
-    with mock.patch("circup.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON), mock.patch(
-        "circup.BUNDLE_CONFIG_LOCAL", TEST_BUNDLE_CONFIG_LOCAL_JSON
+    with mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON
+    ), mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_LOCAL", TEST_BUNDLE_CONFIG_LOCAL_JSON
     ):
-        bundles_dict = circup.get_bundles_dict()
+        bundles_dict = get_bundles_dict()
         expected_dict = {**TEST_BUNDLE_LOCAL_DATA, **TEST_BUNDLE_DATA}
         assert bundles_dict == expected_dict
 
 
 def test_get_bundles_local_dict():
     """
     Check we are getting the bundles list from BUNDLE_CONFIG_LOCAL.
     """
-    with mock.patch("circup.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON), mock.patch(
-        "circup.BUNDLE_CONFIG_LOCAL", ""
-    ):
-        bundles_dict = circup.get_bundles_dict()
+    with mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON
+    ), mock.patch("circup.command_utils.BUNDLE_CONFIG_LOCAL", ""):
+        bundles_dict = get_bundles_dict()
         assert bundles_dict == TEST_BUNDLE_DATA
 
-    with mock.patch("circup.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON), mock.patch(
-        "circup.BUNDLE_CONFIG_LOCAL", TEST_BUNDLE_CONFIG_LOCAL_JSON
+    with mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON
+    ), mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_LOCAL", TEST_BUNDLE_CONFIG_LOCAL_JSON
     ):
-        bundles_dict = circup.get_bundles_dict()
+        bundles_dict = get_bundles_dict()
         expected_dict = {**TEST_BUNDLE_LOCAL_DATA, **TEST_BUNDLE_DATA}
         assert bundles_dict == expected_dict
 
 
 def test_get_bundles_list():
     """
     Check we are getting the bundles list from BUNDLE_CONFIG_FILE.
     """
-    with mock.patch("circup.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON), mock.patch(
-        "circup.BUNDLE_CONFIG_LOCAL", ""
-    ):
+    with mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON
+    ), mock.patch("circup.command_utils.BUNDLE_CONFIG_LOCAL", ""):
         bundles_list = circup.get_bundles_list()
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         assert repr(bundles_list) == repr([bundle])
 
 
 def test_save_local_bundles():
     """
     Pretend to save local bundles.
     """
-    with mock.patch("circup.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON), mock.patch(
-        "circup.BUNDLE_CONFIG_LOCAL", ""
-    ), mock.patch("circup.os.unlink") as mock_unlink, mock.patch(
-        "circup.json.dump"
+    with mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON
+    ), mock.patch("circup.command_utils.BUNDLE_CONFIG_LOCAL", ""), mock.patch(
+        "circup.os.unlink"
+    ) as mock_unlink, mock.patch(
+        "circup.command_utils.json.dump"
     ) as mock_dump, mock.patch(
-        "circup.json.load", return_value=TEST_BUNDLE_DATA
-    ), mock.patch(
-        "circup.open", mock.mock_open()
+        "circup.command_utils.open", mock.mock_open()
     ) as mock_open:
         final_data = {**TEST_BUNDLE_DATA, **TEST_BUNDLE_LOCAL_DATA}
         circup.save_local_bundles(final_data)
         mock_dump.assert_called_once_with(final_data, mock_open())
         mock_unlink.assert_not_called()
 
 
 def test_save_local_bundles_reset():
     """
     Pretend to reset the local bundles.
     """
-    with mock.patch("circup.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON), mock.patch(
-        "circup.BUNDLE_CONFIG_LOCAL", "test/NOTEXISTS"
-    ), mock.patch("circup.os.path.isfile", return_value=True), mock.patch(
+    with mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_FILE", TEST_BUNDLE_CONFIG_JSON
+    ), mock.patch(
+        "circup.command_utils.BUNDLE_CONFIG_LOCAL", "test/NOTEXISTS"
+    ), mock.patch(
+        "circup.os.path.isfile", return_value=True
+    ), mock.patch(
         "circup.os.unlink"
     ) as mock_unlink, mock.patch(
-        "circup.json.load", return_value=TEST_BUNDLE_DATA
+        "circup.command_utils.json.load", return_value=TEST_BUNDLE_DATA
     ), mock.patch(
-        "circup.open", mock.mock_open()
+        "circup.command_utils.open", mock.mock_open()
     ) as mock_open:
         circup.save_local_bundles({})
         mock_open().write.assert_not_called()
         mock_unlink.assert_called_once_with("test/NOTEXISTS")
 
 
 def test_Module_init_file_module():
@@ -213,21 +215,21 @@
     path = os.path.join("mock_device", "lib", name)
     repo = "https://github.com/adafruit/SomeLibrary.git"
     device_version = "1.2.3"
     bundle_version = "3.2.1"
 
     with mock.patch("circup.logger.info") as mock_logger, mock.patch(
         "circup.os.path.isfile", return_value=True
-    ), mock.patch("circup.CPY_VERSION", "4.1.2"), mock.patch(
-        "circup.Bundle.lib_dir",
+    ), mock.patch(
+        "circup.bundle.Bundle.lib_dir",
         return_value="tests",
     ):
         backend = DiskBackend("mock_device", mock_logger)
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        m = circup.Module(
+        m = Module(
             name,
             backend,
             repo,
             device_version,
             bundle_version,
             False,
             bundle,
@@ -246,29 +248,25 @@
 
 def test_Module_init_directory_module():
     """
     Ensure the Module instance is set up as expected and logged, as if for a
     directory based Python module.
     """
     name = "dir_module/"
-    path = os.path.join("mock_device", "lib", f"{name}", "")
+    path = os.path.join("tests", "mock_device", "lib", f"{name}", "")
     repo = "https://github.com/adafruit/SomeLibrary.git"
     device_version = "1.2.3"
     bundle_version = "3.2.1"
     mpy = True
     with mock.patch("circup.logger.info") as mock_logger, mock.patch(
-        "circup.os.path.isfile", return_value=False
-    ), mock.patch("circup.CPY_VERSION", "4.1.2"), mock.patch(
-        "circup.DATA_DIR", "/tests/DATA_DIR"
-    ), mock.patch(
-        "circup.Bundle.lib_dir", return_value="tests"
+        "circup.bundle.Bundle.lib_dir", return_value="tests"
     ):
-        backend = DiskBackend("mock_device", mock_logger)
+        backend = DiskBackend("tests/mock_device", mock_logger)
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        m = circup.Module(
+        m = Module(
             name,
             backend,
             repo,
             device_version,
             bundle_version,
             mpy,
             bundle,
@@ -291,25 +289,19 @@
     boolean value to correctly indicate if the referenced module is, in fact,
     out of date.
     """
     bundle = circup.Bundle(TEST_BUNDLE_NAME)
     name = "module.py"
     repo = "https://github.com/adafruit/SomeLibrary.git"
     with mock.patch("circup.logger.info") as mock_logger:
-        backend = DiskBackend("mock_device", mock_logger)
-        m1 = circup.Module(
-            name, backend, repo, "1.2.3", "3.2.1", False, bundle, (None, None)
-        )
-        m2 = circup.Module(
-            name, backend, repo, "1.2.3", "1.2.3", False, bundle, (None, None)
-        )
+        backend = DiskBackend("tests/mock_device", mock_logger)
+        m1 = Module(name, backend, repo, "1.2.3", "3.2.1", False, bundle, (None, None))
+        m2 = Module(name, backend, repo, "1.2.3", "1.2.3", False, bundle, (None, None))
         # shouldn't happen!
-        m3 = circup.Module(
-            name, backend, repo, "3.2.1", "1.2.3", False, bundle, (None, None)
-        )
+        m3 = Module(name, backend, repo, "3.2.1", "1.2.3", False, bundle, (None, None))
         assert m1.outofdate is True
         assert m2.outofdate is False
         assert m3.outofdate is False
 
 
 def test_Module_outofdate_bad_versions():
     """
@@ -321,16 +313,16 @@
     name = "module.py"
 
     repo = "https://github.com/adafruit/SomeLibrary.git"
     device_version = "hello"
     bundle_version = "3.2.1"
 
     with mock.patch("circup.logger.warning") as mock_logger:
-        backend = DiskBackend("mock_device", mock_logger)
-        m = circup.Module(
+        backend = DiskBackend("tests/mock_device", mock_logger)
+        m = Module(
             name,
             backend,
             repo,
             device_version,
             bundle_version,
             False,
             bundle,
@@ -345,43 +337,45 @@
     """
     Ensure the ``outofdate`` property on a Module instance returns the expected
     boolean value to correctly indicate if the referenced module is, in fact,
     out of date.
     """
     name = "module.py"
     repo = "https://github.com/adafruit/SomeLibrary.git"
-    with mock.patch("circup.CPY_VERSION", "8.0.0"), mock.patch(
-        "circup.logger.warning"
-    ) as mock_logger:
-        backend = DiskBackend("mock_device", mock_logger)
+    with mock.patch("circup.logger.warning") as mock_logger:
+        backend = DiskBackend("tests/mock_device", mock_logger)
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        m1 = circup.Module(
-            name, backend, repo, "1.2.3", "1.2.3", True, bundle, (None, None)
-        )
-        m2 = circup.Module(
+        m1 = Module(name, backend, repo, "1.2.3", "1.2.3", True, bundle, (None, None))
+        m2 = Module(
             name,
             backend,
             repo,
             "1.2.3",
             "1.2.3",
             True,
             bundle,
             ("7.0.0-alpha.1", "8.99.99"),
         )
-        m3 = circup.Module(
+        m3 = Module(
             name, backend, repo, "1.2.3", "1.2.3", True, bundle, (None, "7.0.0-alpha.1")
         )
-    with mock.patch("circup.CPY_VERSION", "6.2.0"):
+    with mock.patch(
+        "circup.backends.DiskBackend.get_circuitpython_version",
+        return_value=("6.2.0", ""),
+    ):
         assert m1.mpy_mismatch is False
         assert m1.outofdate is False
         assert m2.mpy_mismatch is True
         assert m2.outofdate is True
         assert m3.mpy_mismatch is False
         assert m3.outofdate is False
-    with mock.patch("circup.CPY_VERSION", "8.0.0"):
+    with mock.patch(
+        "circup.backends.DiskBackend.get_circuitpython_version",
+        return_value=("8.0.0", ""),
+    ):
         assert m1.mpy_mismatch is False
         assert m1.outofdate is False
         assert m2.mpy_mismatch is False
         assert m2.outofdate is False
         assert m3.mpy_mismatch is True
         assert m3.outofdate is True
 
@@ -397,15 +391,15 @@
     name = "module.py"
     repo = "https://github.com/adafruit/SomeLibrary.git"
     device_version = "1.2.3"
     bundle_version = "version-3"
 
     with mock.patch("circup.logger.warning") as mock_logger:
         backend = DiskBackend("mock_device", mock_logger)
-        m = circup.Module(
+        m = Module(
             name,
             backend,
             repo,
             device_version,
             bundle_version,
             False,
             bundle,
@@ -420,46 +414,41 @@
     Ensure the tuple contains the expected items to be correctly displayed in
     a table of version-related results.
     """
     bundle = circup.Bundle(TEST_BUNDLE_NAME)
     name = "module.py"
     repo = "https://github.com/adafruit/SomeLibrary.git"
     with mock.patch("circup.os.path.isfile", return_value=True), mock.patch(
-        "circup.CPY_VERSION", "8.0.0"
+        "circup.backends.DiskBackend.get_circuitpython_version",
+        return_value=("8.0.0", ""),
     ), mock.patch("circup.logger.warning") as mock_logger:
         backend = DiskBackend("mock_device", mock_logger)
-        m = circup.Module(
-            name, backend, repo, "1.2.3", None, False, bundle, (None, None)
-        )
+        m = Module(name, backend, repo, "1.2.3", None, False, bundle, (None, None))
         assert m.row == ("module", "1.2.3", "unknown", "Major Version")
-        m = circup.Module(
-            name, backend, repo, "1.2.3", "1.3.4", False, bundle, (None, None)
-        )
+        m = Module(name, backend, repo, "1.2.3", "1.3.4", False, bundle, (None, None))
         assert m.row == ("module", "1.2.3", "1.3.4", "Minor Version")
-        m = circup.Module(
-            name, backend, repo, "1.2.3", "1.2.3", True, bundle, ("9.0.0", None)
-        )
+        m = Module(name, backend, repo, "1.2.3", "1.2.3", True, bundle, ("9.0.0", None))
         assert m.row == ("module", "1.2.3", "1.2.3", "MPY Format")
 
 
 def test_Module_update_dir():
     """
     Ensure if the module is a directory, the expected actions take place to
     update the module on the connected device.
     """
     bundle = circup.Bundle(TEST_BUNDLE_NAME)
     name = "adafruit_waveform"
     repo = "https://github.com/adafruit/SomeLibrary.git"
     device_version = "1.2.3"
     bundle_version = None
     with mock.patch("circup.backends.shutil") as mock_shutil, mock.patch(
-        "circup.os.path.isdir", return_value=True
-    ), mock.patch("circup.logger.warning") as mock_logger:
-        backend = DiskBackend("mock_device", mock_logger)
-        m = circup.Module(
+        "circup.logger.warning"
+    ) as mock_logger:
+        backend = DiskBackend("tests/mock_device", mock_logger)
+        m = Module(
             name,
             backend,
             repo,
             device_version,
             bundle_version,
             False,
             bundle,
@@ -480,21 +469,17 @@
     # path = os.path.join("foo", "bar", "baz", "module.py")
     repo = "https://github.com/adafruit/SomeLibrary.git"
     device_version = "1.2.3"
     bundle_version = None
 
     with mock.patch("circup.backends.shutil") as mock_shutil, mock.patch(
         "circup.os.remove"
-    ) as mock_remove, mock.patch(
-        "circup.os.path.isdir", return_value=False
-    ), mock.patch(
-        "circup.logger.warning"
-    ) as mock_logger:
-        backend = circup.DiskBackend("mock_device", mock_logger)
-        m = circup.Module(
+    ) as mock_remove, mock.patch("circup.logger.warning") as mock_logger:
+        backend = circup.DiskBackend("tests/mock_device", mock_logger)
+        m = Module(
             name,
             backend,
             repo,
             device_version,
             bundle_version,
             False,
             bundle,
@@ -511,21 +496,22 @@
     """
     name = "local_module.py"
     path = os.path.join("mock_device", "lib", f"{name}")
     repo = "https://github.com/adafruit/SomeLibrary.git"
     device_version = "1.2.3"
     bundle_version = "3.2.1"
     with mock.patch("circup.os.path.isfile", return_value=True), mock.patch(
-        "circup.CPY_VERSION", "4.1.2"
+        "circup.backends.DiskBackend.get_circuitpython_version",
+        return_value=("4.1.2", ""),
     ), mock.patch("circup.Bundle.lib_dir", return_value="tests"), mock.patch(
         "circup.logger.warning"
     ) as mock_logger:
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         backend = circup.DiskBackend("mock_device", mock_logger)
-        m = circup.Module(
+        m = Module(
             name,
             backend,
             repo,
             device_version,
             bundle_version,
             False,
             bundle,
@@ -551,45 +537,47 @@
     """
     Simulate being on os.name == 'posix' and a call to "mount" returns a
     record indicating a connected device.
     """
     with open("tests/mount_exists.txt", "rb") as fixture_file:
         fixture = fixture_file.read()
         with mock.patch("os.name", "posix"):
-            with mock.patch("circup.check_output", return_value=fixture):
-                assert circup.find_device() == "/media/ntoll/CIRCUITPY"
+            with mock.patch("circup.command_utils.check_output", return_value=fixture):
+                assert find_device() == "/media/ntoll/CIRCUITPY"
 
 
 def test_find_device_posix_no_mount_command():
     """
     When the user doesn't have administrative privileges on OSX then the mount
     command isn't on their path. In which case, check circup uses the more
     explicit /sbin/mount instead.
     """
     with open("tests/mount_exists.txt", "rb") as fixture_file:
         fixture = fixture_file.read()
     mock_check = mock.MagicMock(side_effect=[FileNotFoundError, fixture])
-    with mock.patch("os.name", "posix"), mock.patch("circup.check_output", mock_check):
-        assert circup.find_device() == "/media/ntoll/CIRCUITPY"
+    with mock.patch("os.name", "posix"), mock.patch(
+        "circup.command_utils.check_output", mock_check
+    ):
+        assert find_device() == "/media/ntoll/CIRCUITPY"
         assert mock_check.call_count == 2
         assert mock_check.call_args_list[0][0][0] == "mount"
         assert mock_check.call_args_list[1][0][0] == "/sbin/mount"
 
 
 def test_find_device_posix_missing():
     """
     Simulate being on os.name == 'posix' and a call to "mount" returns no
     records associated with an Adafruit device.
     """
     with open("tests/mount_missing.txt", "rb") as fixture_file:
         fixture = fixture_file.read()
         with mock.patch("os.name", "posix"), mock.patch(
-            "circup.check_output", return_value=fixture
+            "circup.command_utils.check_output", return_value=fixture
         ):
-            assert circup.find_device() is None
+            assert find_device() is None
 
 
 def test_find_device_nt_exists():
     """
     Simulate being on os.name == 'nt' and a disk with a volume name 'CIRCUITPY'
     exists indicating a connected device.
     """
@@ -598,15 +586,15 @@
     mock_windll.kernel32.GetVolumeInformationW = mock.MagicMock()
     mock_windll.kernel32.GetVolumeInformationW.return_value = None
     fake_buffer = ctypes.create_unicode_buffer("CIRCUITPY")
     with mock.patch("os.name", "nt"), mock.patch(
         "os.path.exists", return_value=True
     ), mock.patch("ctypes.create_unicode_buffer", return_value=fake_buffer):
         ctypes.windll = mock_windll
-        assert circup.find_device() == "A:\\"
+        assert find_device() == "A:\\"
 
 
 def test_find_device_nt_missing():
     """
     Simulate being on os.name == 'nt' and a disk with a volume name 'CIRCUITPY'
     does not exist for a device.
     """
@@ -615,40 +603,40 @@
     mock_windll.kernel32.GetVolumeInformationW = mock.MagicMock()
     mock_windll.kernel32.GetVolumeInformationW.return_value = None
     fake_buffer = ctypes.create_unicode_buffer(1024)
     with mock.patch("os.name", "nt"), mock.patch(
         "os.path.exists", return_value=True
     ), mock.patch("ctypes.create_unicode_buffer", return_value=fake_buffer):
         ctypes.windll = mock_windll
-        assert circup.find_device() is None
+        assert find_device() is None
 
 
 def test_find_device_unknown_os():
     """
     Raises a NotImplementedError if the host OS is not supported.
     """
     with mock.patch("os.name", "foo"):
         with pytest.raises(NotImplementedError) as ex:
-            circup.find_device()
+            find_device()
     assert ex.value.args[0] == 'OS "foo" not supported.'
 
 
 def test_get_latest_release_from_url():
     """
     Ensure the expected tag value is extracted from the returned URL (resulting
     from a call to the expected endpoint).
     """
     response = mock.MagicMock()
     response.headers = {
         "Location": "https://github.com/adafruit"
         "/Adafruit_CircuitPython_Bundle/releases/tag/20190903"
     }
     expected_url = "https://github.com/" + TEST_BUNDLE_NAME + "/releases/latest"
-    with mock.patch("circup.requests.head", return_value=response) as mock_get:
-        result = circup.get_latest_release_from_url(expected_url)
+    with mock.patch("circup.shared.requests.head", return_value=response) as mock_get:
+        result = circup.get_latest_release_from_url(expected_url, logger)
         assert result == "20190903"
         mock_get.assert_called_once_with(expected_url, timeout=mock.ANY)
 
 
 def test_extract_metadata_python():
     """
     Ensure the dunder objects assigned in code are extracted into a Python
@@ -706,17 +694,15 @@
         device_modules = json.load(f)
     with open("tests/bundle.json", "rb") as f:
         bundle_modules = json.load(f)
 
     with mock.patch(
         "circup.DiskBackend.get_device_versions", return_value=device_modules
     ), mock.patch(
-        "circup.get_bundle_versions", return_value=bundle_modules
-    ), mock.patch(
-        "circup.os.path.isfile", return_value=True
+        "circup.command_utils.get_bundle_versions", return_value=bundle_modules
     ), mock.patch(
         "circup.logger.warning"
     ) as mock_logger:
         backend = DiskBackend("mock_device", mock_logger)
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         bundles_list = [bundle]
         for module in bundle_modules:
@@ -734,15 +720,15 @@
 def test_find_modules_goes_bang():
     """
     Ensure if there's a problem getting metadata an error message is displayed
     and the utility exists with an error code of 1.
     """
     with mock.patch(
         "circup.DiskBackend.get_device_versions", side_effect=Exception("BANG!")
-    ), mock.patch("circup.click") as mock_click, mock.patch(
+    ), mock.patch("circup.command_utils.click") as mock_click, mock.patch(
         "circup.sys.exit"
     ) as mock_exit, mock.patch(
         "circup.logger.warning"
     ) as mock_logger:
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         bundles_list = [bundle]
         backend = DiskBackend("mock_devcie", mock_logger)
@@ -752,22 +738,27 @@
 
 
 def test_get_bundle_versions():
     """
     Ensure get_modules is called with the path for the library bundle.
     Ensure ensure_latest_bundle is called even if lib_dir exists.
     """
-    with mock.patch("circup.ensure_latest_bundle") as mock_elb, mock.patch(
-        "circup._get_modules_file", return_value={"ok": {"name": "ok"}}
-    ) as mock_gm, mock.patch("circup.CPY_VERSION", "4.1.2"), mock.patch(
-        "circup.Bundle.lib_dir", return_value="foo/bar/lib"
+    with mock.patch(
+        "circup.command_utils.ensure_latest_bundle"
+    ) as mock_elb, mock.patch(
+        "circup.command_utils._get_modules_file", return_value={"ok": {"name": "ok"}}
+    ) as mock_gm, mock.patch(
+        "circup.backends.DiskBackend.get_circuitpython_version",
+        return_value=("4.1.2", ""),
+    ), mock.patch(
+        "circup.bundle.Bundle.lib_dir", return_value="foo/bar/lib"
     ), mock.patch(
         "circup.os.path.isdir", return_value=True
     ), mock.patch(
-        "circup.logger"
+        "circup.command_utils.logger"
     ) as mock_logger:
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         bundles_list = [bundle]
         assert circup.get_bundle_versions(bundles_list) == {
             "ok": {"name": "ok", "bundle": bundle}
         }
         mock_elb.assert_called_once_with(bundle)
@@ -775,20 +766,25 @@
 
 
 def test_get_bundle_versions_avoid_download():
     """
     When avoid_download is True and lib_dir exists, don't ensure_latest_bundle.
     Testing both cases: lib_dir exists and lib_dir doesn't exists.
     """
-    with mock.patch("circup.ensure_latest_bundle") as mock_elb, mock.patch(
-        "circup._get_modules_file", return_value={"ok": {"name": "ok"}}
-    ) as mock_gm, mock.patch("circup.CPY_VERSION", "4.1.2"), mock.patch(
+    with mock.patch(
+        "circup.command_utils.ensure_latest_bundle"
+    ) as mock_elb, mock.patch(
+        "circup.command_utils._get_modules_file", return_value={"ok": {"name": "ok"}}
+    ) as mock_gm, mock.patch(
+        "circup.backends.DiskBackend.get_circuitpython_version",
+        return_value=("4.1.2", ""),
+    ), mock.patch(
         "circup.Bundle.lib_dir", return_value="foo/bar/lib"
     ), mock.patch(
-        "circup.logger"
+        "circup.command_utils.logger"
     ) as mock_logger:
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
         bundles_list = [bundle]
         with mock.patch("circup.os.path.isdir", return_value=True):
             assert circup.get_bundle_versions(bundles_list, avoid_download=True) == {
                 "ok": {"name": "ok", "bundle": bundle}
             }
@@ -806,29 +802,29 @@
     """
     Given valid content of a boot_out.txt file on a connected device, return
     the version number of CircuitPython running on the board.
     """
     with mock.patch("circup.logger.warning") as mock_logger:
         backend = DiskBackend("tests/mock_device", mock_logger)
         assert backend.get_circuitpython_version() == (
-            "4.1.0",
+            "8.1.0",
             "this_is_a_board",
         )
 
 
 def test_get_device_versions():
     """
     Ensure get_modules is called with the path for the attached device.
     """
     with mock.patch(
         "circup.DiskBackend.get_modules", return_value="ok"
     ) as mock_gm, mock.patch("circup.logger.warning") as mock_logger:
-        backend = circup.DiskBackend("mock_device", mock_logger)
+        backend = circup.DiskBackend("tests/mock_device", mock_logger)
         assert backend.get_device_versions() == "ok"
-        mock_gm.assert_called_once_with(os.path.join("mock_device", "lib"))
+        mock_gm.assert_called_once_with(os.path.join("tests", "mock_device", "lib"))
 
 
 def test_get_modules_empty_path():
     """
     Sometimes a path to a device or bundle may be empty. Ensure, if this is the
     case, an empty dictionary is returned.
     """
@@ -843,15 +839,15 @@
     (mocked) results of glob and open on file based Python modules.
     """
     path = "tests"  # mocked away in function.
     mods = [
         os.path.join("tests", "local_module.py"),
         os.path.join("tests", ".hidden_module.py"),
     ]
-    with mock.patch("circup.glob.glob", side_effect=[mods, [], []]), mock.patch(
+    with mock.patch("circup.shared.glob.glob", side_effect=[mods, [], []]), mock.patch(
         "circup.logger.warning"
     ) as mock_logger:
         backend = circup.DiskBackend("mock_device", mock_logger)
         result = backend.get_modules(path)
         assert len(result) == 1  # Hidden files are ignored.
         assert "local_module" in result
         assert result["local_module"]["path"] == os.path.join(
@@ -870,15 +866,15 @@
     path = "tests"  # mocked away in function.
     mods = [
         os.path.join("tests", "dir_module", ""),
         os.path.join("tests", ".hidden_dir", ""),
     ]
     mod_files = ["tests/dir_module/my_module.py", "tests/dir_module/__init__.py"]
     with mock.patch(
-        "circup.glob.glob", side_effect=[[], [], mods, mod_files, []]
+        "circup.shared.glob.glob", side_effect=[[], [], mods, mod_files, []]
     ), mock.patch("circup.logger.warning") as mock_logger:
         backend = circup.DiskBackend("mock_device", mock_logger)
         result = backend.get_modules(path)
         assert len(result) == 1
         assert "dir_module" in result
         assert result["dir_module"]["path"] == os.path.join("tests", "dir_module", "")
         assert result["dir_module"]["__version__"] == "3.2.1"  # from fixture.
@@ -891,15 +887,15 @@
     Check the expected dictionary containing just the path is returned given
     the (mocked) results of glob and open, on directory based Python modules.
     """
     path = "tests"  # mocked away in function.
     mods = [os.path.join("tests", "bad_module", "")]
     mod_files = ["tests/bad_module/my_module.py", "tests/bad_module/__init__.py"]
     with mock.patch(
-        "circup.glob.glob", side_effect=[[], [], mods, mod_files, []]
+        "circup.shared.glob.glob", side_effect=[[], [], mods, mod_files, []]
     ), mock.patch("circup.logger.warning") as mock_logger:
         backend = circup.DiskBackend("mock_device", mock_logger)
         result = backend.get_modules(path)
         assert len(result) == 1
         assert "bad_module" in result
         assert result["bad_module"]["path"] == os.path.join("tests", "bad_module", "")
         assert "__version__" not in result["bad_module"]
@@ -907,67 +903,63 @@
 
 
 def test_ensure_latest_bundle_no_bundle_data():
     """
     If there's no BUNDLE_DATA file (containing previous current version of the
     bundle) then default to update.
     """
-    with mock.patch("circup.Bundle.latest_tag", "12345"), mock.patch(
+    with mock.patch("circup.bundle.Bundle.latest_tag", "12345"), mock.patch(
         "circup.os.path.isfile", return_value=False
-    ), mock.patch("circup.get_bundle") as mock_gb, mock.patch(
-        "circup.json"
+    ), mock.patch("circup.command_utils.get_bundle") as mock_gb, mock.patch(
+        "circup.command_utils.json"
     ) as mock_json, mock.patch(
-        "circup.open"
+        "circup.command_utils.open"
     ):
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        circup.ensure_latest_bundle(bundle)
+        ensure_latest_bundle(bundle)
         mock_gb.assert_called_once_with(bundle, "12345")
         assert mock_json.dump.call_count == 1  # Current version saved to file.
 
 
 def test_ensure_latest_bundle_bad_bundle_data():
     """
     If there's a BUNDLE_DATA file (containing previous current version of the
     bundle) but it has been corrupted (which has sometimes happened during
     manual testing) then default to update.
     """
-    with mock.patch("circup.Bundle.latest_tag", "12345"), mock.patch(
-        "circup.os.path.isfile", return_value=True
-    ), mock.patch("circup.open"), mock.patch(
-        "circup.get_bundle"
-    ) as mock_gb, mock.patch(
-        "circup.json.load", side_effect=json.decoder.JSONDecodeError("BANG!", "doc", 1)
+    with mock.patch("circup.bundle.Bundle.latest_tag", "12345"), mock.patch(
+        "circup.command_utils.open"
+    ), mock.patch("circup.command_utils.get_bundle") as mock_gb, mock.patch(
+        "builtins.open", mock.mock_open(read_data="}{INVALID_JSON")
     ), mock.patch(
-        "circup.json.dump"
+        "circup.command_utils.json.dump"
     ), mock.patch(
-        "circup.logger"
+        "circup.bundle.logger"
     ) as mock_logger:
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        circup.ensure_latest_bundle(bundle)
+        ensure_latest_bundle(bundle)
         mock_gb.assert_called_once_with(bundle, "12345")
-        # wrong file is opened twice (one at __init__, one at save())
-        assert mock_logger.error.call_count == 2
-        assert mock_logger.exception.call_count == 2
+
+        assert mock_logger.error.call_count == 1
+        assert mock_logger.exception.call_count == 1
 
 
 def test_ensure_latest_bundle_to_update():
     """
     If the version found in the BUNDLE_DATA is out of date, then cause an
     update to the bundle.
     """
-    with mock.patch("circup.Bundle.latest_tag", "54321"), mock.patch(
-        "circup.os.path.isfile", return_value=True
-    ), mock.patch("circup.open"), mock.patch(
-        "circup.get_bundle"
-    ) as mock_gb, mock.patch(
-        "circup.json"
+    with mock.patch("circup.bundle.Bundle.latest_tag", "54321"), mock.patch(
+        "circup.command_utils.open"
+    ), mock.patch("circup.command_utils.get_bundle") as mock_gb, mock.patch(
+        "circup.command_utils.json"
     ) as mock_json:
         mock_json.load.return_value = {TEST_BUNDLE_NAME: "12345"}
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        circup.ensure_latest_bundle(bundle)
+        ensure_latest_bundle(bundle)
         mock_gb.assert_called_once_with(bundle, "54321")
         assert mock_json.dump.call_count == 1  # Current version saved to file.
 
 
 def test_ensure_latest_bundle_to_update_http_error():
     """
     If an HTTP error happens during a bundle update, print a friendly
@@ -975,49 +967,50 @@
     """
     tags_data = {TEST_BUNDLE_NAME: "12345"}
     with mock.patch("circup.Bundle.latest_tag", "54321"), mock.patch(
         #         "circup.tags_data_load", return_value=tags_data
         #     ), mock.patch(
         "circup.os.path.isfile",
         return_value=True,
-    ), mock.patch("circup.open"), mock.patch(
-        "circup.get_bundle", side_effect=requests.exceptions.HTTPError("404")
+    ), mock.patch("circup.command_utils.open"), mock.patch(
+        "circup.command_utils.get_bundle",
+        side_effect=requests.exceptions.HTTPError("404"),
     ) as mock_gb, mock.patch(
-        "circup.json"
+        "circup.command_utils.json"
     ) as mock_json, mock.patch(
         "circup.click.secho"
     ) as mock_click:
         circup.Bundle.tags_data = dict()
         mock_json.load.return_value = tags_data
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        circup.ensure_latest_bundle(bundle)
+        ensure_latest_bundle(bundle)
         mock_gb.assert_called_once_with(bundle, "54321")
         assert mock_json.dump.call_count == 0  # not saved.
         assert mock_click.call_count == 1  # friendly message.
 
 
 def test_ensure_latest_bundle_no_update():
     """
     If the version found in the BUNDLE_DATA is NOT out of date, just log the
     fact and don't update.
     """
-    with mock.patch("circup.Bundle.latest_tag", "12345"), mock.patch(
-        "circup.os.path.isfile", return_value=True
-    ), mock.patch("circup.os.path.isdir", return_value=True), mock.patch(
-        "circup.open"
-    ), mock.patch(
-        "circup.get_bundle"
+    with mock.patch("circup.bundle.Bundle.latest_tag", "12345"), mock.patch(
+        "circup.command_utils.os.path.isdir", return_value=True
+    ), mock.patch("circup.command_utils.open"), mock.patch(
+        "circup.command_utils.get_bundle"
     ) as mock_gb, mock.patch(
-        "circup.json"
-    ) as mock_json, mock.patch(
-        "circup.logger"
+        "circup.command_utils.os.path.isfile", return_value=True
+    ), mock.patch(
+        "circup.bundle.Bundle.current_tag", "12345"
+    ), mock.patch(
+        "circup.command_utils.logger"
     ) as mock_logger:
-        mock_json.load.return_value = {TEST_BUNDLE_NAME: "12345"}
+
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        circup.ensure_latest_bundle(bundle)
+        ensure_latest_bundle(bundle)
         assert mock_gb.call_count == 0
         assert mock_logger.info.call_count == 2
 
 
 def test_get_bundle():
     """
     Ensure the expected calls are made to get the referenced bundle and the
@@ -1025,57 +1018,57 @@
     """
     # All these mocks stop IO side effects and allow us to spy on the code to
     # ensure the expected calls are made with the correct values. Warning! Here
     # Be Dragons! (If in doubt, ask ntoll for details).
     mock_progress = mock.MagicMock()
     mock_progress().__enter__ = mock.MagicMock(return_value=["a", "b", "c"])
     mock_progress().__exit__ = mock.MagicMock()
-    with mock.patch("circup.requests") as mock_requests, mock.patch(
+    with mock.patch("circup.command_utils.requests") as mock_requests, mock.patch(
         "circup.click"
     ) as mock_click, mock.patch(
-        "circup.open", mock.mock_open()
+        "circup.command_utils.open", mock.mock_open()
     ) as mock_open, mock.patch(
         "circup.os.path.isdir", return_value=True
     ), mock.patch(
-        "circup.shutil"
+        "circup.command_utils.shutil"
     ) as mock_shutil, mock.patch(
-        "circup.zipfile"
+        "circup.command_utils.zipfile"
     ) as mock_zipfile:
         mock_click.progressbar = mock_progress
         mock_requests.get().status_code = mock_requests.codes.ok
         mock_requests.get.reset_mock()
         tag = "12345"
         bundle = circup.Bundle(TEST_BUNDLE_NAME)
-        circup.get_bundle(bundle, tag)
+        get_bundle(bundle, tag)
         # how many bundles currently supported. i.e. 6x.mpy, 7x.mpy, py = 3 bundles
-        _bundle_count = len(circup.PLATFORMS)
+        _bundle_count = len(PLATFORMS)
         assert mock_requests.get.call_count == _bundle_count
         assert mock_open.call_count == _bundle_count
         assert mock_shutil.rmtree.call_count == _bundle_count
         assert mock_zipfile.ZipFile.call_count == _bundle_count
         assert mock_zipfile.ZipFile().__enter__().extractall.call_count == _bundle_count
 
 
 def test_get_bundle_network_error():
     """
     Ensure that if there is a network related error when grabbing the bundle
     then the error is logged and re-raised for the HTTP status code.
     """
-    with mock.patch("circup.requests") as mock_requests, mock.patch(
-        "circup.tags_data_load", return_value=dict()
-    ), mock.patch("circup.logger") as mock_logger:
+    with mock.patch("circup.command_utils.requests") as mock_requests, mock.patch(
+        "circup.shared.tags_data_load", return_value=dict()
+    ), mock.patch("circup.command_utils.logger") as mock_logger:
         # Force failure with != requests.codes.ok
         mock_requests.get().status_code = mock_requests.codes.BANG
         # Ensure raise_for_status actually raises an exception.
         mock_requests.get().raise_for_status.return_value = Exception("Bang!")
         mock_requests.get.reset_mock()
         tag = "12345"
         with pytest.raises(Exception) as ex:
             bundle = circup.Bundle(TEST_BUNDLE_NAME)
-            circup.get_bundle(bundle, tag)
+            get_bundle(bundle, tag)
             assert ex.value.args[0] == "Bang!"
         url = (
             "https://github.com/" + TEST_BUNDLE_NAME + "/releases/download"
             "/{tag}/adafruit-circuitpython-bundle-py-{tag}.zip".format(tag=tag)
         )
         mock_requests.get.assert_called_once_with(url, stream=True, timeout=mock.ANY)
         assert mock_logger.warning.call_count == 1
@@ -1084,39 +1077,45 @@
 
 def test_show_command():
     """
     test_show_command
     """
     runner = CliRunner()
     test_bundle_modules = ["one.py", "two.py", "three.py"]
-    with mock.patch("circup.get_bundle_versions", return_value=test_bundle_modules):
+    with mock.patch(
+        "circup.commands.get_bundle_versions", return_value=test_bundle_modules
+    ):
         result = runner.invoke(circup.show)
     assert result.exit_code == 0
     assert all(m.replace(".py", "") in result.output for m in test_bundle_modules)
 
 
 def test_show_match_command():
     """
     test_show_match_command
     """
     runner = CliRunner()
     test_bundle_modules = ["one.py", "two.py", "three.py"]
-    with mock.patch("circup.get_bundle_versions", return_value=test_bundle_modules):
+    with mock.patch(
+        "circup.commands.get_bundle_versions", return_value=test_bundle_modules
+    ):
         result = runner.invoke(circup.show, ["t"])
     assert result.exit_code == 0
     assert "one" not in result.output
 
 
 def test_show_match_py_command():
     """
-    Check that py does not match the .py extention in the module names
+    Check that py does not match the .py extension in the module names
     """
     runner = CliRunner()
     test_bundle_modules = ["one.py", "two.py", "three.py"]
-    with mock.patch("circup.get_bundle_versions", return_value=test_bundle_modules):
+    with mock.patch(
+        "circup.commands.get_bundle_versions", return_value=test_bundle_modules
+    ):
         result = runner.invoke(circup.show, ["py"])
     assert result.exit_code == 0
     assert "0 shown" in result.output
 
 
 def test_libraries_from_imports():
     """Ensure that various styles of import all work"""
@@ -1143,15 +1142,17 @@
 
 
 def test_libraries_from_imports_bad():
     """Ensure that we catch an import error"""
     TEST_BUNDLE_MODULES = {"one.py": {}, "two.py": {}, "three.py": {}}
     runner = CliRunner()
 
-    with mock.patch("circup.get_bundle_versions", return_value=TEST_BUNDLE_MODULES):
+    with mock.patch(
+        "circup.commands.get_bundle_versions", return_value=TEST_BUNDLE_MODULES
+    ):
         result = runner.invoke(
             circup.main,
             [
                 "--path",
                 "./tests/mock_device/",
                 "install",
                 "--auto-file",
```

### Comparing `circup-1.6.2/tests/test_module.mpy` & `circup-1.7.0/tests/test_module.mpy`

 * *Files identical despite different names*

