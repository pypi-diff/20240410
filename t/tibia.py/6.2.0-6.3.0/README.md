# Comparing `tmp/tibia.py-6.2.0.tar.gz` & `tmp/tibia.py-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibia.py-6.2.0.tar", last modified: Sun Mar 31 22:03:06 2024, max compression
+gzip compressed data, was "tibia.py-6.3.0.tar", last modified: Sat Apr  6 04:11:49 2024, max compression
```

## Comparing `tibia.py-6.2.0.tar` & `tibia.py-6.3.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.755630 tibia.py-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    24552 2024-03-31 22:02:58.000000 tibia.py-6.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-31 22:02:58.000000 tibia.py-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-31 22:02:58.000000 tibia.py-6.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-31 22:03:06.755630 tibia.py-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-31 22:02:58.000000 tibia.py-6.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-03-31 22:02:58.000000 tibia.py-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-linting.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-server.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements-testing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-31 22:02:58.000000 tibia.py-6.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:03:06.755630 tibia.py-6.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.743630 tibia.py-6.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_character.py
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_creature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_fansites.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_forums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_house.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_leaderboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_tibiapy.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tests/tests_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.751630 tibia.py-6.2.0/tibia.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 22:03:06.000000 tibia.py-6.2.0/tibia.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.743630 tibia.py-6.2.0/tibiapy/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.747630 tibia.py-6.2.0/tibiapy/builders/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14708 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/creature.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/house.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/builders/world.py
--rw-r--r--   0 runner    (1001) docker     (127)    56099 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15773 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.751630 tibia.py-6.2.0/tibiapy/models/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/creature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/fansite.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/house.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/tibia_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/models/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:03:06.751630 tibia.py-6.2.0/tibiapy/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29869 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/creature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/fansite.py
--rw-r--r--   0 runner    (1001) docker     (127)    29449 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)    19036 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/highscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/house.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/kill_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/news.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/spell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/parsers/world.py
--rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-03-31 22:02:58.000000 tibia.py-6.2.0/tibiapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:11:49.552605 tibia.py-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-04-06 04:11:40.000000 tibia.py-6.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-06 04:11:40.000000 tibia.py-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 04:11:40.000000 tibia.py-6.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-06 04:11:49.552605 tibia.py-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-06 04:11:40.000000 tibia.py-6.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-06 04:11:40.000000 tibia.py-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 04:11:40.000000 tibia.py-6.3.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 04:11:40.000000 tibia.py-6.3.0/requirements-linting.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 04:11:40.000000 tibia.py-6.3.0/requirements-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-06 04:11:40.000000 tibia.py-6.3.0/requirements-testing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-06 04:11:40.000000 tibia.py-6.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 04:11:49.552605 tibia.py-6.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:11:49.540604 tibia.py-6.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_fansites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_forums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_leaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_tibiapy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tests/tests_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:11:49.552605 tibia.py-6.3.0/tibia.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-06 04:11:49.000000 tibia.py-6.3.0/tibia.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-06 04:11:49.000000 tibia.py-6.3.0/tibia.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:11:49.000000 tibia.py-6.3.0/tibia.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-06 04:11:49.000000 tibia.py-6.3.0/tibia.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 04:11:49.000000 tibia.py-6.3.0/tibia.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:11:49.544604 tibia.py-6.3.0/tibiapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:11:49.544604 tibia.py-6.3.0/tibiapy/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14708 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/builders/world.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56099 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:11:49.548605 tibia.py-6.3.0/tibiapy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/fansite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/tibia_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/models/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:11:49.552605 tibia.py-6.3.0/tibiapy/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29869 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/creature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/fansite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29449 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19036 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/highscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/house.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/kill_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/parsers/world.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-04-06 04:11:40.000000 tibia.py-6.3.0/tibiapy/utils.py
```

### Comparing `tibia.py-6.2.0/CHANGELOG.rst` & `tibia.py-6.3.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 Changelog
 =========
 
 .. note::
     Due to this library relying on external content, older versions are not guaranteed to work.
     Try to always use the latest version.
 
