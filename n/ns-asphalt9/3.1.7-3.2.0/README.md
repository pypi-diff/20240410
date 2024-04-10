# Comparing `tmp/ns_asphalt9-3.1.7.tar.gz` & `tmp/ns_asphalt9-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-3.1.7.tar", last modified: Wed Apr  3 02:33:19 2024, max compression
+gzip compressed data, was "ns_asphalt9-3.2.0.tar", last modified: Tue Apr  9 07:10:41 2024, max compression
```

## Comparing `ns_asphalt9-3.1.7.tar` & `ns_asphalt9-3.2.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.434921 ns_asphalt9-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-03 02:33:19.434921 ns_asphalt9-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.422921 ns_asphalt9-3.1.7/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.426921 ns_asphalt9-3.1.7/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.426921 ns_asphalt9-3.1.7/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/actions/autocode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.426921 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37553 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.430921 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/console.png
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward.png
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward2.png
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward3.png
--rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/screen.png
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20268 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/reset_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.434921 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/error_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/lifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/online_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/page_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data_win.py
--rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.434921 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-03 02:33:19.000000 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-03 02:33:19.000000 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:33:19.000000 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 02:33:19.000000 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:33:19.000000 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 02:33:19.000000 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:33:19.000000 ns_asphalt9-3.1.7/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-03 02:33:19.434921 ns_asphalt9-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:33:19.434921 ns_asphalt9-3.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-03 02:33:15.000000 ns_asphalt9-3.1.7/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.237784 ns_asphalt9-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 07:10:29.000000 ns_asphalt9-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 07:10:29.000000 ns_asphalt9-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 07:10:41.237784 ns_asphalt9-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-09 07:10:29.000000 ns_asphalt9-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.225784 ns_asphalt9-3.2.0/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.229784 ns_asphalt9-3.2.0/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.229784 ns_asphalt9-3.2.0/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/actions/autocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.229784 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37693 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.233785 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/screen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20268 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/reset_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.237784 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/error_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/lifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/online_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/page_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data_win.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12686 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.237784 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 07:10:41.000000 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-09 07:10:41.000000 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:10:41.000000 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 07:10:41.000000 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:10:41.000000 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 07:10:41.000000 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 07:10:41.000000 ns_asphalt9-3.2.0/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-09 07:10:41.237784 ns_asphalt9-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:10:41.237784 ns_asphalt9-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-09 07:10:30.000000 ns_asphalt9-3.2.0/tests/test_pages.py
```

### Comparing `ns_asphalt9-3.1.7/LICENSE` & `ns_asphalt9-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/PKG-INFO` & `ns_asphalt9-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.1.7
+Version: 3.2.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.1.7/README.md` & `ns_asphalt9-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/actions/__init__.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/actions/autocode.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/actions/autocode.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/cache.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/capture.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/capture.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/consts.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/controller.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,29 +44,38 @@
         reconnect_addresses = self.nx.get_switch_addresses()
         self.controller_index = self.nx.create_controller(
             nxbt.PRO_CONTROLLER, reconnect_address=reconnect_addresses
         )
         self.nx.wait_for_connection(self.controller_index)
         time.sleep(1)
         logger.info("Connected switch.")
-        self.press_buttons(Buttons.A)
 
     def disconnect(self):
         self.nx.remove_controller(self.controller_index)
         logger.info("Disconnected switch.")
 
     def press_buttons(self, button, down=0.13, up=0.1, block=True):
         buttons = []
         logger.info(f"Press button {button}")
         if isinstance(button, str):
             buttons.append(button)
         else:
             buttons = button
         globals.output_queue.put({"按键响应": ",".join(buttons)})
-        self.nx.press_buttons(self.controller_index, buttons, down, up, block)
+        # self.nx.press_buttons(self.controller_index, buttons, down, up, block)
+        for b in buttons:
+            for _ in range(5):
+                packet = globals.input_packet["packet"]
+                packet[b] = True
+                globals.input_packet["packet"] = packet
+                time.sleep(down / 5)
+            for _ in range(5):
+                packet[b] = False
+                globals.input_packet["packet"] = packet
+                time.sleep(up / 5)
 
     def press_group(self, buttons, sleep=1):
         for b in buttons:
             self.press_buttons(b)
             if sleep:
                 time.sleep(sleep)
```

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/event.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/event.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/globals.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/globals.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import multiprocessing
 import queue
 import threading
 
 from . import consts
 from .utils.lifo_queue import LIFOQueue
 
+packet_manager = multiprocessing.Manager()
+input_packet = packet_manager.dict()
 
 input_queue = multiprocessing.Queue()
 output_queue = multiprocessing.Queue()
 notify_queue = multiprocessing.Queue()
 
 frame_queue = LIFOQueue()
```

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,23 +428,25 @@
         def on_key_press(event):
             self.show(f"On key press, key = {event.char}, {event.keysym}")
             key = keysym_mapping.get(event.keysym, event.keysym)
             if key in key_pro_mapping:
                 button: Button = pro_buttons.get(key_pro_mapping[key], None)
                 if button:
                     button._on_enter()
+                    self.queue.put({"action": "press", "key": key})
 
         def on_key_release(event):
             self.show(f"On key release, key = {event.char} {event.keysym}")
             key = keysym_mapping.get(event.keysym, event.keysym)
             if key in key_pro_mapping:
                 button: Button = pro_buttons.get(key_pro_mapping[key], None)
                 if button:
                     button._on_leave()
