# Comparing `tmp/aiosu-2.3.0.tar.gz` & `tmp/aiosu-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosu-2.3.0.tar", max compression
+gzip compressed data, was "aiosu-2.3.1.tar", max compression
```

## Comparing `aiosu-2.3.0.tar` & `aiosu-2.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35149 2024-04-09 07:06:41.745397 aiosu-2.3.0/LICENSE
--rw-r--r--   0        0        0     3862 2024-04-09 07:06:41.745397 aiosu-2.3.0/README.rst
--rw-r--r--   0        0        0      682 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/__init__.py
--rw-r--r--   0        0        0     2292 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/events.py
--rw-r--r--   0        0        0     1053 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/exceptions.py
--rw-r--r--   0        0        0     3286 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/helpers.py
--rw-r--r--   0        0        0      655 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/__init__.py
--rw-r--r--   0        0        0     2717 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/artist.py
--rw-r--r--   0        0        0      407 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/backgrounds.py
--rw-r--r--   0        0        0     1335 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/base.py
--rw-r--r--   0        0        0    19824 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/beatmap.py
--rw-r--r--   0        0        0     2202 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/changelog.py
--rw-r--r--   0        0        0     1742 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/chat.py
--rw-r--r--   0        0        0     1762 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/comment.py
--rw-r--r--   0        0        0     3620 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/common.py
--rw-r--r--   0        0        0     1822 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/event.py
--rw-r--r--   0        0        0      104 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/files/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/files/replay.py
--rw-r--r--   0        0        0     1697 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/forum.py
--rw-r--r--   0        0        0     1903 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/gamemode.py
--rw-r--r--   0        0        0      764 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/kudosu.py
--rw-r--r--   0        0        0     6354 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/lazer.py
--rw-r--r--   0        0        0      133 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/legacy/__init__.py
--rw-r--r--   0        0        0     3442 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/legacy/match.py
--rw-r--r--   0        0        0      272 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/legacy/replay.py
--rw-r--r--   0        0        0     6425 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/mods.py
--rw-r--r--   0        0        0     4874 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/multiplayer.py
--rw-r--r--   0        0        0     1111 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/news.py
--rw-r--r--   0        0        0     1959 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/oauthtoken.py
--rw-r--r--   0        0        0      840 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/performance.py
--rw-r--r--   0        0        0      693 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/rankings.py
--rw-r--r--   0        0        0     1491 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/scopes.py
--rw-r--r--   0        0        0     7893 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/score.py
--rw-r--r--   0        0        0      590 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/search.py
--rw-r--r--   0        0        0      511 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/spotlight.py
--rw-r--r--   0        0        0    10766 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/user.py
--rw-r--r--   0        0        0      386 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/models/wiki.py
--rw-r--r--   0        0        0        0 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/py.typed
--rw-r--r--   0        0        0      218 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/__init__.py
--rw-r--r--   0        0        0     8721 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/accuracy.py
--rw-r--r--   0        0        0     2824 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/auth.py
--rw-r--r--   0        0        0     7976 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/binary.py
--rw-r--r--   0        0        0    22058 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/performance.py
--rw-r--r--   0        0        0     6230 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/utils/replay.py
--rw-r--r--   0        0        0       98 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v1/__init__.py
--rw-r--r--   0        0        0    18341 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v1/client.py
--rw-r--r--   0        0        0      146 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/__init__.py
--rw-r--r--   0        0        0   104324 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/client.py
--rw-r--r--   0        0        0     7792 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/clientstorage.py
--rw-r--r--   0        0        0       95 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/repository/__init__.py
--rw-r--r--   0        0        0     1906 2024-04-09 07:06:41.745397 aiosu-2.3.0/aiosu/v2/repository/oauthtoken.py
--rw-r--r--   0        0        0     2028 2024-04-09 07:06:41.749397 aiosu-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 aiosu-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-10 14:25:14.603444 aiosu-2.3.1/LICENSE
+-rw-r--r--   0        0        0     3862 2024-04-10 14:25:14.603444 aiosu-2.3.1/README.rst
+-rw-r--r--   0        0        0      682 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/__init__.py
+-rw-r--r--   0        0        0     2292 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/events.py
+-rw-r--r--   0        0        0     1053 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/exceptions.py
+-rw-r--r--   0        0        0     3286 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/helpers.py
+-rw-r--r--   0        0        0      655 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/__init__.py
+-rw-r--r--   0        0        0     2717 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/artist.py
+-rw-r--r--   0        0        0      407 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/backgrounds.py
+-rw-r--r--   0        0        0     1335 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/base.py
+-rw-r--r--   0        0        0    19824 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/beatmap.py
+-rw-r--r--   0        0        0     2202 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/changelog.py
+-rw-r--r--   0        0        0     1742 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/chat.py
+-rw-r--r--   0        0        0     1762 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/comment.py
+-rw-r--r--   0        0        0     3637 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/common.py
+-rw-r--r--   0        0        0     1822 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/event.py
+-rw-r--r--   0        0        0      104 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/files/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/files/replay.py
+-rw-r--r--   0        0        0     1697 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/forum.py
+-rw-r--r--   0        0        0     1903 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/gamemode.py
+-rw-r--r--   0        0        0      764 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/kudosu.py
+-rw-r--r--   0        0        0     6354 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/lazer.py
+-rw-r--r--   0        0        0      133 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/legacy/__init__.py
+-rw-r--r--   0        0        0     3442 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/legacy/match.py
+-rw-r--r--   0        0        0      272 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/legacy/replay.py
+-rw-r--r--   0        0        0     6425 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/mods.py
+-rw-r--r--   0        0        0     4874 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/multiplayer.py
+-rw-r--r--   0        0        0     1111 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/news.py
+-rw-r--r--   0        0        0     1959 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/oauthtoken.py
+-rw-r--r--   0        0        0      840 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/performance.py
+-rw-r--r--   0        0        0      693 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/rankings.py
+-rw-r--r--   0        0        0     1491 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/scopes.py
+-rw-r--r--   0        0        0     7893 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/score.py
+-rw-r--r--   0        0        0      590 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/search.py
+-rw-r--r--   0        0        0      511 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/spotlight.py
+-rw-r--r--   0        0        0    10766 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/user.py
+-rw-r--r--   0        0        0      386 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/models/wiki.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/py.typed
+-rw-r--r--   0        0        0      218 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/utils/__init__.py
+-rw-r--r--   0        0        0     8721 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/utils/accuracy.py
+-rw-r--r--   0        0        0     2824 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/utils/auth.py
+-rw-r--r--   0        0        0     7976 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/utils/binary.py
+-rw-r--r--   0        0        0    22058 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/utils/performance.py
+-rw-r--r--   0        0        0     6230 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/utils/replay.py
+-rw-r--r--   0        0        0       98 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/v1/__init__.py
+-rw-r--r--   0        0        0    18341 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/v1/client.py
+-rw-r--r--   0        0        0      146 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/v2/__init__.py
+-rw-r--r--   0        0        0   104324 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/v2/client.py
+-rw-r--r--   0        0        0     7792 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/v2/clientstorage.py
+-rw-r--r--   0        0        0       95 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/v2/repository/__init__.py
+-rw-r--r--   0        0        0     1906 2024-04-10 14:25:14.603444 aiosu-2.3.1/aiosu/v2/repository/oauthtoken.py
+-rw-r--r--   0        0        0     2028 2024-04-10 14:25:14.607444 aiosu-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 aiosu-2.3.1/PKG-INFO
```

### Comparing `aiosu-2.3.0/LICENSE` & `aiosu-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/README.rst` & `aiosu-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/__init__.py` & `aiosu-2.3.1/aiosu/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/events.py` & `aiosu-2.3.1/aiosu/events.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/exceptions.py` & `aiosu-2.3.1/aiosu/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/helpers.py` & `aiosu-2.3.1/aiosu/helpers.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/__init__.py` & `aiosu-2.3.1/aiosu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/artist.py` & `aiosu-2.3.1/aiosu/models/artist.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/base.py` & `aiosu-2.3.1/aiosu/models/base.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/beatmap.py` & `aiosu-2.3.1/aiosu/models/beatmap.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/changelog.py` & `aiosu-2.3.1/aiosu/models/changelog.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/chat.py` & `aiosu-2.3.1/aiosu/models/chat.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/comment.py` & `aiosu-2.3.1/aiosu/models/comment.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/common.py` & `aiosu-2.3.1/aiosu/models/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     raw: Optional[str] = None
     bbcode: Optional[str] = None
 
 
 class PinAttributes(BaseModel):
     is_pinned: bool
     score_id: int
