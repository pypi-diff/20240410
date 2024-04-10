# Comparing `tmp/genshin-1.6.2.tar.gz` & `tmp/genshin-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genshin-1.6.2.tar", last modified: Sat Jan 13 19:40:27 2024, max compression
+gzip compressed data, was "genshin-1.6.3.tar", last modified: Wed Apr 10 17:59:08 2024, max compression
```

## Comparing `genshin-1.6.2.tar` & `genshin-1.6.3.tar`

### file list

```diff
@@ -1,123 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.116468 genshin-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-13 19:40:19.000000 genshin-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-01-13 19:40:27.116468 genshin-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-01-13 19:40:19.000000 genshin-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.096468 genshin-1.6.2/genshin/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.100468 genshin-1.6.2/genshin/client/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.100468 genshin-1.6.2/genshin/client/components/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18521 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.100468 genshin-1.6.2/genshin/client/components/calculator/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/calculator/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12339 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/calculator/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.104468 genshin-1.6.2/genshin/client/components/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/chronicle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/chronicle/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/chronicle/genshin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/chronicle/honkai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/chronicle/starrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/gacha.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.104468 genshin-1.6.2/genshin/client/components/geetest/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/geetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/geetest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/geetest/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/hoyolab.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/lineup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/teapot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/components/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.104468 genshin-1.6.2/genshin/client/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/manager/cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/manager/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/client/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.104468 genshin-1.6.2/genshin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.104468 genshin-1.6.2/genshin/models/genshin/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.108468 genshin-1.6.2/genshin/models/genshin/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/chronicle/abyss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/chronicle/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/chronicle/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/chronicle/notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/chronicle/tcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/lineup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/teapot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/genshin/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.108468 genshin-1.6.2/genshin/models/honkai/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/honkai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/honkai/battlesuit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.108468 genshin-1.6.2/genshin/models/honkai/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/honkai/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/honkai/chronicle/battlesuits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/honkai/chronicle/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/honkai/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/honkai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.108468 genshin-1.6.2/genshin/models/hoyolab/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/hoyolab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/hoyolab/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/hoyolab/private.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/hoyolab/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.108468 genshin-1.6.2/genshin/models/starrail/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.112468 genshin-1.6.2/genshin/models/starrail/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/chronicle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/chronicle/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/chronicle/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/chronicle/notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/chronicle/rogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/models/starrail/chronicle/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.112468 genshin-1.6.2/genshin/paginators/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/paginators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/paginators/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/paginators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.112468 genshin-1.6.2/genshin/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/ds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/extdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/geetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/logfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-01-13 19:40:19.000000 genshin-1.6.2/genshin/utility/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.112468 genshin-1.6.2/genshin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-01-13 19:40:27.000000 genshin-1.6.2/genshin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-01-13 19:40:27.000000 genshin-1.6.2/genshin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 19:40:27.000000 genshin-1.6.2/genshin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-13 19:40:27.000000 genshin-1.6.2/genshin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-13 19:40:27.000000 genshin-1.6.2/genshin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-13 19:40:19.000000 genshin-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 19:40:27.116468 genshin-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-01-13 19:40:19.000000 genshin-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:27.112468 genshin-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 19:40:19.000000 genshin-1.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-01-13 19:40:19.000000 genshin-1.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-01-13 19:40:19.000000 genshin-1.6.2/tests/test_paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.444755 genshin-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 17:59:04.000000 genshin-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 17:59:08.444755 genshin-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-10 17:59:04.000000 genshin-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.424755 genshin-1.6.3/genshin/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.428755 genshin-1.6.3/genshin/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.428755 genshin-1.6.3/genshin/client/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18522 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.428755 genshin-1.6.3/genshin/client/components/calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/calculator/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/calculator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/client/components/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/genshin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/honkai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/chronicle/starrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/gacha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/client/components/geetest/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/geetest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/geetest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/geetest/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/hoyolab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/components/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/client/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/manager/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/manager/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/client/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.432755 genshin-1.6.3/genshin/models/genshin/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/genshin/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/abyss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/chronicle/tcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/genshin/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/honkai/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/battlesuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/honkai/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/battlesuits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/honkai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/hoyolab/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/hoyolab/record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/miyoushe/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/miyoushe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/miyoushe/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/miyoushe/qrcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.436755 genshin-1.6.3/genshin/models/starrail/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin/models/starrail/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/rogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/models/starrail/chronicle/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin/paginators/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/paginators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/paginators/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/paginators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/extdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/geetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/logfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-10 17:59:04.000000 genshin-1.6.3/genshin/utility/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/genshin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 17:59:08.000000 genshin-1.6.3/genshin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-10 17:59:04.000000 genshin-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:59:08.444755 genshin-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 17:59:04.000000 genshin-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:08.440755 genshin-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:59:04.000000 genshin-1.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-10 17:59:04.000000 genshin-1.6.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-10 17:59:04.000000 genshin-1.6.3/tests/test_paginators.py
```

### Comparing `genshin-1.6.2/LICENSE` & `genshin-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/PKG-INFO` & `genshin-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.6.2
+Version: 1.6.3
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
@@ -25,18 +25,20 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: pydantic
 Provides-Extra: all
 Requires-Dist: browser-cookie3; extra == "all"
 Requires-Dist: rsa; extra == "all"
 Requires-Dist: click; extra == "all"
+Requires-Dist: qrcode[pil]; extra == "all"
 Provides-Extra: cookies
 Requires-Dist: browser-cookie3; extra == "cookies"
 Provides-Extra: geetest
 Requires-Dist: rsa; extra == "geetest"
