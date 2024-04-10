# Comparing `tmp/blackboardsync-0.9.8.tar.gz` & `tmp/blackboardsync-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.8.tar", last modified: Wed Sep  6 23:21:13 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.9.tar", last modified: Sun Sep 17 01:59:43 2023, max compression
```

## Comparing `blackboardsync-0.9.8.tar` & `blackboardsync-0.9.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.273540 blackboardsync-0.9.8/.github/
--rw-r--r--   0 runner    (1001) docker     (999)       94 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.273540 blackboardsync-0.9.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (999)     2659 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (999)      501 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.273540 blackboardsync-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     3907 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (999)     3291 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)     3537 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (999)     1666 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)    18092 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     6025 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      839 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (999)   116060 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (999)     5363 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (999)     3265 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.273540 blackboardsync-0.9.8/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (999)     1260 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1138 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      979 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.273540 blackboardsync-0.9.8/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (999)     1619 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (999)     2275 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (999)   110234 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (999)    31742 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (999)    36877 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.273540 blackboardsync-0.9.8/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (999)     1803 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    29706 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (999)     6587 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (999)     4081 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (999)    11226 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (999)     4081 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (999)     1120 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (999)     5032 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (999)     8488 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (999)     6564 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (999)     3187 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (999)     1560 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    21822 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (999)    11177 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (999)     7760 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (999)    13787 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (999)     1421 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (999)     2075 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     6025 2023-09-06 23:21:13.000000 blackboardsync-0.9.8/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1623 2023-09-06 23:21:13.000000 blackboardsync-0.9.8/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-06 23:21:13.000000 blackboardsync-0.9.8/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      205 2023-09-06 23:21:13.000000 blackboardsync-0.9.8/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       16 2023-09-06 23:21:13.000000 blackboardsync-0.9.8/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/docs/
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (999)       70 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (999)     3080 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (999)      385 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (999)      194 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (999)      362 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1291 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      795 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (999)      994 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/main.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/packaging/
--rw-r--r--   0 runner    (1001) docker     (999)      842 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (999)     2757 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (999)     1319 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (999)     1270 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 23:21:13.277540 blackboardsync-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3120 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (999)     4589 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     2376 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (999)     5336 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (999)    12707 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (999)     1618 2023-09-06 23:20:29.000000 blackboardsync-0.9.8/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.640570 blackboardsync-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.632569 blackboardsync-0.9.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.632569 blackboardsync-0.9.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.632569 blackboardsync-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2023-09-17 01:59:43.640570 blackboardsync-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)   116060 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.632569 blackboardsync-0.9.9/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.636569 blackboardsync-0.9.9/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   110234 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    31742 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36877 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.636569 blackboardsync-0.9.9/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29706 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.636569 blackboardsync-0.9.9/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13787 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.636569 blackboardsync-0.9.9/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2023-09-17 01:59:43.000000 blackboardsync-0.9.9/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-09-17 01:59:43.000000 blackboardsync-0.9.9/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 01:59:43.000000 blackboardsync-0.9.9/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-09-17 01:59:43.000000 blackboardsync-0.9.9/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-17 01:59:43.000000 blackboardsync-0.9.9/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.636569 blackboardsync-0.9.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.636569 blackboardsync-0.9.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.636569 blackboardsync-0.9.9/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.640570 blackboardsync-0.9.9/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-17 01:59:43.640570 blackboardsync-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 01:59:43.640570 blackboardsync-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12707 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-09-17 01:58:41.000000 blackboardsync-0.9.9/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.8/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.9/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/.github/workflows/build.yml` & `blackboardsync-0.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/.gitignore` & `blackboardsync-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/CHANGELOG.md` & `blackboardsync-0.9.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+
+## [0.9.9] - 2023-09-17
+
+### Fixed
+- Bug with pydantic Url typing
+
 ## [0.9.8] - 2023-09-07
 
 ### Changed
 - Multiple dependency updates including a security update
 
 ## [0.9.7] - 2023-06-30
