# Comparing `tmp/tweety-ns-1.1.1b0.tar.gz` & `tmp/tweety-ns-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-1.1.1b0.tar", last modified: Thu Apr  4 20:58:11 2024, max compression
+gzip compressed data, was "tweety-ns-1.1.2.tar", last modified: Wed Apr 10 16:36:42 2024, max compression
```

## Comparing `tweety-ns-1.1.1b0.tar` & `tweety-ns-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-04 20:58:11.769182 tweety-ns-1.1.1b0/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1893 2024-04-04 20:58:11.769182 tweety-ns-1.1.1b0/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety-ns-1.1.1b0/README.md
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-1.1.1b0/pyproject.toml
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      673 2024-04-04 20:58:11.769182 tweety-ns-1.1.1b0/setup.cfg
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      787 2024-04-04 20:57:38.000000 tweety-ns-1.1.1b0/setup.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-04 20:58:11.757182 tweety-ns-1.1.1b0/src/
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-04 20:58:11.761182 tweety-ns-1.1.1b0/src/tweety/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      278 2024-04-04 20:57:25.000000 tweety-ns-1.1.1b0/src/tweety/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7504 2024-03-04 12:19:25.000000 tweety-ns-1.1.1b0/src/tweety/auth.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31680 2024-03-20 05:30:39.000000 tweety-ns-1.1.1b0/src/tweety/bot.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    95767 2024-03-20 11:19:15.000000 tweety-ns-1.1.1b0/src/tweety/builder.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-04 20:58:11.761182 tweety-ns-1.1.1b0/src/tweety/events/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety-ns-1.1.1b0/src/tweety/events/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2119 2024-03-31 11:29:17.000000 tweety-ns-1.1.1b0/src/tweety/events/newmessage.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    21984 2024-03-19 11:58:49.000000 tweety-ns-1.1.1b0/src/tweety/exceptions_.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2341 2024-03-03 15:25:23.000000 tweety-ns-1.1.1b0/src/tweety/filters.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20098 2024-03-20 05:50:42.000000 tweety-ns-1.1.1b0/src/tweety/http.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1844 2024-03-20 17:15:35.000000 tweety-ns-1.1.1b0/src/tweety/session.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-04 20:58:11.765182 tweety-ns-1.1.1b0/src/tweety/types/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety-ns-1.1.1b0/src/tweety/types/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3039 2024-02-12 12:06:11.000000 tweety-ns-1.1.1b0/src/tweety/types/base.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety-ns-1.1.1b0/src/tweety/types/bookmarks.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety-ns-1.1.1b0/src/tweety/types/community.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety-ns-1.1.1b0/src/tweety/types/follow.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety-ns-1.1.1b0/src/tweety/types/gifs.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    17540 2024-04-04 20:48:50.000000 tweety-ns-1.1.1b0/src/tweety/types/inbox.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety-ns-1.1.1b0/src/tweety/types/likes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety-ns-1.1.1b0/src/tweety/types/lists.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety-ns-1.1.1b0/src/tweety/types/mentions.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9019 2024-03-20 17:11:54.000000 tweety-ns-1.1.1b0/src/tweety/types/n_types.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety-ns-1.1.1b0/src/tweety/types/notification.py
--rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety-ns-1.1.1b0/src/tweety/types/places.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety-ns-1.1.1b0/src/tweety/types/retweets.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety-ns-1.1.1b0/src/tweety/types/search.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety-ns-1.1.1b0/src/tweety/types/topic.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58413 2024-03-27 06:41:42.000000 tweety-ns-1.1.1b0/src/tweety/types/twDataTypes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-03-18 07:58:43.000000 tweety-ns-1.1.1b0/src/tweety/types/usertweet.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety-ns-1.1.1b0/src/tweety/updates.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36036 2024-03-20 05:54:31.000000 tweety-ns-1.1.1b0/src/tweety/user.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6192 2024-03-04 11:48:15.000000 tweety-ns-1.1.1b0/src/tweety/utils.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-04 20:58:11.769182 tweety-ns-1.1.1b0/src/tweety_ns.egg-info/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1893 2024-04-04 20:58:11.000000 tweety-ns-1.1.1b0/src/tweety_ns.egg-info/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-04 20:58:11.000000 tweety-ns-1.1.1b0/src/tweety_ns.egg-info/SOURCES.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-04 20:58:11.000000 tweety-ns-1.1.1b0/src/tweety_ns.egg-info/dependency_links.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-04 20:58:11.000000 tweety-ns-1.1.1b0/src/tweety_ns.egg-info/requires.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-04 20:58:11.000000 tweety-ns-1.1.1b0/src/tweety_ns.egg-info/top_level.txt
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety-ns-1.1.2/README.md
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-1.1.2/pyproject.toml
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/setup.cfg
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-10 16:36:05.000000 tweety-ns-1.1.2/setup.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.181096 tweety-ns-1.1.2/src/
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.185096 tweety-ns-1.1.2/src/tweety/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-10 16:35:52.000000 tweety-ns-1.1.2/src/tweety/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7504 2024-03-04 12:19:25.000000 tweety-ns-1.1.2/src/tweety/auth.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31876 2024-04-10 16:30:28.000000 tweety-ns-1.1.2/src/tweety/bot.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    95767 2024-03-20 11:19:15.000000 tweety-ns-1.1.2/src/tweety/builder.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.185096 tweety-ns-1.1.2/src/tweety/events/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety-ns-1.1.2/src/tweety/events/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2119 2024-03-31 11:29:17.000000 tweety-ns-1.1.2/src/tweety/events/newmessage.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22014 2024-04-10 16:25:45.000000 tweety-ns-1.1.2/src/tweety/exceptions_.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2341 2024-03-03 15:25:23.000000 tweety-ns-1.1.2/src/tweety/filters.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20098 2024-03-20 05:50:42.000000 tweety-ns-1.1.2/src/tweety/http.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety-ns-1.1.2/src/tweety/session.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/src/tweety/types/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety-ns-1.1.2/src/tweety/types/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3039 2024-02-12 12:06:11.000000 tweety-ns-1.1.2/src/tweety/types/base.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety-ns-1.1.2/src/tweety/types/bookmarks.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety-ns-1.1.2/src/tweety/types/community.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety-ns-1.1.2/src/tweety/types/follow.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety-ns-1.1.2/src/tweety/types/gifs.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    17540 2024-04-04 20:48:50.000000 tweety-ns-1.1.2/src/tweety/types/inbox.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety-ns-1.1.2/src/tweety/types/likes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety-ns-1.1.2/src/tweety/types/lists.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety-ns-1.1.2/src/tweety/types/mentions.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9022 2024-04-10 16:29:13.000000 tweety-ns-1.1.2/src/tweety/types/n_types.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety-ns-1.1.2/src/tweety/types/notification.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety-ns-1.1.2/src/tweety/types/places.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety-ns-1.1.2/src/tweety/types/retweets.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety-ns-1.1.2/src/tweety/types/search.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety-ns-1.1.2/src/tweety/types/topic.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58413 2024-03-27 06:41:42.000000 tweety-ns-1.1.2/src/tweety/types/twDataTypes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-03-18 07:58:43.000000 tweety-ns-1.1.2/src/tweety/types/usertweet.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety-ns-1.1.2/src/tweety/updates.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36036 2024-03-20 05:54:31.000000 tweety-ns-1.1.2/src/tweety/user.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6192 2024-03-04 11:48:15.000000 tweety-ns-1.1.2/src/tweety/utils.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/src/tweety_ns.egg-info/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/requires.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-1.1.1b0/PKG-INFO` & `tweety-ns-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.1b0
+Version: 1.1.2
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-1.1.1b0/README.md` & `tweety-ns-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/setup.cfg` & `tweety-ns-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tweety-ns
-version = 1.1.1b0
+version = 1.1.2
 author = Tayyab Kharl
 author_email = tayyabmahr@gmail.com
 description = An easy Twitter Scraper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mahrtayyab/tweety
 project_urls =