-                    self.queue.put(key)
+                    self.queue.put({"action": "release", "key": key})
+                    # self.queue.put(key)
 
         self.key_label.bind("<KeyRelease>", on_key_release)
         self.key_label.bind("<KeyPress>", on_key_press)
 
     def update_race_data(self, data):
         for d in data:
             if d in self.race_data_containers:
```

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/console.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/console.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward1.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward1.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward2.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward2.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward3.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward3.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/reward_qrcode.jpeg` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/screen.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/screen.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-3.2.0/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/ocr.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/pages.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/reset_data.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/reset_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/tasks.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/test.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/test.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/count.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/count.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/credits.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/credits.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/error_process.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/error_process.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/lifo_queue.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/lifo_queue.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/notify.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/notify.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/online_tracker.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/online_tracker.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/page_stack.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/page_stack.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_data.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data_update.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data_update.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data_v2.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data_v2.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/core/utils/track_navi_data_win.py` & `ns_asphalt9-3.2.0/ns_asphalt9/core/utils/track_navi_data_win.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9/main.py` & `ns_asphalt9-3.2.0/ns_asphalt9/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 from .core.utils.notify import Notify
 from .core.actions import *  # noqa
 from .core.utils.page_stack import page_stack
 from .core.event import Event
 from .core.reset_data import reset_data
 
 
+G.input_packet["packet"] = pro.nx.create_input_packet()
+
+
 def process_screen(page: Page):
     """根据显示内容执行动作"""
 
     page_stack.add_item(page.name)
     if page.name != consts.empty and page.action:
         page.call_action()
 
@@ -185,16 +188,30 @@
                         logger.info(f"{command} process end!")
                     except Exception as err:
                         logger.info(f"{command} process err = {err}")
                 else:
                     logger.info(f"{command} command not support!")
 
         elif isinstance(command, dict):
-            logger.info("Received config update message.")
-            G.CONFIG = command
+            try:
+                if "action" in command:
+                    control_data = consts.KEY_MAPPING.get(command["key"])
+                    packet = G.input_packet["packet"]
+                    if command["action"] == "press":
+                        packet[control_data] = True
+                    else:
+                        packet[control_data] = False
+                    G.input_packet["packet"] = packet
+                else:
+                    logger.info("Received config update message.")
+                    G.CONFIG = command
+            except Exception as err:
+                logger.info(
+                    f"{command} process err = {err} traceback = {traceback.format_exc()}"
+                )
 
         else:
             logger.info(f"{command} command not support!")
 
 
 def start_command_input(queue):
     t = threading.Thread(target=command_input, args=(queue,), daemon=True)
@@ -320,20 +337,64 @@
 
 
 def start_stream_worker():
     t = threading.Thread(target=stream_worker, args=(), daemon=True)
     t.start()
 
 
+def input_worker(nxbt, controller_index):
+    while True:
+        packet = G.input_packet["packet"]
+
+        # Calculating left x/y stick values
+        ls_x_value = 0
+        ls_y_value = 0
+        if packet["L_STICK"]["LS_LEFT"]:
+            ls_x_value -= 100
+        if packet["L_STICK"]["LS_RIGHT"]:
+            ls_x_value += 100
+        if packet["L_STICK"]["LS_UP"]:
+            ls_y_value += 100
+        if packet["L_STICK"]["LS_DOWN"]:
+            ls_y_value -= 100
+        packet["L_STICK"]["X_VALUE"] = ls_x_value
+        packet["L_STICK"]["Y_VALUE"] = ls_y_value
+
+        # Calculating right x/y stick values
+        rs_x_value = 0
+        rs_y_value = 0
+        if packet["R_STICK"]["RS_LEFT"]:
+            rs_x_value -= 100
+        if packet["R_STICK"]["RS_RIGHT"]:
+            rs_x_value += 100
+        if packet["R_STICK"]["RS_UP"]:
+            rs_y_value += 100
+        if packet["R_STICK"]["RS_DOWN"]:
+            rs_y_value -= 100
+        packet["R_STICK"]["X_VALUE"] = rs_x_value
+        packet["R_STICK"]["Y_VALUE"] = rs_y_value
+
+        nxbt.set_controller_input(controller_index, packet)
+        time.sleep(1 / 150)
+
+
+def start_input_worker():
+    input_process = multiprocessing.Process(
+        target=input_worker, args=(pro.nx, pro.controller_index)
+    )
+    input_process.start()
+
+
 def main():
     G.G_OUT_WORKER.set()
     config_name = init_config()
     start_worker()
     app = App(G.input_queue, config_name, G.video_queue)
     start_output_worker(app)
+    start_input_worker()
     start_notify_worker()
     start_stream_worker()
     G.notify_queue.put({"event": "open", "content": {}})
     app.protocol("WM_DELETE_WINDOW", lambda: on_closing(app))
     app.mainloop()
     print("App quit quit.")
```

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-3.2.0/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.1.7
+Version: 3.2.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.1.7/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-3.2.0/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.1.7/setup.cfg` & `ns_asphalt9-3.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 3.1.7
+version = 3.2.0
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-3.1.7/tests/test_pages.py` & `ns_asphalt9-3.2.0/tests/test_pages.py`

 * *Files identical despite different names*

