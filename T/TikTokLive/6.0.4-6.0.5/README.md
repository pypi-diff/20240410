# Comparing `tmp/TikTokLive-6.0.4.tar.gz` & `tmp/TikTokLive-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/isaackogan/PycharmProjects/TikTokLive/dist/.tmp-imn6ynu3/TikTokLive-6.0.4.tar", last modified: Mon Apr  8 20:01:17 2024, max compression
+gzip compressed data, was "/Users/isaackogan/PycharmProjects/TikTokLive/dist/.tmp-7z108tdr/TikTokLive-6.0.5.tar", last modified: Wed Apr 10 04:51:42 2024, max compression
```

## Comparing `TikTokLive-6.0.4.tar` & `TikTokLive-6.0.5.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.894157 TikTokLive-6.0.4/
--rw-r--r--   0 isaackogan   (501) staff       (20)     1068 2024-02-22 06:19:06.000000 TikTokLive-6.0.4/LICENSE
--rw-r--r--   0 isaackogan   (501) staff       (20)    17700 2024-04-08 20:01:17.893797 TikTokLive-6.0.4/PKG-INFO
--rw-r--r--   0 isaackogan   (501) staff       (20)    16568 2024-04-01 02:18:03.000000 TikTokLive-6.0.4/README.md
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.878011 TikTokLive-6.0.4/TikTokLive/
--rw-r--r--   0 isaackogan   (501) staff       (20)       43 2024-02-22 03:47:28.000000 TikTokLive-6.0.4/TikTokLive/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.880232 TikTokLive-6.0.4/TikTokLive/client/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-11 08:02:27.000000 TikTokLive-6.0.4/TikTokLive/client/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    16353 2024-04-08 19:55:17.000000 TikTokLive-6.0.4/TikTokLive/client/client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      658 2024-04-01 02:16:57.000000 TikTokLive-6.0.4/TikTokLive/client/errors.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4209 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/logger.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.881298 TikTokLive-6.0.4/TikTokLive/client/web/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-20 23:59:08.000000 TikTokLive-6.0.4/TikTokLive/client/web/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.884333 TikTokLive-6.0.4/TikTokLive/client/web/routes/
--rw-r--r--   0 isaackogan   (501) staff       (20)      303 2024-04-08 19:26:24.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      925 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_gift_list.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      619 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_image.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2355 2024-04-08 19:57:30.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_is_live.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2803 2024-04-08 19:57:30.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_id_api.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1889 2024-04-08 19:26:01.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_id_html.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1424 2024-04-08 19:50:54.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_info.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     5209 2024-04-03 17:28:04.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_sign.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     6065 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_video.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4918 2024-04-08 19:22:45.000000 TikTokLive-6.0.4/TikTokLive/client/web/web_base.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1532 2024-04-08 19:57:30.000000 TikTokLive-6.0.4/TikTokLive/client/web/web_client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2607 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/client/web/web_settings.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.884686 TikTokLive-6.0.4/TikTokLive/client/ws/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2024-02-03 19:50:49.000000 TikTokLive-6.0.4/TikTokLive/client/ws/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7748 2024-03-22 01:02:42.000000 TikTokLive-6.0.4/TikTokLive/client/ws/ws_client.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.886070 TikTokLive-6.0.4/TikTokLive/events/
--rw-r--r--   0 isaackogan   (501) staff       (20)      567 2024-02-22 06:22:04.000000 TikTokLive-6.0.4/TikTokLive/events/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      439 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/events/base_event.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2316 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLive/events/custom_events.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7061 2024-02-28 19:23:41.000000 TikTokLive-6.0.4/TikTokLive/events/proto_events.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.887176 TikTokLive-6.0.4/TikTokLive/proto/
--rw-r--r--   0 isaackogan   (501) staff       (20)       55 2024-02-04 07:15:00.000000 TikTokLive-6.0.4/TikTokLive/proto/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1819 2024-02-28 18:54:40.000000 TikTokLive-6.0.4/TikTokLive/proto/custom_proto.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    98737 2024-02-04 08:14:43.000000 TikTokLive-6.0.4/TikTokLive/proto/tiktok_proto.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.893387 TikTokLive-6.0.4/TikTokLive.egg-info/
--rw-r--r--   0 isaackogan   (501) staff       (20)    17700 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/PKG-INFO
--rw-r--r--   0 isaackogan   (501) staff       (20)     1732 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/SOURCES.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)        1 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/dependency_links.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)      162 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/requires.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)       28 2024-04-08 20:01:17.000000 TikTokLive-6.0.4/TikTokLive.egg-info/top_level.txt
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.888722 TikTokLive-6.0.4/TikTokLiveLegacy/
--rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.890691 TikTokLive-6.0.4/TikTokLiveLegacy/client/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    22144 2024-03-22 00:18:26.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/base.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7425 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2032 2024-02-17 18:22:43.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/config.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    10349 2024-02-22 06:31:30.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/httpx.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4736 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/client/wsclient.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.891751 TikTokLive-6.0.4/TikTokLiveLegacy/proto/
--rw-r--r--   0 isaackogan   (501) staff       (20)       50 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/proto/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    46393 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/proto/tiktok_schema_pb2.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     3003 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/proto/utilities.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-08 20:01:17.892996 TikTokLive-6.0.4/TikTokLiveLegacy/types/
--rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     3362 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/errors.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    16175 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/events.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    15122 2024-02-22 06:29:21.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/objects.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1023 2023-06-16 17:56:57.000000 TikTokLive-6.0.4/TikTokLiveLegacy/types/utilities.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1350 2024-02-24 20:23:34.000000 TikTokLive-6.0.4/TikTokLiveLegacy/utilities.py
--rw-r--r--   0 isaackogan   (501) staff       (20)       38 2024-04-08 20:01:17.894212 TikTokLive-6.0.4/setup.cfg
--rw-r--r--   0 isaackogan   (501) staff       (20)     1937 2024-04-08 20:00:14.000000 TikTokLive-6.0.4/setup.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.188356 TikTokLive-6.0.5/
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1068 2024-02-22 06:19:06.000000 TikTokLive-6.0.5/LICENSE
+-rw-r--r--   0 isaackogan   (501) staff       (20)    17683 2024-04-10 04:51:42.188045 TikTokLive-6.0.5/PKG-INFO
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16551 2024-04-08 20:25:06.000000 TikTokLive-6.0.5/README.md
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.173507 TikTokLive-6.0.5/TikTokLive/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       43 2024-02-22 03:47:28.000000 TikTokLive-6.0.5/TikTokLive/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.175511 TikTokLive-6.0.5/TikTokLive/client/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-11 08:02:27.000000 TikTokLive-6.0.5/TikTokLive/client/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16401 2024-04-10 00:48:55.000000 TikTokLive-6.0.5/TikTokLive/client/client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      659 2024-04-08 20:08:19.000000 TikTokLive-6.0.5/TikTokLive/client/errors.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4209 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/logger.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.176403 TikTokLive-6.0.5/TikTokLive/client/web/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-20 23:59:08.000000 TikTokLive-6.0.5/TikTokLive/client/web/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.179626 TikTokLive-6.0.5/TikTokLive/client/web/routes/
+-rw-r--r--   0 isaackogan   (501) staff       (20)      303 2024-04-08 19:26:24.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      925 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_gift_list.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      619 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_image.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2355 2024-04-08 19:57:30.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_is_live.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2803 2024-04-08 19:57:30.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_api.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1889 2024-04-08 19:26:01.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_html.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1424 2024-04-08 19:50:54.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_info.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     5209 2024-04-03 17:28:04.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_sign.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     6065 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_video.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4918 2024-04-08 19:22:45.000000 TikTokLive-6.0.5/TikTokLive/client/web/web_base.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1532 2024-04-08 19:57:30.000000 TikTokLive-6.0.5/TikTokLive/client/web/web_client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2607 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/web_settings.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.179890 TikTokLive-6.0.5/TikTokLive/client/ws/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2024-02-03 19:50:49.000000 TikTokLive-6.0.5/TikTokLive/client/ws/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7748 2024-03-22 01:02:42.000000 TikTokLive-6.0.5/TikTokLive/client/ws/ws_client.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.180814 TikTokLive-6.0.5/TikTokLive/events/
+-rw-r--r--   0 isaackogan   (501) staff       (20)      567 2024-02-22 06:22:04.000000 TikTokLive-6.0.5/TikTokLive/events/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      439 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/events/base_event.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2316 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/events/custom_events.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7061 2024-02-28 19:23:41.000000 TikTokLive-6.0.5/TikTokLive/events/proto_events.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.181971 TikTokLive-6.0.5/TikTokLive/proto/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       55 2024-02-04 07:15:00.000000 TikTokLive-6.0.5/TikTokLive/proto/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     5166 2024-04-10 04:48:50.000000 TikTokLive-6.0.5/TikTokLive/proto/custom_proto.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2603 2024-04-10 04:24:02.000000 TikTokLive-6.0.5/TikTokLive/proto/proto_utils.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    98737 2024-02-04 08:14:43.000000 TikTokLive-6.0.5/TikTokLive/proto/tiktok_proto.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.187739 TikTokLive-6.0.5/TikTokLive.egg-info/
+-rw-r--r--   0 isaackogan   (501) staff       (20)    17683 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/PKG-INFO
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1764 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/SOURCES.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)        1 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/dependency_links.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)      162 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/requires.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)       28 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/top_level.txt
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.183157 TikTokLive-6.0.5/TikTokLiveLegacy/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.185074 TikTokLive-6.0.5/TikTokLiveLegacy/client/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    22144 2024-03-22 00:18:26.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/base.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7425 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2032 2024-02-17 18:22:43.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/config.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    10349 2024-02-22 06:31:30.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/httpx.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4736 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/wsclient.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.186145 TikTokLive-6.0.5/TikTokLiveLegacy/proto/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       50 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/proto/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    46393 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/proto/tiktok_schema_pb2.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     3003 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/proto/utilities.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.187389 TikTokLive-6.0.5/TikTokLiveLegacy/types/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     3362 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/errors.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16175 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/events.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    15122 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/objects.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1023 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/utilities.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1350 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLiveLegacy/utilities.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)       38 2024-04-10 04:51:42.188403 TikTokLive-6.0.5/setup.cfg
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1937 2024-04-10 04:51:36.000000 TikTokLive-6.0.5/setup.py
```

### Comparing `TikTokLive-6.0.4/LICENSE` & `TikTokLive-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/PKG-INFO` & `TikTokLive-6.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TikTokLive
-Version: 6.0.4
+Version: 6.0.5
 Summary: TikTok Live Python Client
 Home-page: https://github.com/isaackogan/TikTokLive
-Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.4
+Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5
 Author: Isaac Kogan
 Author-email: info@isaackogan.com
 License: MIT
 Keywords: tiktok,tiktok live,python3,api,unofficial
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -260,33 +260,32 @@
 Using the low-level direct proto:
 ```python
 @client.on(GiftEvent)
 async def on_gift(event: GiftEvent):
     # If it's type 1 and the streak is over
     if event.gift.info.type == 1:
         if event.gift.is_repeating == 1:
-            print(f"{event.user.unique_id} sent {event.gift.count}x \"{event.gift.info.name}\"")
+            print(f"{event.user.unique_id} sent {event.repeat_count}x \"{event.gift.name}\"")
 
     # It's not type 1, which means it can't have a streak & is automatically over
     elif event.gift.info.type != 1:
-        print(f"{event.user.unique_id} sent \"{event.gift.info.name}\"")
+        print(f"{event.user.unique_id} sent \"{event.gift.name}\"")
 ```
 
 Using the TikTokLive extended proto:
 ```python
 @client.on("gift")
 async def on_gift(event: GiftEvent):
     # Streakable gift & streak is over
     if event.gift.streakable and not event.streaking:
-        print(f"{event.user.unique_id} sent {event.gift.count}x \"{event.gift.info.name}\"")
+        print(f"{event.user.unique_id} sent {event.repeat_count}x \"{event.gift.name}\"")
 
     # Non-streakable gift
     elif not event.gift.streakable:
-        print(f"{event.user.unique_id} sent \"{event.gift.info.name}\"")
-
+        print(f"{event.user.unique_id} sent \"{event.gift.name}\"")
 ```
 
 ### `SubscribeEvent`
 
 This event will only fire when a session ID (account login) is passed to the HTTP client *before* connecting to TikTok LIVE.
 You can set the session ID with [`client.web.set_session_id(...)`](https://github.com/isaackogan/TikTokLive/blob/master/examples/logged_in.py).
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.4 Summary: TikTok Live
+Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.5 Summary: TikTok Live
 Python Client Home-page: https://github.com/isaackogan/TikTokLive Download-URL:
-https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.4 Author: Isaac
+https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5 Author: Isaac
 Kogan Author-email: info@isaackogan.com License: MIT Keywords: tiktok,tiktok
 live,python3,api,unofficial Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -175,34 +175,33 @@
 this time new gift events are triggered again and again with an > increased
 `event.gift.repeat_count` value. It should be noted that after the end of a
 streak, a final gift event is > triggered, which signals the end of the streak
 with `event.repeat_end`:`1`. The following handlers show how you can deal with
 this in your code. Using the low-level direct proto: ```python @client.on
 (GiftEvent) async def on_gift(event: GiftEvent): # If it's type 1 and the
 streak is over if event.gift.info.type == 1: if event.gift.is_repeating == 1:
-print(f"{event.user.unique_id} sent {event.gift.count}x \"
-{event.gift.info.name}\"") # It's not type 1, which means it can't have a
-streak & is automatically over elif event.gift.info.type != 1: print(f"
-{event.user.unique_id} sent \"{event.gift.info.name}\"") ``` Using the
-TikTokLive extended proto: ```python @client.on("gift") async def on_gift
-(event: GiftEvent): # Streakable gift & streak is over if event.gift.streakable
-and not event.streaking: print(f"{event.user.unique_id} sent
-{event.gift.count}x \"{event.gift.info.name}\"") # Non-streakable gift elif not
-event.gift.streakable: print(f"{event.user.unique_id} sent \"
-{event.gift.info.name}\"") ``` ### `SubscribeEvent` This event will only fire
-when a session ID (account login) is passed to the HTTP client *before*
-connecting to TikTok LIVE. You can set the session ID with
-[`client.web.set_session_id(...)`](https://github.com/isaackogan/TikTokLive/
-blob/master/examples/logged_in.py). ## Checking If A User Is Live It is
-considered inefficient to use the connect method to check if a user is live. It
-is better to use the dedicated `await client.is_live()` method. There is a
-[complete example](https://github.com/isaackogan/TikTokLive/blob/master/
-examples/check_live.py) of how to do this in the [examples](https://github.com/
-isaackogan/TikTokLive/tree/master/examples) folder. ## Contributors * **Isaac
-Kogan** - *Creator, Primary Maintainer, and Reverse-Engineering* - [isaackogan]
-(https://github.com/isaackogan) * **Zerody** - *Initial Reverse-Engineering
-Protobuf & Support* - [Zerody](https://github.com/zerodytrash/) *
+print(f"{event.user.unique_id} sent {event.repeat_count}x \"
+{event.gift.name}\"") # It's not type 1, which means it can't have a streak &
+is automatically over elif event.gift.info.type != 1: print(f"
+{event.user.unique_id} sent \"{event.gift.name}\"") ``` Using the TikTokLive
+extended proto: ```python @client.on("gift") async def on_gift(event:
+GiftEvent): # Streakable gift & streak is over if event.gift.streakable and not
+event.streaking: print(f"{event.user.unique_id} sent {event.repeat_count}x \"
+{event.gift.name}\"") # Non-streakable gift elif not event.gift.streakable:
+print(f"{event.user.unique_id} sent \"{event.gift.name}\"") ``` ###
+`SubscribeEvent` This event will only fire when a session ID (account login) is
+passed to the HTTP client *before* connecting to TikTok LIVE. You can set the
+session ID with [`client.web.set_session_id(...)`](https://github.com/
+isaackogan/TikTokLive/blob/master/examples/logged_in.py). ## Checking If A User
+Is Live It is considered inefficient to use the connect method to check if a
+user is live. It is better to use the dedicated `await client.is_live()`
+method. There is a [complete example](https://github.com/isaackogan/TikTokLive/
+blob/master/examples/check_live.py) of how to do this in the [examples](https:/
+/github.com/isaackogan/TikTokLive/tree/master/examples) folder. ## Contributors
+* **Isaac Kogan** - *Creator, Primary Maintainer, and Reverse-Engineering* -
+[isaackogan](https://github.com/isaackogan) * **Zerody** - *Initial Reverse-
+Engineering Protobuf & Support* - [Zerody](https://github.com/zerodytrash/) *
 **Davincible** - *Reverse-Engineering Stream Downloads* - [davincible](https://
 github.com/davincible) See also the full list of [contributors](https://
 github.com/isaackogan/TikTokLive/contributors) who have participated in this
 project. ## License This project is licensed under the MIT License - see the
 [LICENSE](LICENSE) file for details.
```

### Comparing `TikTokLive-6.0.4/README.md` & `TikTokLive-6.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -229,33 +229,32 @@
 Using the low-level direct proto:
 ```python
 @client.on(GiftEvent)
 async def on_gift(event: GiftEvent):
     # If it's type 1 and the streak is over
     if event.gift.info.type == 1:
         if event.gift.is_repeating == 1:
-            print(f"{event.user.unique_id} sent {event.gift.count}x \"{event.gift.info.name}\"")
+            print(f"{event.user.unique_id} sent {event.repeat_count}x \"{event.gift.name}\"")
 
     # It's not type 1, which means it can't have a streak & is automatically over
     elif event.gift.info.type != 1:
-        print(f"{event.user.unique_id} sent \"{event.gift.info.name}\"")
+        print(f"{event.user.unique_id} sent \"{event.gift.name}\"")
 ```
 
 Using the TikTokLive extended proto:
 ```python
 @client.on("gift")
 async def on_gift(event: GiftEvent):
     # Streakable gift & streak is over
     if event.gift.streakable and not event.streaking:
-        print(f"{event.user.unique_id} sent {event.gift.count}x \"{event.gift.info.name}\"")
+        print(f"{event.user.unique_id} sent {event.repeat_count}x \"{event.gift.name}\"")
 
     # Non-streakable gift
     elif not event.gift.streakable:
-        print(f"{event.user.unique_id} sent \"{event.gift.info.name}\"")
-
+        print(f"{event.user.unique_id} sent \"{event.gift.name}\"")
 ```
 
 ### `SubscribeEvent`
 
 This event will only fire when a session ID (account login) is passed to the HTTP client *before* connecting to TikTok LIVE.
 You can set the session ID with [`client.web.set_session_id(...)`](https://github.com/isaackogan/TikTokLive/blob/master/examples/logged_in.py).
```

### Comparing `TikTokLive-6.0.4/TikTokLive/client/client.py` & `TikTokLive-6.0.5/TikTokLive/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         if event_type is None:
             return [response_event, UnknownEvent().from_pydict(response.to_dict())]
 
         # Get the underlying events
         try:
             proto_event: ProtoEvent = event_type().parse(response.payload)
         except Exception:
-            self._logger.error(traceback.format_exc())
+            self._logger.error(traceback.format_exc() + "\nBroken Payload:\n" + str(response.payload))
             return [response_event]
 
         parsed_events: List[Event] = [response_event, proto_event]
         custom_event: Optional[Event] = self._parse_custom_event(response, proto_event)
 
         # Add the custom event IF not null
         return [custom_event, *parsed_events] if custom_event else parsed_events
```

### Comparing `TikTokLive-6.0.4/TikTokLive/client/errors.py` & `TikTokLive-6.0.5/TikTokLive/client/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 
 class UserOfflineError(RuntimeError):
     """
     Thrown when the requested streamer to watch is offline
 
     """
 
+
 class AgeRestrictedError(RuntimeError):
     """
     Thrown when a LIVE is age restricted. Pass sessionid to bypass.
     """
 
+
 class InitialCursorMissingError(RuntimeError):
     """
     Thrown when the cursor for connecting to TikTok is missing (blocked)
 
     """
 
 
 class WebsocketURLMissingError(RuntimeError):
     """
     Thrown when the websocket URL to connect to TikTok is missing (blocked)
 
     """
-
```

### Comparing `TikTokLive-6.0.4/TikTokLive/client/logger.py` & `TikTokLive-6.0.5/TikTokLive/client/logger.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_gift_list.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_gift_list.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_image.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_image.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_is_live.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_is_live.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_id_api.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_api.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_id_html.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_html.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_room_info.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_info.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_sign.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_sign.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/routes/fetch_video.py` & `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_video.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/web_base.py` & `TikTokLive-6.0.5/TikTokLive/client/web/web_base.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/web_client.py` & `TikTokLive-6.0.5/TikTokLive/client/web/web_client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/web/web_settings.py` & `TikTokLive-6.0.5/TikTokLive/client/web/web_settings.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/client/ws/ws_client.py` & `TikTokLive-6.0.5/TikTokLive/client/ws/ws_client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/events/__init__.py` & `TikTokLive-6.0.5/TikTokLive/events/__init__.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/events/custom_events.py` & `TikTokLive-6.0.5/TikTokLive/events/custom_events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/events/proto_events.py` & `TikTokLive-6.0.5/TikTokLive/events/proto_events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive/proto/tiktok_proto.py` & `TikTokLive-6.0.5/TikTokLive/proto/tiktok_proto.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLive.egg-info/PKG-INFO` & `TikTokLive-6.0.5/TikTokLive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TikTokLive
-Version: 6.0.4
+Version: 6.0.5
 Summary: TikTok Live Python Client
 Home-page: https://github.com/isaackogan/TikTokLive
-Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.4
+Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5
 Author: Isaac Kogan
 Author-email: info@isaackogan.com
 License: MIT
 Keywords: tiktok,tiktok live,python3,api,unofficial
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -260,33 +260,32 @@
 Using the low-level direct proto:
 ```python
 @client.on(GiftEvent)
 async def on_gift(event: GiftEvent):
     # If it's type 1 and the streak is over
     if event.gift.info.type == 1:
         if event.gift.is_repeating == 1:
-            print(f"{event.user.unique_id} sent {event.gift.count}x \"{event.gift.info.name}\"")
+            print(f"{event.user.unique_id} sent {event.repeat_count}x \"{event.gift.name}\"")
 
     # It's not type 1, which means it can't have a streak & is automatically over
     elif event.gift.info.type != 1:
-        print(f"{event.user.unique_id} sent \"{event.gift.info.name}\"")
+        print(f"{event.user.unique_id} sent \"{event.gift.name}\"")
 ```
 
 Using the TikTokLive extended proto:
 ```python
 @client.on("gift")
 async def on_gift(event: GiftEvent):
     # Streakable gift & streak is over
     if event.gift.streakable and not event.streaking:
-        print(f"{event.user.unique_id} sent {event.gift.count}x \"{event.gift.info.name}\"")
+        print(f"{event.user.unique_id} sent {event.repeat_count}x \"{event.gift.name}\"")
 
     # Non-streakable gift
     elif not event.gift.streakable:
-        print(f"{event.user.unique_id} sent \"{event.gift.info.name}\"")
-
+        print(f"{event.user.unique_id} sent \"{event.gift.name}\"")
 ```
 
 ### `SubscribeEvent`
 
 This event will only fire when a session ID (account login) is passed to the HTTP client *before* connecting to TikTok LIVE.
 You can set the session ID with [`client.web.set_session_id(...)`](https://github.com/isaackogan/TikTokLive/blob/master/examples/logged_in.py).
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.4 Summary: TikTok Live
+Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.5 Summary: TikTok Live
 Python Client Home-page: https://github.com/isaackogan/TikTokLive Download-URL:
-https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.4 Author: Isaac
+https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5 Author: Isaac
 Kogan Author-email: info@isaackogan.com License: MIT Keywords: tiktok,tiktok
 live,python3,api,unofficial Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -175,34 +175,33 @@
 this time new gift events are triggered again and again with an > increased
 `event.gift.repeat_count` value. It should be noted that after the end of a
 streak, a final gift event is > triggered, which signals the end of the streak
 with `event.repeat_end`:`1`. The following handlers show how you can deal with
 this in your code. Using the low-level direct proto: ```python @client.on
 (GiftEvent) async def on_gift(event: GiftEvent): # If it's type 1 and the
 streak is over if event.gift.info.type == 1: if event.gift.is_repeating == 1:
-print(f"{event.user.unique_id} sent {event.gift.count}x \"
-{event.gift.info.name}\"") # It's not type 1, which means it can't have a
-streak & is automatically over elif event.gift.info.type != 1: print(f"
-{event.user.unique_id} sent \"{event.gift.info.name}\"") ``` Using the
-TikTokLive extended proto: ```python @client.on("gift") async def on_gift
-(event: GiftEvent): # Streakable gift & streak is over if event.gift.streakable
-and not event.streaking: print(f"{event.user.unique_id} sent
-{event.gift.count}x \"{event.gift.info.name}\"") # Non-streakable gift elif not
-event.gift.streakable: print(f"{event.user.unique_id} sent \"
-{event.gift.info.name}\"") ``` ### `SubscribeEvent` This event will only fire
-when a session ID (account login) is passed to the HTTP client *before*
-connecting to TikTok LIVE. You can set the session ID with
-[`client.web.set_session_id(...)`](https://github.com/isaackogan/TikTokLive/
-blob/master/examples/logged_in.py). ## Checking If A User Is Live It is
-considered inefficient to use the connect method to check if a user is live. It
-is better to use the dedicated `await client.is_live()` method. There is a
-[complete example](https://github.com/isaackogan/TikTokLive/blob/master/
-examples/check_live.py) of how to do this in the [examples](https://github.com/
-isaackogan/TikTokLive/tree/master/examples) folder. ## Contributors * **Isaac
-Kogan** - *Creator, Primary Maintainer, and Reverse-Engineering* - [isaackogan]
-(https://github.com/isaackogan) * **Zerody** - *Initial Reverse-Engineering
-Protobuf & Support* - [Zerody](https://github.com/zerodytrash/) *
+print(f"{event.user.unique_id} sent {event.repeat_count}x \"
+{event.gift.name}\"") # It's not type 1, which means it can't have a streak &
+is automatically over elif event.gift.info.type != 1: print(f"
+{event.user.unique_id} sent \"{event.gift.name}\"") ``` Using the TikTokLive
+extended proto: ```python @client.on("gift") async def on_gift(event:
+GiftEvent): # Streakable gift & streak is over if event.gift.streakable and not
+event.streaking: print(f"{event.user.unique_id} sent {event.repeat_count}x \"
+{event.gift.name}\"") # Non-streakable gift elif not event.gift.streakable:
+print(f"{event.user.unique_id} sent \"{event.gift.name}\"") ``` ###
+`SubscribeEvent` This event will only fire when a session ID (account login) is
+passed to the HTTP client *before* connecting to TikTok LIVE. You can set the
+session ID with [`client.web.set_session_id(...)`](https://github.com/
+isaackogan/TikTokLive/blob/master/examples/logged_in.py). ## Checking If A User
+Is Live It is considered inefficient to use the connect method to check if a
+user is live. It is better to use the dedicated `await client.is_live()`
+method. There is a [complete example](https://github.com/isaackogan/TikTokLive/
+blob/master/examples/check_live.py) of how to do this in the [examples](https:/
+/github.com/isaackogan/TikTokLive/tree/master/examples) folder. ## Contributors
+* **Isaac Kogan** - *Creator, Primary Maintainer, and Reverse-Engineering* -
+[isaackogan](https://github.com/isaackogan) * **Zerody** - *Initial Reverse-
+Engineering Protobuf & Support* - [Zerody](https://github.com/zerodytrash/) *
 **Davincible** - *Reverse-Engineering Stream Downloads* - [davincible](https://
 github.com/davincible) See also the full list of [contributors](https://
 github.com/isaackogan/TikTokLive/contributors) who have participated in this
 project. ## License This project is licensed under the MIT License - see the
 [LICENSE](LICENSE) file for details.
```

### Comparing `TikTokLive-6.0.4/TikTokLive.egg-info/SOURCES.txt` & `TikTokLive-6.0.5/TikTokLive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 TikTokLive/client/ws/ws_client.py
 TikTokLive/events/__init__.py
 TikTokLive/events/base_event.py
 TikTokLive/events/custom_events.py
 TikTokLive/events/proto_events.py
 TikTokLive/proto/__init__.py
 TikTokLive/proto/custom_proto.py
+TikTokLive/proto/proto_utils.py
 TikTokLive/proto/tiktok_proto.py
 TikTokLiveLegacy/__init__.py
 TikTokLiveLegacy/utilities.py
 TikTokLiveLegacy/client/__init__.py
 TikTokLiveLegacy/client/base.py
 TikTokLiveLegacy/client/client.py
 TikTokLiveLegacy/client/config.py
```

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/client/base.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/client/base.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/client/client.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/client/client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/client/config.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/client/config.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/client/httpx.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/client/httpx.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/client/wsclient.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/client/wsclient.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/proto/tiktok_schema_pb2.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/proto/tiktok_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/proto/utilities.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/proto/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/types/errors.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/types/errors.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/types/events.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/types/events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/types/objects.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/types/objects.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/types/utilities.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/types/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/TikTokLiveLegacy/utilities.py` & `TikTokLive-6.0.5/TikTokLiveLegacy/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.4/setup.py` & `TikTokLive-6.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PyPi upload Command
 # rm -r dist ; python setup.py sdist ; python -m twine upload dist/*
 
 manifest: dict = {
     "name": "TikTokLive",
     "license": "MIT",
     "author": "Isaac Kogan",
-    "version": "6.0.4",
+    "version": "6.0.5",
     "email": "info@isaackogan.com"
 }
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
```