+.. v6.3.0
+
+6.3.0 (2024-04-05)
+==================
+- Add Ocenia world location.
+
 .. v6.2.0
 
 6.2.0 (2024-03-31)
 ==================
 - Add support for parsing the fansites section.
 
 .. v6.1.0
```

### Comparing `tibia.py-6.2.0/LICENSE` & `tibia.py-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/PKG-INFO` & `tibia.py-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibia.py
-Version: 6.2.0
+Version: 6.3.0
 Summary: API that parses website content into python data.
 Author-email: Allan Galarza <allan.galarza@gmail.com>
 Maintainer-email: Allan Galarza <allan.galarza@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://tibiapy.readthedocs.io/
 Project-URL: Documentation, https://tibiapy.readthedocs.io/
 Project-URL: Repository, https://github.com/Galarzaa90/tibia.py
```

### Comparing `tibia.py-6.2.0/README.md` & `tibia.py-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/pyproject.toml` & `tibia.py-6.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_bazaar.py` & `tibia.py-6.3.0/tests/tests_bazaar.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_character.py` & `tibia.py-6.3.0/tests/tests_character.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_client.py` & `tibia.py-6.3.0/tests/tests_client.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_creature.py` & `tibia.py-6.3.0/tests/tests_creature.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_enums.py` & `tibia.py-6.3.0/tests/tests_enums.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_events.py` & `tibia.py-6.3.0/tests/tests_events.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_fansites.py` & `tibia.py-6.3.0/tests/tests_fansites.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_forums.py` & `tibia.py-6.3.0/tests/tests_forums.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_guild.py` & `tibia.py-6.3.0/tests/tests_guild.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_highscores.py` & `tibia.py-6.3.0/tests/tests_highscores.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_house.py` & `tibia.py-6.3.0/tests/tests_house.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_kill_statistics.py` & `tibia.py-6.3.0/tests/tests_kill_statistics.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_leaderboards.py` & `tibia.py-6.3.0/tests/tests_leaderboards.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_news.py` & `tibia.py-6.3.0/tests/tests_news.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_spell.py` & `tibia.py-6.3.0/tests/tests_spell.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_tibiapy.py` & `tibia.py-6.3.0/tests/tests_tibiapy.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_utils.py` & `tibia.py-6.3.0/tests/tests_utils.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tests/tests_world.py` & `tibia.py-6.3.0/tests/tests_world.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibia.py.egg-info/PKG-INFO` & `tibia.py-6.3.0/tibia.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibia.py
-Version: 6.2.0
+Version: 6.3.0
 Summary: API that parses website content into python data.
 Author-email: Allan Galarza <allan.galarza@gmail.com>
 Maintainer-email: Allan Galarza <allan.galarza@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://tibiapy.readthedocs.io/
 Project-URL: Documentation, https://tibiapy.readthedocs.io/
 Project-URL: Repository, https://github.com/Galarzaa90/tibia.py
```

### Comparing `tibia.py-6.2.0/tibia.py.egg-info/SOURCES.txt` & `tibia.py-6.3.0/tibia.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/bazaar.py` & `tibia.py-6.3.0/tibiapy/builders/bazaar.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/character.py` & `tibia.py-6.3.0/tibiapy/builders/character.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/creature.py` & `tibia.py-6.3.0/tibiapy/builders/creature.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/event.py` & `tibia.py-6.3.0/tibiapy/builders/event.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/forum.py` & `tibia.py-6.3.0/tibiapy/builders/forum.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/guild.py` & `tibia.py-6.3.0/tibiapy/builders/guild.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/highscores.py` & `tibia.py-6.3.0/tibiapy/builders/highscores.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/house.py` & `tibia.py-6.3.0/tibiapy/builders/house.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/kill_statistics.py` & `tibia.py-6.3.0/tibiapy/builders/kill_statistics.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/leaderboard.py` & `tibia.py-6.3.0/tibiapy/builders/leaderboard.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/news.py` & `tibia.py-6.3.0/tibiapy/builders/news.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/spell.py` & `tibia.py-6.3.0/tibiapy/builders/spell.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/builders/world.py` & `tibia.py-6.3.0/tibiapy/builders/world.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/client.py` & `tibia.py-6.3.0/tibiapy/client.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/enums.py` & `tibia.py-6.3.0/tibiapy/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,8 +572,9 @@
 
 
 class WorldLocation(StringEnum):
     """The possible physical locations for servers."""
 
     EUROPE = "Europe"
     NORTH_AMERICA = "North America"
