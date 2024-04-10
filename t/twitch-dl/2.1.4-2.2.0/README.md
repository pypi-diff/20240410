# Comparing `tmp/twitch-dl-2.1.4.tar.gz` & `tmp/twitch-dl-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-dl-2.1.4.tar", last modified: Sat Jan  6 18:49:59 2024, max compression
+gzip compressed data, was "twitch-dl-2.2.0.tar", last modified: Wed Apr 10 06:32:59 2024, max compression
```

## Comparing `twitch-dl-2.1.4.tar` & `twitch-dl-2.2.0.tar`

### file list

```diff
@@ -1,36 +1,68 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-01-06 18:49:59.525444 twitch-dl-2.1.4/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      759 2024-01-06 18:49:59.525444 twitch-dl-2.1.4/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2023-08-11 10:29:32.000000 twitch-dl-2.1.4/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-01-06 18:49:59.525444 twitch-dl-2.1.4/setup.cfg
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1128 2024-01-06 18:43:39.000000 twitch-dl-2.1.4/setup.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-01-06 18:49:59.523444 twitch-dl-2.1.4/tests/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1409 2023-08-11 10:29:32.000000 twitch-dl-2.1.4/tests/test_api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2020 2023-08-11 10:29:32.000000 twitch-dl-2.1.4/tests/test_patterns.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2023-08-11 10:29:32.000000 twitch-dl-2.1.4/tests/test_progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2023-08-11 10:29:32.000000 twitch-dl-2.1.4/tests/test_utils.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-01-06 18:49:59.524443 twitch-dl-2.1.4/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      759 2024-01-06 18:49:59.000000 twitch-dl-2.1.4/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      676 2024-01-06 18:49:59.000000 twitch-dl-2.1.4/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-01-06 18:49:59.000000 twitch-dl-2.1.4/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       52 2024-01-06 18:49:59.000000 twitch-dl-2.1.4/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       40 2024-01-06 18:49:59.000000 twitch-dl-2.1.4/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-01-06 18:49:59.000000 twitch-dl-2.1.4/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-01-06 18:49:59.524443 twitch-dl-2.1.4/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       69 2024-01-06 18:43:43.000000 twitch-dl-2.1.4/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       42 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/__main__.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-01-06 18:49:59.524443 twitch-dl-2.1.4/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      198 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2702 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12820 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      182 2023-10-08 19:39:41.000000 twitch-dl-2.1.4/twitchdl/commands/env.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2592 2024-01-06 18:39:42.000000 twitch-dl-2.1.4/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1892 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10603 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/console.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      882 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      113 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3892 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4374 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4435 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9435 2024-01-06 18:41:10.000000 twitch-dl-2.1.4/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2938 2023-08-11 10:29:42.000000 twitch-dl-2.1.4/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.236628 twitch-dl-2.2.0/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/.flake8
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/.vermin
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9663 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/CHANGELOG.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      951 2024-03-25 07:34:51.000000 twitch-dl-2.2.0/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-10 06:32:59.235628 twitch-dl-2.2.0/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2022-11-13 13:02:23.000000 twitch-dl-2.2.0/TODO.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/book.css
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/book.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8103 2024-04-10 06:31:31.000000 twitch-dl-2.2.0/changelog.yaml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.229628 twitch-dl-2.2.0/docs/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/SUMMARY.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/advanced.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9663 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/changelog.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.230628 twitch-dl-2.2.0/docs/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/commands/auth_token.png
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/clips.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/download.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/env.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/info.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/videos.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/environment_variables.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/installation.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/introduction.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/license.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/shell_completion.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/usage.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1269 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/pyproject.toml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.231628 twitch-dl-2.2.0/scripts/
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2022-11-13 13:02:23.000000 twitch-dl-2.2.0/scripts/generate_changelog
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/scripts/generate_docs
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-10 06:26:52.000000 twitch-dl-2.2.0/scripts/tag_version
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-10 06:32:59.236628 twitch-dl-2.2.0/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.231628 twitch-dl-2.2.0/tests/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1578 2024-04-10 06:03:56.000000 twitch-dl-2.2.0/tests/test_api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2020 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/tests/test_patterns.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2022-11-13 13:02:23.000000 twitch-dl-2.2.0/tests/test_progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/tests/test_utils.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/twitch-dl.1.scd
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.235628 twitch-dl-2.2.0/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1195 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      111 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.234628 twitch-dl-2.2.0/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9521 2024-04-10 06:24:49.000000 twitch-dl-2.2.0/twitchdl/cli.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.235628 twitch-dl-2.2.0/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2539 2024-04-06 08:39:48.000000 twitch-dl-2.2.0/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11573 2024-04-05 06:57:32.000000 twitch-dl-2.2.0/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2929 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2049 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      931 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      482 2024-04-04 08:48:56.000000 twitch-dl-2.2.0/twitchdl/entities.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-06 08:15:38.000000 twitch-dl-2.2.0/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4558 2024-04-06 08:40:29.000000 twitch-dl-2.2.0/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3630 2024-04-10 05:59:56.000000 twitch-dl-2.2.0/twitchdl/playlists.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4627 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11118 2024-04-04 06:57:51.000000 twitch-dl-2.2.0/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3037 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/utils.py
```

### Comparing `twitch-dl-2.1.4/LICENSE` & `twitch-dl-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.4/README.md` & `twitch-dl-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 * [Source code](https://github.com/ihabunek/twitch-dl)
 * [Issues](https://github.com/ihabunek/twitch-dl/issues)
 * [Python package](https://pypi.org/project/twitch-dl/)
 
 Requirements
 ------------
 
-* Python 3.7 or later
+* Python 3.8 or later
 * [ffmpeg](https://ffmpeg.org/download.html), installed and on the system path
 
 Quick start
 -----------
 
 See [installation instructions](https://twitch-dl.bezdomni.net/installation.html)
 to set up twitch-dl.
```

### Comparing `twitch-dl-2.1.4/tests/test_patterns.py` & `twitch-dl-2.2.0/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.4/tests/test_progress.py` & `twitch-dl-2.2.0/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.4/twitchdl/commands/clips.py` & `twitch-dl-2.2.0/twitchdl/commands/clips.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,95 @@
 import re
 import sys
-
-from itertools import islice
 from os import path
+from typing import Callable, Generator
+
+import click
 
 from twitchdl import twitch, utils
 from twitchdl.commands.download import get_clip_authenticated_url
 from twitchdl.download import download_file
-from twitchdl.output import print_out, print_clip, print_json
+from twitchdl.output import green, print_clip, print_clip_compact, print_json, print_paged, yellow
+from twitchdl.twitch import Clip
 
 
-def clips(args):
+def clips(
+    channel_name: str,
+    *,
+    all: bool = False,
+    compact: bool = False,
+    download: bool = False,
+    json: bool = False,
+    limit: int | None = None,
+    pager: int | None = None,
+    period: twitch.ClipsPeriod = "all_time",
+):
+    # Set different defaults for limit for compact display
+    default_limit = 40 if compact else 10
+
     # Ignore --limit if --pager or --all are given
-    limit = sys.maxsize if args.all or args.pager else args.limit
+    limit = sys.maxsize if all or pager else (limit or default_limit)
 
-    generator = twitch.channel_clips_generator(args.channel_name, args.period, limit)
+    generator = twitch.channel_clips_generator(channel_name, period, limit)
 
-    if args.json:
+    if json:
         return print_json(list(generator))
 
-    if args.download:
+    if download:
         return _download_clips(generator)
 
-    if args.pager:
-        print(args)
-        return _print_paged(generator, args.pager)
-
-    return _print_all(generator, args)
+    print_fn = print_clip_compact if compact else print_clip
 
+    if pager:
+        return print_paged("Clips", generator, print_fn, pager)
 
-def _continue():
-    print_out("Press <green><b>Enter</green> to continue, <yellow><b>Ctrl+C</yellow> to break.")
+    return _print_all(generator, print_fn, all)
 
-    try:
-        input()
-    except KeyboardInterrupt:
-        return False
 
-    return True
-
-
-def _target_filename(clip):
+def _target_filename(clip: Clip):
     url = clip["videoQualities"][0]["sourceURL"]
     _, ext = path.splitext(url)
     ext = ext.lstrip(".")
 
     match = re.search(r"^(\d{4})-(\d{2})-(\d{2})T", clip["createdAt"])
+    if not match:
+        raise ValueError(f"Failed parsing date from: {clip['createdAt']}")
     date = "".join(match.groups())
 
-    name = "_".join([
-        date,
-        clip["id"],
-        clip["broadcaster"]["login"],
-        utils.slugify(clip["title"]),
-    ])
+    name = "_".join(
+        [
+            date,
+            clip["id"],
+            clip["broadcaster"]["login"],
+            utils.slugify(clip["title"]),
+        ]
+    )
 
-    return "{}.{}".format(name, ext)
+    return f"{name}.{ext}"
 
 
-def _download_clips(generator):
+def _download_clips(generator: Generator[Clip, None, None]):
     for clip in generator:
         target = _target_filename(clip)
 
         if path.exists(target):
-            print_out("Already downloaded: <green>{}</green>".format(target))
+            click.echo(f"Already downloaded: {green(target)}")
         else:
             url = get_clip_authenticated_url(clip["slug"], "source")
-            print_out("Downloading: <yellow>{}</yellow>".format(target))
+            click.echo(f"Downloading: {yellow(target)}")
             download_file(url, target)
 
 
-def _print_all(generator, args):
+def _print_all(
+    generator: Generator[Clip, None, None],
+    print_fn: Callable[[Clip], None],
+    all: bool,
+):
     for clip in generator:
-        print_out()
-        print_clip(clip)
+        print_fn(clip)
 
-    if not args.all:
-        print_out(
-            "\n<dim>There may be more clips. " +
-            "Increase the --limit, use --all or --pager to see the rest.</dim>"
+    if not all:
+        click.secho(
+            "\nThere may be more clips. "
+            + "Increase the --limit, use --all or --pager to see the rest.",
+            dim=True,
         )
-
-
-def _print_paged(generator, page_size):
-    iterator = iter(generator)
-    page = list(islice(iterator, page_size))
-
-    first = 1
-    last = first + len(page) - 1
-
-    while True:
-        print_out("-" * 80)
-
-        print_out()
-        for clip in page:
-            print_clip(clip)
-            print_out()
-
-        last = first + len(page) - 1
-
-        print_out("-" * 80)
-        print_out("<yellow>Clips {}-{}</yellow>".format(first, last))
-
-        first = first + len(page)
-        last = first + 1
-
-        page = list(islice(iterator, page_size))
-        if not page or not _continue():
-            break
```

### Comparing `twitch-dl-2.1.4/twitchdl/commands/download.py` & `twitch-dl-2.2.0/twitchdl/commands/download.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,117 +1,127 @@
 import asyncio
-import httpx
-import m3u8
 import os
+import platform
 import re
 import shutil
 import subprocess
 import tempfile
-
 from os import path
 from pathlib import Path
-from typing import List, Optional, OrderedDict
-from urllib.parse import urlparse, urlencode
+from urllib.parse import urlencode, urlparse
+
+import click
+import httpx
 
 from twitchdl import twitch, utils
 from twitchdl.download import download_file
+from twitchdl.entities import DownloadOptions
 from twitchdl.exceptions import ConsoleError
 from twitchdl.http import download_all
-from twitchdl.output import print_out
-
-
-def _parse_playlists(playlists_m3u8):
-    playlists = m3u8.loads(playlists_m3u8)
-
-    for p in sorted(playlists.playlists, key=lambda p: p.stream_info.resolution is None):
-        if p.stream_info.resolution:
-            name = p.media[0].name
-            description = "x".join(str(r) for r in p.stream_info.resolution)
-        else:
-            name = p.media[0].group_id
-            description = None
-
-        yield name, description, p.uri
+from twitchdl.output import blue, bold, green, print_log, yellow
+from twitchdl.playlists import (
+    enumerate_vods,
+    load_m3u8,
+    make_join_playlist,
+    parse_playlists,
+    select_playlist,
+)
+from twitchdl.twitch import Chapter, Clip, ClipAccessToken, Video
 
 
-def _get_playlist_by_name(playlists, quality):
-    if quality == "source":
-        _, _, uri = playlists[0]
-        return uri
+def download(ids: list[str], args: DownloadOptions):
+    for video_id in ids:
+        download_one(video_id, args)
 
-    for name, _, uri in playlists:
-        if name == quality:
-            return uri
 
-    available = ", ".join([name for (name, _, _) in playlists])
-    msg = "Quality '{}' not found. Available qualities are: {}".format(quality, available)
-    raise ConsoleError(msg)
+def download_one(video: str, args: DownloadOptions):
+    video_id = utils.parse_video_identifier(video)
+    if video_id:
+        return _download_video(video_id, args)
 
+    clip_slug = utils.parse_clip_identifier(video)
+    if clip_slug:
+        return _download_clip(clip_slug, args)
 
-def _select_playlist_interactive(playlists):
-    print_out("\nAvailable qualities:")
-    for n, (name, resolution, uri) in enumerate(playlists):
-        if resolution:
-            print_out("{}) <b>{}</b> <dim>({})</dim>".format(n + 1, name, resolution))
-        else:
-            print_out("{}) <b>{}</b>".format(n + 1, name))
+    raise ConsoleError(f"Invalid input: {video}")
 
-    no = utils.read_int("Choose quality", min=1, max=len(playlists) + 1, default=1)
-    _, _, uri = playlists[no - 1]
-    return uri
 
+def _join_vods(playlist_path: str, target: str, overwrite: bool, video: Video):
+    description = video["description"] or ""
+    description = description.strip()
 
-def _join_vods(playlist_path, target, overwrite, video):
     command = [
         "ffmpeg",
-        "-i", playlist_path,
-        "-c", "copy",
-        "-metadata", "artist={}".format(video["creator"]["displayName"]),
-        "-metadata", "title={}".format(video["title"]),
-        "-metadata", "encoded_by=twitch-dl",
+        "-i",
+        playlist_path,
+        "-c",
+        "copy",
+        "-metadata",
+        f"artist={video['creator']['displayName']}",
+        "-metadata",
+        f"title={video['title']}",
+        "-metadata",
+        f"description={description}",
+        "-metadata",
+        "encoded_by=twitch-dl",
         "-stats",
-        "-loglevel", "warning",
-        "file:{}".format(target),
+        "-loglevel",
+        "warning",
+        f"file:{target}",
     ]
 
     if overwrite:
         command.append("-y")
 
-    print_out("<dim>{}</dim>".format(" ".join(command)))
+    click.secho(f"{' '.join(command)}", dim=True)
     result = subprocess.run(command)
     if result.returncode != 0:
         raise ConsoleError("Joining files failed")
 
 
-def _video_target_filename(video, args):
-    date, time = video['publishedAt'].split("T")
+def _concat_vods(vod_paths: list[str], target: str):
+    tool = "type" if platform.system() == "Windows" else "cat"
+    command = [tool] + vod_paths
+
+    with open(target, "wb") as target_file:
+        result = subprocess.run(command, stdout=target_file)
+        if result.returncode != 0:
+            raise ConsoleError(f"Joining files failed: {result.stderr}")
+
+
+def get_video_placeholders(video: Video, format: str) -> dict[str, str]:
+    date, time = video["publishedAt"].split("T")
     game = video["game"]["name"] if video["game"] else "Unknown"
 
-    subs = {
+    return {
         "channel": video["creator"]["displayName"],
         "channel_login": video["creator"]["login"],
         "date": date,
         "datetime": video["publishedAt"],
-        "format": args.format,
+        "format": format,
         "game": game,
         "game_slug": utils.slugify(game),
         "id": video["id"],
         "time": time,
         "title": utils.titlify(video["title"]),
         "title_slug": utils.slugify(video["title"]),
     }
 
+
+def _video_target_filename(video: Video, args: DownloadOptions):
+    subs = get_video_placeholders(video, args.format)
+
     try:
         return args.output.format(**subs)
     except KeyError as e:
         supported = ", ".join(subs.keys())
-        raise ConsoleError("Invalid key {} used in --output. Supported keys are: {}".format(e, supported))
+        raise ConsoleError(f"Invalid key {e} used in --output. Supported keys are: {supported}")
 
 
-def _clip_target_filename(clip, args):
+def _clip_target_filename(clip: Clip, args: DownloadOptions):
     date, time = clip["createdAt"].split("T")
     game = clip["game"]["name"] if clip["game"] else "Unknown"
 
     url = clip["videoQualities"][0]["sourceURL"]
     _, ext = path.splitext(url)
     ext = ext.lstrip(".")
 
@@ -130,254 +140,221 @@
         "title_slug": utils.slugify(clip["title"]),
     }
 
     try:
         return args.output.format(**subs)
     except KeyError as e:
         supported = ", ".join(subs.keys())
-        raise ConsoleError("Invalid key {} used in --output. Supported keys are: {}".format(e, supported))
-
-
-def _get_vod_paths(playlist, start: Optional[int], end: Optional[int]) -> List[str]:
-    """Extract unique VOD paths for download from playlist."""
-    files = []
-    vod_start = 0
-    for segment in playlist.segments:
-        vod_end = vod_start + segment.duration
-
-        # `vod_end > start` is used here becuase it's better to download a bit
-        # more than a bit less, similar for the end condition
-        start_condition = not start or vod_end > start
-        end_condition = not end or vod_start < end
-
-        if start_condition and end_condition and segment.uri not in files:
-            files.append(segment.uri)
-
-        vod_start = vod_end
-
-    return files
+        raise ConsoleError(f"Invalid key {e} used in --output. Supported keys are: {supported}")
 
 
 def _crete_temp_dir(base_uri: str) -> str:
     """Create a temp dir to store downloads if it doesn't exist."""
     path = urlparse(base_uri).path.lstrip("/")
     temp_dir = Path(tempfile.gettempdir(), "twitch-dl", path)
     temp_dir.mkdir(parents=True, exist_ok=True)
     return str(temp_dir)
 
 
-def download(args):
-    for video_id in args.videos:
-        download_one(video_id, args)
-
-
-def download_one(video: str, args):
-    video_id = utils.parse_video_identifier(video)
-    if video_id:
-        return _download_video(video_id, args)
-
-    clip_slug = utils.parse_clip_identifier(video)
-    if clip_slug:
-        return _download_clip(clip_slug, args)
-
-    raise ConsoleError("Invalid input: {}".format(video))
-
-
-def _get_clip_url(clip, quality):
-    qualities = clip["videoQualities"]
+def _get_clip_url(access_token: ClipAccessToken, quality: str) -> str:
+    qualities = access_token["videoQualities"]
 
     # Quality given as an argument
     if quality:
         if quality == "source":
             return qualities[0]["sourceURL"]
 
         selected_quality = quality.rstrip("p")  # allow 720p as well as 720
         for q in qualities:
             if q["quality"] == selected_quality:
                 return q["sourceURL"]
 
         available = ", ".join([str(q["quality"]) for q in qualities])
-        msg = "Quality '{}' not found. Available qualities are: {}".format(quality, available)
+        msg = f"Quality '{quality}' not found. Available qualities are: {available}"
         raise ConsoleError(msg)
 
     # Ask user to select quality
-    print_out("\nAvailable qualities:")
+    click.echo("\nAvailable qualities:")
     for n, q in enumerate(qualities):
-        print_out("{}) {} [{} fps]".format(n + 1, q["quality"], q["frameRate"]))
-    print_out()
+        click.echo(f"{n + 1}) {bold(q['quality'])} [{q['frameRate']} fps]")
+    click.echo()
 
     no = utils.read_int("Choose quality", min=1, max=len(qualities), default=1)
     selected_quality = qualities[no - 1]
     return selected_quality["sourceURL"]
 
 
-def get_clip_authenticated_url(slug, quality):
-    print_out("<dim>Fetching access token...</dim>")
+def get_clip_authenticated_url(slug: str, quality: str):
+    print_log("Fetching access token...")
     access_token = twitch.get_clip_access_token(slug)
 
     if not access_token:
-        raise ConsoleError("Access token not found for slug '{}'".format(slug))
+        raise ConsoleError(f"Access token not found for slug '{slug}'")
 
     url = _get_clip_url(access_token, quality)
 
-    query = urlencode({
-        "sig": access_token["playbackAccessToken"]["signature"],
-        "token": access_token["playbackAccessToken"]["value"],
-    })
+    query = urlencode(
+        {
+            "sig": access_token["playbackAccessToken"]["signature"],
+            "token": access_token["playbackAccessToken"]["value"],
+        }
+    )
 
-    return "{}?{}".format(url, query)
+    return f"{url}?{query}"
 
 
-def _download_clip(slug: str, args) -> None:
-    print_out("<dim>Looking up clip...</dim>")
+def _download_clip(slug: str, args: DownloadOptions) -> None:
+    print_log("Looking up clip...")
     clip = twitch.get_clip(slug)
-    game = clip["game"]["name"] if clip["game"] else "Unknown"
 
     if not clip:
-        raise ConsoleError("Clip '{}' not found".format(slug))
+        raise ConsoleError(f"Clip '{slug}' not found")
 
-    print_out("Found: <green>{}</green> by <yellow>{}</yellow>, playing <blue>{}</blue> ({})".format(
-        clip["title"],
-        clip["broadcaster"]["displayName"],
-        game,
-        utils.format_duration(clip["durationSeconds"])
-    ))
+    title = clip["title"]
+    user = clip["broadcaster"]["displayName"]
+    game = clip["game"]["name"] if clip["game"] else "Unknown"
+    duration = utils.format_duration(clip["durationSeconds"])
+    click.echo(f"Found: {green(title)} by {yellow(user)}, playing {blue(game)} ({duration})")
 
     target = _clip_target_filename(clip, args)
-    print_out("Target: <blue>{}</blue>".format(target))
+    click.echo(f"Target: {blue(target)}")
 
     if not args.overwrite and path.exists(target):
-        response = input("File exists. Overwrite? [Y/n]: ")
-        if response.lower().strip() not in ["", "y"]:
-            raise ConsoleError("Aborted")
+        response = click.prompt("File exists. Overwrite? [Y/n]", default="Y", show_default=False)
+        if response.lower().strip() != "y":
+            raise click.Abort()
         args.overwrite = True
 
     url = get_clip_authenticated_url(slug, args.quality)
-    print_out("<dim>Selected URL: {}</dim>".format(url))
+    print_log(f"Selected URL: {url}")
 
-    print_out("<dim>Downloading clip...</dim>")
-    download_file(url, target)
-
-    print_out("Downloaded: <blue>{}</blue>".format(target))
+    if args.dry_run:
+        click.echo("Dry run, clip not downloaded.")
+    else:
+        print_log("Downloading clip...")
+        download_file(url, target)
+        click.echo(f"Downloaded: {blue(target)}")
 
 
-def _download_video(video_id, args) -> None:
+def _download_video(video_id: str, args: DownloadOptions) -> None:
     if args.start and args.end and args.end <= args.start:
         raise ConsoleError("End time must be greater than start time")
 
-    print_out("<dim>Looking up video...</dim>")
+    print_log("Looking up video...")
     video = twitch.get_video(video_id)
 
     if not video:
-        raise ConsoleError("Video {} not found".format(video_id))
+        raise ConsoleError(f"Video {video_id} not found")
 
-    print_out("Found: <blue>{}</blue> by <yellow>{}</yellow>".format(
-        video['title'], video['creator']['displayName']))
+    click.echo(f"Found: {blue(video['title'])} by {yellow(video['creator']['displayName'])}")
 
     target = _video_target_filename(video, args)
-    print_out("Output: <blue>{}</blue>".format(target))
+    click.echo(f"Output: {blue(target)}")
 
     if not args.overwrite and path.exists(target):
-        response = input("File exists. Overwrite? [Y/n]: ")
-        if response.lower().strip() not in ["", "y"]:
-            raise ConsoleError("Aborted")
+        response = click.prompt("File exists. Overwrite? [Y/n]: ", default="Y", show_default=False)
+        if response.lower().strip() != "y":
+            raise click.Abort()
         args.overwrite = True
 
     # Chapter select or manual offset
     start, end = _determine_time_range(video_id, args)
 
-    print_out("<dim>Fetching access token...</dim>")
+    print_log("Fetching access token...")
     access_token = twitch.get_access_token(video_id, auth_token=args.auth_token)
 
-    print_out("<dim>Fetching playlists...</dim>")
-    playlists_m3u8 = twitch.get_playlists(video_id, access_token)
-    playlists = list(_parse_playlists(playlists_m3u8))
-    playlist_uri = (_get_playlist_by_name(playlists, args.quality) if args.quality
-            else _select_playlist_interactive(playlists))
+    print_log("Fetching playlists...")
+    playlists_text = twitch.get_playlists(video_id, access_token)
+    playlists = parse_playlists(playlists_text)
+    playlist = select_playlist(playlists, args.quality)
+
+    print_log("Fetching playlist...")
+    vods_text = http_get(playlist.url)
+    vods_m3u8 = load_m3u8(vods_text)
+    vods = enumerate_vods(vods_m3u8, start, end)
 
-    print_out("<dim>Fetching playlist...</dim>")
-    response = httpx.get(playlist_uri)
-    response.raise_for_status()
-    playlist = m3u8.loads(response.text)
-
-    base_uri = re.sub("/[^/]+$", "/", playlist_uri)
+    base_uri = re.sub("/[^/]+$", "/", playlist.url)
     target_dir = _crete_temp_dir(base_uri)
-    vod_paths = _get_vod_paths(playlist, start, end)
 
     # Save playlists for debugging purposes
     with open(path.join(target_dir, "playlists.m3u8"), "w") as f:
-        f.write(playlists_m3u8)
+        f.write(playlists_text)
     with open(path.join(target_dir, "playlist.m3u8"), "w") as f:
-        f.write(response.text)
+        f.write(vods_text)
 
-    print_out("\nDownloading {} VODs using {} workers to {}".format(
-        len(vod_paths), args.max_workers, target_dir))
-    sources = [base_uri + path for path in vod_paths]
-    targets = [os.path.join(target_dir, "{:05d}.ts".format(k)) for k, _ in enumerate(vod_paths)]
-    asyncio.run(download_all(sources, targets, args.max_workers, rate_limit=args.rate_limit))
+    click.echo(f"\nDownloading {len(vods)} VODs using {args.max_workers} workers to {target_dir}")
 
-    # Make a modified playlist which references downloaded VODs
-    # Keep only the downloaded segments and skip the rest
-    org_segments = playlist.segments.copy()
-
-    path_map = OrderedDict(zip(vod_paths, targets))
-    playlist.segments.clear()
-    for segment in org_segments:
-        if segment.uri in path_map:
-            segment.uri = path_map[segment.uri]
-            playlist.segments.append(segment)
+    sources = [base_uri + vod.path for vod in vods]
+    targets = [os.path.join(target_dir, f"{vod.index:05d}.ts") for vod in vods]
+    asyncio.run(download_all(sources, targets, args.max_workers, rate_limit=args.rate_limit))
 
-    playlist_path = path.join(target_dir, "playlist_downloaded.m3u8")
-    playlist.dump(playlist_path)
+    join_playlist = make_join_playlist(vods_m3u8, vods, targets)
+    join_playlist_path = path.join(target_dir, "playlist_downloaded.m3u8")
+    join_playlist.dump(join_playlist_path)  # type: ignore
+    click.echo()
 
     if args.no_join:
-        print_out("\n\n<dim>Skipping joining files...</dim>")
-        print_out("VODs downloaded to:\n<blue>{}</blue>".format(target_dir))
+        print_log("Skipping joining files...")
+        click.echo(f"VODs downloaded to:\n{blue(target_dir)}")
         return
 
-    print_out("\n\nJoining files...")
-    _join_vods(playlist_path, target, args.overwrite, video)
+    if args.concat:
+        print_log("Concating files...")
+        _concat_vods(targets, target)
+    else:
+        print_log("Joining files...")
+        _join_vods(join_playlist_path, target, args.overwrite, video)
+
+    click.echo()
 
     if args.keep:
-        print_out("\n<dim>Temporary files not deleted: {}</dim>".format(target_dir))
+        click.echo(f"Temporary files not deleted: {target_dir}")
     else:
-        print_out("\n<dim>Deleting temporary files...</dim>")
+        print_log("Deleting temporary files...")
         shutil.rmtree(target_dir)
 
-    print_out("\nDownloaded: <green>{}</green>".format(target))
+    click.echo(f"\nDownloaded: {green(target)}")
+
+
+def http_get(url: str) -> str:
+    response = httpx.get(url)
+    response.raise_for_status()
+    return response.text
 
 
-def _determine_time_range(video_id, args):
+def _determine_time_range(video_id: str, args: DownloadOptions):
     if args.start or args.end:
         return args.start, args.end
 
     if args.chapter is not None:
-        print_out("<dim>Fetching chapters...</dim>")
+        print_log("Fetching chapters...")
         chapters = twitch.get_video_chapters(video_id)
 
         if not chapters:
             raise ConsoleError("This video has no chapters")
 
         if args.chapter == 0:
             chapter = _choose_chapter_interactive(chapters)
         else:
             try:
                 chapter = chapters[args.chapter - 1]
             except IndexError:
-                raise ConsoleError(f"Chapter {args.chapter} does not exist. This video has {len(chapters)} chapters.")
+                raise ConsoleError(
+                    f"Chapter {args.chapter} does not exist. This video has {len(chapters)} chapters."
+                )
 
-        print_out(f'Chapter selected: <blue>{chapter["description"]}</blue>\n')
+        click.echo(f'Chapter selected: {blue(chapter["description"])}\n')
         start = chapter["positionMilliseconds"] // 1000
         duration = chapter["durationMilliseconds"] // 1000
         return start, start + duration
 
     return None, None
 
 
-def _choose_chapter_interactive(chapters):
-    print_out("\nChapters:")
+def _choose_chapter_interactive(chapters: list[Chapter]):
+    click.echo("\nChapters:")
     for index, chapter in enumerate(chapters):
         duration = utils.format_time(chapter["durationMilliseconds"] // 1000)
-        print_out(f'{index + 1}) <b>{chapter["description"]}</b> <dim>({duration})</dim>')
+        click.echo(f'{index + 1}) {bold(chapter["description"])} ({duration})')
     index = utils.read_int("Select a chapter", 1, len(chapters))
     chapter = chapters[index - 1]
     return chapter
```

### Comparing `twitch-dl-2.1.4/twitchdl/commands/info.py` & `twitch-dl-2.2.0/twitchdl/commands/info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,99 @@
+import click
 import m3u8
 
-from twitchdl import utils, twitch
+from twitchdl import twitch, utils
+from twitchdl.commands.download import get_video_placeholders
 from twitchdl.exceptions import ConsoleError
-from twitchdl.output import print_video, print_clip, print_json, print_out, print_log
+from twitchdl.output import bold, print_clip, print_json, print_log, print_table, print_video
+from twitchdl.twitch import Chapter, Clip, Video
 
 
-def info(args):
-    video_id = utils.parse_video_identifier(args.video)
+def info(id: str, *, json: bool = False):
+    video_id = utils.parse_video_identifier(id)
     if video_id:
         print_log("Fetching video...")
         video = twitch.get_video(video_id)
 
         if not video:
-            raise ConsoleError("Video {} not found".format(video_id))
+            raise ConsoleError(f"Video {video_id} not found")
 
         print_log("Fetching access token...")
         access_token = twitch.get_access_token(video_id)
 
         print_log("Fetching playlists...")
         playlists = twitch.get_playlists(video_id, access_token)
 
         print_log("Fetching chapters...")
         chapters = twitch.get_video_chapters(video_id)
 
-        if args.json:
+        if json:
             video_json(video, playlists, chapters)
         else:
             video_info(video, playlists, chapters)
         return
 
-    clip_slug = utils.parse_clip_identifier(args.video)
+    clip_slug = utils.parse_clip_identifier(id)
     if clip_slug:
         print_log("Fetching clip...")
         clip = twitch.get_clip(clip_slug)
         if not clip:
-            raise ConsoleError("Clip {} not found".format(clip_slug))
+            raise ConsoleError(f"Clip {clip_slug} not found")
 
-        if args.json:
+        if json:
             print_json(clip)
         else:
             clip_info(clip)
         return
 
-    raise ConsoleError("Invalid input: {}".format(args.video))
+    raise ConsoleError(f"Invalid input: {id}")
 
 
-def video_info(video, playlists, chapters):
-    print_out()
+def video_info(video: Video, playlists, chapters: list[Chapter]):
+    click.echo()
     print_video(video)
 
-    print_out()
-    print_out("Playlists:")
+    click.echo("Playlists:")
     for p in m3u8.loads(playlists).playlists:
-        print_out("<b>{}</b> {}".format(p.stream_info.video, p.uri))
+        click.echo(f"{bold(p.stream_info.video)} {p.uri}")
 
     if chapters:
-        print_out()
-        print_out("Chapters:")
+        click.echo()
+        click.echo("Chapters:")
         for chapter in chapters:
             start = utils.format_time(chapter["positionMilliseconds"] // 1000, force_hours=True)
             duration = utils.format_time(chapter["durationMilliseconds"] // 1000)
-            print_out(f'{start} <b>{chapter["description"]}</b> ({duration})')
+            click.echo(f'{start} {bold(chapter["description"])} ({duration})')
+
+    placeholders = get_video_placeholders(video, format="mkv")
+    placeholders = [[f"{{{k}}}", v] for k, v in placeholders.items()]
+    click.echo("")
+    print_table(["Placeholder", "Value"], placeholders)
 
 
 def video_json(video, playlists, chapters):
     playlists = m3u8.loads(playlists).playlists
 
     video["playlists"] = [
         {
             "bandwidth": p.stream_info.bandwidth,
             "resolution": p.stream_info.resolution,
             "codecs": p.stream_info.codecs,
             "video": p.stream_info.video,
-            "uri": p.uri
-        } for p in playlists
+            "uri": p.uri,
+        }
+        for p in playlists
     ]
 
     video["chapters"] = chapters
 
     print_json(video)
 
 
-def clip_info(clip):
-    print_out()
+def clip_info(clip: Clip):
+    click.echo()
     print_clip(clip)
-    print_out()
-    print_out("Download links:")
+    click.echo()
+    click.echo("Download links:")
 
     for q in clip["videoQualities"]:
-        print_out("<b>{quality}p{frameRate}</b> {sourceURL}".format(**q))
+        click.echo(f"{bold(q['quality'])} [{q['frameRate']} fps] {q['sourceURL']}")
```

### Comparing `twitch-dl-2.1.4/twitchdl/download.py` & `twitch-dl-2.2.0/twitchdl/download.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import os
 import httpx
 
+from twitchdl.exceptions import ConsoleError
+
 CHUNK_SIZE = 1024
 CONNECT_TIMEOUT = 5
 RETRY_COUNT = 5
 
 
-class DownloadFailed(Exception):
-    pass
-
-
 def _download(url: str, path: str):
     tmp_path = path + ".tmp"
     size = 0
     with httpx.stream("GET", url, timeout=CONNECT_TIMEOUT) as response:
         with open(tmp_path, "wb") as target:
             for chunk in response.iter_bytes(chunk_size=CHUNK_SIZE):
                 target.write(chunk)
@@ -31,8 +29,8 @@
     from_disk = False
     for _ in range(retries):
         try:
             return (_download(url, path), from_disk)
         except httpx.RequestError:
             pass
 
-    raise DownloadFailed(":(")
+    raise ConsoleError(f"Failed downloading after {retries} attempts: {url}")
```

### Comparing `twitch-dl-2.1.4/twitchdl/http.py` & `twitch-dl-2.2.0/twitchdl/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
-import httpx
 import logging
 import os
 import time
+from abc import ABC, abstractmethod
+from typing import List, Optional
 
-from typing import List, Optional, Union
+import httpx
 
 from twitchdl.progress import Progress
 
 logger = logging.getLogger(__name__)
 
 KB = 1024
 
@@ -21,15 +22,21 @@
 TIMEOUT = 30
 """
 Number of seconds to wait before aborting when there is no network activity.
 https://www.python-httpx.org/advanced/#timeout-configuration
 """
 
 
-class TokenBucket:
+class TokenBucket(ABC):
+    @abstractmethod
+    def advance(self, size: int):
+        pass
+
+
+class LimitingTokenBucket(TokenBucket):
     """Limit the download speed by strategically inserting sleeps."""
 
     def __init__(self, rate: int, capacity: Optional[int] = None):
         self.rate: int = rate
         self.capacity: int = capacity or rate * 2
         self.available: int = 0
         self.last_refilled: float = time.time()
@@ -49,30 +56,28 @@
         now = time.time()
         elapsed = now - self.last_refilled
         refill_amount = int(elapsed * self.rate)
         self.available = min(self.available + refill_amount, self.capacity)
         self.last_refilled = now
 
 
-class EndlessTokenBucket:
+class EndlessTokenBucket(TokenBucket):
     """Used when download speed is not limited."""
+
     def advance(self, size: int):
         pass
 
 
-AnyTokenBucket = Union[TokenBucket, EndlessTokenBucket]
-
-
 async def download(
     client: httpx.AsyncClient,
     task_id: int,
     source: str,
     target: str,
     progress: Progress,
-    token_bucket: AnyTokenBucket,
+    token_bucket: TokenBucket,
 ):
     # Download to a temp file first, then copy to target when over to avoid
     # getting saving chunks which may persist if canceled or --keep is used
     tmp_target = f"{target}.tmp"
     with open(tmp_target, "wb") as f:
         async with client.stream("GET", source) as response:
             size = int(response.headers.get("content-length"))
@@ -89,15 +94,15 @@
 async def download_with_retries(
     client: httpx.AsyncClient,
     semaphore: asyncio.Semaphore,
     task_id: int,
     source: str,
     target: str,
     progress: Progress,
-    token_bucket: AnyTokenBucket,
+    token_bucket: TokenBucket,
 ):
     async with semaphore:
         if os.path.exists(target):
             size = os.path.getsize(target)
             progress.already_downloaded(task_id, size)
             return
 
@@ -114,16 +119,26 @@
 
 
 async def download_all(
     sources: List[str],
     targets: List[str],
     workers: int,
     *,
-    rate_limit: Optional[int] = None
+    rate_limit: Optional[int] = None,
 ):
     progress = Progress(len(sources))
-    token_bucket = TokenBucket(rate_limit) if rate_limit else EndlessTokenBucket()
+    token_bucket = LimitingTokenBucket(rate_limit) if rate_limit else EndlessTokenBucket()
     async with httpx.AsyncClient(timeout=TIMEOUT) as client:
         semaphore = asyncio.Semaphore(workers)
-        tasks = [download_with_retries(client, semaphore, task_id, source, target, progress, token_bucket)
-                 for task_id, (source, target) in enumerate(zip(sources, targets))]
+        tasks = [
+            download_with_retries(
+                client,
+                semaphore,
+                task_id,
+                source,
+                target,
+                progress,
+                token_bucket,
+            )
+            for task_id, (source, target) in enumerate(zip(sources, targets))
+        ]
         await asyncio.gather(*tasks)
```

### Comparing `twitch-dl-2.1.4/twitchdl/progress.py` & `twitch-dl-2.2.0/twitchdl/progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import logging
 import time
-
 from collections import deque
 from dataclasses import dataclass, field
 from statistics import mean
-from typing import Dict, NamedTuple, Optional, Deque
+from typing import Deque, Dict, NamedTuple, Optional
+
+import click
 
-from twitchdl.output import print_out
+from twitchdl.output import blue
 from twitchdl.utils import format_size, format_time
 
 logger = logging.getLogger(__name__)
 
 
 TaskId = int
 
 
 @dataclass
 class Task:
     id: TaskId
     size: int
     downloaded: int = 0
 
-    def advance(self, size):
+    def advance(self, size: int):
         self.downloaded += size
 
 
 class Sample(NamedTuple):
     downloaded: int
     timestamp: float
 
@@ -89,26 +90,36 @@
 
     def end(self, task_id: int):
         if task_id not in self.tasks:
             raise ValueError(f"Task {task_id}: cannot end, not started")
 
         task = self.tasks[task_id]
         if task.size != task.downloaded:
-            logger.warn(f"Taks {task_id} ended with {task.downloaded}b downloaded, expected {task.size}b.")
+            logger.warn(
+                f"Taks {task_id} ended with {task.downloaded}b downloaded, expected {task.size}b."
+            )
 
         self.vod_downloaded_count += 1
         self.print()
 
     def _calculate_total(self):
-        self.estimated_total = int(mean(t.size for t in self.tasks.values()) * self.vod_count) if self.tasks else None
+        self.estimated_total = (
+            int(mean(t.size for t in self.tasks.values()) * self.vod_count) if self.tasks else None
+        )
 
     def _calculate_progress(self):
         self.speed = self._calculate_speed()
-        self.progress_perc = int(100 * self.progress_bytes / self.estimated_total) if self.estimated_total else 0
-        self.remaining_time = int((self.estimated_total - self.progress_bytes) / self.speed) if self.estimated_total and self.speed else None
+        self.progress_perc = (
+            int(100 * self.progress_bytes / self.estimated_total) if self.estimated_total else 0
+        )
+        self.remaining_time = (
+            int((self.estimated_total - self.progress_bytes) / self.speed)
+            if self.estimated_total and self.speed
+            else None
+        )
 
     def _calculate_speed(self):
         if len(self.samples) < 2:
             return None
 
         first_sample = self.samples[0]
         last_sample = self.samples[-1]
@@ -121,17 +132,21 @@
     def print(self):
         now = time.time()
 
         # Don't print more often than 10 times per second
         if now - self.last_printed < 0.1:
             return
 
-        progress = " ".join([
-            f"Downloaded {self.vod_downloaded_count}/{self.vod_count} VODs",
-            f"<blue>{self.progress_perc}%</blue>",
-            f"of <blue>~{format_size(self.estimated_total)}</blue>" if self.estimated_total else "",
-            f"at <blue>{format_size(self.speed)}/s</blue>" if self.speed else "",
-            f"ETA <blue>{format_time(self.remaining_time)}</blue>" if self.remaining_time is not None else "",
-        ])
+        progress = " ".join(
+            [
+                f"Downloaded {self.vod_downloaded_count}/{self.vod_count} VODs",
+                f"{blue(self.progress_perc)}%",
+                f"of ~{blue(format_size(self.estimated_total))}" if self.estimated_total else "",
+                f"at {blue(format_size(self.speed))}/s" if self.speed else "",
+                f"ETA {blue(format_time(self.remaining_time))}"
+                if self.remaining_time is not None
+                else "",
+            ]
+        )
 
-        print_out(f"\r{progress}     ", end="")
+        click.echo(f"\r{progress}     ", nl=False)
         self.last_printed = now
```

### Comparing `twitch-dl-2.1.4/twitchdl/twitch.py` & `twitch-dl-2.2.0/twitchdl/twitch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,139 @@
 """
 Twitch API access.
 """
 
-import httpx
 import json
+from typing import Dict, Generator, Literal, TypedDict
+
+import click
+import httpx
 
-from typing import Dict
 from twitchdl import CLIENT_ID
+from twitchdl.entities import Data
 from twitchdl.exceptions import ConsoleError
 
-
-class GQLError(Exception):
-    def __init__(self, errors):
-        super().__init__("GraphQL query failed")
-        self.errors = errors
+ClipsPeriod = Literal["last_day", "last_week", "last_month", "all_time"]
+VideosSort = Literal["views", "time"]
+VideosType = Literal["archive", "highlight", "upload"]
+
+
+class AccessToken(TypedDict):
+    signature: str
+    value: str
+
+
+class User(TypedDict):
+    login: str
+    displayName: str
+
+
+class Game(TypedDict):
+    id: str
+    name: str
+
+
+class VideoQuality(TypedDict):
+    frameRate: str
+    quality: str
+    sourceURL: str
+
+
+class ClipAccessToken(TypedDict):
+    id: str
+    playbackAccessToken: AccessToken
+    videoQualities: list[VideoQuality]
+
+
+class Clip(TypedDict):
+    id: str
+    slug: str
+    title: str
+    createdAt: str
+    viewCount: int
+    durationSeconds: int
+    url: str
+    videoQualities: list[VideoQuality]
+    game: Game
+    broadcaster: User
+
+
+class Video(TypedDict):
+    id: str
+    title: str
+    description: str
+    publishedAt: str
+    broadcastType: str
+    lengthSeconds: int
+    game: Game
+    creator: User
+
+
+class Chapter(TypedDict):
+    id: str
+    durationMilliseconds: int
+    positionMilliseconds: int
+    type: str
+    description: str
+    subDescription: str
+    thumbnailURL: str
+    game: Game
+
+
+class GQLError(click.ClickException):
+    def __init__(self, errors: list[str]):
+        message = "GraphQL query failed."
+        for error in errors:
+            message += f"\n* {error}"
+        super().__init__(message)
 
 
 def authenticated_post(url, data=None, json=None, headers={}):
-    headers['Client-ID'] = CLIENT_ID
+    headers["Client-ID"] = CLIENT_ID
 
     response = httpx.post(url, data=data, json=json, headers=headers)
     if response.status_code == 400:
         data = response.json()
         raise ConsoleError(data["message"])
 
     response.raise_for_status()
 
     return response
 
 
-def gql_post(query):
+def gql_post(query: str):
     url = "https://gql.twitch.tv/gql"
-    response = authenticated_post(url, data=query).json()
-
-    if "errors" in response:
-        raise GQLError(response["errors"])
-
-    return response
+    response = authenticated_post(url, data=query)
+    gql_raise_on_error(response)
+    return response.json()
 
 
 def gql_query(query: str, headers: Dict[str, str] = {}):
     url = "https://gql.twitch.tv/gql"
-    response = authenticated_post(url, json={"query": query}, headers=headers).json()
+    response = authenticated_post(url, json={"query": query}, headers=headers)
+    gql_raise_on_error(response)
+    return response.json()
 
-    if "errors" in response:
-        raise GQLError(response["errors"])
 
-    return response
+def gql_raise_on_error(response: httpx.Response):
+    data = response.json()
+    if "errors" in data:
+        errors = [e["message"] for e in data["errors"]]
+        raise GQLError(errors)
 
 
 VIDEO_FIELDS = """
     id
     title
+    description
     publishedAt
     broadcastType
     lengthSeconds
     game {
+        id
         name
     }
     creator {
         login
         displayName
     }
 """
@@ -85,109 +159,103 @@
     broadcaster {
         displayName
         login
     }
 """
 
 
-def get_video(video_id):
-    query = """
+def get_video(video_id: str) -> Video | None:
+    query = f"""
     {{
         video(id: "{video_id}") {{
-            {fields}
+            {VIDEO_FIELDS}
         }}
     }}
     """
 
-    query = query.format(video_id=video_id, fields=VIDEO_FIELDS)
-
     response = gql_query(query)
     return response["data"]["video"]
 
 
-def get_clip(slug):
-    query = """
+def get_clip(slug: str) -> Clip | None:
+    query = f"""
     {{
-        clip(slug: "{}") {{
-            {fields}
+        clip(slug: "{slug}") {{
+            {CLIP_FIELDS}
         }}
     }}
     """
 
-    response = gql_query(query.format(slug, fields=CLIP_FIELDS))
+    response = gql_query(query)
     return response["data"]["clip"]
 
 
-def get_clip_access_token(slug):
-    query = """
+def get_clip_access_token(slug: str) -> ClipAccessToken:
+    query = f"""
     {{
         "operationName": "VideoAccessToken_Clip",
         "variables": {{
             "slug": "{slug}"
         }},
         "extensions": {{
             "persistedQuery": {{
                 "version": 1,
                 "sha256Hash": "36b89d2507fce29e5ca551df756d27c1cfe079e2609642b4390aa4c35796eb11"
             }}
         }}
     }}
     """
 
-    response = gql_post(query.format(slug=slug).strip())
+    response = gql_post(query.strip())
     return response["data"]["clip"]
 
 
-def get_channel_clips(channel_id, period, limit, after=None):
+def get_channel_clips(channel_id: str, period: ClipsPeriod, limit: int, after: str | None = None):
     """
     List channel clips.
 
     At the time of writing this:
     * filtering by game name returns an error
     * sorting by anything but VIEWS_DESC or TRENDING returns an error
     * sorting by VIEWS_DESC and TRENDING returns the same results
     * there is no totalCount
     """
-    query = """
+    query = f"""
     {{
       user(login: "{channel_id}") {{
-        clips(first: {limit}, after: "{after}", criteria: {{ period: {period}, sort: VIEWS_DESC }}) {{
+        clips(first: {limit}, after: "{after or ''}", criteria: {{ period: {period.upper()}, sort: VIEWS_DESC }}) {{
           pageInfo {{
             hasNextPage
             hasPreviousPage
           }}
           edges {{
             cursor
             node {{
-              {fields}
+              {CLIP_FIELDS}
             }}
           }}
         }}
       }}
     }}
     """
 
-    query = query.format(
-        channel_id=channel_id,
-        after=after if after else "",
-        limit=limit,
-        period=period.upper(),
-        fields=CLIP_FIELDS
-    )
-
     response = gql_query(query)
     user = response["data"]["user"]
     if not user:
-        raise ConsoleError("Channel {} not found".format(channel_id))
+        raise ConsoleError(f"Channel {channel_id} not found")
 
     return response["data"]["user"]["clips"]
 
 
-def channel_clips_generator(channel_id, period, limit):
-    def _generator(clips, limit):
+def channel_clips_generator(
+    channel_id: str,
+    period: ClipsPeriod,
+    limit: int,
+) -> Generator[Clip, None, None]:
+    def _generator(clips: Data, limit: int) -> Generator[Clip, None, None]:
         for clip in clips["edges"]:
             if limit < 1:
                 return
             yield clip["node"]
             limit -= 1
 
         has_next = clips["pageInfo"]["hasNextPage"]
@@ -200,80 +268,86 @@
         yield from _generator(clips, limit)
 
     req_limit = min(limit, 100)
     clips = get_channel_clips(channel_id, period, req_limit)
     return _generator(clips, limit)
 
 
-def channel_clips_generator_old(channel_id, period, limit):
+def channel_clips_generator_old(channel_id: str, period: ClipsPeriod, limit: int):
     cursor = ""
     while True:
-        clips = get_channel_clips(
-            channel_id, period, limit, after=cursor)
+        clips = get_channel_clips(channel_id, period, limit, after=cursor)
 
         if not clips["edges"]:
             break
 
         has_next = clips["pageInfo"]["hasNextPage"]
         cursor = clips["edges"][-1]["cursor"] if has_next else None
 
         yield clips, has_next
 
         if not cursor:
             break
 
 
-def get_channel_videos(channel_id, limit, sort, type="archive", game_ids=[], after=None):
-    query = """
+def get_channel_videos(
+    channel_id: str,
+    limit: int,
+    sort: str,
+    type: str = "archive",
+    game_ids: list[str] | None = None,
+    after: str | None = None,
+):
+    game_ids = game_ids or []
+
+    query = f"""
     {{
         user(login: "{channel_id}") {{
             videos(
                 first: {limit},
-                type: {type},
-                sort: {sort},
-                after: "{after}",
+                type: {type.upper()},
+                sort: {sort.upper()},
+                after: "{after or ''}",
                 options: {{
                     gameIDs: {game_ids}
                 }}
             ) {{
                 totalCount
                 pageInfo {{
                     hasNextPage
                 }}
                 edges {{
                     cursor
                     node {{
-                        {fields}
+                        {VIDEO_FIELDS}
                     }}
                 }}
             }}
         }}
     }}
     """
 
-    query = query.format(
-        channel_id=channel_id,
-        game_ids=game_ids,
-        after=after if after else "",
-        limit=limit,
-        sort=sort.upper(),
-        type=type.upper(),
-        fields=VIDEO_FIELDS
-    )
-
     response = gql_query(query)
 
     if not response["data"]["user"]:
-        raise ConsoleError("Channel {} not found".format(channel_id))
+        raise ConsoleError(f"Channel {channel_id} not found")
 
     return response["data"]["user"]["videos"]
 
 
-def channel_videos_generator(channel_id, max_videos, sort, type, game_ids=[]):
-    def _generator(videos, max_videos):
+def channel_videos_generator(
+    channel_id: str,
+    max_videos: int,
+    sort: VideosSort,
+    type: VideosType,
+    game_ids: list[str] | None = None,
+) -> tuple[int, Generator[Video, None, None]]:
+    game_ids = game_ids or []
+
+    def _generator(videos: Data, max_videos: int) -> Generator[Video, None, None]:
         for video in videos["edges"]:
             if max_videos < 1:
                 return
             yield video["node"]
             max_videos -= 1
 
         has_next = videos["pageInfo"]["hasNextPage"]
@@ -286,16 +360,16 @@
         yield from _generator(videos, max_videos)
 
     limit = min(max_videos, 100)
     videos = get_channel_videos(channel_id, limit, sort, type, game_ids)
     return videos["totalCount"], _generator(videos, max_videos)
 
 
-def get_access_token(video_id, auth_token=None):
-    query = """
+def get_access_token(video_id: str, auth_token: str | None = None) -> AccessToken:
+    query = f"""
     {{
         videoPlaybackAccessToken(
             id: {video_id},
             params: {{
                 platform: "web",
                 playerBackend: "mediaplayer",
                 playerType: "site"
@@ -303,19 +377,17 @@
         ) {{
             signature
             value
         }}
     }}
     """
 
-    query = query.format(video_id=video_id)
-
-    headers = {}
+    headers: dict[str, str] = {}
     if auth_token is not None:
-        headers['authorization'] = f'OAuth {auth_token}'
+        headers["authorization"] = f"OAuth {auth_token}"
 
     try:
         response = gql_query(query, headers=headers)
         return response["data"]["videoPlaybackAccessToken"]
     except httpx.HTTPStatusError as error:
         # Provide a more useful error message when server returns HTTP 401
         # Unauthorized while using a user-provided auth token.
@@ -327,66 +399,68 @@
                     "Unauthorized. This video may be subscriber-only. See docs:\n"
                     "https://twitch-dl.bezdomni.net/commands/download.html#downloading-subscriber-only-vods"
                 )
 
         raise
 
 
-def get_playlists(video_id, access_token):
+def get_playlists(video_id: str, access_token: AccessToken) -> str:
     """
     For a given video return a playlist which contains possible video qualities.
     """
-    url = "https://usher.ttvnw.net/vod/{}".format(video_id)
+    url = f"https://usher.ttvnw.net/vod/{video_id}"
 
-    response = httpx.get(url, params={
-        "nauth": access_token['value'],
-        "nauthsig": access_token['signature'],
-        "allow_audio_only": "true",
-        "allow_source": "true",
-        "player": "twitchweb",
-    })
+    response = httpx.get(
+        url,
+        params={
+            "nauth": access_token["value"],
+            "nauthsig": access_token["signature"],
+            "allow_audio_only": "true",
+            "allow_source": "true",
+            "player": "twitchweb",
+        },
+    )
     response.raise_for_status()
-    return response.content.decode('utf-8')
+    return response.content.decode("utf-8")
 
 
-def get_game_id(name):
-    query = """
+def get_game_id(name: str):
+    query = f"""
     {{
-        game(name: "{}") {{
+        game(name: "{name.strip()}") {{
             id
         }}
     }}
     """
 
-    response = gql_query(query.format(name.strip()))
+    response = gql_query(query)
     game = response["data"]["game"]
     if game:
         return game["id"]
 
 
-def get_video_chapters(video_id):
+def get_video_chapters(video_id: str) -> list[Chapter]:
     query = {
         "operationName": "VideoPlayer_ChapterSelectButtonVideo",
-        "variables":
-        {
+        "variables": {
             "includePrivate": False,
-            "videoID": video_id
+            "videoID": video_id,
         },
-        "extensions":
-        {
-            "persistedQuery":
-            {
+        "extensions": {
+            "persistedQuery": {
                 "version": 1,
-                "sha256Hash": "8d2793384aac3773beab5e59bd5d6f585aedb923d292800119e03d40cd0f9b41"
+                "sha256Hash": "8d2793384aac3773beab5e59bd5d6f585aedb923d292800119e03d40cd0f9b41",
             }
-        }
+        },
     }
 
     response = gql_post(json.dumps(query))
     return list(_chapter_nodes(response["data"]["video"]["moments"]))
 
 
-def _chapter_nodes(collection):
-    for edge in collection["edges"]:
+def _chapter_nodes(moments: Data) -> Generator[Chapter, None, None]:
+    for edge in moments["edges"]:
         node = edge["node"]
+        node["game"] = node["details"]["game"]
+        del node["details"]
         del node["moments"]
         yield node
```

### Comparing `twitch-dl-2.1.4/twitchdl/utils.py` & `twitch-dl-2.2.0/twitchdl/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,87 @@
 import re
 import unicodedata
 
+import click
 
-def _format_size(value, digits, unit):
+
+def _format_size(value: float, digits: int, unit: str):
     if digits > 0:
-        return "{{:.{}f}}{}".format(digits, unit).format(value)
+        return f"{{:.{digits}f}}{unit}".format(value)
     else:
-        return "{{:d}}{}".format(unit).format(value)
+        return f"{int(value)}{unit}"
 
 
-def format_size(bytes_, digits=1):
+def format_size(bytes_: int | float, digits: int = 1):
     if bytes_ < 1024:
         return _format_size(bytes_, digits, "B")
 
     kilo = bytes_ / 1024
     if kilo < 1024:
         return _format_size(kilo, digits, "kB")
 
     mega = kilo / 1024
     if mega < 1024:
         return _format_size(mega, digits, "MB")
 
     return _format_size(mega / 1024, digits, "GB")
 
 
-def format_duration(total_seconds):
+def format_duration(total_seconds: int | float) -> str:
     total_seconds = int(total_seconds)
     hours = total_seconds // 3600
     remainder = total_seconds % 3600
     minutes = remainder // 60
     seconds = total_seconds % 60
 
     if hours:
-        return "{} h {} min".format(hours, minutes)
+        return f"{hours} h {minutes} min"
 
     if minutes:
-        return "{} min {} sec".format(minutes, seconds)
+        return f"{minutes} min {seconds} sec"
 
-    return "{} sec".format(seconds)
+    return f"{seconds} sec"
 
 
-def format_time(total_seconds, force_hours=False):
+def format_time(total_seconds: int | float, force_hours: bool = False) -> str:
     total_seconds = int(total_seconds)
     hours = total_seconds // 3600
     remainder = total_seconds % 3600
     minutes = remainder // 60
     seconds = total_seconds % 60
 
     if hours or force_hours:
         return f"{hours:02}:{minutes:02}:{seconds:02}"
 
     return f"{minutes:02}:{seconds:02}"
 
 
-def read_int(msg, min, max, default=None):
-    if default:
-        msg = msg + f" [default {default}]"
-
-    msg += ": "
-
+def read_int(msg: str, min: int, max: int, default: int | None = None) -> int:
     while True:
         try:
-            val = input(msg)
+            val = click.prompt(msg, default=default, type=int)
             if default and not val:
                 return default
             if min <= int(val) <= max:
                 return int(val)
         except ValueError:
             pass
 
 
-def slugify(value):
-    value = unicodedata.normalize('NFKC', str(value))
-    value = re.sub(r'[^\w\s_-]', '', value)
-    value = re.sub(r'[\s_-]+', '_', value)
+def slugify(value: str) -> str:
+    value = unicodedata.normalize("NFKC", str(value))
+    value = re.sub(r"[^\w\s_-]", "", value)
+    value = re.sub(r"[\s_-]+", "_", value)
     return value.strip("_").lower()
 
 
-def titlify(value):
-    value = unicodedata.normalize('NFKC', str(value))
-    value = re.sub(r'[^\w\s\[\]().-]', '', value)
-    value = re.sub(r'\s+', ' ', value)
+def titlify(value: str) -> str:
+    value = unicodedata.normalize("NFKC", str(value))
+    value = re.sub(r"[^\w\s\[\]().-]", "", value)
+    value = re.sub(r"\s+", " ", value)
     return value.strip()
 
 
 VIDEO_PATTERNS = [
     r"^(?P<id>\d+)?$",
     r"^https://(www.)?twitch.tv/videos/(?P<id>\d+)(\?.+)?$",
 ]
@@ -92,21 +89,21 @@
 CLIP_PATTERNS = [
     r"^(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)$",
     r"^https://(www.)?twitch.tv/\w+/clip/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
     r"^https://clips.twitch.tv/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
 ]
 
 
-def parse_video_identifier(identifier):
+def parse_video_identifier(identifier: str) -> str | None:
     """Given a video ID or URL returns the video ID, or null if not matched"""
     for pattern in VIDEO_PATTERNS:
         match = re.match(pattern, identifier)
         if match:
             return match.group("id")
 
 
-def parse_clip_identifier(identifier):
+def parse_clip_identifier(identifier: str) -> str | None:
     """Given a clip slug or URL returns the clip slug, or null if not matched"""
     for pattern in CLIP_PATTERNS:
         match = re.match(pattern, identifier)
         if match:
             return match.group("slug")
```