-    score_type: ScoreType
+    score_type: Optional[ScoreType] = None
 
 
 class CurrentUserAttributes(BaseModel):
     can_beatmap_update_owner: Optional[bool] = None
     can_delete: Optional[bool] = None
     can_edit_metadata: Optional[bool] = None
     can_edit_tags: Optional[bool] = None
```

### Comparing `aiosu-2.3.0/aiosu/models/event.py` & `aiosu-2.3.1/aiosu/models/event.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/files/replay.py` & `aiosu-2.3.1/aiosu/models/files/replay.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/forum.py` & `aiosu-2.3.1/aiosu/models/forum.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/gamemode.py` & `aiosu-2.3.1/aiosu/models/gamemode.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/kudosu.py` & `aiosu-2.3.1/aiosu/models/kudosu.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/lazer.py` & `aiosu-2.3.1/aiosu/models/lazer.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/legacy/match.py` & `aiosu-2.3.1/aiosu/models/legacy/match.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/mods.py` & `aiosu-2.3.1/aiosu/models/mods.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/multiplayer.py` & `aiosu-2.3.1/aiosu/models/multiplayer.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/news.py` & `aiosu-2.3.1/aiosu/models/news.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/oauthtoken.py` & `aiosu-2.3.1/aiosu/models/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/performance.py` & `aiosu-2.3.1/aiosu/models/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/rankings.py` & `aiosu-2.3.1/aiosu/models/rankings.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/scopes.py` & `aiosu-2.3.1/aiosu/models/scopes.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/score.py` & `aiosu-2.3.1/aiosu/models/score.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/search.py` & `aiosu-2.3.1/aiosu/models/search.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/models/user.py` & `aiosu-2.3.1/aiosu/models/user.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/utils/accuracy.py` & `aiosu-2.3.1/aiosu/utils/accuracy.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/utils/auth.py` & `aiosu-2.3.1/aiosu/utils/auth.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/utils/binary.py` & `aiosu-2.3.1/aiosu/utils/binary.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/utils/performance.py` & `aiosu-2.3.1/aiosu/utils/performance.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/utils/replay.py` & `aiosu-2.3.1/aiosu/utils/replay.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/v1/client.py` & `aiosu-2.3.1/aiosu/v1/client.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/v2/client.py` & `aiosu-2.3.1/aiosu/v2/client.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/v2/clientstorage.py` & `aiosu-2.3.1/aiosu/v2/clientstorage.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/aiosu/v2/repository/oauthtoken.py` & `aiosu-2.3.1/aiosu/v2/repository/oauthtoken.py`

 * *Files identical despite different names*

### Comparing `aiosu-2.3.0/pyproject.toml` & `aiosu-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 profile = "black"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.poetry]
 name = "aiosu"
-version = "2.3.0"
+version = "2.3.1"
 description = "Simple and fast osu! API v1 and v2 library"
 authors = ["Nice Aesthetics <nice@aesth.dev>"]
 license = "GPLv3+"
 readme = "README.rst"
 repository = "https://github.com/NiceAesth/aiosu"
 documentation = "https://aiosu.readthedocs.io/"
 keywords = ["osu!", "osu", "api"]
```

### Comparing `aiosu-2.3.0/PKG-INFO` & `aiosu-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosu
-Version: 2.3.0
+Version: 2.3.1
 Summary: Simple and fast osu! API v1 and v2 library
 Home-page: https://github.com/NiceAesth/aiosu
 License: GPLv3+
 Keywords: osu!,osu,api
 Author: Nice Aesthetics
 Author-email: nice@aesth.dev
 Requires-Python: >=3.9,<4.0
```