+    OCEANIA = "Oceania"
     SOUTH_AMERICA = "South America"
```

### Comparing `tibia.py-6.2.0/tibiapy/errors.py` & `tibia.py-6.3.0/tibiapy/errors.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/__init__.py` & `tibia.py-6.3.0/tibiapy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/base.py` & `tibia.py-6.3.0/tibiapy/models/base.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/bazaar.py` & `tibia.py-6.3.0/tibiapy/models/bazaar.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/character.py` & `tibia.py-6.3.0/tibiapy/models/character.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/creature.py` & `tibia.py-6.3.0/tibiapy/models/creature.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/event.py` & `tibia.py-6.3.0/tibiapy/models/event.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/fansite.py` & `tibia.py-6.3.0/tibiapy/models/fansite.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/forum.py` & `tibia.py-6.3.0/tibiapy/models/forum.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/guild.py` & `tibia.py-6.3.0/tibiapy/models/guild.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/highscores.py` & `tibia.py-6.3.0/tibiapy/models/highscores.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/house.py` & `tibia.py-6.3.0/tibiapy/models/house.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/kill_statistics.py` & `tibia.py-6.3.0/tibiapy/models/kill_statistics.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/leaderboard.py` & `tibia.py-6.3.0/tibiapy/models/leaderboard.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/news.py` & `tibia.py-6.3.0/tibiapy/models/news.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/pagination.py` & `tibia.py-6.3.0/tibiapy/models/pagination.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/spell.py` & `tibia.py-6.3.0/tibiapy/models/spell.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/tibia_response.py` & `tibia.py-6.3.0/tibiapy/models/tibia_response.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/models/world.py` & `tibia.py-6.3.0/tibiapy/models/world.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/__init__.py` & `tibia.py-6.3.0/tibiapy/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/bazaar.py` & `tibia.py-6.3.0/tibiapy/parsers/bazaar.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/character.py` & `tibia.py-6.3.0/tibiapy/parsers/character.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/creature.py` & `tibia.py-6.3.0/tibiapy/parsers/creature.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/event.py` & `tibia.py-6.3.0/tibiapy/parsers/event.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/fansite.py` & `tibia.py-6.3.0/tibiapy/parsers/fansite.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/forum.py` & `tibia.py-6.3.0/tibiapy/parsers/forum.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/guild.py` & `tibia.py-6.3.0/tibiapy/parsers/guild.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/highscores.py` & `tibia.py-6.3.0/tibiapy/parsers/highscores.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/house.py` & `tibia.py-6.3.0/tibiapy/parsers/house.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/kill_statistics.py` & `tibia.py-6.3.0/tibiapy/parsers/kill_statistics.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/leaderboard.py` & `tibia.py-6.3.0/tibiapy/parsers/leaderboard.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/news.py` & `tibia.py-6.3.0/tibiapy/parsers/news.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/spell.py` & `tibia.py-6.3.0/tibiapy/parsers/spell.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/parsers/world.py` & `tibia.py-6.3.0/tibiapy/parsers/world.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/urls.py` & `tibia.py-6.3.0/tibiapy/urls.py`

 * *Files identical despite different names*

### Comparing `tibia.py-6.2.0/tibiapy/utils.py` & `tibia.py-6.3.0/tibiapy/utils.py`

 * *Files identical despite different names*

