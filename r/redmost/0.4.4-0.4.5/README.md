# Comparing `tmp/redmost-0.4.4.tar.gz` & `tmp/redmost-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmost-0.4.4.tar", last modified: Thu Mar 21 11:13:14 2024, max compression
+gzip compressed data, was "redmost-0.4.5.tar", last modified: Wed Apr 10 06:15:15 2024, max compression
```

## Comparing `redmost-0.4.4.tar` & `redmost-0.4.5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.873338 redmost-0.4.4/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.863338 redmost-0.4.4/.github/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.866671 redmost-0.4.4/.github/workflows/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1124 2024-03-20 13:43:32.000000 redmost-0.4.4/.github/workflows/pre-release.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1051 2024-03-20 13:43:36.000000 redmost-0.4.4/.github/workflows/tagged-release.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1228 2024-03-20 13:43:41.000000 redmost-0.4.4/.github/workflows/test_linux_lint.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1462 2024-03-19 19:35:03.000000 redmost-0.4.4/.github/workflows/test_linux_pyqt5.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2024-03-19 09:56:49.000000 redmost-0.4.4/.github/workflows/test_linux_pyqt6.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1468 2024-03-19 09:57:41.000000 redmost-0.4.4/.github/workflows/test_linux_pyside6.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2024-03-18 13:57:53.000000 redmost-0.4.4/.readthedocs.yaml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1535 2024-03-11 07:22:12.000000 redmost-0.4.4/LICENSE
--rw-r--r--   0 daddona   (1000) daddona   (1000)     6878 2024-03-21 11:13:14.873338 redmost-0.4.4/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3890 2024-03-20 10:51:05.000000 redmost-0.4.4/README.md
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.866671 redmost-0.4.4/docs/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.863338 redmost-0.4.4/docs/_static/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.866671 redmost-0.4.4/docs/_static/css/
--rw-r--r--   0 daddona   (1000) daddona   (1000)       60 2023-09-21 08:50:12.000000 redmost-0.4.4/docs/_static/css/custom.css
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2905 2024-03-18 14:10:16.000000 redmost-0.4.4/docs/conf.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      192 2024-03-19 12:03:17.000000 redmost-0.4.4/docs/docs.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2860 2024-03-20 10:51:01.000000 redmost-0.4.4/docs/index.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2548 2024-03-19 13:12:54.000000 redmost-0.4.4/docs/installation.rst
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.866671 redmost-0.4.4/docs/module_docs/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      113 2024-03-18 13:06:03.000000 redmost-0.4.4/docs/module_docs/backends_rrock.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       80 2024-03-18 12:38:22.000000 redmost-0.4.4/docs/module_docs/gui.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 13:46:27.000000 redmost-0.4.4/docs/module_docs/lines.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       92 2024-03-18 13:35:21.000000 redmost-0.4.4/docs/module_docs/loaders.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       98 2024-03-19 12:02:51.000000 redmost-0.4.4/docs/module_docs/qt_compat.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 12:59:15.000000 redmost-0.4.4/docs/module_docs/utils.rst
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.866671 redmost-0.4.4/docs/pics/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     6393 2022-12-01 11:40:24.000000 redmost-0.4.4/docs/pics/github-mark.png
--rw-r--r--   0 daddona   (1000) daddona   (1000)    75781 2024-03-18 10:56:41.000000 redmost-0.4.4/docs/pics/redmost.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      105 2024-03-18 13:56:27.000000 redmost-0.4.4/docs/requirements.txt
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.866671 redmost-0.4.4/docs/tutorials/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      116 2024-03-18 13:51:24.000000 redmost-0.4.4/docs/tutorials/tut_01.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       63 2024-03-18 12:54:00.000000 redmost-0.4.4/docs/tutorials.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1644 2024-03-20 10:48:33.000000 redmost-0.4.4/pyproject.toml
--rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2024-03-21 11:13:14.873338 redmost-0.4.4/setup.cfg
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.863338 redmost-0.4.4/src/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.866671 redmost-0.4.4/src/redmost/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2873 2024-03-20 13:21:47.000000 redmost-0.4.4/src/redmost/__init__.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      411 2024-03-21 11:13:14.000000 redmost-0.4.4/src/redmost/_version.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.870005 redmost-0.4.4/src/redmost/backends/
--rw-r--r--   0 daddona   (1000) daddona   (1000)       72 2024-03-14 12:08:37.000000 redmost-0.4.4/src/redmost/backends/__init__.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     7860 2024-03-18 13:50:35.000000 redmost-0.4.4/src/redmost/backends/rrock.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)   118345 2024-03-21 11:10:28.000000 redmost-0.4.4/src/redmost/gui.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    10928 2024-03-21 09:37:05.000000 redmost-0.4.4/src/redmost/lines.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     6496 2024-03-18 13:47:36.000000 redmost-0.4.4/src/redmost/loaders.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)        2 2024-03-14 08:09:46.000000 redmost-0.4.4/src/redmost/py.typed
--rw-r--r--   0 daddona   (1000) daddona   (1000)     9322 2024-03-20 13:39:09.000000 redmost-0.4.4/src/redmost/qt_compat.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.870005 redmost-0.4.4/src/redmost/ui/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     5479 2024-03-21 11:12:13.000000 redmost-0.4.4/src/redmost/ui/control_mapping_dialog.ui
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.863338 redmost-0.4.4/src/redmost/ui/icons/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.870005 redmost-0.4.4/src/redmost/ui/icons/feather/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      343 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/book.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      358 2024-03-20 10:22:19.000000 redmost-0.4.4/src/redmost/ui/icons/feather/camera.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/check-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.4/src/redmost/ui/icons/feather/chevrons-left.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.4/src/redmost/ui/icons/feather/chevrons-right.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/delete.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/file-minus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/file-plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/file.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/folder.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/info.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      369 2024-03-20 10:22:19.000000 redmost-0.4.4/src/redmost/ui/icons/feather/log-out.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      333 2024-03-20 10:22:19.000000 redmost-0.4.4/src/redmost/ui/icons/feather/maximize.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/minus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      265 2024-03-20 10:22:19.000000 redmost-0.4.4/src/redmost/ui/icons/feather/play.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/plus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/save.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      484 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/save_as.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/settings.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/share.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/sliders.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/table.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/x-octagon.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/zoom-in.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 10:20:06.000000 redmost-0.4.4/src/redmost/ui/icons/feather/zoom-out.svg
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.873338 redmost-0.4.4/src/redmost/ui/icons/feather-dark/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/book.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      353 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/camera.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/check-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/chevrons-left.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/chevrons-right.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/delete.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/file-minus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/file-plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/file.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/folder.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/info.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      364 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/log-out.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      328 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/maximize.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/minus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      260 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/play.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/plus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/save.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1712 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/save_as.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/settings.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/share.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/sliders.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/table.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/x-octagon.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/zoom-in.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/zoom-out.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1304 2024-03-20 20:08:34.000000 redmost-0.4.4/src/redmost/ui/icons/feather-dark/zoom.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)    44979 2024-03-21 09:40:40.000000 redmost-0.4.4/src/redmost/ui/main_window.ui
--rw-r--r--   0 daddona   (1000) daddona   (1000)    37667 2024-03-18 10:57:10.000000 redmost-0.4.4/src/redmost/ui/redmost.png
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3777 2024-03-20 20:53:24.000000 redmost-0.4.4/src/redmost/ui/settings_dialog.ui
--rw-r--r--   0 daddona   (1000) daddona   (1000)     4859 2024-03-20 09:06:53.000000 redmost-0.4.4/src/redmost/utils.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.873338 redmost-0.4.4/src/redmost.egg-info/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     6878 2024-03-21 11:13:14.000000 redmost-0.4.4/src/redmost.egg-info/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3939 2024-03-21 11:13:14.000000 redmost-0.4.4/src/redmost.egg-info/SOURCES.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2024-03-21 11:13:14.000000 redmost-0.4.4/src/redmost.egg-info/dependency_links.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)       45 2024-03-21 11:13:14.000000 redmost-0.4.4/src/redmost.egg-info/entry_points.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)      155 2024-03-21 11:13:14.000000 redmost-0.4.4/src/redmost.egg-info/requires.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        8 2024-03-21 11:13:14.000000 redmost-0.4.4/src/redmost.egg-info/top_level.txt
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.873338 redmost-0.4.4/test/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      386 2024-03-18 14:30:36.000000 redmost-0.4.4/test/__init__.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-03-21 11:13:14.873338 redmost-0.4.4/test/data/
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:15.000000 redmost-0.4.4/test/data/spec_95.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_955.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_963.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_965.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_966.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_971.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_988.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_991.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_994.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.4/test/data/spec_997.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1845 2024-03-19 14:41:10.000000 redmost-0.4.4/test/data/test_project_1.json
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3549 2024-03-18 14:22:13.000000 redmost-0.4.4/test/data/test_project_2.json
--rw-r--r--   0 daddona   (1000) daddona   (1000)     8640 2024-03-18 14:28:57.000000 redmost-0.4.4/test/data/test_zcat.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3737 2024-03-20 21:34:44.000000 redmost-0.4.4/test/test_pyqt_basic.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.520000 redmost-0.4.5/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.513333 redmost-0.4.5/.github/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/.github/workflows/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1124 2024-03-20 13:43:32.000000 redmost-0.4.5/.github/workflows/pre-release.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1051 2024-03-20 13:43:36.000000 redmost-0.4.5/.github/workflows/tagged-release.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1228 2024-03-20 13:43:41.000000 redmost-0.4.5/.github/workflows/test_linux_lint.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1462 2024-03-19 19:35:03.000000 redmost-0.4.5/.github/workflows/test_linux_pyqt5.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2024-03-19 09:56:49.000000 redmost-0.4.5/.github/workflows/test_linux_pyqt6.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1468 2024-03-19 09:57:41.000000 redmost-0.4.5/.github/workflows/test_linux_pyside6.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2024-03-18 13:57:53.000000 redmost-0.4.5/.readthedocs.yaml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1535 2024-03-11 07:22:12.000000 redmost-0.4.5/LICENSE
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     6878 2024-04-10 06:15:15.520000 redmost-0.4.5/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3890 2024-03-20 10:51:05.000000 redmost-0.4.5/README.md
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/docs/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.513333 redmost-0.4.5/docs/_static/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/docs/_static/css/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       60 2023-09-21 08:50:12.000000 redmost-0.4.5/docs/_static/css/custom.css
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2905 2024-03-18 14:10:16.000000 redmost-0.4.5/docs/conf.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      192 2024-03-19 12:03:17.000000 redmost-0.4.5/docs/docs.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2860 2024-03-20 10:51:01.000000 redmost-0.4.5/docs/index.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2663 2024-04-03 07:55:12.000000 redmost-0.4.5/docs/installation.rst
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/docs/module_docs/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      113 2024-03-18 13:06:03.000000 redmost-0.4.5/docs/module_docs/backends_rrock.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       80 2024-03-18 12:38:22.000000 redmost-0.4.5/docs/module_docs/gui.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 13:46:27.000000 redmost-0.4.5/docs/module_docs/lines.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       92 2024-03-18 13:35:21.000000 redmost-0.4.5/docs/module_docs/loaders.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       98 2024-03-19 12:02:51.000000 redmost-0.4.5/docs/module_docs/qt_compat.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 12:59:15.000000 redmost-0.4.5/docs/module_docs/utils.rst
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/docs/pics/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     6393 2022-12-01 11:40:24.000000 redmost-0.4.5/docs/pics/github-mark.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    75781 2024-03-18 10:56:41.000000 redmost-0.4.5/docs/pics/redmost.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      105 2024-03-18 13:56:27.000000 redmost-0.4.5/docs/requirements.txt
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/docs/tutorials/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      116 2024-03-18 13:51:24.000000 redmost-0.4.5/docs/tutorials/tut_01.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       63 2024-03-18 12:54:00.000000 redmost-0.4.5/docs/tutorials.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1644 2024-03-20 10:48:33.000000 redmost-0.4.5/pyproject.toml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2024-04-10 06:15:15.520000 redmost-0.4.5/setup.cfg
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.513333 redmost-0.4.5/src/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/src/redmost/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2873 2024-03-20 13:21:47.000000 redmost-0.4.5/src/redmost/__init__.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      411 2024-04-10 06:15:15.000000 redmost-0.4.5/src/redmost/_version.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/src/redmost/backends/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       72 2024-03-14 12:08:37.000000 redmost-0.4.5/src/redmost/backends/__init__.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     7860 2024-03-18 13:50:35.000000 redmost-0.4.5/src/redmost/backends/rrock.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)   118352 2024-04-10 06:13:02.000000 redmost-0.4.5/src/redmost/gui.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    10928 2024-03-21 09:37:05.000000 redmost-0.4.5/src/redmost/lines.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     6496 2024-03-18 13:47:36.000000 redmost-0.4.5/src/redmost/loaders.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        2 2024-03-14 08:09:46.000000 redmost-0.4.5/src/redmost/py.typed
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     9322 2024-03-20 13:39:09.000000 redmost-0.4.5/src/redmost/qt_compat.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.516667 redmost-0.4.5/src/redmost/ui/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     5479 2024-03-21 11:12:13.000000 redmost-0.4.5/src/redmost/ui/control_mapping_dialog.ui
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.513333 redmost-0.4.5/src/redmost/ui/icons/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.520000 redmost-0.4.5/src/redmost/ui/icons/feather/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      343 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/book.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      358 2024-03-20 10:22:19.000000 redmost-0.4.5/src/redmost/ui/icons/feather/camera.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/check-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.5/src/redmost/ui/icons/feather/chevrons-left.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.5/src/redmost/ui/icons/feather/chevrons-right.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/delete.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/file-minus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/file-plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/file.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/folder.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/info.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      369 2024-03-20 10:22:19.000000 redmost-0.4.5/src/redmost/ui/icons/feather/log-out.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      333 2024-03-20 10:22:19.000000 redmost-0.4.5/src/redmost/ui/icons/feather/maximize.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/minus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      265 2024-03-20 10:22:19.000000 redmost-0.4.5/src/redmost/ui/icons/feather/play.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/plus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/save.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      484 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/save_as.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/settings.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/share.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/sliders.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/table.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/x-octagon.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/zoom-in.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 10:20:06.000000 redmost-0.4.5/src/redmost/ui/icons/feather/zoom-out.svg
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.520000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/book.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      353 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/camera.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/check-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/chevrons-left.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/chevrons-right.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/delete.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/file-minus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/file-plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/file.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/folder.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/info.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      364 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/log-out.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      328 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/maximize.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/minus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      260 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/play.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/plus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/save.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1712 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/save_as.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/settings.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/share.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/sliders.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/table.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/x-octagon.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/zoom-in.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/zoom-out.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1304 2024-03-20 20:08:34.000000 redmost-0.4.5/src/redmost/ui/icons/feather-dark/zoom.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    44979 2024-03-21 09:40:40.000000 redmost-0.4.5/src/redmost/ui/main_window.ui
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    37667 2024-03-18 10:57:10.000000 redmost-0.4.5/src/redmost/ui/redmost.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3777 2024-03-20 20:53:24.000000 redmost-0.4.5/src/redmost/ui/settings_dialog.ui
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4859 2024-03-20 09:06:53.000000 redmost-0.4.5/src/redmost/utils.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.520000 redmost-0.4.5/src/redmost.egg-info/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     6878 2024-04-10 06:15:15.000000 redmost-0.4.5/src/redmost.egg-info/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3939 2024-04-10 06:15:15.000000 redmost-0.4.5/src/redmost.egg-info/SOURCES.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2024-04-10 06:15:15.000000 redmost-0.4.5/src/redmost.egg-info/dependency_links.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       45 2024-04-10 06:15:15.000000 redmost-0.4.5/src/redmost.egg-info/entry_points.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      155 2024-04-10 06:15:15.000000 redmost-0.4.5/src/redmost.egg-info/requires.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        8 2024-04-10 06:15:15.000000 redmost-0.4.5/src/redmost.egg-info/top_level.txt
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.520000 redmost-0.4.5/test/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      386 2024-03-18 14:30:36.000000 redmost-0.4.5/test/__init__.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 06:15:15.520000 redmost-0.4.5/test/data/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:15.000000 redmost-0.4.5/test/data/spec_95.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_955.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_963.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_965.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_966.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_971.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_988.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_991.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_994.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.5/test/data/spec_997.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1845 2024-03-19 14:41:10.000000 redmost-0.4.5/test/data/test_project_1.json
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3549 2024-03-18 14:22:13.000000 redmost-0.4.5/test/data/test_project_2.json
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     8640 2024-03-18 14:28:57.000000 redmost-0.4.5/test/data/test_zcat.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3737 2024-03-20 21:34:44.000000 redmost-0.4.5/test/test_pyqt_basic.py
```

### Comparing `redmost-0.4.4/.github/workflows/pre-release.yml` & `redmost-0.4.5/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/.github/workflows/tagged-release.yml` & `redmost-0.4.5/.github/workflows/tagged-release.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/.github/workflows/test_linux_lint.yml` & `redmost-0.4.5/.github/workflows/test_linux_lint.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/.github/workflows/test_linux_pyqt5.yml` & `redmost-0.4.5/.github/workflows/test_linux_pyqt5.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/.github/workflows/test_linux_pyqt6.yml` & `redmost-0.4.5/.github/workflows/test_linux_pyqt6.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/.github/workflows/test_linux_pyside6.yml` & `redmost-0.4.5/.github/workflows/test_linux_pyside6.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/.readthedocs.yaml` & `redmost-0.4.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/LICENSE` & `redmost-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/PKG-INFO` & `redmost-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmost
-Version: 0.4.4
+Version: 0.4.5
 Summary: Display spectra and estimate their redshifts.
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
```

### Comparing `redmost-0.4.4/README.md` & `redmost-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/docs/conf.py` & `redmost-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/docs/index.rst` & `redmost-0.4.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/docs/installation.rst` & `redmost-0.4.5/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,38 @@
 
     source astro/bin/activate
 
 Redmost supports supports both PyQt6 and PySide6 backends, with precedence to PyQt6 if both are installed. PyQt5 backend is also supported for compatibility but it is not fully tested and may not work as expected. You can tell pip to install the appropriate dependencies using the commands:
 
 .. code-block:: bash
 