```

### Comparing `tweety-ns-1.1.1b0/setup.py` & `tweety-ns-1.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types', 'tweety.events'],
-    version='1.1.1b0',
+    version='1.1.2',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
```

### Comparing `tweety-ns-1.1.1b0/src/tweety/auth.py` & `tweety-ns-1.1.2/src/tweety/auth.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/bot.py` & `tweety-ns-1.1.2/src/tweety/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import warnings
 from typing import Union
 from .utils import find_objects, AuthRequired, get_user_from_typehead, get_tweet_id
 from .types import (Proxy, TweetComments, UserTweets, Search, User, Tweet, Trends, Community, CommunityTweets,
                     CommunityMembers, UserFollowers, UserFollowings, TweetHistory, UserMedia, GifSearch,
                     ShortUser, TypeHeadSearch, TweetTranslate, AudioSpace, UserHighlights, UserLikes, Places)
 from .exceptions_ import *
-from .session import Session
+from .session import Session, MemorySession, FileSession
 from .http import Request
 
 
 class BotMethods:
     LOGIN_URL = "https://api.twitter.com/1.1/onboarding/task.json?flow_name=login"
 
     def __init__(self, session_name: Union[str, Session], proxy: Union[dict, Proxy] = None, **httpx_kwargs):
@@ -26,17 +26,23 @@
         self._password = None
         self._extra = None
         self._login_flow = None
         self._login_flow_state = None
         self._last_json = {}
         self._cached_users = {}
         self._proxy = proxy.get_dict() if isinstance(proxy, Proxy) else proxy