```

### Comparing `blackboardsync-0.9.8/CONTRIBUTING.md` & `blackboardsync-0.9.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/LICENSE` & `blackboardsync-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/PKG-INFO` & `blackboardsync-0.9.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: blackboardsync
-Version: 0.9.8
-Summary: Sync your blackboard content to your device
-Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
-Project-URL: Homepage, https://bbsync.app
-Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
-Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: package
-License-File: LICENSE
-
 # BlackboardSync
 ### Automatic Syncing Of Your Blackboard Content
 
 [![Get on PyPI][pypi-shield]][pypi] [![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
 
 **BlackboardSync** performs a periodic, incremental download of all your Blackboard content, such as lecture slides, lab sheets, and other attachments.
```

### Comparing `blackboardsync-0.9.8/Pipfile` & `blackboardsync-0.9.9/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/Pipfile.lock` & `blackboardsync-0.9.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/README.md` & `blackboardsync-0.9.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: blackboardsync
+Version: 0.9.9
+Summary: Sync your blackboard content to your device
+Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
+Project-URL: Homepage, https://bbsync.app
+Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
+Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyqt5>=5.15.9
+Requires-Dist: pyqtwebengine
+Requires-Dist: beautifulsoup4
+Requires-Dist: pydantic
+Requires-Dist: pathvalidate
+Requires-Dist: python-dateutil
+Requires-Dist: appdirs
+Requires-Dist: lxml
+Requires-Dist: requests
+Requires-Dist: packaging
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: hypothesis; extra == "test"
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest-qt; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Provides-Extra: package
+Requires-Dist: pyinstaller; extra == "package"
+Requires-Dist: build; extra == "package"
+Requires-Dist: twine; extra == "package"
+
 # BlackboardSync
 ### Automatic Syncing Of Your Blackboard Content
 
 [![Get on PyPI][pypi-shield]][pypi] [![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
 
 **BlackboardSync** performs a periodic, incremental download of all your Blackboard content, such as lecture slides, lab sheets, and other attachments.
```

### Comparing `blackboardsync-0.9.8/UNIVERSITIES.md` & `blackboardsync-0.9.9/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/__about__.py` & `blackboardsync-0.9.9/blackboard_sync/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.8/blackboard_sync/__init__.py` & `blackboardsync-0.9.9/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/__main__.py` & `blackboardsync-0.9.9/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.9/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.9/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.9/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.9/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.9/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.9/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.9/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.9/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/config.py` & `blackboardsync-0.9.9/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/download.py` & `blackboardsync-0.9.9/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/institutions.py` & `blackboardsync-0.9.9/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.9/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.9/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.9/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.9/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.9/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.9/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.9/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/sync.py` & `blackboardsync-0.9.9/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.9/blackboard_sync/sync_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,16 @@
                          self.setup_window.download_location,
                          self.setup_window.min_year)
         self._build_login_window(self.model.university.login)
         self._show_login_window()
 
     def _build_login_window(self, uni_login_info: InstitutionLogin) -> None:
         # Get login url from uni DB
-        self.login_window = LoginWebView(start_url=uni_login_info.start_url,
-                                         target_url=uni_login_info.target_url)
+        self.login_window = LoginWebView(start_url=str(uni_login_info.start_url),
+                                         target_url=str(uni_login_info.target_url))
         self.login_window.login_complete_signal.connect(self._login_complete)
 
     def _login_complete(self) -> None:
         if self.login_window is None:
             return
 
         self.app.setOverrideCursor(Qt.WaitCursor)
```

### Comparing `blackboardsync-0.9.8/blackboard_sync/universities.json` & `blackboardsync-0.9.9/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/updates.py` & `blackboardsync-0.9.9/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboard_sync/webdav.py` & `blackboardsync-0.9.9/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.9/blackboardsync.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.8
+Version: 0.9.9
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyqt5>=5.15.9
+Requires-Dist: pyqtwebengine
+Requires-Dist: beautifulsoup4
+Requires-Dist: pydantic
+Requires-Dist: pathvalidate
+Requires-Dist: python-dateutil
+Requires-Dist: appdirs
+Requires-Dist: lxml
+Requires-Dist: requests
+Requires-Dist: packaging
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: hypothesis; extra == "test"
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest-qt; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: package
-License-File: LICENSE
+Requires-Dist: pyinstaller; extra == "package"
+Requires-Dist: build; extra == "package"
+Requires-Dist: twine; extra == "package"
 
 # BlackboardSync
 ### Automatic Syncing Of Your Blackboard Content
 
 [![Get on PyPI][pypi-shield]][pypi] [![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
 
 **BlackboardSync** performs a periodic, incremental download of all your Blackboard content, such as lecture slides, lab sheets, and other attachments.
```

### Comparing `blackboardsync-0.9.8/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.9/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/docs/Makefile` & `blackboardsync-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/docs/conf.py` & `blackboardsync-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/docs/index.rst` & `blackboardsync-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/docs/make.bat` & `blackboardsync-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/main.py` & `blackboardsync-0.9.9/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/packaging/pkg_macos.sh` & `blackboardsync-0.9.9/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/packaging/pkg_win.nsi` & `blackboardsync-0.9.9/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/packaging/pyinst.py` & `blackboardsync-0.9.9/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/pyproject.toml` & `blackboardsync-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/tests/strategies.py` & `blackboardsync-0.9.9/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/tests/test_api.py` & `blackboardsync-0.9.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/tests/test_blackboard.py` & `blackboardsync-0.9.9/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/tests/test_download.py` & `blackboardsync-0.9.9/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/tests/test_qt.py` & `blackboardsync-0.9.9/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.8/tests/test_sync_config.py` & `blackboardsync-0.9.9/tests/test_sync_config.py`

 * *Files identical despite different names*

