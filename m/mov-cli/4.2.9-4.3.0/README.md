# Comparing `tmp/mov-cli-4.2.9.tar.gz` & `tmp/mov-cli-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-4.2.9.tar", last modified: Wed Apr  3 20:55:36 2024, max compression
+gzip compressed data, was "mov-cli-4.3.0.tar", last modified: Tue Apr  9 23:40:37 2024, max compression
```

## Comparing `mov-cli-4.2.9.tar` & `mov-cli-4.3.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.737147 mov-cli-4.2.9/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.727147 mov-cli-4.2.9/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.727147 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/addprovider.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.727147 mov-cli-4.2.9/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov-cli-4.2.9/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov-cli-4.2.9/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      291 2024-03-23 15:35:14.000000 mov-cli-4.2.9/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7269 2024-04-03 20:55:36.737147 mov-cli-4.2.9/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4612 2024-03-25 22:44:43.000000 mov-cli-4.2.9/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1841 2024-03-13 15:29:53.000000 mov-cli-4.2.9/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.730480 mov-cli-4.2.9/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-03 20:28:42.000000 mov-cli-4.2.9/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.730480 mov-cli-4.2.9/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4860 2024-03-26 01:19:10.000000 mov-cli-4.2.9/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      457 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2150 2024-04-03 20:45:12.000000 mov-cli-4.2.9/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2101 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2927 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4201 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1276 2024-03-26 17:57:30.000000 mov-cli-4.2.9/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3460 2024-03-27 21:54:10.000000 mov-cli-4.2.9/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3417 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/cli/utils.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1357 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6551 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      514 2024-03-16 14:22:02.000000 mov-cli-4.2.9/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1038 2024-03-24 17:18:21.000000 mov-cli-4.2.9/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      942 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-03 20:53:58.000000 mov-cli-4.2.9/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov-cli-4.2.9/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-03-27 21:58:28.000000 mov-cli-4.2.9/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2259 2024-03-27 22:06:47.000000 mov-cli-4.2.9/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1724 2024-03-21 11:42:05.000000 mov-cli-4.2.9/mov_cli/media/metadata.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       89 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2147 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2072 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1086 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1849 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov-cli-4.2.9/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       90 2024-03-04 00:54:59.000000 mov-cli-4.2.9/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      940 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/utils/scraper/fuzzy.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5533 2024-03-22 14:36:19.000000 mov-cli-4.2.9/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      312 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7269 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1435 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      218 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1736 2024-03-30 22:00:17.000000 mov-cli-4.2.9/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-03-25 22:44:50.000000 mov-cli-4.2.9/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov-cli-4.2.9/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-03 20:55:36.737147 mov-cli-4.2.9/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.269852 mov-cli-4.3.0/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.269852 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/addprovider.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.269852 mov-cli-4.3.0/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov-cli-4.3.0/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov-cli-4.3.0/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      291 2024-04-04 00:43:21.000000 mov-cli-4.3.0/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7713 2024-04-09 23:40:37.279852 mov-cli-4.3.0/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5059 2024-04-08 23:54:10.000000 mov-cli-4.3.0/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-08 22:18:54.000000 mov-cli-4.3.0/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.273186 mov-cli-4.3.0/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-08 22:17:33.000000 mov-cli-4.3.0/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5589 2024-04-09 23:28:23.000000 mov-cli-4.3.0/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2938 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1926 2024-04-09 23:06:10.000000 mov-cli-4.3.0/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4079 2024-04-09 22:27:43.000000 mov-cli-4.3.0/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1248 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6423 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6913 2024-04-08 23:54:12.000000 mov-cli-4.3.0/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      583 2024-04-08 23:54:12.000000 mov-cli-4.3.0/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      942 2024-04-04 00:48:22.000000 mov-cli-4.3.0/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov-cli-4.3.0/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2158 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-09 23:14:07.000000 mov-cli-4.3.0/mov_cli/media/metadata.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       89 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2556 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2319 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-08 23:54:12.000000 mov-cli-4.3.0/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-09 22:52:58.000000 mov-cli-4.3.0/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov-cli-4.3.0/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-09 22:26:17.000000 mov-cli-4.3.0/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7713 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1406 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1733 2024-04-08 23:54:10.000000 mov-cli-4.3.0/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov-cli-4.3.0/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov-cli-4.3.0/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-09 23:40:37.279852 mov-cli-4.3.0/setup.cfg
```

### Comparing `mov-cli-4.2.9/.github/ISSUE_TEMPLATE/bug-report.md` & `mov-cli-4.3.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/.github/workflows/pypi.yml` & `mov-cli-4.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/.github/workflows/ruff.yml` & `mov-cli-4.3.0/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/LICENSE` & `mov-cli-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/PKG-INFO` & `mov-cli-4.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.2.9
+Version: 4.3.0
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,105 +40,111 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: toml
 Requires-Dist: devgoldyutils>=2.5.7
-Requires-Dist: typer[all]==0.10.0
+Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer
 Requires-Dist: beautifulsoup4
 Requires-Dist: Unidecode
-Requires-Dist: thefuzz
 Requires-Dist: deprecation