-
         self._event_builders = []
-        self.session = Session(self, session_name) if isinstance(session_name, str) else session_name
+
+        if isinstance(session_name, MemorySession):
+            self.session = session_name(self)
+        elif isinstance(session_name, FileSession):
+            self.session = session_name
+        else:
+            self.session = FileSession(self, session_name)
+
         self.logged_in = False
         self.request = self.http = Request(self, max_retries=10, proxy=self._proxy, **httpx_kwargs)
         self.user = None
 
     def get_user_info(self, username: Union[str, int, list] = None):
         """
         Get the User Info of the specified username
```

### Comparing `tweety-ns-1.1.1b0/src/tweety/builder.py` & `tweety-ns-1.1.2/src/tweety/builder.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/events/newmessage.py` & `tweety-ns-1.1.2/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/exceptions_.py` & `tweety-ns-1.1.2/src/tweety/exceptions_.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             message
     ):
         self.message = message
         self.error_code = error_code
         self.error_name = error_name
         self.response = response
 
-        if not isinstance(self.response, dict) and not self.response.json_() and self.response.text:
+        if self.response is not None and not isinstance(self.response, dict) and not self.response.json_() and self.response.text:
             self.message = self.response.text
         elif str(self.error_code) == "404":
             self.message = "Page not Found. Most likely you need elevated authorization to access this resource"
 
         super().__init__(self.message)
```

### Comparing `tweety-ns-1.1.1b0/src/tweety/filters.py` & `tweety-ns-1.1.2/src/tweety/filters.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/http.py` & `tweety-ns-1.1.2/src/tweety/http.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/session.py` & `tweety-ns-1.1.2/src/tweety/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,63 @@
 import json
 import os.path
 
 
 class Session:
-    def __init__(self, client, session_name):
+    def __init__(self, client):
         self._client = client
         self.user = None
-        self.session_name = os.path.basename(session_name)
-        self.session_file_path = self._get_session_file_path(session_name, self.session_name)
         self.logged_in = False
         self.cookies = ""
+
+    def cookies_dict(self):
+        result = {}
+        split = str(self.cookies).split(";")
+        for i in split:
+            try:
+                key, value = i.split("=")
+                result[key] = value
+            except:
+                pass
+
+        return result
+
+    def __str__(self):
+        return self.cookies
+
+
+class MemorySession(Session):
+
+    def __init__(self):
+        super().__init__(None)
+
+    def __call__(self, client):
+        self._client = client
+        return self
+
+    def set_session_user(self, user):
+        self.user = dict(user)
+
+    def save_session(self, cookies):
+        self.cookies = str(cookies)
+        self.logged_in = True
+
+
+class FileSession(Session):
+    def __init__(self, client, session_name):
+        super().__init__(client)
+        self.session_name = os.path.basename(session_name)
+        self.session_file_path = self._get_session_file_path(session_name, self.session_name)
         self._load_session()
 
     @staticmethod
     def _get_session_file_path(session_path, session_name):
+        _session = session_name.replace(".tw_session", "")
         directory = os.path.dirname(session_path) or os.getcwd()
-        return os.path.abspath(os.path.join(directory, f"{session_name}.tw_session"))
+        return os.path.abspath(os.path.join(directory, f"{_session}.tw_session"))
 
     def _load_session(self):
         if os.path.exists(self.session_file_path):
             with open(self.session_file_path, "r") as f:
                 session_data = json.load(f)
                 self.cookies = session_data['cookies']
                 self.user = session_data['user']
@@ -36,22 +74,7 @@
     def save_session(self, cookies):
         self.cookies = str(cookies)
         self.logged_in = True
         with open(self.session_file_path, "w") as f:
             session_data = dict(cookies=str(cookies))
             json.dump(session_data, f, indent=4)
 
-    def cookies_dict(self):
-        result = {}
-        split = str(self.cookies).split(";")
-        for i in split:
-            try:
-                key, value = i.split("=")
-                result[key] = value
-            except:
-                pass
-
-        return result
-
-    def __str__(self):
-        return self.cookies
-
```

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/__init__.py` & `tweety-ns-1.1.2/src/tweety/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/base.py` & `tweety-ns-1.1.2/src/tweety/types/base.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/bookmarks.py` & `tweety-ns-1.1.2/src/tweety/types/bookmarks.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/community.py` & `tweety-ns-1.1.2/src/tweety/types/community.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/follow.py` & `tweety-ns-1.1.2/src/tweety/types/follow.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/gifs.py` & `tweety-ns-1.1.2/src/tweety/types/gifs.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/inbox.py` & `tweety-ns-1.1.2/src/tweety/types/inbox.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/likes.py` & `tweety-ns-1.1.2/src/tweety/types/likes.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/lists.py` & `tweety-ns-1.1.2/src/tweety/types/lists.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/mentions.py` & `tweety-ns-1.1.2/src/tweety/types/mentions.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/n_types.py` & `tweety-ns-1.1.2/src/tweety/types/n_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                         key, value = str(p.split(';')[0]).split("=", 1)
                         setattr(self, key.strip(), value.strip())
             else:
                 true_cookies = dict()
                 if isinstance(self._raw_cookies, str):
                     cookie_list = self._raw_cookies.split(";")
                     for cookie in cookie_list:
-                        split_cookie = cookie.strip().split("=")
+                        split_cookie = cookie.strip().split("=", 1)
 
                         if len(split_cookie) >= 2:
                             cookie_key = split_cookie[0]
                             cookie_value = split_cookie[1]
                             true_cookies[cookie_key] = cookie_value
                 elif isinstance(self._raw_cookies, dict):
                     true_cookies = self._raw_cookies
```

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/notification.py` & `tweety-ns-1.1.2/src/tweety/types/notification.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/places.py` & `tweety-ns-1.1.2/src/tweety/types/places.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/retweets.py` & `tweety-ns-1.1.2/src/tweety/types/retweets.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/search.py` & `tweety-ns-1.1.2/src/tweety/types/search.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/topic.py` & `tweety-ns-1.1.2/src/tweety/types/topic.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/twDataTypes.py` & `tweety-ns-1.1.2/src/tweety/types/twDataTypes.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/types/usertweet.py` & `tweety-ns-1.1.2/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/user.py` & `tweety-ns-1.1.2/src/tweety/user.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety/utils.py` & `tweety-ns-1.1.2/src/tweety/utils.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1b0/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-1.1.2/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.1b0
+Version: 1.1.2
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-1.1.1b0/src/tweety_ns.egg-info/SOURCES.txt` & `tweety-ns-1.1.2/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