-    pip install .[pyqt6]
+    pip install redmost[pyqt6]
 
 for PyQt6 backend or
 
 .. code-block:: bash
 
-    pip install .[pyside6]
+    pip install redmost[pyside6]
 
 for PySide6 backend, or
 
 .. code-block:: bash
 
-    pip install .[pyqt5]
+    pip install redmost[pyqt5]
+    
+After the installation, to update redmost to the most recent release, use
+
+.. code-block:: bash
+
+    pip install redmost --upgrade
 
 Installing from GitHub
 ======================
 
-If you like to use the bleeding-edge version, you can install Specex directly from the |github_mark| `GitHub repository <https://github.com/mauritiusdadd/redmost>`_
+If you like to use the bleeding-edge version, you can install Redmost directly from the |github_mark| `GitHub repository <https://github.com/mauritiusdadd/redmost>`_
 
 .. code-block:: bash
 
     git clone 'https://github.com/mauritiusdadd/redmost.git'
     cd redmost
 
 and then run pip specifyng which Qt backend you want to use either
@@ -65,22 +71,20 @@
 
 or
 
 .. code-block:: bash
 
     pip install .[pyqt5]
 
-Updating
-========
 
-After the installation, to update redmost to the most recent release, use
+After the installation, to update redmost use
 
 .. code-block:: bash