+Requires-Dist: packaging
 Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
 
 [![Stargazers][stars-shield]][stars-url]
 [![Pypi Version][pypi-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-url]
 [![Python Versions][python-shield]][pypi-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
-[![Discord][discord-shield]][discord-url]
+
 
 <div align="center">
 
   <a href="https://github.com/mov-cli/mov-cli">
     <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
   </a>
 
   <sub>Watch everything from your terminal.</sub>
   <br>
   <br>
   <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
   ·
   <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
 
-</div>
+  <br>
+  <br>
+  <a href="https://discord.gg/BMzC7ePsBV">
+    <img src="https://invidget.switchblade.xyz/BMzC7ePsBV" alt="Logo" width="400">
+  </a>
 
+</div>
 <br>
 
 > [!Note]
-> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
+> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also I would advise not using it as a library yet as the API still has many breaking changes.
 
 ## Installation 🛠️
 
 > [!TIP]
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
 - **A supported platform:**
   - Linux
   - Windows
   - Android (via [Termux](https://termux.dev/en/))
   - iOS (via [iSH Shell](https://ish.app/))
-  - *MacOS* (**Not tested**)
+  - MacOS
 - **[python](https://www.python.org/downloads/)** (**required**, with pip)
 - **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
 - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
 - **[mpv](https://mpv.io/installation/)** (recommended & default media player)
 
 To get running these are all the prerequisites you'll need.
 
 With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
 
 ```sh
 pip install mov-cli -U
 ```
+> Check out the [wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation) for more in-depth guidance on installing mov-cli.
 
 ## Usage 🖱️
 mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
 
 > [!NOTE]
 > You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
 > Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
 
 1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
 ```sh
 mov-cli -e
 ```
-Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
+Alternatively, you may also edit by manually opening the config file. See this [Wiki page](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.  
 ```toml
 [mov-cli.plugins]
-films = "package_name"
+youtube = "mov-cli-youtube"
 ```
 
-
-2. Scraper away!
+2. Scrape away!
 ```sh
-mov-cli -s films spider man no way home
+mov-cli -s youtube flight 370
 ```
-<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
+<img src="https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118">
 
-> The above command should search for `spider man no way home` with the following scraper.
+> The command above searches for `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-cli is plugin based and there are many of them [in the wild](https://github.com/topics/mov-cli-plugin). 😉**
 
 ## Contributing ✨
 Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
 
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
@@ -158,9 +164,8 @@
 [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/
 [python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
 [license-url]: ./LICENSE
-[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
-[discord-url]: https://discord.gg/BMzC7ePsBV
+[pypi-dl-shield]: https://img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.2.9 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.0 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -23,69 +23,74 @@
 Windows 10 Classifier: Operating System :: POSIX :: Linux Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
-toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer[all]==0.10.0
-Requires-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode
-Requires-Dist: thefuzz Requires-Dist: deprecation Requires-Dist: mov-cli-
-test>=1.1.0 Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-
-Dist: build; extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra
-== "dev" [![Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-
-shield]][pypi-url] [![Python Versions][python-shield]][pypi-url] [![Issues]
-[issues-shield]][issues-url] [![MIT License][license-shield]][license-url] [!
-[Discord][discord-shield]][discord-url]
+toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer>=0.12.2 Requires-
+Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode Requires-
+Dist: deprecation Requires-Dist: packaging Requires-Dist: mov-cli-test>=1.1.0
+Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build;
+extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
+[Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-url] [![Python Versions][python-
+shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
+[license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
-> [!Note] > v4 is constantly changing so be sure to keep the tool up to date
-and with that said I would advise not using it as a library yet. ##
-Installation ð ï¸ > [!TIP] > For in-depth installation instructions hit the
-[wiki](https://github.com/mov-cli/mov-cli/wiki/Installation). ### Prerequisites
-- **A supported platform:** - Linux - Windows - Android (via [Termux](https://
-termux.dev/en/)) - iOS (via [iSH Shell](https://ish.app/)) - *MacOS* (**Not
-tested**) - **[python](https://www.python.org/downloads/)** (**required**, with
-pip) - **[lxml](https://pypi.org/project/lxml/)** (optional, â¡ faster
-scraping) - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-
-file#installation)** (optional but **highly recommended**) - **[mpv](https://
-mpv.io/installation/)** (recommended & default media player) To get running
-these are all the prerequisites you'll need. With the prerequisites installed,
-mov-cli can be installed via the pip command on all platforms with Python
-version 3.8 or above. ```sh pip install mov-cli -U ``` ## Usage ð±ï¸ mov-cli
+                                    _[_L_o_g_o_]
+
+> [!Note] > v4 is constantly changing so be sure to **keep the tool and your
+plugins up to date**. Also I would advise not using it as a library yet as the
+API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
+depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
+cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
+Windows - Android (via [Termux](https://termux.dev/en/)) - iOS (via [iSH Shell]
+(https://ish.app/)) - MacOS - **[python](https://www.python.org/downloads/)**
+(**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
+(optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
+fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
+**[mpv](https://mpv.io/installation/)** (recommended & default media player) To
+get running these are all the prerequisites you'll need. With the prerequisites
+installed, mov-cli can be installed via the pip command on all platforms with
+Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
+[wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation)
+for more in-depth guidance on installing mov-cli. ## Usage ð±ï¸ mov-cli
 comes packaged with a CLI interface via the `mov-cli` command you can use in
 your respective terminal. > [!NOTE] > You may notice mov-cli doesn't ship with
 any scrapers (or previously known as providers) by default, this is because v4
 is plugin-based and scrapers are now part of plugins that must be chosen to be
 installed. > Find out how to do so at the [wiki](https://github.com/mov-cli/
 mov-cli/wiki#plugins). 1. Install the scraper plugin of your choice. Visit this
 [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so
 and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a
 list of **third-party** mov-cli plugins. ```sh mov-cli -e ``` Alternatively,
-you may also edit by manually opening the config file. See the [Wiki](https://
-github.com/mov-cli/mov-cli/wiki/Configuration#introduction). ```toml [mov-
-cli.plugins] films = "package_name" ``` 2. Scraper away! ```sh mov-cli -s films
-spider man no way home ``` [https://github.com/mov-cli/mov-cli/assets/66202304/
-86189cab-b246-405e-a266-6c624bee2d36]> The above command should search for
-`spider man no way home` with the following scraper. ## Contributing â¨ Pull
-requests are welcome and *appreciated*. For major changes, please open an issue
-first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-cli](https://
-github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/
-lobster) and [animdl](https://github.com/justfoolingaround/animdl)
-[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-
-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/mov-
-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
-mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/mov-
-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
+you may also edit by manually opening the config file. See this [Wiki page]
+(https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
+```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
+mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
+132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
+`flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
+plugin, **however once again mov-cli is plugin based and there are many of them
+[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Contributing
+â¨ Pull requests are welcome and *appreciated*. For major changes, please open
+an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
+cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
+justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
+animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
+cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
+cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
+forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
+mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/ [python-shield]: https://
 img.shields.io/pypi/pyversions/mov-cli?style=flat [issues-shield]: https://
 img.shields.io/github/issues/mov-cli/mov-cli?style=flat [issues-url]: https://
 github.com/mov-cli/mov-cli/issues [license-shield]: https://img.shields.io/
-github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [discord-
-shield]: https://img.shields.io/badge/Discord-
-7289da?logo=discord&logoColor=white [discord-url]: https://discord.gg/
-BMzC7ePsBV
+github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [pypi-dl-
+shield]: https://img.shields.io/pypi/dm/mov-
+cli?color=informational&label=pypi%20downloads
```

### Comparing `mov-cli-4.2.9/README.md` & `mov-cli-4.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,92 @@
 <a name="readme-top"></a>
 
 [![Stargazers][stars-shield]][stars-url]
 [![Pypi Version][pypi-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-url]
 [![Python Versions][python-shield]][pypi-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
-[![Discord][discord-shield]][discord-url]
+
 
 <div align="center">
 
   <a href="https://github.com/mov-cli/mov-cli">
     <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
   </a>
 
   <sub>Watch everything from your terminal.</sub>
   <br>
   <br>
   <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
   ·
   <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
 
-</div>
+  <br>
+  <br>
+  <a href="https://discord.gg/BMzC7ePsBV">
+    <img src="https://invidget.switchblade.xyz/BMzC7ePsBV" alt="Logo" width="400">
+  </a>
 
+</div>
 <br>
 
 > [!Note]
-> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
+> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also I would advise not using it as a library yet as the API still has many breaking changes.
 
 ## Installation 🛠️
 
 > [!TIP]
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
 - **A supported platform:**
   - Linux
   - Windows
   - Android (via [Termux](https://termux.dev/en/))
   - iOS (via [iSH Shell](https://ish.app/))
-  - *MacOS* (**Not tested**)
+  - MacOS
 - **[python](https://www.python.org/downloads/)** (**required**, with pip)
 - **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
 - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
 - **[mpv](https://mpv.io/installation/)** (recommended & default media player)
 
 To get running these are all the prerequisites you'll need.
 
 With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
 
 ```sh
 pip install mov-cli -U
 ```
+> Check out the [wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation) for more in-depth guidance on installing mov-cli.
 
 ## Usage 🖱️
 mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
 
 > [!NOTE]
 > You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
 > Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
 
 1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
 ```sh
 mov-cli -e
 ```
-Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
+Alternatively, you may also edit by manually opening the config file. See this [Wiki page](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.  
 ```toml
 [mov-cli.plugins]
-films = "package_name"
+youtube = "mov-cli-youtube"
 ```
 
-
-2. Scraper away!
+2. Scrape away!
 ```sh
-mov-cli -s films spider man no way home
+mov-cli -s youtube flight 370
 ```
-<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
+<img src="https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118">
 
-> The above command should search for `spider man no way home` with the following scraper.
+> The command above searches for `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-cli is plugin based and there are many of them [in the wild](https://github.com/topics/mov-cli-plugin). 😉**
 
 ## Contributing ✨
 Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
 
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
@@ -100,9 +106,8 @@
 [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/
 [python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
 [license-url]: ./LICENSE
-[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
-[discord-url]: https://discord.gg/BMzC7ePsBV
+[pypi-dl-shield]: https://img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

#### html2text {}

```diff
@@ -1,57 +1,62 @@
 [![Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-
-url] [![Python Versions][python-shield]][pypi-url] [![Issues][issues-shield]]
-[issues-url] [![MIT License][license-shield]][license-url] [![Discord][discord-
-shield]][discord-url]
+url] [![Pypi Downloads][pypi-dl-shield]][pypi-url] [![Python Versions][python-
+shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
+[license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
-> [!Note] > v4 is constantly changing so be sure to keep the tool up to date
-and with that said I would advise not using it as a library yet. ##
-Installation ð ï¸ > [!TIP] > For in-depth installation instructions hit the
-[wiki](https://github.com/mov-cli/mov-cli/wiki/Installation). ### Prerequisites
-- **A supported platform:** - Linux - Windows - Android (via [Termux](https://
-termux.dev/en/)) - iOS (via [iSH Shell](https://ish.app/)) - *MacOS* (**Not
-tested**) - **[python](https://www.python.org/downloads/)** (**required**, with
-pip) - **[lxml](https://pypi.org/project/lxml/)** (optional, â¡ faster
-scraping) - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-
-file#installation)** (optional but **highly recommended**) - **[mpv](https://
-mpv.io/installation/)** (recommended & default media player) To get running
-these are all the prerequisites you'll need. With the prerequisites installed,
-mov-cli can be installed via the pip command on all platforms with Python
-version 3.8 or above. ```sh pip install mov-cli -U ``` ## Usage ð±ï¸ mov-cli
+                                    _[_L_o_g_o_]
+
+> [!Note] > v4 is constantly changing so be sure to **keep the tool and your
+plugins up to date**. Also I would advise not using it as a library yet as the
+API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
+depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
+cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
+Windows - Android (via [Termux](https://termux.dev/en/)) - iOS (via [iSH Shell]
+(https://ish.app/)) - MacOS - **[python](https://www.python.org/downloads/)**
+(**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
+(optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
+fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
+**[mpv](https://mpv.io/installation/)** (recommended & default media player) To
+get running these are all the prerequisites you'll need. With the prerequisites
+installed, mov-cli can be installed via the pip command on all platforms with
+Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
+[wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation)
+for more in-depth guidance on installing mov-cli. ## Usage ð±ï¸ mov-cli
 comes packaged with a CLI interface via the `mov-cli` command you can use in
 your respective terminal. > [!NOTE] > You may notice mov-cli doesn't ship with
 any scrapers (or previously known as providers) by default, this is because v4
 is plugin-based and scrapers are now part of plugins that must be chosen to be
 installed. > Find out how to do so at the [wiki](https://github.com/mov-cli/
 mov-cli/wiki#plugins). 1. Install the scraper plugin of your choice. Visit this
 [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so
 and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a
 list of **third-party** mov-cli plugins. ```sh mov-cli -e ``` Alternatively,
-you may also edit by manually opening the config file. See the [Wiki](https://
-github.com/mov-cli/mov-cli/wiki/Configuration#introduction). ```toml [mov-
-cli.plugins] films = "package_name" ``` 2. Scraper away! ```sh mov-cli -s films
-spider man no way home ``` [https://github.com/mov-cli/mov-cli/assets/66202304/
-86189cab-b246-405e-a266-6c624bee2d36]> The above command should search for
-`spider man no way home` with the following scraper. ## Contributing â¨ Pull
-requests are welcome and *appreciated*. For major changes, please open an issue
-first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-cli](https://
-github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/
-lobster) and [animdl](https://github.com/justfoolingaround/animdl)
-[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-
-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/mov-
-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
-mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/mov-
-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
+you may also edit by manually opening the config file. See this [Wiki page]
+(https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
+```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
+mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
+132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
+`flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
+plugin, **however once again mov-cli is plugin based and there are many of them
+[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Contributing
+â¨ Pull requests are welcome and *appreciated*. For major changes, please open
+an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
+cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
+justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
+animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
+cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
+cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
+forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
+mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/ [python-shield]: https://
 img.shields.io/pypi/pyversions/mov-cli?style=flat [issues-shield]: https://
 img.shields.io/github/issues/mov-cli/mov-cli?style=flat [issues-url]: https://
 github.com/mov-cli/mov-cli/issues [license-shield]: https://img.shields.io/
-github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [discord-
-shield]: https://img.shields.io/badge/Discord-
-7289da?logo=discord&logoColor=white [discord-url]: https://discord.gg/
-BMzC7ePsBV
+github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [pypi-dl-
+shield]: https://img.shields.io/pypi/dm/mov-
+cli?color=informational&label=pypi%20downloads
```

### Comparing `mov-cli-4.2.9/mov_cli/cli/__main__.py` & `mov-cli-4.3.0/mov_cli/cli/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 import typer
 import logging
 from devgoldyutils import Colours
 
 from .play import play
 from .search import search
+from .ui import welcome_msg
 from .episode import handle_episode
-from .scraper import select_scraper, use_scraper, scrape
+from .plugins import show_all_plugins
+from .scraper import select_scraper, use_scraper, scrape, steal_scraper_args
 from .configuration import open_config_file, set_cli_config
-from .utils import welcome_msg, steal_scraper_args
 
 from ..config import Config
 from ..download import Download
 from ..logger import mov_cli_logger
 from ..http_client import HTTPClient
 
 __all__ = ("mov_cli",)
@@ -33,58 +34,70 @@
     episode: Optional[str] = typer.Option(None, "--episode", "-ep", help = "Episode and season you wanna scrape. E.g. {episode}:{season} like -> 26:3"), 
     auto_select: Optional[int] = typer.Option(None, "--choice", "-c", help = "Auto select the search results. E.g. Setting it to 1 with query 'nyan cat' will pick " \
         "the first nyan cat video to show up in search results."
     ), 
 
     version: bool = typer.Option(False, "--version", help = "Display what version mov-cli is currently on."), 
     edit: bool = typer.Option(False, "--edit", "-e", help = "Opens the mov-cli config with your respective editor."), 
-    download: bool = typer.Option(False, "--download", "-d", help = "Downloads the media instead of playing.")
+    download: bool = typer.Option(False, "--download", "-d", help = "Downloads the media instead of playing."),
+    list_plugins: bool = typer.Option(False, "--list-plugins", "-lp", help = "Prints all configured plugins and their scrapers."),
 ):
     config = Config()
 
     config = set_cli_config(
         config,
         debug = debug,
         player = player,
         scraper = scraper,
         fzf = fzf
     )
 
     if config.debug:
         mov_cli_logger.setLevel(logging.DEBUG)
 
-    print(
-        welcome_msg(True if query is None else False, version)
-    )
-
     mov_cli_logger.debug(f"Config -> {config.data}")
 
-    if edit is True:
+    if edit:
         open_config_file(config)
         return None
 
+    plugins = config.plugins
+
+    if list_plugins:
+        show_all_plugins(plugins)
+        return None
+
+    welcome_message = welcome_msg(
+        plugins = plugins, 
+        check_for_updates = True if query is None and config.skip_update_checker is False else False, 
+        display_hint = True if query is None else False, 
+        display_version = version
+    )
+
+    print(welcome_message)
+
     if query is not None:
-        scrape_args = steal_scraper_args(query) 
+        scrape_options = steal_scraper_args(query) 
         # This allows passing arguments to scrapers like this: 
         # https://github.com/mov-cli/mov-cli-youtube/commit/b538d82745a743cd74a02530d6a3d476cd60b808#diff-4e5b064838aa74a5375265f4dfbd94024b655ee24a191290aacd3673abed921a
 
         query: str = " ".join(query)
 
         http_client = HTTPClient(config)
 
-        selected_scraper = select_scraper(config.plugins, config.fzf_enabled, config.default_scraper)
+        selected_scraper = select_scraper(plugins, config.fzf_enabled, config.default_scraper)
 
         if selected_scraper is None:
             mov_cli_logger.error(
                 "You must choose a scraper to scrape with! " \
                     "You can set a default scraper with the default key in config.toml."
             )
             return False
 
-        chosen_scraper = use_scraper(selected_scraper, config, http_client)
+        chosen_scraper = use_scraper(selected_scraper, config, http_client, scrape_options)
 
         choice = search(query, auto_select, chosen_scraper, config.fzf_enabled)
 
         if choice is None:
             mov_cli_logger.error("There was no results or you didn't select anything.")
             return False
 
@@ -95,25 +108,32 @@
             fzf_enabled = config.fzf_enabled
         )
 
         if chosen_episode is None:
             mov_cli_logger.error("You didn't select a season/episode.")
             return False
 
-        media = scrape(choice, chosen_episode, chosen_scraper, **scrape_args)
+        media = scrape(choice, chosen_episode, chosen_scraper)
+
+        if media.url is None:
+            mov_cli_logger.error(
+                "Scraper didn't return a streamable url." \
+                    "\nThis is NOT a mov-cli issue. This IS an plugin issue"
+            )
+            return False
 
         if download:
             dl = Download(config)
             mov_cli_logger.debug(f"Downloading from this url -> '{media.url}'")
 
             popen = dl.download(media)
             popen.wait()
 
         else:
-            option = play(media, choice, chosen_scraper, chosen_episode, config, scrape_args)
+            option = play(media, choice, chosen_scraper, chosen_episode, config)
 
             if option == "search":
                 query = input(Colours.BLUE.apply("  Enter Query: "))
 
                 mov_cli(
                     query = [query], 
                     debug = debug, 
@@ -121,13 +141,14 @@
                     scraper = scraper, 
                     fzf = fzf,
                     episode = None,
                     auto_select = None,
 
                     version = False,
                     edit = False,
-                    download = False
+                    download = False,
+                    list_plugins = False
                 )
 
 def app():
     uwu_app.command()(mov_cli)
-    uwu_app() # Wait whaaaaa.
+    uwu_app()
```

### Comparing `mov-cli-4.2.9/mov_cli/cli/configuration.py` & `mov-cli-4.3.0/mov_cli/cli/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 
 import os
 from subprocess import check_call, CalledProcessError
 
 from .. import utils
 from ..logger import mov_cli_logger
 
-__all__ = (
-    "set_cli_config", 
-    "open_config_file"
-)
-
 def set_cli_config(config: Config, **kwargs: Optional[Any]) -> Config:
     debug = kwargs.get("debug")
     player = kwargs.get("player")
     scraper = kwargs.get("scraper")
     fzf = kwargs.get("fzf")
 
     if debug is not None:
```

### Comparing `mov-cli-4.2.9/mov_cli/cli/episode.py` & `mov-cli-4.3.0/mov_cli/cli/episode.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 
 from .ui import prompt
 
 from ..media import MetadataType
 from ..utils import EpisodeSelector
 from ..logger import mov_cli_logger
 
-__all__ = (
-    "handle_episode", 
-)
-
 def handle_episode(episode_string: Optional[str], scraper: Scraper, choice: Metadata, fzf_enabled: bool) -> Optional[EpisodeSelector]:
     if choice.type == MetadataType.MOVIE:
         return EpisodeSelector()
 
     if episode_string is None:
         mov_cli_logger.info(f"Scrapping episodes for '{Colours.CLAY.apply(choice.title)}'...")
         metadata_episodes = scraper.scrape_episodes(choice)
```

### Comparing `mov-cli-4.2.9/mov_cli/cli/play.py` & `mov-cli-4.3.0/mov_cli/cli/play.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Optional, Literal, Dict
+    from typing import Optional, Literal
 
     from ..config import Config
     from ..scraper import Scraper
     from ..media import Media, Metadata
-    from ..players import Player
 
     from utils.episode_selector import EpisodeSelector
 
+from devgoldyutils import Colours
+
 from .scraper import scrape
 from .episode import handle_episode
 from .watch_options import watch_options
 
 from ..utils import what_platform
 from ..logger import mov_cli_logger
 
-__all__ = (
-    "play",
-)
-
-def play(media: Media, metadata: Metadata, scraper: Scraper, episode: EpisodeSelector, config: Config, scrape_args: Dict[str, bool]) -> Optional[Literal["search"]]:
+def play(media: Media, metadata: Metadata, scraper: Scraper, episode: EpisodeSelector, config: Config) -> Optional[Literal["search"]]:
     platform = what_platform()
 
-    chosen_player: Player = config.player
+    chosen_player = config.player
+
+    mov_cli_logger.info(f"Playing '{Colours.BLUE.apply(media.display_name)}' with the '{chosen_player.__class__.__name__}' player...")
 
     popen = chosen_player.play(media)
 
     if popen is None and platform != "iOS":
         mov_cli_logger.error(
             f"The player '{config.player.__class__.__name__.lower()}' is not supported on this platform ({platform}). " \
             "We recommend VLC for iOS and MPV for every other platform."
@@ -63,29 +62,29 @@
 
         result = __handle_next_season(episode, season_episode_count, media_episodes)
 
         if result is False:
             mov_cli_logger.info("No more episodes :(")
             return None
 
-        media = scrape(metadata, episode, scraper, **scrape_args)
+        media = scrape(metadata, episode, scraper)
 
-        return play(media, metadata, scraper, episode, config, scrape_args)
+        return play(media, metadata, scraper, episode, config)
 
     elif option == "select":
         popen.kill()
 
         episode = handle_episode(None, scraper, metadata, config.fzf_enabled)
 
         if episode is None:
             return None
 
-        media = scrape(metadata, episode, scraper, **scrape_args)
+        media = scrape(metadata, episode, scraper)
 
-        return play(media, metadata, scraper, episode, config, scrape_args)
+        return play(media, metadata, scraper, episode, config)
 
     popen.wait()
 
     return None
 
 def __handle_next_season(episode: EpisodeSelector, season_episode_count: int, media_episodes: dict) -> bool:
```

### Comparing `mov-cli-4.2.9/mov_cli/cli/scraper.py` & `mov-cli-4.3.0/mov_cli/cli/scraper.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,52 +5,46 @@
     from typing import Type, Optional, Tuple, List, Dict
 
     from ..config import Config
     from ..media import Metadata, Media
     from ..http_client import HTTPClient
     from ..utils.episode_selector import EpisodeSelector
 
-    from ..scraper import Scraper
     from ..plugins import PluginHookData
+    from ..scraper import Scraper, ScraperOptionsT
 
 from devgoldyutils import Colours
 
 from .ui import prompt
-from .utils import handle_internal_plugin_error
+from .plugins import get_plugins_data, handle_internal_plugin_error
 
-from ..plugins import load_plugin
 from ..logger import mov_cli_logger
 
-__all__ = (
-    "scrape", 
-    "use_scraper", 
-    "select_scraper", 
-)
-
-def scrape(choice: Metadata, episode: EpisodeSelector, scraper: Scraper, **kwargs) -> Media:
+def scrape(choice: Metadata, episode: EpisodeSelector, scraper: Scraper) -> Media:
     mov_cli_logger.info(f"Scrapping media for '{Colours.CLAY.apply(choice.title)}'...")
 
     try:
-        media = scraper.scrape(choice, episode, **kwargs)
+        media = scraper.scrape(choice, episode)
     except Exception as e:
         handle_internal_plugin_error(e)
 
     return media
 
 def use_scraper(
-    selected_scraper: Optional[Tuple[str, Type[Scraper]]], 
+    selected_scraper: Tuple[str, Type[Scraper]], 
     config: Config, 
-    http_client: HTTPClient
+    http_client: HTTPClient,
+    scraper_options: ScraperOptionsT
 ) -> Scraper:
     scraper_name, scraper_class = selected_scraper
 
     mov_cli_logger.info(f"Using '{Colours.BLUE.apply(scraper_name)}' scraper...")
 
     try:
-        chosen_scraper = scraper_class(config, http_client)
+        chosen_scraper = scraper_class(config, http_client, scraper_options)
     except Exception as e:
         handle_internal_plugin_error(e)
 
     return chosen_scraper
 
 def select_scraper(plugins: Dict[str, str], fzf_enabled: bool, default_scraper: Optional[str] = None) -> Optional[Tuple[str, Type[Scraper]]]:
     plugins_data = get_plugins_data(plugins)
@@ -91,14 +85,26 @@
 
         scraper_name, scraper = chosen_scraper
 
         return f"{plugin_namespace}.{scraper_name}".lower(), scraper
 
     return None
 
+def steal_scraper_args(query: List[str]) -> ScraperOptionsT:
+    scrape_arguments = [x for x in query if "--" in x]
+
+    mov_cli_logger.debug(f"Scraper args picked up on --> {scrape_arguments}")
+
+    for scrape_arg in scrape_arguments:
+        query.remove(scrape_arg)
+
+    return dict(
+        [(x.replace("--", "").replace("-", "_"), True) for x in scrape_arguments]
+    )
+
 def get_scraper(scraper_id: str, plugins_data: List[Tuple[str, str, PluginHookData]]) -> Tuple[str, Type[Scraper] | Tuple[None, List[str]]]:
     available_scrapers = []
 
     for plugin_namespace, _, plugin_hook_data in plugins_data:
         scrapers = plugin_hook_data["scrapers"]
 
         if scraper_id.lower() == plugin_namespace.lower() and "DEFAULT" in scrapers:
@@ -108,23 +114,8 @@
             id = f"{plugin_namespace}.{scraper_name}".lower()
 
             available_scrapers.append(id)
 
             if scraper_id.lower() == id:
                 return id, scraper
 
-    return None, available_scrapers
-
-def get_plugins_data(plugins: Dict[str, str]) -> List[Tuple[str, str, PluginHookData]]:
-    plugins_data: List[Tuple[str, str, PluginHookData]] = []
-
-    for plugin_namespace, plugin_module_name in plugins.items():
-        plugin_data = load_plugin(plugin_module_name)
-
-        if plugin_data is None:
-            continue
-
-        plugins_data.append(
-            (plugin_namespace, plugin_module_name, plugin_data)
-        )
-
-    return plugins_data
+    return None, available_scrapers
```

### Comparing `mov-cli-4.2.9/mov_cli/cli/search.py` & `mov-cli-4.3.0/mov_cli/cli/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,19 @@
     from ..media import Metadata
     from ..scraper import Scraper
 
 from devgoldyutils import Colours
 
 from .ui import prompt
 from .auto_select import auto_select_choice
-from .utils import handle_internal_plugin_error
+from .plugins import handle_internal_plugin_error
 
 from ..media import MetadataType
 from ..logger import mov_cli_logger
 
-__all__ = (
-    "search", 
-)
-
 def search(query: str, auto_select: Optional[int], scraper: Scraper, fzf_enabled: bool) -> Optional[Metadata]:
     choice = None
 
     mov_cli_logger.info(f"Searching for '{Colours.ORANGE.apply(query)}'...")
 
     try:
         search_results = scraper.search(query)
```

### Comparing `mov-cli-4.2.9/mov_cli/cli/watch_options.py` & `mov-cli-4.3.0/mov_cli/cli/watch_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 
 import time
 from subprocess import Popen
 
 from .ui import prompt
 from ..media import Series
 
-__all__ = (
-    "watch_options", 
-)
-
 def watch_options(
     popen: Popen, 
     player: Player, 
     platform: SUPPORTED_PLATFORMS, 
     media: Media, 
     fzf_enabled: bool
 ) -> Optional[Literal["search", "next", "previous", "select"]]:
```

### Comparing `mov-cli-4.2.9/mov_cli/config.py` & `mov-cli-4.3.0/mov_cli/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, TypedDict, final
 
 if TYPE_CHECKING:
     from .players import Player
-    from typing import Dict, Union, Literal, Any, Optional, Type
+    from typing import Dict, Union, Literal, Any, Optional
 
     JSON_VALUES = Union[str, bool, int, dict]
     SUPPORTED_PARSERS = Literal["lxml", "html.parser"]
 
 import os
 import toml
+import shutil
 from pathlib import Path
 from importlib.util import find_spec
 from devgoldyutils import LoggerAdapter
 
 from . import players, utils
 from .logger import mov_cli_logger
 
-__all__ = ("Config",)
+__all__ = ("Config", )
 
 @final
 class ConfigUIData(TypedDict):
     fzf: bool
 
 @final
 class ConfigHTTPData(TypedDict):
@@ -42,14 +43,16 @@
     player: str
     parser: SUPPORTED_PARSERS
     ui: ConfigUIData
     http: ConfigHTTPData
     downloads: ConfigDownloadsData
     scrapers: ScrapersData
     plugins: Dict[str, str]
+    resolution: int
+    
 
 logger = LoggerAdapter(mov_cli_logger, prefix = "Config")
 
 class Config():
     """Class that wraps the mov-cli configuration file. Mostly used under the CLI interface."""
     def __init__(self, override_config: ConfigData = None, config_path: Path = None) -> None:
         self.config_path = config_path
@@ -71,45 +74,49 @@
             self.data = override_config
 
     @property
     def version(self) -> int:
         return self.data.get("version", 1)
 
     @property
-    def player(self) -> Type[Player]:
+    def player(self) -> Player:
         """Returns the player class that was configured in the config. Defaults to MPV."""
         value = self.data.get("player", "mpv")
 
         platform = utils.what_platform()
 
         if value.lower() == "mpv":
-            return players.MPV(platform)
+            return players.MPV(platform, self)
         elif value.lower() == "vlc":
-            return players.VLC(platform)
+            return players.VLC(platform, self)
 
         return players.CustomPlayer(value)
 
     @property
     def plugins(self) -> Dict[str, str]:
         return self.data.get("plugins", {"test": "mov-cli-test"})
 
     @property
     def editor(self) -> Optional[str]:
         """Returns the editor that should be opened while editing."""
         return self.data.get("editor")
 
     @property
+    def skip_update_checker(self) -> bool:
+        return self.data.get("skip_update_checker", False)
+
+    @property
     def default_scraper(self) -> Optional[str]:
         """Returns the scraper that should be used to scrape by default."""
         return self.data.get("scrapers", {}).get("default", None)
 
     @property
     def fzf_enabled(self) -> bool:
-        """Returns whether fzf is allowed to be used."""
-        return self.data.get("ui", {}).get("fzf", True)
+        """Returns whether fzf is allowed to be used. Defaults to True of fzf is available."""
+        return self.data.get("ui", {}).get("fzf", True if shutil.which("fzf") is not None else False)
 
     @property
     def parser(self) -> SUPPORTED_PARSERS | Any:
         """Returns the parser type configured by the user else it just returns the default."""
         default_parser = "lxml" if find_spec("lxml") else "html.parser"
         return self.data.get("parser", default_parser)
 
@@ -153,14 +160,18 @@
         default_headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0",
             "Accept-Language": "en-US,en;q=0.5",
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
         }
 
         return self.data.get("http", {}).get("headers", default_headers)
+        
+    @property
+    def resolution(self) -> int:
+        return self.data.get("quality", {}).get("resolution", {})
 
     def __get_config_file(self) -> Path:
         """Function that returns the path to the config file with multi platform support."""
         platform = utils.what_platform()
 
         appdata_dir = Path("./mov-cli-temp")
 
@@ -195,8 +206,8 @@
 
             with open(template_config_path, "r") as config_template:
                 config_file.write(config_template.read())
 
             config_file.close()
             logger.info(f"Config created at '{config_path}'.")
 
-        return config_path
+        return config_path
```

### Comparing `mov-cli-4.2.9/mov_cli/config.template.toml` & `mov-cli-4.3.0/mov_cli/config.template.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [mov-cli]
 version = 1
 player = "mpv"
 debug = false
 # parser = "lxml"
 # editor = "nano"
+skip_update_checker = false
 
 [mov-cli.ui]
-fzf = true
+# fzf = true
 
 [mov-cli.plugins] # E.g: namespace = "package-name"
 test = "mov-cli-test"
 
 # [mov-cli.scrapers]
 # default = "films"
 
 # [mov-cli.http] # Don't mess with it if you don't know what you are doing!
 # headers = { User-Agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0" }
 
 # [mov-cli.downloads] # Do not use backslashes use forward slashes
 # save_path = "~/Downloads"
+
+# [mov-cli.quality]
+# resolution = 720
```

### Comparing `mov-cli-4.2.9/mov_cli/download.py` & `mov-cli-4.3.0/mov_cli/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,17 @@
         self.config = config
 
     def download(self, media: Series | Movie, subtitles: str = None) -> subprocess.Popen:
         title = unicodedata.normalize('NFKD', media.display_name).encode('ascii', 'ignore').decode('ascii') # normalize title
         
         file = os.path.join(self.config.download_location, title + ".mp4")
 
-        args = [
+        args = [ # TODO: Check if url is a m3u8 if not use aria2
             "ffmpeg",
             "-n",
-            "-thread_queue_size",
-            "4096",
             "-headers",
             f"Referer: {media.referrer}",
             "-i",
             media.url,
             "-c",
             "copy",
         ]
```

### Comparing `mov-cli-4.2.9/mov_cli/errors.py` & `mov-cli-4.3.0/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/http_client.py` & `mov-cli-4.3.0/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/iterfzf/LICENSE.txt` & `mov-cli-4.3.0/mov_cli/iterfzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/iterfzf/__init__.py` & `mov-cli-4.3.0/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/media/media.py` & `mov-cli-4.3.0/mov_cli/media/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 if TYPE_CHECKING:
     from typing import Optional
     from ..utils import EpisodeSelector
 
 from abc import abstractmethod
 
 __all__ = (
-    "Media", 
-    "Series", 
-    "Movie"
+    "Media",
+    "Multi", 
+    "Single", 
+    "Movie", 
+    "Series"
 )
 
 class Media():
     """Represents any piece of media in mov-cli that can be streamed or downloaded."""
     def __init__(self, url: str, title: str, referrer: Optional[str]) -> None:
         self.url = url
         """The stream-able url."""
@@ -25,16 +27,16 @@
 
     @property
     @abstractmethod
     def display_name(self) -> str:
         """The title that should be displayed by the player."""
         ...
 
-class Series(Media):
-    """Represents a TV Show. E.g an Anime or Cartoon."""
+class Multi(Media):
+    """Represents a media that has multiple episodes like a TV Series, Anime or Cartoon."""
     def __init__(
         self, 
         url: str, 
         title: str, 
         episode: EpisodeSelector, 
         referrer: Optional[str] = None, 
         subtitles: Optional[dict] = None
@@ -47,16 +49,16 @@
             url, title, referrer
         )
 
     @property
     def display_name(self) -> str:
         return f"{self.title} - S{self.episode.season} EP{self.episode.episode}"
 
-class Movie(Media):
-    """Represents a Film/Movie."""
+class Single(Media):
+    """Represents a media with a single episode, like a Film/Movie or a YouTube video."""
     def __init__(
         self, 
         url: str,
         title: str,
         referrer: Optional[str] = None,
         year: Optional[str] = None,
         subtitles: Optional[dict] = None
@@ -69,20 +71,10 @@
             url, title, referrer
         )
 
     @property
     def display_name(self) -> str:
         return f"{self.title} ({self.year})"
 
-
-# class LiveTV(Media):
-#     """Represents media that is live, like a tv channel or a live stream."""
-#     def __init__(
-#         self, 
-#         url: str, 
-#         title: str, 
-#         referrer: str, 
-#     ) -> None:
-
-#         super().__init__(
-#             url, title, referrer
-#         )
+# Backwards compatibility for post v4.3.0 extensions.
+Series = Multi
+Movie = Single
```

### Comparing `mov-cli-4.2.9/mov_cli/media/metadata.py` & `mov-cli-4.3.0/mov_cli/media/metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 
 from enum import Enum
 from dataclasses import dataclass, field
 
 __all__ = ("MetadataType", "Metadata", "ExtraMetadata", "AiringType")
 
 class MetadataType(Enum):
-    SERIES = 0
+    MULTI = 0
     """Media with multiple seasons and episodes."""
-    MOVIE = 1
+    SINGLE = 1
     """Media with no seasons and episodes. Like a film or short animation."""
-    LIVE = 2
-    """Media that is live, like a tv channel or a live stream."""
+
+    SERIES = 0
+    """DEPRECATED!!! USE 'MetadataType.MULTI' INSTEAD! This will be removed after v4.4."""
+    MOVIE = 1
+    """DEPRECATED!!! USE 'MetadataType.SINGLE' INSTEAD!. This will be removed after v4.4."""
 
 class AiringType(Enum):
     DONE = 0
     ONGOING = 1
     PRODUCTION = 2
     RELEASED = 3
     CANCELED = 4
```

### Comparing `mov-cli-4.2.9/mov_cli/players/custom_player.py` & `mov-cli-4.3.0/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/players/mpv.py` & `mov-cli-4.3.0/mov_cli/players/vlc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Optional
+
     from ..media import Media
+    from .. import Config
     from ..utils.platform import SUPPORTED_PLATFORMS
 
 import subprocess
 from devgoldyutils import Colours, LoggerAdapter
 
 from .. import errors
 from ..logger import mov_cli_logger
 from .player import Player
 
-__all__ = ("MPV",)
+__all__ = ("VLC",)
 
-logger = LoggerAdapter(mov_cli_logger, prefix = Colours.PURPLE.apply("MPV"))
+logger = LoggerAdapter(mov_cli_logger, prefix = Colours.ORANGE.apply("VLC"))
 
-class MPV(Player):
-    def __init__(self, platform: SUPPORTED_PLATFORMS, **kwargs) -> None:
+class VLC(Player):
+    def __init__(self, platform: SUPPORTED_PLATFORMS, config: Config, **kwargs) -> None:
         self.platform = platform
+        self.config = config
 
         super().__init__(**kwargs)
 
     def play(self, media: Media) -> Optional[subprocess.Popen]:
-        """Plays this media in the MPV media player."""
+        """Plays this media in the VLC media player."""
 
-        logger.info("Launching MPV Media Player...")
+        logger.info("Launching VLC Media Player...")
 
         if self.platform == "Android":
             return subprocess.Popen(
                 [
                     "am",
                     "start",
                     "-n",
-                    "is.xyz.mpv/is.xyz.mpv.MPVActivity",
+                    "org.videolan.vlc/org.videolan.vlc.gui.video.VideoPlayerActivity",
                     "-e",
-                    "filepath",
+                    "title",
+                    media.display_name,
                     media.url,
                 ]
             )
 
-        try:
+        elif self.platform == "iOS":
+            logger.debug("Detected your using iOS. \r\n")
 
-            if self.platform == "Linux" or self.platform == "Windows":
-                args = [
-                    "mpv",
-                    media.url,
-                    f"--force-media-title={media.display_name}",
-                    "--no-terminal",
-                ]
+            with open('/dev/clipboard', 'w') as f:
+                f.write(f"vlc://{media.url}")
 
-                if media.referrer is not None:
-                    args.append(f"--referrer={media.referrer}")
+            logger.info("The URL was copied into your clipboard. To play it, open a browser and paste the URL.")
 
-                return subprocess.Popen(args)
+            return None
 
-            elif self.platform == "Darwin":
+        elif self.platform == "Linux" or self.platform == "Windows":
+            try:
                 args = [
-                    "iina",
-                    "--no-stdin",
-                    "--keep-running",
-                    media.url,
-                    f"--mpv-force-media-title={media.display_name}",
+                    "vlc", 
+                    f'--meta-title="{media.display_name}"', 
+                    media.url
                 ]
 
                 if media.referrer is not None:
-                    args.append(f"--mpv-referrer={media.referrer}")
+                    args.append(f'--http-referrer="{media.referrer}"')
+
+                if self.config.resolution:
+                    args.append(f"--adaptive-maxwidth={self.config.resolution}") # NOTE: I don't really know if that works ~ Ananas
 
                 return subprocess.Popen(args)
 
-        except ModuleNotFoundError:
-            raise errors.PlayerNotFound(self)
+            except ModuleNotFoundError:
+                raise errors.PlayerNotFound(self)
 
         return None
```

### Comparing `mov-cli-4.2.9/mov_cli/players/player.py` & `mov-cli-4.3.0/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/plugins.py` & `mov-cli-4.3.0/mov_cli/plugins.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Module containing mov-cli plugin related stuff.
 """
 from __future__ import annotations
 from typing import TYPE_CHECKING, TypedDict
 
 if TYPE_CHECKING:
-    from typing import Optional, Dict, Literal
+    from types import ModuleType
+    from typing import Optional, Dict, Literal, Tuple
 
     from .scraper import Scraper
 
 import importlib
 from devgoldyutils import LoggerAdapter
 
 from .logger import mov_cli_logger
@@ -19,22 +20,25 @@
     "PluginHookData"
 )
 
 logger = LoggerAdapter(mov_cli_logger, prefix = "Plugins")
 
 class PluginHookData(TypedDict):
     version: int
+    """The version of the plugin hook to use. Version 1 is latest currently."""
+    package_name: str
+    """The name of the pypi package. This is required for the plugin update notifier to work."""
     scrapers: Dict[str, Scraper] | Dict[Literal["DEFAULT"], Scraper]
 
-def load_plugin(module_name: str) -> Optional[PluginHookData]:
+def load_plugin(module_name: str) -> Optional[Tuple[Optional[PluginHookData], ModuleType]]:
     try:
         plugin_module = importlib.import_module(module_name.replace("-", "_"))
     except ModuleNotFoundError as e:
         logger.error(f"Failed to import a plugin from the module '{module_name}'! Error --> {e}")
         return None
 
     plugin_data = getattr(plugin_module, "plugin", None)
 
     if plugin_data is None:
         logger.warning(f"Failed to load the plugin '{module_name}'! It doesn't contain a plugin hook!")
 
-    return plugin_data
+    return plugin_data, plugin_module
```

### Comparing `mov-cli-4.2.9/mov_cli/scraper.py` & `mov-cli-4.3.0/mov_cli/scraper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Dict, Literal, Optional, Iterable
+    from typing import Dict, Literal, Iterable, Optional
+
     from .config import Config
-    from .http_client import HTTPClient
-    from .media import Metadata, Series, Movie
     from .utils import EpisodeSelector
+    from .http_client import HTTPClient
+    from .media import Metadata, Multi, Single
+
+    ScraperOptionsT = Dict[str, str | bool]
 
 from bs4 import BeautifulSoup
 from abc import ABC, abstractmethod
 from devgoldyutils import LoggerAdapter
 
 from . import errors
 from .logger import mov_cli_logger
 
 __all__ = ("Scraper", "MediaNotFound")
 
 class Scraper(ABC):
-    def __init__(self, config: Config, http_client: HTTPClient) -> None:
-        """A base class for building scrapers from."""
+    """A base class for building scrapers from."""
+    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         self.config = config
         self.http_client = http_client
+        self.options = options or {}
+
         self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
 
         super().__init__()
 
-    def soup(self, html: str) -> BeautifulSoup:
-        return BeautifulSoup(html, self.config.parser)
+    def soup(self, html: str, **kwargs) -> BeautifulSoup:
+        """A ready to use beautiful soup instance."""
+        return BeautifulSoup(html, self.config.parser, **kwargs)
 
     @abstractmethod
     def search(self, query: str, limit: int = 20) -> Iterable[Metadata]:
+        """Where your searching for media should be done. Should return or yield Metadata."""
         ...
 
     @abstractmethod
-    def scrape(self, metadata: Metadata, episode: Optional[EpisodeSelector] = None, **kwargs) -> Series | Movie:
+    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Multi | Single:
         """
-        Where your searching and scraping for the media should be performed done. 
-        Should return an instance of Media.
+        Where your scraping for the media should be performed. 
+        Should return or yield an instance of Media.
         """
         ...
 
     @abstractmethod
-    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[int, int] | Dict[None, Literal[1]]:
+    def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
         """Returns episode count for each season in that Movie/Series."""
         ...
 
 class MediaNotFound(errors.MovCliException):
     """Raises when a scraper fails to find a show/movie/tv-station."""
     def __init__(self, message, scraper: Scraper) -> None:
         super().__init__(
```

### Comparing `mov-cli-4.2.9/mov_cli/utils/episode_selector.py` & `mov-cli-4.3.0/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/utils/platform.py` & `mov-cli-4.3.0/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.2.9/mov_cli/utils/scraper/the_movie_db.py` & `mov-cli-4.3.0/mov_cli/utils/scraper/the_movie_db.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 if TYPE_CHECKING:
     from typing import List, Any, Generator, Dict, Literal
     from ...http_client import HTTPClient
 
 from ...media import Metadata, MetadataType, ExtraMetadata, AiringType
 from base64 import b64decode
-from thefuzz import fuzz
 
 __all__ = ("TheMovieDB",)
 
 class TMDbSerial:
     def __init__(self, data, type: MetadataType):
         self.id: int = data.get("id")
         self.title: str = self.__extract_title(data)
@@ -58,20 +57,15 @@
             item = TMDbSerial(item, MetadataType.SERIES)
 
             if not item.release_date:
                 continue
 
             serial_list.append(item)
 
-        sorted_list: List[TMDbSerial] = self.__sort(serial_list, query)[:limit]
-        # Is there are point in fuzzy sorting? The search api (tmdb) should do that for us and fzf exists for that reason. ~ Goldy
-
-        # Also yield won't actually do anything performance wise if we've already appended the items into a list.
-        # Actually in this case we can't really take advantage of yield as the api returns all results at once. ~ Goldy
-        for item in sorted_list:
+        for item in serial_list:
             yield Metadata(
                 id = item.id,
                 title = item.title,
                 type = item.type,
                 year = item.year,
                 extra_func = lambda: self.__extra_metadata(item)
             )
@@ -135,17 +129,8 @@
         return ExtraMetadata(
             description = description,
             image_url = image_url,
             cast = cast,
             alternate_titles = alternate_titles,
             genres = genres,
             airing = airing
-        )
-
-    def __sort_key(self, query):
-        def similarity_score(item: TMDbSerial):
-            return fuzz.ratio(item.title, query)
-        return similarity_score
-
-    def __sort(self, unsorted, query):
-        sorted_list = sorted(unsorted, key=self.__sort_key(query), reverse=True)
-        return sorted_list
+        )
```

### Comparing `mov-cli-4.2.9/mov_cli.egg-info/PKG-INFO` & `mov-cli-4.3.0/mov_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.2.9
+Version: 4.3.0
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,105 +40,111 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: toml
 Requires-Dist: devgoldyutils>=2.5.7
-Requires-Dist: typer[all]==0.10.0
+Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer
 Requires-Dist: beautifulsoup4
 Requires-Dist: Unidecode
-Requires-Dist: thefuzz
 Requires-Dist: deprecation
+Requires-Dist: packaging
 Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
 
 [![Stargazers][stars-shield]][stars-url]
 [![Pypi Version][pypi-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-url]
 [![Python Versions][python-shield]][pypi-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
-[![Discord][discord-shield]][discord-url]
+
 
 <div align="center">
 
   <a href="https://github.com/mov-cli/mov-cli">
     <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
   </a>
 
   <sub>Watch everything from your terminal.</sub>
   <br>
   <br>
   <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
   ·
   <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
 
-</div>
+  <br>
+  <br>
+  <a href="https://discord.gg/BMzC7ePsBV">
+    <img src="https://invidget.switchblade.xyz/BMzC7ePsBV" alt="Logo" width="400">
+  </a>
 
+</div>
 <br>
 
 > [!Note]
-> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
+> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also I would advise not using it as a library yet as the API still has many breaking changes.
 
 ## Installation 🛠️
 
 > [!TIP]
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
 - **A supported platform:**
   - Linux
   - Windows
   - Android (via [Termux](https://termux.dev/en/))
   - iOS (via [iSH Shell](https://ish.app/))
-  - *MacOS* (**Not tested**)
+  - MacOS
 - **[python](https://www.python.org/downloads/)** (**required**, with pip)
 - **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
 - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
 - **[mpv](https://mpv.io/installation/)** (recommended & default media player)
 
 To get running these are all the prerequisites you'll need.
 
 With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
 
 ```sh
 pip install mov-cli -U
 ```
+> Check out the [wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation) for more in-depth guidance on installing mov-cli.
 
 ## Usage 🖱️
 mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
 
 > [!NOTE]
 > You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
 > Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
 
 1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
 ```sh
 mov-cli -e
 ```
-Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
+Alternatively, you may also edit by manually opening the config file. See this [Wiki page](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.  
 ```toml
 [mov-cli.plugins]
-films = "package_name"
+youtube = "mov-cli-youtube"
 ```
 
-
-2. Scraper away!
+2. Scrape away!
 ```sh
-mov-cli -s films spider man no way home
+mov-cli -s youtube flight 370
 ```
-<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
+<img src="https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118">
 
-> The above command should search for `spider man no way home` with the following scraper.
+> The command above searches for `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-cli is plugin based and there are many of them [in the wild](https://github.com/topics/mov-cli-plugin). 😉**
 
 ## Contributing ✨
 Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
 
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
@@ -158,9 +164,8 @@
 [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/
 [python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
 [license-url]: ./LICENSE
-[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
-[discord-url]: https://discord.gg/BMzC7ePsBV
+[pypi-dl-shield]: https://img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.2.9 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.0 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -23,69 +23,74 @@
 Windows 10 Classifier: Operating System :: POSIX :: Linux Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
-toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer[all]==0.10.0
-Requires-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode
-Requires-Dist: thefuzz Requires-Dist: deprecation Requires-Dist: mov-cli-
-test>=1.1.0 Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-
-Dist: build; extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra
-== "dev" [![Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-
-shield]][pypi-url] [![Python Versions][python-shield]][pypi-url] [![Issues]
-[issues-shield]][issues-url] [![MIT License][license-shield]][license-url] [!
-[Discord][discord-shield]][discord-url]
+toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer>=0.12.2 Requires-
+Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode Requires-
+Dist: deprecation Requires-Dist: packaging Requires-Dist: mov-cli-test>=1.1.0
+Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build;
+extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
+[Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-url] [![Python Versions][python-
+shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
+[license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
-> [!Note] > v4 is constantly changing so be sure to keep the tool up to date
-and with that said I would advise not using it as a library yet. ##
-Installation ð ï¸ > [!TIP] > For in-depth installation instructions hit the
-[wiki](https://github.com/mov-cli/mov-cli/wiki/Installation). ### Prerequisites
-- **A supported platform:** - Linux - Windows - Android (via [Termux](https://
-termux.dev/en/)) - iOS (via [iSH Shell](https://ish.app/)) - *MacOS* (**Not
-tested**) - **[python](https://www.python.org/downloads/)** (**required**, with
-pip) - **[lxml](https://pypi.org/project/lxml/)** (optional, â¡ faster
-scraping) - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-
-file#installation)** (optional but **highly recommended**) - **[mpv](https://
-mpv.io/installation/)** (recommended & default media player) To get running
-these are all the prerequisites you'll need. With the prerequisites installed,
-mov-cli can be installed via the pip command on all platforms with Python
-version 3.8 or above. ```sh pip install mov-cli -U ``` ## Usage ð±ï¸ mov-cli
+                                    _[_L_o_g_o_]
+
+> [!Note] > v4 is constantly changing so be sure to **keep the tool and your
+plugins up to date**. Also I would advise not using it as a library yet as the
+API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
+depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
+cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
+Windows - Android (via [Termux](https://termux.dev/en/)) - iOS (via [iSH Shell]
+(https://ish.app/)) - MacOS - **[python](https://www.python.org/downloads/)**
+(**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
+(optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
+fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
+**[mpv](https://mpv.io/installation/)** (recommended & default media player) To
+get running these are all the prerequisites you'll need. With the prerequisites
+installed, mov-cli can be installed via the pip command on all platforms with
+Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
+[wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation)
+for more in-depth guidance on installing mov-cli. ## Usage ð±ï¸ mov-cli
 comes packaged with a CLI interface via the `mov-cli` command you can use in
 your respective terminal. > [!NOTE] > You may notice mov-cli doesn't ship with
 any scrapers (or previously known as providers) by default, this is because v4
 is plugin-based and scrapers are now part of plugins that must be chosen to be
 installed. > Find out how to do so at the [wiki](https://github.com/mov-cli/
 mov-cli/wiki#plugins). 1. Install the scraper plugin of your choice. Visit this
 [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so
 and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a
 list of **third-party** mov-cli plugins. ```sh mov-cli -e ``` Alternatively,
-you may also edit by manually opening the config file. See the [Wiki](https://
-github.com/mov-cli/mov-cli/wiki/Configuration#introduction). ```toml [mov-
-cli.plugins] films = "package_name" ``` 2. Scraper away! ```sh mov-cli -s films
-spider man no way home ``` [https://github.com/mov-cli/mov-cli/assets/66202304/
-86189cab-b246-405e-a266-6c624bee2d36]> The above command should search for
-`spider man no way home` with the following scraper. ## Contributing â¨ Pull
-requests are welcome and *appreciated*. For major changes, please open an issue
-first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-cli](https://
-github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/
-lobster) and [animdl](https://github.com/justfoolingaround/animdl)
-[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-
-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/mov-
-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
-mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/mov-
-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
+you may also edit by manually opening the config file. See this [Wiki page]
+(https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
+```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
+mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
+132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
+`flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
+plugin, **however once again mov-cli is plugin based and there are many of them
+[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Contributing
+â¨ Pull requests are welcome and *appreciated*. For major changes, please open
+an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
+cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
+justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
+animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
+cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
+cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
+forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
+mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/ [python-shield]: https://
 img.shields.io/pypi/pyversions/mov-cli?style=flat [issues-shield]: https://
 img.shields.io/github/issues/mov-cli/mov-cli?style=flat [issues-url]: https://
 github.com/mov-cli/mov-cli/issues [license-shield]: https://img.shields.io/
-github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [discord-
-shield]: https://img.shields.io/badge/Discord-
-7289da?logo=discord&logoColor=white [discord-url]: https://discord.gg/
-BMzC7ePsBV
+github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [pypi-dl-
+shield]: https://img.shields.io/pypi/dm/mov-
+cli?color=informational&label=pypi%20downloads
```

### Comparing `mov-cli-4.2.9/mov_cli.egg-info/SOURCES.txt` & `mov-cli-4.3.0/mov_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 mov_cli.egg-info/top_level.txt
 mov_cli/cli/__init__.py
 mov_cli/cli/__main__.py
 mov_cli/cli/auto_select.py
 mov_cli/cli/configuration.py
 mov_cli/cli/episode.py
 mov_cli/cli/play.py
+mov_cli/cli/plugins.py
 mov_cli/cli/scraper.py
 mov_cli/cli/search.py
 mov_cli/cli/ui.py
-mov_cli/cli/utils.py
 mov_cli/cli/watch_options.py
 mov_cli/iterfzf/LICENSE.txt
 mov_cli/iterfzf/__init__.py
 mov_cli/media/__init__.py
 mov_cli/media/media.py
 mov_cli/media/metadata.py
 mov_cli/players/__init__.py
@@ -49,10 +49,9 @@
 mov_cli/players/player.py
 mov_cli/players/vlc.py
 mov_cli/utils/__init__.py
 mov_cli/utils/episode_selector.py
 mov_cli/utils/platform.py
 mov_cli/utils/version.py
 mov_cli/utils/scraper/__init__.py
-mov_cli/utils/scraper/fuzzy.py
 mov_cli/utils/scraper/the_movie_db.py
 scripts/test_cli.py
```

### Comparing `mov-cli-4.2.9/pyproject.toml` & `mov-cli-4.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     'Programming Language :: Python :: 3.12'
 ]
 dependencies = [
     "httpx",
     "importlib-metadata; python_version<'3.8'",
     "toml",
     "devgoldyutils>=2.5.7",
-    "typer[all]==0.10.0",
+    "typer>=0.12.2",
     "inquirer",
     "beautifulsoup4",
     "Unidecode",
-    "thefuzz",
     "deprecation",
+    "packaging",
 
     # Included plugins
     "mov-cli-test>=1.1.0"
 ]
 
 dynamic = ["version"]
```