+Requires-Dist: qrcode[pil]; extra == "geetest"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 # genshin.py
 
 [![Downloads](https://pepy.tech/badge/genshin)](https://pepy.tech/project/genshin)
 [![PyPI package](https://img.shields.io/pypi/v/genshin)](https://pypi.org/project/genshin/)
```

### Comparing `genshin-1.6.2/README.md` & `genshin-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/genshin/client/cache.py` & `genshin-1.6.3/genshin/client/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Cache for client."""
+
 from __future__ import annotations
 
 import abc
 import dataclasses
 import enum
 import json
 import sys
```

### Comparing `genshin-1.6.2/genshin/client/clients.py` & `genshin-1.6.3/genshin/client/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A simple HTTP client for API endpoints."""
+
 from .components import (
     calculator,
     chronicle,
     daily,
     diary,
     gacha,
     geetest,
```

### Comparing `genshin-1.6.2/genshin/client/compatibility.py` & `genshin-1.6.3/genshin/client/compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Reverse-compatibility layer for previous versions."""
+
 from __future__ import annotations
 
 import typing
 
 import aiohttp
 
 from genshin import models, types
```

### Comparing `genshin-1.6.2/genshin/client/components/base.py` & `genshin-1.6.3/genshin/client/components/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base ABC Client."""
+
 import abc
 import asyncio
 import base64
 import json
 import logging
 import os
 import typing
```

### Comparing `genshin-1.6.2/genshin/client/components/calculator/calculator.py` & `genshin-1.6.3/genshin/client/components/calculator/calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Calculator builder object.
 
 Over-engineered for the sake of extendability and maintainability.
 """
+
 from __future__ import annotations
 
 import abc
 import asyncio
 import typing
 
 import genshin.models.genshin as genshin_models
```

### Comparing `genshin-1.6.2/genshin/client/components/calculator/client.py` & `genshin-1.6.3/genshin/client/components/calculator/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Calculator client."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import typing
 import warnings
```

### Comparing `genshin-1.6.2/genshin/client/components/chronicle/base.py` & `genshin-1.6.3/genshin/client/components/chronicle/base.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/genshin/client/components/chronicle/genshin.py` & `genshin-1.6.3/genshin/client/components/chronicle/genshin.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/genshin/client/components/chronicle/honkai.py` & `genshin-1.6.3/genshin/client/components/chronicle/honkai.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/genshin/client/components/chronicle/starrail.py` & `genshin-1.6.3/genshin/client/components/chronicle/starrail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """StarRail battle chronicle component."""
+
 import asyncio
 import typing
 
 from genshin import errors, types, utility
 from genshin.models.starrail import chronicle as models
 
 from . import base
@@ -122,7 +123,19 @@
         schedule_type: int = 3,
         lang: typing.Optional[str] = None,
     ) -> models.StarRailRogue:
         """Get starrail rogue runs."""
         payload = dict(schedule_type=schedule_type, need_detail="true")
         data = await self._request_starrail_record("rogue", uid, lang=lang, payload=payload)
         return models.StarRailRogue(**data)
+
+    async def get_starrail_pure_fiction(
+        self,
+        uid: typing.Optional[int] = None,
+        *,
+        previous: bool = False,
+        lang: typing.Optional[str] = None,
+    ) -> models.StarRailPureFiction:
+        """Get starrail pure fiction runs."""
+        payload = dict(schedule_type=2 if previous else 1, need_all="true")
+        data = await self._request_starrail_record("challenge_story", uid, lang=lang, payload=payload)
+        return models.StarRailPureFiction(**data)
```

### Comparing `genshin-1.6.2/genshin/client/components/daily.py` & `genshin-1.6.3/genshin/client/components/daily.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Daily reward component."""
+
 import asyncio
 import datetime
 import functools
 import typing
 import uuid
 
 import aiohttp.typedefs
@@ -146,27 +147,25 @@
     async def claim_daily_reward(  # noqa: D102 missing docstring in overload?
         self,
         *,
         game: typing.Optional[types.Game] = None,
         lang: typing.Optional[str] = None,
         reward: typing.Literal[True] = ...,
         challenge: typing.Optional[typing.Mapping[str, str]] = None,
-    ) -> models.DailyReward:
-        ...
+    ) -> models.DailyReward: ...
 
     @typing.overload
     async def claim_daily_reward(  # noqa: D102 missing docstring in overload?
         self,
         *,
         game: typing.Optional[types.Game] = None,
         lang: typing.Optional[str] = None,
         reward: typing.Literal[False],
         challenge: typing.Optional[typing.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     async def claim_daily_reward(
         self,
         *,
         game: typing.Optional[types.Game] = None,
         lang: typing.Optional[str] = None,
         reward: bool = True,
```

### Comparing `genshin-1.6.2/genshin/client/components/diary.py` & `genshin-1.6.3/genshin/client/components/diary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Diary component."""
+
 import datetime
 import functools
 import typing
 
 from genshin import paginators, types, utility
 from genshin.client import cache, routes
 from genshin.client.components import base
```

### Comparing `genshin-1.6.2/genshin/client/components/gacha.py` & `genshin-1.6.3/genshin/client/components/gacha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wish component."""
+
 import asyncio
 import functools
 import typing
 import urllib.parse
 import warnings
 
 from genshin import paginators, types, utility
@@ -217,15 +218,15 @@
         if game == types.Game.STARRAIL:
             warnings.warn("Banner details for Star Rail are not fully supported.")
 
         region = "hkrpg" if game == types.Game.STARRAIL else "hk4e"
         server = "prod_official_asia" if game == types.Game.STARRAIL else "os_asia"
 
         data = await self.request_webstatic(
-            f"/{region}/gacha_info/{server}/{banner_id}/{lang}.json",
+            f"/gacha_info/{region}/{server}/{banner_id}/{lang}.json",
             cache=client_cache.cache_key("banner", endpoint="details", banner=banner_id, lang=lang),
         )
         return models.BannerDetails(**data, banner_id=banner_id)
 
     @deprecation.deprecated("get_genshin_banner_ids")
     async def get_banner_ids(self) -> typing.Sequence[str]:
         """Get a list of banner ids.
@@ -235,20 +236,27 @@
         return await self.get_genshin_banner_ids()
 
     async def get_genshin_banner_ids(self) -> typing.Sequence[str]:
         """Get a list of banner ids.
 
         Uses the current cn banners.
         """
+
+        def process_gacha(data: typing.Mapping[str, typing.Any]) -> str:
+            # Temporary fix for 4.5 chronicled wish
+            if data["gacha_type"] == 500:
+                return "8b10b48c52dd6870f92d72e9963b44bb8968ed2f"
+            return data["gacha_id"]
+
         data = await self.request_webstatic(
-            "hk4e/gacha_info/cn_gf01/gacha/list.json",
+            "gacha_info/hk4e/cn_gf01/gacha/list.json",
             region=types.Region.CHINESE,
             cache=client_cache.cache_key("banner", endpoint="ids"),
         )
-        return [i["gacha_id"] for i in data["data"]["list"]]
+        return list(map(process_gacha, data["data"]["list"]))
 
     async def get_banner_details(
         self,
         banner_ids: typing.Optional[typing.Sequence[str]] = None,
         *,
         game: typing.Optional[types.Game] = None,
         lang: typing.Optional[str] = None,
```

### Comparing `genshin-1.6.2/genshin/client/components/geetest/server.py` & `genshin-1.6.3/genshin/client/components/geetest/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Aiohttp webserver used for captcha solving and email verification."""
+
 from __future__ import annotations
 
 import asyncio
 import typing
 import webbrowser
 
 import aiohttp
 from aiohttp import web
 
 from . import client
 
-__all__ = ["get_page", "launch_webapp", "solve_geetest", "verify_email"]
-
+__all__ = ["PAGES", "launch_webapp", "solve_geetest", "verify_email"]
 
-def get_page(page: typing.Literal["captcha", "verify-email"]) -> str:
-    """Get the HTML page."""
-    return (
-        """
+PAGES: typing.Final[typing.Dict[typing.Literal["captcha", "verify-email", "enter-otp"], str]] = {
+    "captcha": """
     <!DOCTYPE html>
     <html>
       <body></body>
       <script src="./gt.js"></script>
       <script>
         fetch("/mmt")
           .then((response) => response.json())
@@ -50,59 +48,82 @@
                 document.body.innerHTML = "You may now close this window.";
               });
             }
           )
         );
       </script>
     </html>
-    """
-        if page == "captcha"
-        else """
+    """,
+    "verify-email": """
     <!DOCTYPE html>
     <html>
       <body>
         <input id="code" type="number">
         <button id="verify">Send</button>
       </body>
       <script>
-        document.getElementById("verify").onClick = () => {
+        document.getElementById("verify").onclick = () => {
           fetch("/send-data", {
             method: "POST",
             body: JSON.stringify({
               code: document.getElementById("code").value
             }),
           });
           document.body.innerHTML = "You may now close this window.";
         };
       </script>
     </html>
-    """
-    )
+    """,
+    "enter-otp": """
+    <!DOCTYPE html>
+    <html>
+      <body>
+        <input id="code" type="number">
+        <button id="verify">Send</button>
+      </body>
+      <script>
+        document.getElementById("verify").onclick = () => {
+          fetch("/send-data", {
+            method: "POST",
+            body: JSON.stringify({
+              code: document.getElementById("code").value
+            }),
+          });
+          document.body.innerHTML = "You may now close this window.";
+        };
+      </script>
+    </html>
+    """,
+}
 
 
 GT_URL = "https://raw.githubusercontent.com/GeeTeam/gt3-node-sdk/master/demo/static/libs/gt.js"
 
 
 async def launch_webapp(
-    page: typing.Literal["captcha", "verify-email"],
+    page: typing.Literal["captcha", "verify-email", "enter-otp"],
     *,
     port: int = 5000,
     mmt: typing.Optional[typing.Dict[str, typing.Any]] = None,
 ) -> typing.Any:
     """Create and run a webapp to solve captcha or send verification code."""
     routes = web.RouteTableDef()
     future: asyncio.Future[typing.Any] = asyncio.Future()
 
     @routes.get("/captcha")
     async def captcha(request: web.Request) -> web.StreamResponse:
-        return web.Response(body=get_page("captcha"), content_type="text/html")
+        return web.Response(body=PAGES["captcha"], content_type="text/html")
 
     @routes.get("/verify-email")
     async def verify_email(request: web.Request) -> web.StreamResponse:
-        return web.Response(body=get_page("verify-email"), content_type="text/html")
+        return web.Response(body=PAGES["verify-email"], content_type="text/html")
+
+    @routes.get("/enter-otp")
+    async def enter_otp(request: web.Request) -> web.StreamResponse:
+        return web.Response(body=PAGES["enter-otp"], content_type="text/html")
 
     @routes.get("/gt.js")
     async def gt(request: web.Request) -> web.StreamResponse:
         async with aiohttp.ClientSession() as session:
             r = await session.get(GT_URL)
             content = await r.read()
 
@@ -132,14 +153,15 @@
     await site.start()
 
     try:
         data = await future
     finally:
         await asyncio.sleep(0.3)
         await runner.shutdown()
+        await runner.cleanup()
 
     return data
 
 
 async def solve_geetest(
     mmt: typing.Dict[str, typing.Any],
     *,
@@ -155,8 +177,16 @@
     *,
     port: int = 5000,
 ) -> None:
     """Verify email to login via HoYoLab app endpoint."""
     data = await launch_webapp("verify-email", port=port)
     code = data["code"]
 
-    return await client.verify_email(code, ticket)
+    return await client._verify_email(code, ticket)
+
+
+async def enter_otp(port: int = 5000) -> str:
+    """Lets user enter the OTP."""
+    # The enter-otp page is the same as verify-email page.
+    data = await launch_webapp("enter-otp", port=port)
+    code = data["code"]
+    return code
```

### Comparing `genshin-1.6.2/genshin/client/components/hoyolab.py` & `genshin-1.6.3/genshin/client/components/hoyolab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hoyolab component."""
+
 import asyncio
 import typing
 
 from genshin import types, utility
 from genshin.client import cache as client_cache
 from genshin.client import routes
 from genshin.client.components import base
```

### Comparing `genshin-1.6.2/genshin/client/components/lineup.py` & `genshin-1.6.3/genshin/client/components/lineup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Lineup component."""
+
 import functools
 import typing
 
 import genshin.models.genshin as genshin_models
 from genshin import paginators, types, utility
 from genshin.client import cache, routes
 from genshin.client.components import base
```

### Comparing `genshin-1.6.2/genshin/client/components/teapot.py` & `genshin-1.6.3/genshin/client/components/teapot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Teapot component."""
+
 import functools
 import typing
 
 from genshin import paginators, utility
 from genshin.client import routes
 from genshin.client.components import base
 from genshin.models.genshin import teapot as models
```

### Comparing `genshin-1.6.2/genshin/client/components/transaction.py` & `genshin-1.6.3/genshin/client/components/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Transaction client."""
+
 import functools
 import typing
 import urllib.parse
 
 from genshin import paginators, utility
 from genshin.client import routes
 from genshin.client.components import base
```

### Comparing `genshin-1.6.2/genshin/client/components/wiki.py` & `genshin-1.6.3/genshin/client/components/wiki.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wiki component."""
+
 import typing
 
 from genshin import types
 from genshin.client import cache, routes
 from genshin.client.components import base
 from genshin.models.genshin import wiki as models
 
@@ -30,52 +31,47 @@
 
     @typing.overload
     async def get_wiki_previews(  # noqa: D102 missing docstring in overload?
         self,
         menu: typing.Literal[models.WikiPageType.CHARACTER],
         *,
         lang: typing.Optional[str] = None,
-    ) -> typing.Sequence[models.CharacterPreview]:
-        ...
+    ) -> typing.Sequence[models.CharacterPreview]: ...
 
     @typing.overload
     async def get_wiki_previews(  # noqa: D102 missing docstring in overload?
         self,
         menu: typing.Literal[models.WikiPageType.WEAPON],
         *,
         lang: typing.Optional[str] = None,
-    ) -> typing.Sequence[models.WeaponPreview]:
-        ...
+    ) -> typing.Sequence[models.WeaponPreview]: ...
 
     @typing.overload
     async def get_wiki_previews(  # noqa: D102 missing docstring in overload?
         self,
         menu: typing.Literal[models.WikiPageType.ARTIFACT],
         *,
         lang: typing.Optional[str] = None,
-    ) -> typing.Sequence[models.ArtifactPreview]:
-        ...
+    ) -> typing.Sequence[models.ArtifactPreview]: ...
 
     @typing.overload
     async def get_wiki_previews(  # noqa: D102 missing docstring in overload?
         self,
         menu: typing.Literal[models.WikiPageType.ENEMY],
         *,
         lang: typing.Optional[str] = None,
-    ) -> typing.Sequence[models.EnemyPreview]:
-        ...
+    ) -> typing.Sequence[models.EnemyPreview]: ...
 
     @typing.overload
     async def get_wiki_previews(  # noqa: D102 missing docstring in overload?
         self,
         menu: int,
         *,
         lang: typing.Optional[str] = None,
-    ) -> typing.Sequence[models.BaseWikiPreview]:
-        ...
+    ) -> typing.Sequence[models.BaseWikiPreview]: ...
 
     async def get_wiki_previews(
         self,
         menu: int,
         *,
         lang: typing.Optional[str] = None,
     ) -> typing.Sequence[models.BaseWikiPreview]:
```

### Comparing `genshin-1.6.2/genshin/client/manager/cookie.py` & `genshin-1.6.3/genshin/client/manager/cookie.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,34 +11,55 @@
 - fetch_cookie_token_info
     - cookie_token -> cookie_token
     - login_ticket -> cookie_token
 - fetch_cookie_with_stoken_v2
     - stoken (v2) + mid -> ltoken_v2 (token_type=2)
     - stoken (v2) + mid -> cookie_token_v2 (token_type=4)
 """
+
 from __future__ import annotations
 
+import random
 import typing
+import uuid
+from string import ascii_letters, digits
 
 import aiohttp
 import aiohttp.typedefs
 
 from genshin import constants, errors, types
 from genshin.client import routes
 from genshin.client.manager import managers
+from genshin.models.miyoushe.cookie import StokenResult
 from genshin.utility import ds as ds_utility
 
 __all__ = [
     "complete_cookies",
+    "fetch_cookie_token_by_game_token",
     "fetch_cookie_token_info",
     "fetch_cookie_with_cookie",
     "fetch_cookie_with_stoken_v2",
+    "fetch_stoken_by_game_token",
     "refresh_cookie_token",
 ]
 
+STOKEN_BY_GAME_TOKEN_HEADERS = {
+    "x-rpc-app_version": "2.41.0",
+    "x-rpc-aigis": "",
+    "Content-Type": "application/json",
+    "Accept": "application/json",
+    "x-rpc-game_biz": "bbs_cn",
+    "x-rpc-sys_version": "11",
+    "x-rpc-device_name": "GenshinUid_login_device_lulu",
+    "x-rpc-device_model": "GenshinUid_login_device_lulu",
+    "x-rpc-app_id": "bll8iq97cem8",
+    "x-rpc-client_type": "2",
+    "User-Agent": "okhttp/4.8.0",
+}
+
 
 async def fetch_cookie_with_cookie(
     cookies: managers.CookieOrHeader,
     *,
     source: typing.Literal["CookieToken", "SToken"],
     target: typing.Literal["CookieAccountInfo", "LToken", "ActionTicket"],
     region: types.Region = types.Region.OVERSEAS,
@@ -161,7 +182,49 @@
     """
     cookies = managers.parse_cookie(cookies)
 
     if refresh:
         cookies = await refresh_cookie_token(cookies, region=region)  # type: ignore[assignment]
 
     return cookies
+
+
+async def fetch_cookie_token_by_game_token(*, game_token: str, account_id: str) -> str:
+    """Fetch cookie token by game token, which is obtained by scanning a QR code."""
+    url = routes.GET_COOKIE_TOKEN_BY_GAME_TOKEN_URL.get_url()
+    params = {
+        "game_token": game_token,
+        "account_id": account_id,
+    }
+
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url, params=params) as r:
+            data = await r.json()
+
+    if not data["data"]:
+        errors.raise_for_retcode(data)
+
+    return data["data"]["cookie_token"]
+
+
+async def fetch_stoken_by_game_token(*, game_token: str, account_id: int) -> StokenResult:
+    """Fetch cookie token by game token, which is obtained by scanning a QR code."""
+    url = routes.GET_STOKEN_BY_GAME_TOKEN_URL.get_url()
+    payload = {
+        "account_id": account_id,
+        "game_token": game_token,
+    }
+    headers = {
+        "DS": ds_utility.generate_passport_ds(body=payload),
+        "x-rpc-device_id": uuid.uuid4().hex,
+        "x-rpc-device_fp": "".join(random.choices(ascii_letters + digits, k=13)),
+        **STOKEN_BY_GAME_TOKEN_HEADERS,
+    }
+
+    async with aiohttp.ClientSession() as session:
+        async with session.post(url, json=payload, headers=headers) as r:
+            data = await r.json()
+
+    if not data["data"]:
+        errors.raise_for_retcode(data)
+
+    return StokenResult(**data["data"])
```

### Comparing `genshin-1.6.2/genshin/client/manager/managers.py` & `genshin-1.6.3/genshin/client/manager/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Cookie managers for making authenticated requests."""
+
 from __future__ import annotations
 
 import abc
 import functools
 import http.cookies
 import logging
 import typing
@@ -245,14 +246,17 @@
     def user_id(self) -> typing.Optional[int]:
         """The id of the user that owns cookies.
 
         Returns None if cookies are not set.
         """
         for name, value in self.cookies.items():
             if name in ("ltuid", "account_id", "ltuid_v2", "account_id_v2"):
+                if not value:
+                    raise ValueError(f"{name} can not be an empty string.")
+
                 return int(value)
 
         return None
 
     async def request(
         self,
         url: aiohttp.typedefs.StrOrURL,
```

### Comparing `genshin-1.6.2/genshin/client/ratelimit.py` & `genshin-1.6.3/genshin/client/ratelimit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Ratelimit handlers."""
+
 import asyncio
 import functools
 import typing
 
 from genshin import errors
 
 CallableT = typing.TypeVar("CallableT", bound=typing.Callable[..., typing.Awaitable[typing.Any]])
```

### Comparing `genshin-1.6.2/genshin/client/routes.py` & `genshin-1.6.3/genshin/client/routes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 """API routes."""
+
 import abc
 import typing
 
 import yarl
 
 from genshin import types
 
 __all__ = [
     "ACCOUNT_URL",
     "APP_LOGIN_URL",
     "BBS_REFERER_URL",
     "BBS_URL",
     "CALCULATOR_URL",
+    "CHECK_QRCODE_URL",
+    "CN_WEB_LOGIN_URL",
     "COMMUNITY_URL",
     "COOKIE_V2_REFRESH_URL",
+    "CREATE_QRCODE_URL",
     "DETAIL_LEDGER_URL",
     "GACHA_URL",
+    "GET_COOKIE_TOKEN_BY_GAME_TOKEN_URL",
+    "GET_STOKEN_BY_GAME_TOKEN_URL",
     "HK4E_URL",
     "INFO_LEDGER_URL",
     "LINEUP_URL",
     "MI18N",
     "RECORD_URL",
     "REWARD_URL",
     "Route",
@@ -92,16 +98,16 @@
         if not self.urls[region].get(game):
             raise RuntimeError(f"URL does not support {game.name} game for {region.name} region.")
 
         return self.urls[region][game]
 
 
 WEBSTATIC_URL = InternationalRoute(
-    "https://webstatic-sea.hoyoverse.com/",
-    "https://webstatic.mihoyo.com/",
+    "https://operation-webstatic.hoyoverse.com/",
+    "https://operation-webstatic.mihoyo.com/",
 )
 
 WEBAPI_URL = InternationalRoute(
     "https://webapi-os.account.hoyoverse.com/Api/",
     "https://webapi.account.mihoyo.com/Api/",
 )
 ACCOUNT_URL = InternationalRoute(
@@ -204,20 +210,30 @@
 )
 YSULOG_URL = InternationalRoute(
     overseas="https://hk4e-api-os.hoyoverse.com/common/hk4e_self_help_query/User/",
     chinese="https://hk4e-api.mihoyo.com/common/hk4e_self_help_query/User/",
 )
 
 MI18N = dict(
-    bbs="https://webstatic-sea.mihoyo.com/admin/mi18n/bbs_cn/m11241040191111/m11241040191111-{lang}.json",
+    bbs="https://fastcdn.hoyoverse.com/mi18n/bbs_oversea/m11241040191111/m11241040191111-{lang}.json",
     inquiry="https://mi18n-os.hoyoverse.com/webstatic/admin/mi18n/hk4e_global/m02251421001311/m02251421001311-{lang}.json",
 )
 
 COOKIE_V2_REFRESH_URL = Route("https://sg-public-api.hoyoverse.com/account/ma-passport/token/getBySToken")
+GET_COOKIE_TOKEN_BY_GAME_TOKEN_URL = Route("https://api-takumi.mihoyo.com/auth/api/getCookieAccountInfoByGameToken")
+GET_STOKEN_BY_GAME_TOKEN_URL = Route("https://passport-api.mihoyo.com/account/ma-cn-session/app/getTokenByGameToken")
 
 WEB_LOGIN_URL = Route("https://sg-public-api.hoyolab.com/account/ma-passport/api/webLoginByPassword")
 APP_LOGIN_URL = Route("https://sg-public-api.hoyoverse.com/account/ma-passport/api/appLoginByPassword")
+CN_WEB_LOGIN_URL = Route("https://passport-api.miyoushe.com/account/ma-cn-passport/web/loginByPassword")
 
 SEND_VERIFICATION_CODE_URL = Route(
     "https://sg-public-api.hoyoverse.com/account/ma-verifier/api/createEmailCaptchaByActionTicket"
 )
 VERIFY_EMAIL_URL = Route("https://sg-public-api.hoyoverse.com/account/ma-verifier/api/verifyActionTicketPartly")
+
+CHECK_MOBILE_VALIDITY_URL = Route("https://webapi.account.mihoyo.com/Api/is_mobile_registrable")
+MOBILE_OTP_URL = Route("https://passport-api.miyoushe.com/account/ma-cn-verifier/verifier/createLoginCaptcha")
+MOBILE_LOGIN_URL = Route("https://passport-api.miyoushe.com/account/ma-cn-passport/web/loginByMobileCaptcha")
+
+CREATE_QRCODE_URL = Route("https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/fetch")
+CHECK_QRCODE_URL = Route("https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/query")
```

### Comparing `genshin-1.6.2/genshin/constants.py` & `genshin-1.6.3/genshin/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants hardcoded for optimizations."""
+
 from . import types
 
 __all__ = ["LANGS"]
 
 
 LANGS = {
     "zh-cn": "简体中文",
@@ -24,9 +25,10 @@
 """Languages supported by the API."""
 
 DS_SALT = {
     types.Region.OVERSEAS: "6s25p5ox5y14umn1p61aqyyvbvvl3lrt",
     types.Region.CHINESE: "xV8v4Qu54lUKrEYFZkJhB8cuOh9Asafs",
     "app_login": "IZPgfb0dRPtBeLuFkdDznSZ6f4wWt6y2",
     "cn_signin": "9nQiU3AV0rJSIBWgdynfoGMGKaklfbM7",
+    "cn_passport": "JwYDpKvLj6MrMqqYU6jTKF17KNO2PXoS",
 }
 """Dynamic Secret Salts."""
```

### Comparing `genshin-1.6.2/genshin/errors.py` & `genshin-1.6.3/genshin/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Errors received from the API."""
+
 import typing
 
 __all__ = [
     "AccountNotFound",
     "AlreadyClaimed",
     "AuthkeyException",
     "AuthkeyTimeout",
@@ -26,15 +27,19 @@
 class GenshinException(Exception):
     """A base genshin exception."""
 
     retcode: int = 0
     original: str = ""
     msg: str = ""
 
-    def __init__(self, response: typing.Mapping[str, typing.Any] = {}, msg: typing.Optional[str] = None) -> None:
+    def __init__(
+        self,
+        response: typing.Mapping[str, typing.Any] = {},
+        msg: typing.Optional[str] = None,
+    ) -> None:
         self.retcode = response.get("retcode", self.retcode)
         self.original = response.get("message", "")
         self.msg = msg or self.msg or self.original
 
         if self.retcode:
             msg = f"[{self.retcode}] {self.msg}"
         else:
@@ -171,28 +176,37 @@
 
 class AccountHasLocked(GenshinException):
     """Account has logged incorrect over than 3 - 5 time(s). It's will be locked and wait 20 minute."""
 
     msg = "Account has been locked because exceeded password limit. Please wait 20 minute and try again"
 
 
+class WrongOTP(GenshinException):
+    """Wrong OTP code."""
+
+    msg = "The provided OTP code is wrong."
+
+
 _TGE = typing.Type[GenshinException]
 _errors: typing.Dict[int, typing.Union[_TGE, str, typing.Tuple[_TGE, typing.Optional[str]]]] = {
     # misc hoyolab
     -100: InvalidCookies,
     -108: "Invalid language.",
     -110: VisitsTooFrequently,
     # game record
     10001: InvalidCookies,
     -10001: "Malformed request.",
     -10002: "No game account associated with cookies.",
     # database game record
     10101: TooManyRequests,
     10102: DataNotPublic,
-    10103: (InvalidCookies, "Cookies are valid but do not have a hoyolab account bound to them."),
+    10103: (
+        InvalidCookies,
+        "Cookies are valid but do not have a hoyolab account bound to them.",
+    ),
     10104: "Cannot view real-time notes of other users.",
     # calculator
     -500001: "Invalid fields in calculation.",
     -500004: VisitsTooFrequently,
     -502001: "User does not have this character.",
     -502002: "Calculator sync is not enabled.",
     # mixin
@@ -205,23 +219,27 @@
     -2001: (RedemptionInvalid, "Redemption code has expired."),
     -2003: (RedemptionInvalid, "Redemption code is incorrectly formatted."),
     -2004: RedemptionInvalid,
     -2014: (RedemptionInvalid, "Redemption code not activated"),
     -2016: RedemptionCooldown,
     -2017: RedemptionClaimed,
     -2018: RedemptionClaimed,
-    -2021: (RedemptionException, "Cannot claim codes for accounts with adventure rank lower than 10."),
+    -2021: (
+        RedemptionException,
+        "Cannot claim codes for accounts with adventure rank lower than 10.",
+    ),
     # rewards
     -5003: AlreadyClaimed,
     # chinese
     1008: AccountNotFound,
     -1104: "This action must be done in the app.",
     # account
     -3208: AccountLoginFail,
     -3202: AccountHasLocked,
+    -3205: WrongOTP,
 }
 
 ERRORS: typing.Dict[int, typing.Tuple[_TGE, typing.Optional[str]]] = {
     retcode: ((exc, None) if isinstance(exc, type) else (GenshinException, exc) if isinstance(exc, str) else exc)
     for retcode, exc in _errors.items()
 }
```

### Comparing `genshin-1.6.2/genshin/models/genshin/calculator.py` & `genshin-1.6.3/genshin/models/genshin/calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin calculator models."""
+
 from __future__ import annotations
 
 import collections
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
```

### Comparing `genshin-1.6.2/genshin/models/genshin/character.py` & `genshin-1.6.3/genshin/models/genshin/character.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Genshin character model."""
 
 import logging
 import re
 import typing
 
+from genshin.utility import deprecation
+
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
 else:
     try:
         import pydantic.v1 as pydantic
     except ImportError:
         import pydantic
@@ -16,15 +18,15 @@
 
 from . import constants
 
 __all__ = ["BaseCharacter"]
 
 _LOGGER = logging.getLogger(__name__)
 
-ICON_BASE = "https://upload-os-bbs.mihoyo.com/game_record/genshin/"
+ICON_BASE = "https://enka.network/ui/"
 
 
 def _parse_icon(icon: typing.Union[str, int]) -> str:
     if isinstance(icon, int):
         for names in constants.CHARACTER_NAMES.values():
             char = names.get(icon)
             if char:
@@ -82,15 +84,22 @@
         # might as well just update the CHARACTER_NAMES if we have all required data
         if id and name and icon and element and rarity:
             char = constants.DBChar(id, icon_name, name, element, rarity, guessed=True)
             _LOGGER.debug("Updating CHARACTER_NAMES with %s", char)
             constants.CHARACTER_NAMES[lang][char.id] = char
             return char
 
-        return constants.DBChar(id or 0, icon_name, name or icon_name, element or "Anemo", rarity or 5, guessed=True)
+        return constants.DBChar(
+            id or 0,
+            icon_name,
+            name or icon_name,
+            element or "Anemo",
+            rarity or 5,
+            guessed=True,
+        )
 
     if name:
         for char in constants.CHARACTER_NAMES[lang].values():
             if char.name == name:
                 return char
 
         return constants.DBChar(id or 0, icon or name, name, element or "Anemo", rarity or 5, guessed=True)
@@ -111,15 +120,15 @@
 
     @pydantic.root_validator(pre=True)
     def __autocomplete(cls, values: typing.Dict[str, typing.Any]) -> typing.Dict[str, typing.Any]:
         """Complete missing data."""
         id, name, icon, element, rarity = (values.get(x) for x in ("id", "name", "icon", "element", "rarity"))
 
         char = _get_db_char(id, name, icon, element, rarity, lang=values["lang"])
-        icon = _create_icon(char.icon_name, "character_icon/UI_AvatarIcon_{}")
+        icon = _create_icon(char.icon_name, "UI_AvatarIcon_{}")
 
         values["id"] = char.id
         values["name"] = char.name
         values["element"] = char.element
         values["rarity"] = char.rarity
 
         if values.get("icon"):
@@ -139,24 +148,29 @@
         elif values["id"] == 10000062:
             # sometimes Aloy has 5* if no background is needed
             values["collab"] = True
 
         return values
 
     @property
+    @deprecation.deprecated("gacha_art")
     def image(self) -> str:
-        return _create_icon(self.icon, "character_image/UI_AvatarIcon_{}@2x")
+        return _create_icon(self.icon, "UI_Gacha_AvatarImg_{}")
+
+    @property
+    def gacha_art(self) -> str:
+        return _create_icon(self.icon, "UI_Gacha_AvatarImg_{}")
 
     @property
     def side_icon(self) -> str:
-        return _create_icon(self.icon, "character_side_icon/UI_AvatarIcon_Side_{}")
+        return _create_icon(self.icon, "UI_AvatarIcon_Side_{}")
 
     @property
     def card_icon(self) -> str:
-        return _create_icon(self.icon, "character_card_icon/UI_AvatarIcon_{}_Card")
+        return _create_icon(self.icon, "UI_AvatarIcon_{}_Card")
 
     @property
     def traveler_name(self) -> str:
         if self.id == 10000005:
             return "Aether"
         elif self.id == 10000007:
             return "Lumine"
```

### Comparing `genshin-1.6.2/genshin/models/genshin/chronicle/abyss.py` & `genshin-1.6.3/genshin/models/genshin/chronicle/abyss.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 class CharacterRanks(APIModel):
     """Collection of rankings achieved during spiral abyss runs."""
 
     # fmt: off
     most_played: typing.Sequence[AbyssRankCharacter] =      Aliased("reveal_rank",       default=[], mi18n="bbs/go_fight_count")
     most_kills: typing.Sequence[AbyssRankCharacter] =       Aliased("defeat_rank",       default=[], mi18n="bbs/max_rout_count")
     strongest_strike: typing.Sequence[AbyssRankCharacter] = Aliased("damage_rank",       default=[], mi18n="bbs/powerful_attack")
-    most_damage_taken: typing.Sequence[AbyssRankCharacter] = Aliased("take_damage_rank", default=[], mi18n="bbs/receive_max_damage")
-    most_bursts_used: typing.Sequence[AbyssRankCharacter] = Aliased("energy_skill_rank", default=[], mi18n="bbs/element_break_count")
-    most_skills_used: typing.Sequence[AbyssRankCharacter] = Aliased("normal_skill_rank", default=[], mi18n="bbs/element_skill_use_count")
+    most_damage_taken: typing.Sequence[AbyssRankCharacter] = Aliased("take_damage_rank", default=[], mi18n="bbs/receive_max_damage")  # noqa: E501
+    most_bursts_used: typing.Sequence[AbyssRankCharacter] = Aliased("energy_skill_rank", default=[], mi18n="bbs/element_break_count") # noqa: E501
+    most_skills_used: typing.Sequence[AbyssRankCharacter] = Aliased("normal_skill_rank", default=[], mi18n="bbs/element_skill_use_count") # noqa: E501
     # fmt: on
 
     def as_dict(self, lang: typing.Optional[str] = None) -> typing.Mapping[str, typing.Any]:
-        """Helper function which turns fields into properly named ones"""
+        """Turn fields into properly named ones."""
         return {
             self._get_mi18n(field, lang or self.lang): getattr(self, field.name)
             for field in self.__fields__.values()
             if field.name != "lang"
         }
```

### Comparing `genshin-1.6.2/genshin/models/genshin/chronicle/activities.py` & `genshin-1.6.3/genshin/models/genshin/chronicle/activities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chronicle activities models."""
+
 import datetime
 import re
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
     import pydantic.v1.generics as pydantic_generics
```

### Comparing `genshin-1.6.2/genshin/models/genshin/chronicle/characters.py` & `genshin-1.6.3/genshin/models/genshin/chronicle/characters.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/genshin/models/genshin/chronicle/notes.py` & `genshin-1.6.3/genshin/models/genshin/chronicle/notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin chronicle notes."""
+
 import datetime
 import enum
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
 else:
```

### Comparing `genshin-1.6.2/genshin/models/genshin/chronicle/stats.py` & `genshin-1.6.3/genshin/models/genshin/chronicle/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     luxurious_chests: int =   Aliased("luxurious_chest_number", mi18n="bbs/magnificent_treasure_box_count")
     remarkable_chests: int =  Aliased("magic_chest_number",     mi18n="bbs/magic_chest_number")
     unlocked_waypoints: int = Aliased("way_point_number",       mi18n="bbs/unlock_portal")
     unlocked_domains: int =   Aliased("domain_number",          mi18n="bbs/unlock_secret_area")
     # fmt: on
 
     def as_dict(self, lang: typing.Optional[str] = None) -> typing.Mapping[str, typing.Any]:
-        """Helper function which turns fields into properly named ones"""
+        """Turn fields into properly named ones."""
         return {
             self._get_mi18n(field, lang or self.lang): getattr(self, field.name)
             for field in self.__fields__.values()
             if field.name != "lang"
         }
```

### Comparing `genshin-1.6.2/genshin/models/genshin/chronicle/tcg.py` & `genshin-1.6.3/genshin/models/genshin/chronicle/tcg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin serenitea pot replica display models."""
+
 from __future__ import annotations
 
 import enum
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
```

### Comparing `genshin-1.6.2/genshin/models/genshin/constants.py` & `genshin-1.6.3/genshin/models/genshin/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin model constants."""
+
 import typing
 
 __all__ = ["CHARACTER_NAMES", "DBChar"]
 
 
 class DBChar(typing.NamedTuple):
     """Partial genshin character data."""
```

### Comparing `genshin-1.6.2/genshin/models/genshin/daily.py` & `genshin-1.6.3/genshin/models/genshin/daily.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Daily reward models."""
-import calendar
+
 import datetime
 import typing
 
 from genshin.models.model import Aliased, APIModel, Unique
 
 __all__ = ["ClaimedDailyReward", "DailyReward", "DailyRewardInfo"]
 
@@ -14,16 +14,15 @@
     signed_in: bool
     claimed_rewards: int
 
     @property
     def missed_rewards(self) -> int:
         cn_timezone = datetime.timezone(datetime.timedelta(hours=8))
         now = datetime.datetime.now(cn_timezone)
-        month_days = calendar.monthrange(now.year, now.month)[1]
-        return month_days - self.claimed_rewards
+        return now.day - self.claimed_rewards
 
 
 class DailyReward(APIModel):
     """Claimable daily reward."""
 
     name: str
     amount: int = Aliased("cnt")
```

### Comparing `genshin-1.6.2/genshin/models/genshin/diary.py` & `genshin-1.6.3/genshin/models/genshin/diary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin diary models."""
+
 import datetime
 import enum
 import typing
 
 from genshin.models.model import Aliased, APIModel
 
 __all__ = [
```

### Comparing `genshin-1.6.2/genshin/models/genshin/gacha.py` & `genshin-1.6.3/genshin/models/genshin/gacha.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin wish models."""
+
 import datetime
 import enum
 import re
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
```

### Comparing `genshin-1.6.2/genshin/models/genshin/lineup.py` & `genshin-1.6.3/genshin/models/genshin/lineup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin lineup models."""
+
 from __future__ import annotations
 
 import datetime
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
@@ -291,15 +292,15 @@
     original_lang: str = Aliased("trans_from")
 
     @pydantic.validator("characters", pre=True)
     def __parse_characters(cls, value: typing.Any) -> typing.Any:
         if isinstance(value[0], typing.Sequence):
             return value
 
-        return [[character for character in group["group"]] for group in value]
+        return [list(group["group"]) for group in value]
 
 
 class Lineup(LineupPreview):
     """Lineup."""
 
     description: str
     views: int = Aliased("view_cnt")
```

### Comparing `genshin-1.6.2/genshin/models/genshin/teapot.py` & `genshin-1.6.3/genshin/models/genshin/teapot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin serenitea pot replica display models."""
+
 from __future__ import annotations
 
 import datetime
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
```

### Comparing `genshin-1.6.2/genshin/models/genshin/transaction.py` & `genshin-1.6.3/genshin/models/genshin/transaction.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/genshin/models/genshin/wiki.py` & `genshin-1.6.3/genshin/models/genshin/wiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genshin wish models."""
+
 import enum
 import json
 import typing
 import unicodedata
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
```

### Comparing `genshin-1.6.2/genshin/models/honkai/battlesuit.py` & `genshin-1.6.3/genshin/models/honkai/battlesuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Honkai battlesuit model."""
+
 import logging
 import re
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
 else:
```

### Comparing `genshin-1.6.2/genshin/models/honkai/chronicle/battlesuits.py` & `genshin-1.6.3/genshin/models/honkai/chronicle/battlesuits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Honkai chronicle battlesuits."""
+
 import re
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
 else:
     try:
```

### Comparing `genshin-1.6.2/genshin/models/honkai/chronicle/modes.py` & `genshin-1.6.3/genshin/models/honkai/chronicle/modes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Honkai battle chronicle models."""
+
 from __future__ import annotations
 
 import datetime
 import re
 import typing
 
 if typing.TYPE_CHECKING:
```

### Comparing `genshin-1.6.2/genshin/models/honkai/chronicle/stats.py` & `genshin-1.6.3/genshin/models/honkai/chronicle/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Honkai stats models."""
+
 import typing
 
 if typing.TYPE_CHECKING:
     import pydantic.v1 as pydantic
 else:
     try:
         import pydantic.v1 as pydantic
@@ -19,15 +20,15 @@
     "FullHonkaiUserStats",
     "HonkaiStats",
     "HonkaiUserStats",
 ]
 
 
 def _model_to_dict(model: APIModel, lang: str = "en-us") -> typing.Mapping[str, typing.Any]:
-    """Helper function which turns fields into properly named ones"""
+    """Turn fields into properly named ones."""
     ret: typing.Dict[str, typing.Any] = {}
     for field in model.__fields__.values():
         if not field.field_info.extra.get("mi18n"):
             continue
 
         mi18n = model._get_mi18n(field, lang)
         val = getattr(model, field.name)
@@ -118,15 +119,15 @@
     # fmt: off
     raw_q_singularis_rank: typing.Optional[int] = Aliased("level_of_quantum", mi18n="bbs/Quantum")
     raw_dirac_sea_rank: typing.Optional[int] =    Aliased("level_of_ow",      mi18n="bbs/level_of_ow")
     score: int =                                  Aliased("abyss_score",      mi18n="bbs/explain_text_2")
     raw_tier: int =                               Aliased("latest_area",      mi18n="bbs/settled_level")
     raw_latest_rank: typing.Optional[int] =       Aliased("latest_level",     mi18n="bbs/rank")
     # TODO: Add proper key
-    latest_type: str =                            Aliased(                    mi18n="bbs/latest_type")  
+    latest_type: str =                            Aliased(                    mi18n="bbs/latest_type")
     # fmt: on
 
     @pydantic.validator("raw_q_singularis_rank", "raw_dirac_sea_rank", "raw_latest_rank", pre=True)
     def __normalize_rank(cls, rank: typing.Optional[str]) -> typing.Optional[int]:  # modes.OldAbyss.__normalize_rank
         if isinstance(rank, int):
             return rank
 
@@ -235,14 +236,15 @@
 
         if "elysian_realm" not in values:
             values["elysian_realm"] = ElysianRealmStats(**values)
 
         return values
 
     def as_dict(self, lang: str = "en-us") -> typing.Mapping[str, typing.Any]:
+        """Turn fields into properly named ones."""
         return _model_to_dict(self, lang)
 
 
 class HonkaiUserStats(APIModel):
     """Represents basic user stats, showing only generic user data and stats."""
 
     info: hoyolab.UserInfo = Aliased("role")
```

### Comparing `genshin-1.6.2/genshin/models/honkai/constants.py` & `genshin-1.6.3/genshin/models/honkai/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Honkai model constants."""
+
 import typing
 
 __all__ = ["BATTLESUIT_IDENTIFIERS"]
 
 # TODO: Make this more dynamic
 # fmt: off
 BATTLESUIT_IDENTIFIERS: typing.Dict[int, str] = {
```

### Comparing `genshin-1.6.2/genshin/models/hoyolab/announcements.py` & `genshin-1.6.3/genshin/models/hoyolab/announcements.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/genshin/models/hoyolab/record.py` & `genshin-1.6.3/genshin/models/hoyolab/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base hoyolab APIModels."""
+
 from __future__ import annotations
 
 import enum
 import re
 import typing
 
 if typing.TYPE_CHECKING:
```

### Comparing `genshin-1.6.2/genshin/models/model.py` & `genshin-1.6.3/genshin/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Modified pydantic model."""
+
 from __future__ import annotations
 
 import abc
 import datetime
 import sys
 import types
 import typing
```

### Comparing `genshin-1.6.2/genshin/models/starrail/character.py` & `genshin-1.6.3/genshin/models/starrail/character.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Starrail base character model."""
+
 from genshin.models.model import APIModel, Unique
 
 
 class StarRailBaseCharacter(APIModel, Unique):
     """Base character model."""
 
     id: int
```

### Comparing `genshin-1.6.2/genshin/models/starrail/chronicle/notes.py` & `genshin-1.6.3/genshin/models/starrail/chronicle/notes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Starrail chronicle notes."""
+
 import datetime
 import typing
 
 from genshin.models.model import Aliased, APIModel
 
 __all__ = ["StarRailExpedition", "StarRailNote"]
 
@@ -10,14 +11,15 @@
 class StarRailExpedition(APIModel):
     """StarRail expedition."""
 
     avatars: typing.List[str]
     status: typing.Literal["Ongoing", "Finished"]
     remaining_time: datetime.timedelta
     name: str
+    item_url: str
 
     @property
     def finished(self) -> bool:
         """Whether the expedition has finished."""
         return self.remaining_time <= datetime.timedelta(0)
 
     @property
```

### Comparing `genshin-1.6.2/genshin/models/starrail/chronicle/rogue.py` & `genshin-1.6.3/genshin/models/starrail/chronicle/rogue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Starrail Rogue models."""
+
 from typing import List
 
 from genshin.models.model import APIModel
 
 from ..character import RogueCharacter
 from .base import PartialTime
```

### Comparing `genshin-1.6.2/genshin/models/starrail/chronicle/stats.py` & `genshin-1.6.3/genshin/models/starrail/chronicle/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Starrail chronicle stats."""
+
 import typing
 
 from genshin.models.model import Aliased, APIModel
 
 from .. import character
 
 __all__ = [
```

### Comparing `genshin-1.6.2/genshin/paginators/api.py` & `genshin-1.6.3/genshin/paginators/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base paginators made specifically for interaction with the api."""
+
 from __future__ import annotations
 
 import abc
 import typing
 import warnings
 
 from . import base
```

### Comparing `genshin-1.6.2/genshin/paginators/base.py` & `genshin-1.6.3/genshin/paginators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,15 @@
         """Flatten the paginator."""
         return [item async for item in self]
 
     def __await__(self) -> typing.Generator[None, None, typing.Sequence[T]]:
         return self.flatten().__await__()
 
     @abc.abstractmethod
-    async def __anext__(self) -> T:
-        ...
+    async def __anext__(self) -> T: ...
 
 
 class BasicPaginator(typing.Generic[T], Paginator[T], abc.ABC):
     """Paginator that simply iterates over an iterable."""
 
     __slots__ = ("iterator",)
```

### Comparing `genshin-1.6.2/genshin/types.py` & `genshin-1.6.3/genshin/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Types used in the library."""
+
 import enum
 import typing
 
 if typing.TYPE_CHECKING:
     from genshin.models.model import Unique
 
 __all__ = ["Game", "Region"]
```

### Comparing `genshin-1.6.2/genshin/utility/concurrency.py` & `genshin-1.6.3/genshin/utility/concurrency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for concurrency optimizations."""
+
 from __future__ import annotations
 
 import asyncio
 import functools
 import typing
 
 __all__ = ["prevent_concurrency"]
```

### Comparing `genshin-1.6.2/genshin/utility/deprecation.py` & `genshin-1.6.3/genshin/utility/deprecation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deprecation decorator."""
+
 import functools
 import inspect
 import typing
 import warnings
 
 __all__ = ["deprecated", "warn_deprecated"]
```

### Comparing `genshin-1.6.2/genshin/utility/ds.py` & `genshin-1.6.3/genshin/utility/ds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Dynamic secret generation."""
+
 import hashlib
 import json
 import random
 import string
 import time
 import typing
 
 from genshin import constants, types
 
-__all__ = ["generate_cn_dynamic_secret", "generate_dynamic_secret", "get_ds_headers"]
+__all__ = ["generate_cn_dynamic_secret", "generate_dynamic_secret", "generate_passport_ds", "get_ds_headers"]
 
 
 def generate_dynamic_secret(salt: str = constants.DS_SALT[types.Region.OVERSEAS]) -> str:
     """Create a new overseas dynamic secret."""
     t = int(time.time())
     r = "".join(random.choices(string.ascii_letters, k=6))
     h = hashlib.md5(f"salt={salt}&t={t}&r={r}".encode()).hexdigest()
@@ -54,7 +55,18 @@
             "x-rpc-app_version": "2.11.1",
             "x-rpc-client_type": "5",
             "ds": generate_cn_dynamic_secret(data, params),
         }
     else:
         raise TypeError(f"{region!r} is not a valid region.")
     return ds_headers
+
+
+def generate_passport_ds(body: typing.Mapping[str, typing.Any]) -> str:
+    """Create a dynamic secret for Miyoushe passport API."""
+    salt = constants.DS_SALT["cn_passport"]
+    t = int(time.time())
+    r = "".join(random.sample(string.ascii_letters, 6))
+    b = json.dumps(body)
+    h = hashlib.md5(f"salt={salt}&t={t}&r={r}&b={b}&q=".encode()).hexdigest()
+    result = f"{t},{r},{h}"
+    return result
```

### Comparing `genshin-1.6.2/genshin/utility/extdb.py` & `genshin-1.6.3/genshin/utility/extdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """External databases for Genshin Impact data."""
 
 import asyncio
 import json
+import logging
 import time
 import typing
 import warnings
 from base64 import b64decode as parse_token
 
 import aiohttp
 
@@ -16,14 +17,16 @@
 __all__ = (
     "update_characters_ambr",
     "update_characters_any",
     "update_characters_enka",
     "update_characters_genshindata",
 )
 
+LOGGER_ = logging.getLogger(__name__)
+
 CACHE_FILE = fs.get_tempdir() / "characters.json"
 
 if CACHE_FILE.exists() and time.time() - CACHE_FILE.stat().st_mtime < 7 * 24 * 60 * 60:
     names: typing.Mapping[str, typing.Any] = json.loads(CACHE_FILE.read_text())
     try:
         model_constants.CHARACTER_NAMES = {
             lang: {int(char_id): model_constants.DBChar(*char) for char_id, char in chars.items()}
@@ -166,16 +169,18 @@
     characters, locs = await _fetch_jsons(ENKA_CHARACTERS_URL, ENKA_LOC_URL)
 
     for strid, char in characters.items():
         if "-" in strid:
             continue  # traveler element
 
         for short_lang, loc in locs.items():
+            if (lang := ENKA_LANG_MAP.get(short_lang)) is None:
+                continue
             update_character_name(
-                lang=ENKA_LANG_MAP[short_lang],
+                lang=lang,
                 id=int(strid),
                 icon_name=char["SideIconName"][len("UI_AvatarIcon_Side_") :],  # noqa: E203
                 name=loc[str(char["NameTextMapHash"])],
                 element=ELEMENTS_MAP[char["Element"]],
                 rarity=RARITY_MAP[char["QualityType"]],
             )
 
@@ -231,12 +236,12 @@
 
     updators.append(update_characters_genshindata)
 
     for updator in updators:
         try:
             await updator(langs)
         except Exception:
-            continue
+            LOGGER_.exception("Failed to update characters with %s", updator.__name__)
         else:
             return
 
     raise Exception("Failed to update characters, all functions raised an error.")
```

### Comparing `genshin-1.6.2/genshin/utility/fs.py` & `genshin-1.6.3/genshin/utility/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """File system related utilities."""
+
 import functools
 import pathlib
 import tempfile
 import typing
 
 __all__ = ["get_browser_cookies"]
```

### Comparing `genshin-1.6.2/genshin/utility/logfile.py` & `genshin-1.6.3/genshin/utility/logfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Search logfile for authkeys."""
+
 import pathlib
 import re
 import typing
 import urllib.parse
 
 from genshin import types
 from genshin.utility import fs
```

### Comparing `genshin-1.6.2/genshin/utility/uid.py` & `genshin-1.6.3/genshin/utility/uid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions related to genshin."""
+
 import typing
 
 from genshin import types
 
 __all__ = [
     "create_short_lang_code",
     "get_prod_game_biz",
@@ -10,50 +11,61 @@
     "recognize_genshin_server",
     "recognize_honkai_server",
     "recognize_region",
     "recognize_server",
     "recognize_starrail_server",
 ]
 
-UID_RANGE: typing.Mapping[types.Game, typing.Mapping[types.Region, typing.Sequence[int]]] = {
+UID_RANGE: typing.Mapping[types.Game, typing.Mapping[types.Region, typing.Sequence[str]]] = {
     types.Game.GENSHIN: {
-        types.Region.OVERSEAS: (6, 7, 8, 9),
-        types.Region.CHINESE: (1, 2, 5),
+        types.Region.OVERSEAS: ("6", "7", "8", "18", "9"),
+        types.Region.CHINESE: ("1", "2", "3", "5"),
     },
     types.Game.STARRAIL: {
-        types.Region.OVERSEAS: (6, 7, 8, 9),
-        types.Region.CHINESE: (1, 2, 5),
+        types.Region.OVERSEAS: ("6", "7", "8", "9"),
+        types.Region.CHINESE: ("1", "2", "5"),
     },
     types.Game.HONKAI: {
-        types.Region.OVERSEAS: (1, 2),
-        types.Region.CHINESE: (3, 4),
+        types.Region.OVERSEAS: ("1", "2"),
+        types.Region.CHINESE: ("3", "4"),
     },
 }
 """Mapping of games and regions to their respective UID ranges."""
 
+GENSHIN_SERVER_RANGE: typing.Mapping[str, typing.Sequence[str]] = {
+    "cn_gf01": ("1", "2", "3"),
+    "cn_qd01": ("5",),
+    "os_usa": ("6",),
+    "os_euro": ("7",),
+    "os_asia": ("8", "18"),
+    "os_cht": ("9",),
+}
+"""Mapping of Genshin servers to their respective UID ranges."""
+
+STARRAIL_SERVER_RANGE: typing.Mapping[str, typing.Sequence[str]] = {
+    "prod_gf_cn": ("1", "2"),
+    "prod_qd_cn": ("5",),
+    "prod_official_usa": ("6",),
+    "prod_official_eur": ("7",),
+    "prod_official_asia": ("8",),
+    "prod_official_cht": ("9",),
+}
+"""Mapping of Star Rail servers to their respective UID ranges."""
+
 
 def create_short_lang_code(lang: str) -> str:
     """Create an alternative short lang code."""
     return lang if "zh" in lang else lang.split("-")[0]
 
 
 def recognize_genshin_server(uid: int) -> str:
     """Recognize which server a Genshin UID is from."""
-    server = {
-        "1": "cn_gf01",
-        "2": "cn_gf01",
-        "5": "cn_qd01",
-        "6": "os_usa",
-        "7": "os_euro",
-        "8": "os_asia",
-        "9": "os_cht",
-    }.get(str(uid)[0])
-
-    if server:
-        return server
+    for server_name, digits in GENSHIN_SERVER_RANGE.items():
+        if str(uid)[:-8] in digits:
+            return server_name
 
     raise ValueError(f"UID {uid} isn't associated with any server")
 
 
 def get_prod_game_biz(region: types.Region, game: types.Game) -> str:
     """Get the game_biz value corresponding to a game and region."""
     game_biz = ""
@@ -86,26 +98,17 @@
     # Probably gonna need some input from actual CN players here, but I know none.
     # It could be that e.g. global range is 2e8 ~ 2.5e8
     raise ValueError(f"UID {uid} isn't associated with any server")
 
 
 def recognize_starrail_server(uid: int) -> str:
     """Recognize which server a Star Rail UID is from."""
-    server = {
-        "1": "prod_gf_cn",
-        "2": "prod_gf_cn",
-        "5": "prod_qd_cn",
-        "6": "prod_official_usa",
-        "7": "prod_official_eur",
-        "8": "prod_official_asia",
-        "9": "prod_official_cht",
-    }.get(str(uid)[0])
-
-    if server:
-        return server
+    for server, digits in STARRAIL_SERVER_RANGE.items():
+        if str(uid)[:-8] in digits:
+            return server
 
     raise ValueError(f"UID {uid} isn't associated with any server")
 
 
 def recognize_server(uid: int, game: types.Game) -> str:
     """Recognizes which server a UID is from."""
     if game == types.Game.HONKAI:
@@ -119,25 +122,21 @@
 
 
 def recognize_game(uid: int, region: types.Region) -> typing.Optional[types.Game]:
     """Recognize the game of a uid."""
     if len(str(uid)) == 8:
         return types.Game.HONKAI
 
-    first = int(str(uid)[0])
-
     for game, digits in UID_RANGE.items():
-        if first in digits[region]:
+        if str(uid)[:-8] in digits[region]:
             return game
 
     return None
 
 
 def recognize_region(uid: int, game: types.Game) -> typing.Optional[types.Region]:
     """Recognize the region of a uid."""
-    first = int(str(uid)[0])
-
     for region, digits in UID_RANGE[game].items():
-        if first in digits:
+        if str(uid)[:-8] in digits:
             return region
 
     return None
```

### Comparing `genshin-1.6.2/genshin.egg-info/PKG-INFO` & `genshin-1.6.3/genshin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.6.2
+Version: 1.6.3
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
@@ -25,18 +25,20 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: pydantic
 Provides-Extra: all
 Requires-Dist: browser-cookie3; extra == "all"
 Requires-Dist: rsa; extra == "all"
 Requires-Dist: click; extra == "all"
+Requires-Dist: qrcode[pil]; extra == "all"
 Provides-Extra: cookies
 Requires-Dist: browser-cookie3; extra == "cookies"
 Provides-Extra: geetest
 Requires-Dist: rsa; extra == "geetest"
+Requires-Dist: qrcode[pil]; extra == "geetest"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 # genshin.py
 
 [![Downloads](https://pepy.tech/badge/genshin)](https://pepy.tech/project/genshin)
 [![PyPI package](https://img.shields.io/pypi/v/genshin)](https://pypi.org/project/genshin/)
```

### Comparing `genshin-1.6.2/genshin.egg-info/SOURCES.txt` & `genshin-1.6.3/genshin.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 genshin/models/honkai/chronicle/battlesuits.py
 genshin/models/honkai/chronicle/modes.py
 genshin/models/honkai/chronicle/stats.py
 genshin/models/hoyolab/__init__.py
 genshin/models/hoyolab/announcements.py
 genshin/models/hoyolab/private.py
 genshin/models/hoyolab/record.py
+genshin/models/miyoushe/__init__.py
+genshin/models/miyoushe/cookie.py
+genshin/models/miyoushe/qrcode.py
 genshin/models/starrail/__init__.py
 genshin/models/starrail/character.py
 genshin/models/starrail/chronicle/__init__.py
 genshin/models/starrail/chronicle/base.py
 genshin/models/starrail/chronicle/challenge.py
 genshin/models/starrail/chronicle/characters.py
 genshin/models/starrail/chronicle/notes.py
```

### Comparing `genshin-1.6.2/setup.py` & `genshin-1.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Run setuptools."""
+
 from setuptools import find_packages, setup
 
 setup(
     name="genshin",
-    version="1.6.2",
+    version="1.6.3",
     author="thesadru",
     author_email="thesadru@gmail.com",
     description="An API wrapper for Genshin Impact.",
     keywords="hoyoverse mihoyo genshin genshin-impact honkai".split(),
     url="https://github.com/thesadru/genshin.py",
     project_urls={
         "Documentation": "https://thesadru.github.io/genshin.py",
         "Issue tracker": "https://github.com/thesadru/genshin.py/issues",
     },
     packages=find_packages(exclude=["tests.*"]),
     python_requires=">=3.8",
     install_requires=["aiohttp", "pydantic"],
     extras_require={
-        "all": ["browser-cookie3", "rsa", "click"],
+        "all": ["browser-cookie3", "rsa", "click", "qrcode[pil]"],
         "cookies": ["browser-cookie3"],
-        "geetest": ["rsa"],
+        "geetest": ["rsa", "qrcode[pil]"],
         "cli": ["click"],
     },
     include_package_data=True,
     package_data={"genshin": ["py.typed"]},
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `genshin-1.6.2/tests/conftest.py` & `genshin-1.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `genshin-1.6.2/tests/test_paginators.py` & `genshin-1.6.3/tests/test_paginators.py`

 * *Files identical despite different names*