-
-    pip install redmost --upgrade
+    git pull
+    pip install . --upgrade
 
 Install third party backends
 ============================
 
 Redmost uses modular backends to measure the redshift, although only redrock is currently supported. Please check and follow the installation instructions of the single packages!
 
 - redrock backend: `<https://github.com/desihub/redrock>`_
```

### Comparing `redmost-0.4.4/docs/pics/github-mark.png` & `redmost-0.4.5/docs/pics/github-mark.png`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/docs/pics/redmost.svg` & `redmost-0.4.5/docs/pics/redmost.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/pyproject.toml` & `redmost-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/__init__.py` & `redmost-0.4.5/src/redmost/__init__.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/backends/rrock.py` & `redmost-0.4.5/src/redmost/backends/rrock.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/gui.py` & `redmost-0.4.5/src/redmost/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -3082,15 +3082,15 @@
 
             lines_list = []
             for line_info in obj_info['lines']['list']:
                 lines_list.append({
                     'row': int(line_info['row']),
                     'data': float(line_info['data']),
                     'text': str(line_info['text']),
-                    'checked': QtCore.Qt.CheckState(
+                    'checked': qt_api.QtCore.Qt.CheckState(
                         line_info['checked']
                     )
                 })
 
             z_list = []
             for z_info in obj_info['lines']['redshifts']:
                 z_list.append({
```

### Comparing `redmost-0.4.4/src/redmost/lines.py` & `redmost-0.4.5/src/redmost/lines.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/loaders.py` & `redmost-0.4.5/src/redmost/loaders.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/qt_compat.py` & `redmost-0.4.5/src/redmost/qt_compat.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/control_mapping_dialog.ui` & `redmost-0.4.5/src/redmost/ui/control_mapping_dialog.ui`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/icons/feather/settings.svg` & `redmost-0.4.5/src/redmost/ui/icons/feather/settings.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/icons/feather/sliders.svg` & `redmost-0.4.5/src/redmost/ui/icons/feather/sliders.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/icons/feather-dark/save_as.svg` & `redmost-0.4.5/src/redmost/ui/icons/feather-dark/save_as.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/icons/feather-dark/settings.svg` & `redmost-0.4.5/src/redmost/ui/icons/feather-dark/settings.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/icons/feather-dark/sliders.svg` & `redmost-0.4.5/src/redmost/ui/icons/feather-dark/sliders.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/icons/feather-dark/zoom.svg` & `redmost-0.4.5/src/redmost/ui/icons/feather-dark/zoom.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/main_window.ui` & `redmost-0.4.5/src/redmost/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/redmost.png` & `redmost-0.4.5/src/redmost/ui/redmost.png`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/ui/settings_dialog.ui` & `redmost-0.4.5/src/redmost/ui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost/utils.py` & `redmost-0.4.5/src/redmost/utils.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/src/redmost.egg-info/PKG-INFO` & `redmost-0.4.5/src/redmost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmost
-Version: 0.4.4
+Version: 0.4.5
 Summary: Display spectra and estimate their redshifts.
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
```

### Comparing `redmost-0.4.4/src/redmost.egg-info/SOURCES.txt` & `redmost-0.4.5/src/redmost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_95.fits` & `redmost-0.4.5/test/data/spec_95.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_955.fits` & `redmost-0.4.5/test/data/spec_955.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_963.fits` & `redmost-0.4.5/test/data/spec_963.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_965.fits` & `redmost-0.4.5/test/data/spec_965.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_966.fits` & `redmost-0.4.5/test/data/spec_966.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_971.fits` & `redmost-0.4.5/test/data/spec_971.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_988.fits` & `redmost-0.4.5/test/data/spec_988.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_991.fits` & `redmost-0.4.5/test/data/spec_991.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_994.fits` & `redmost-0.4.5/test/data/spec_994.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/spec_997.fits` & `redmost-0.4.5/test/data/spec_997.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/test_project_1.json` & `redmost-0.4.5/test/data/test_project_1.json`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/test_project_2.json` & `redmost-0.4.5/test/data/test_project_2.json`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/data/test_zcat.fits` & `redmost-0.4.5/test/data/test_zcat.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.4/test/test_pyqt_basic.py` & `redmost-0.4.5/test/test_pyqt_basic.py`

 * *Files identical despite different names*

