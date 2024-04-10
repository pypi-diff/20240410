# Comparing `tmp/comiccrawler-2024.4.10.tar.gz` & `tmp/comiccrawler-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comiccrawler-2024.4.10.tar", last modified: Wed Apr 10 12:18:39 2024, max compression
+gzip compressed data, was "comiccrawler-2024.4.2.tar", last modified: Tue Apr  2 15:12:09 2024, max compression
```

## Comparing `comiccrawler-2024.4.10.tar` & `comiccrawler-2024.4.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:18:39.110966 comiccrawler-2024.4.10/
--rw-rw-rw-   0        0        0    41559 2024-04-10 12:18:39.108968 comiccrawler-2024.4.10/PKG-INFO
--rw-rw-rw-   0        0        0    40286 2024-04-10 12:16:21.000000 comiccrawler-2024.4.10/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-10 12:18:38.402965 comiccrawler-2024.4.10/comiccrawler/
--rw-rw-rw-   0        0        0       27 2024-04-10 12:17:56.000000 comiccrawler-2024.4.10/comiccrawler/__init__.py
--rw-rw-rw-   0        0        0       63 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/__main__.py
--rw-rw-rw-   0        0        0     4971 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/analyzer.py
--rw-rw-rw-   0        0        0     1662 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/batch_analyzer.py
--rw-rw-rw-   0        0        0      117 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/channel.py
--rw-rw-rw-   0        0        0     1639 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/cli.py
--rw-rw-rw-   0        0        0     1821 2024-04-10 12:14:55.000000 comiccrawler-2024.4.10/comiccrawler/config.py
--rw-rw-rw-   0        0        0      128 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/core.py
--rw-rw-rw-   0        0        0    10553 2024-04-10 12:14:55.000000 comiccrawler-2024.4.10/comiccrawler/crawler.py
--rw-rw-rw-   0        0        0     8215 2024-04-10 12:14:55.000000 comiccrawler-2024.4.10/comiccrawler/download_manager.py
--rw-rw-rw-   0        0        0      596 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/episode.py
--rw-rw-rw-   0        0        0     1957 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/episode_loader.py
--rw-rw-rw-   0        0        0     1126 2023-07-14 09:58:51.000000 comiccrawler-2024.4.10/comiccrawler/error.py
--rw-rw-rw-   0        0        0     8013 2024-04-10 12:14:55.000000 comiccrawler-2024.4.10/comiccrawler/grabber.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:18:38.603965 comiccrawler-2024.4.10/comiccrawler/gui/
--rw-rw-rw-   0        0        0        0 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/gui/__init__.py
--rw-rw-rw-   0        0        0     1657 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/gui/core.py
--rw-rw-rw-   0        0        0     1671 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/gui/dialog.py
--rw-rw-rw-   0        0        0    19540 2024-04-10 11:56:53.000000 comiccrawler-2024.4.10/comiccrawler/gui/main_window.py
--rw-rw-rw-   0        0        0     4704 2022-01-19 05:34:52.000000 comiccrawler-2024.4.10/comiccrawler/gui/select_episodes.py
--rw-rw-rw-   0        0        0     2911 2020-06-03 15:30:48.000000 comiccrawler-2024.4.10/comiccrawler/gui/table.py
--rw-rw-rw-   0        0        0      941 2023-07-14 09:58:51.000000 comiccrawler-2024.4.10/comiccrawler/image.py
--rw-rw-rw-   0        0        0     4481 2021-11-15 12:30:12.000000 comiccrawler-2024.4.10/comiccrawler/io.py
--rw-rw-rw-   0        0        0      228 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/logger.py
--rw-rw-rw-   0        0        0     1130 2023-11-13 12:18:43.000000 comiccrawler-2024.4.10/comiccrawler/mission.py
--rw-rw-rw-   0        0        0     5433 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mission_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:18:39.086966 comiccrawler-2024.4.10/comiccrawler/mods/
--rw-rw-rw-   0        0        0      703 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/_177pic.py
--rw-rw-rw-   0        0        0      964 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/_99.py
--rw-rw-rw-   0        0        0     3794 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/mods/__init__.py
--rw-rw-rw-   0        0        0     1940 2024-04-02 15:09:12.000000 comiccrawler-2024.4.10/comiccrawler/mods/aacomic.py
--rw-rw-rw-   0        0        0      842 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/acgn.py
--rw-rw-rw-   0        0        0     1971 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/artstation.py
--rw-rw-rw-   0        0        0     1028 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/bilibili.py
--rw-rw-rw-   0        0        0     3580 2023-12-24 09:53:20.000000 comiccrawler-2024.4.10/comiccrawler/mods/bilibili_manga.py
--rw-rw-rw-   0        0        0      675 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/buka.py
--rw-rw-rw-   0        0        0      725 2023-12-24 09:18:13.000000 comiccrawler-2024.4.10/comiccrawler/mods/cartoonmad.py
--rw-rw-rw-   0        0        0     1136 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/chuixue.py
--rw-rw-rw-   0        0        0     1824 2023-10-08 15:32:19.000000 comiccrawler-2024.4.10/comiccrawler/mods/copy.py
--rw-rw-rw-   0        0        0     1047 2023-07-14 09:58:51.000000 comiccrawler-2024.4.10/comiccrawler/mods/danbooru.py
--rw-rw-rw-   0        0        0     2751 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/deviantart.py
--rw-rw-rw-   0        0        0     1986 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/dm5.py
--rw-rw-rw-   0        0        0     2033 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/dmzj.py
--rw-rw-rw-   0        0        0     1070 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/dmzj_m.py
--rw-rw-rw-   0        0        0     1121 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/dmzj_www.py
--rw-rw-rw-   0        0        0     2647 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/eight.py
--rw-rw-rw-   0        0        0     2338 2021-11-15 12:30:12.000000 comiccrawler-2024.4.10/comiccrawler/mods/exh.py
--rw-rw-rw-   0        0        0     1841 2023-03-21 06:51:55.000000 comiccrawler-2024.4.10/comiccrawler/mods/facebook.py
--rw-rw-rw-   0        0        0     2006 2024-04-06 16:33:56.000000 comiccrawler-2024.4.10/comiccrawler/mods/fanbox.py
--rw-rw-rw-   0        0        0     1972 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/mods/fantia.py
--rw-rw-rw-   0        0        0     4186 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/flickr.py
--rw-rw-rw-   0        0        0     1668 2021-08-24 08:48:41.000000 comiccrawler-2024.4.10/comiccrawler/mods/gelbooru.py
--rw-rw-rw-   0        0        0     1205 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/gufeng.py
--rw-rw-rw-   0        0        0     2113 2024-04-02 15:09:12.000000 comiccrawler-2024.4.10/comiccrawler/mods/hhxiee.py
--rw-rw-rw-   0        0        0     1330 2024-04-02 15:09:12.000000 comiccrawler-2024.4.10/comiccrawler/mods/iibq.py
--rw-rw-rw-   0        0        0      617 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/imgbox.py
--rw-rw-rw-   0        0        0     4820 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/mods/instagram.py
--rw-rw-rw-   0        0        0     1210 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/mods/kemono.py
--rw-rw-rw-   0        0        0     1139 2020-09-02 04:45:21.000000 comiccrawler-2024.4.10/comiccrawler/mods/konachan.py
--rw-rw-rw-   0        0        0     3072 2023-07-14 09:58:51.000000 comiccrawler-2024.4.10/comiccrawler/mods/linevoom.py
--rw-rw-rw-   0        0        0     2358 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/manhuabei_m.py
--rw-rw-rw-   0        0        0     2157 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/manhuadui.py
--rw-rw-rw-   0        0        0      751 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/manhuaren.py
--rw-rw-rw-   0        0        0     1205 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/mh160.py
--rw-rw-rw-   0        0        0     1842 2020-08-31 08:55:09.000000 comiccrawler-2024.4.10/comiccrawler/mods/nico.py
--rw-rw-rw-   0        0        0     1597 2020-08-14 04:59:34.000000 comiccrawler-2024.4.10/comiccrawler/mods/nijie.py
--rw-rw-rw-   0        0        0     2237 2024-03-17 17:30:14.000000 comiccrawler-2024.4.10/comiccrawler/mods/oh.py
--rw-rw-rw-   0        0        0     1028 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/pixabay.py
--rw-rw-rw-   0        0        0     8075 2021-08-24 09:08:27.000000 comiccrawler-2024.4.10/comiccrawler/mods/pixiv.py
--rw-rw-rw-   0        0        0     1664 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/qq.py
--rw-rw-rw-   0        0        0     1738 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/mods/sankaku.py
--rw-rw-rw-   0        0        0     1826 2020-09-02 04:32:13.000000 comiccrawler-2024.4.10/comiccrawler/mods/sankaku_beta.py
--rw-rw-rw-   0        0        0     3987 2024-04-02 15:09:12.000000 comiccrawler-2024.4.10/comiccrawler/mods/seemh.py
--rw-rw-rw-   0        0        0     1067 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/senmanga.py
--rw-rw-rw-   0        0        0     2079 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/setnmh.py
--rw-rw-rw-   0        0        0      962 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/sfacg.py
--rw-rw-rw-   0        0        0     1395 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/toho.py
--rw-rw-rw-   0        0        0      813 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/tsundora.py
--rw-rw-rw-   0        0        0      803 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/tuchong.py
--rw-rw-rw-   0        0        0     2595 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/tumblr.py
--rw-rw-rw-   0        0        0     7434 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/mods/twitter.py
--rw-rw-rw-   0        0        0     1690 2020-08-31 10:59:29.000000 comiccrawler-2024.4.10/comiccrawler/mods/weibo.py
--rw-rw-rw-   0        0        0     1162 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/wix.py
--rw-rw-rw-   0        0        0     1470 2023-10-11 03:22:38.000000 comiccrawler-2024.4.10/comiccrawler/mods/xznj120.py
--rw-rw-rw-   0        0        0     1186 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/yandere.py
--rw-rw-rw-   0        0        0      703 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/yoedge.py
--rw-rw-rw-   0        0        0      869 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/mods/youhui.py
--rw-rw-rw-   0        0        0     1679 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/module_grabber.py
--rw-rw-rw-   0        0        0      348 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/profile.py
--rw-rw-rw-   0        0        0       93 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/safeprint.py
--rw-rw-rw-   0        0        0     1688 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/save_path.py
--rw-rw-rw-   0        0        0     1606 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/session_manager.py
--rw-rw-rw-   0        0        0      694 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/comiccrawler/url.py
--rw-rw-rw-   0        0        0     2133 2024-03-25 06:11:21.000000 comiccrawler-2024.4.10/comiccrawler/util.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:18:39.098977 comiccrawler-2024.4.10/comiccrawler.egg-info/
--rw-rw-rw-   0        0        0    41559 2024-04-10 12:18:37.000000 comiccrawler-2024.4.10/comiccrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2817 2024-04-10 12:18:37.000000 comiccrawler-2024.4.10/comiccrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:18:37.000000 comiccrawler-2024.4.10/comiccrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-10 12:18:37.000000 comiccrawler-2024.4.10/comiccrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 12:18:37.000000 comiccrawler-2024.4.10/comiccrawler.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-10 12:18:37.000000 comiccrawler-2024.4.10/comiccrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 12:18:37.000000 comiccrawler-2024.4.10/comiccrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1253 2024-04-10 12:18:39.117974 comiccrawler-2024.4.10/setup.cfg
--rw-rw-rw-   0        0        0       55 2020-06-03 06:54:45.000000 comiccrawler-2024.4.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:09.351167 comiccrawler-2024.4.2/
+-rw-rw-rw-   0        0        0    41269 2024-04-02 15:12:09.348156 comiccrawler-2024.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    40028 2024-04-02 15:10:13.000000 comiccrawler-2024.4.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:07.838713 comiccrawler-2024.4.2/comiccrawler/
+-rw-rw-rw-   0        0        0       26 2024-04-02 15:11:40.000000 comiccrawler-2024.4.2/comiccrawler/__init__.py
+-rw-rw-rw-   0        0        0       63 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/__main__.py
+-rw-rw-rw-   0        0        0     4971 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/analyzer.py
+-rw-rw-rw-   0        0        0     1662 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/batch_analyzer.py
+-rw-rw-rw-   0        0        0      117 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/channel.py
+-rw-rw-rw-   0        0        0     1639 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/cli.py
+-rw-rw-rw-   0        0        0     1800 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/config.py
+-rw-rw-rw-   0        0        0      128 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/core.py
+-rw-rw-rw-   0        0        0    10543 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/crawler.py
+-rw-rw-rw-   0        0        0     7585 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/download_manager.py
+-rw-rw-rw-   0        0        0      596 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/episode.py
+-rw-rw-rw-   0        0        0     1957 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/episode_loader.py
+-rw-rw-rw-   0        0        0     1126 2023-07-14 09:58:51.000000 comiccrawler-2024.4.2/comiccrawler/error.py
+-rw-rw-rw-   0        0        0     7914 2024-04-02 15:09:12.000000 comiccrawler-2024.4.2/comiccrawler/grabber.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:08.052713 comiccrawler-2024.4.2/comiccrawler/gui/
+-rw-rw-rw-   0        0        0        0 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/gui/__init__.py
+-rw-rw-rw-   0        0        0     1657 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/gui/core.py
+-rw-rw-rw-   0        0        0     1671 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/gui/dialog.py
+-rw-rw-rw-   0        0        0    19540 2024-03-25 00:29:58.000000 comiccrawler-2024.4.2/comiccrawler/gui/main_window.py
+-rw-rw-rw-   0        0        0     4704 2022-01-19 05:34:52.000000 comiccrawler-2024.4.2/comiccrawler/gui/select_episodes.py
+-rw-rw-rw-   0        0        0     2911 2020-06-03 15:30:48.000000 comiccrawler-2024.4.2/comiccrawler/gui/table.py
+-rw-rw-rw-   0        0        0      941 2023-07-14 09:58:51.000000 comiccrawler-2024.4.2/comiccrawler/image.py
+-rw-rw-rw-   0        0        0     4481 2021-11-15 12:30:12.000000 comiccrawler-2024.4.2/comiccrawler/io.py
+-rw-rw-rw-   0        0        0      228 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/logger.py
+-rw-rw-rw-   0        0        0     1130 2023-11-13 12:18:43.000000 comiccrawler-2024.4.2/comiccrawler/mission.py
+-rw-rw-rw-   0        0        0     5433 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mission_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:09.312157 comiccrawler-2024.4.2/comiccrawler/mods/
+-rw-rw-rw-   0        0        0      703 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/_177pic.py
+-rw-rw-rw-   0        0        0      964 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/_99.py
+-rw-rw-rw-   0        0        0     3794 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/mods/__init__.py
+-rw-rw-rw-   0        0        0     1940 2024-04-02 15:09:12.000000 comiccrawler-2024.4.2/comiccrawler/mods/aacomic.py
+-rw-rw-rw-   0        0        0      842 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/acgn.py
+-rw-rw-rw-   0        0        0     1971 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/artstation.py
+-rw-rw-rw-   0        0        0     1028 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/bilibili.py
+-rw-rw-rw-   0        0        0     3580 2023-12-24 09:53:20.000000 comiccrawler-2024.4.2/comiccrawler/mods/bilibili_manga.py
+-rw-rw-rw-   0        0        0      675 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/buka.py
+-rw-rw-rw-   0        0        0      725 2023-12-24 09:18:13.000000 comiccrawler-2024.4.2/comiccrawler/mods/cartoonmad.py
+-rw-rw-rw-   0        0        0     1136 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/chuixue.py
+-rw-rw-rw-   0        0        0     1824 2023-10-08 15:32:19.000000 comiccrawler-2024.4.2/comiccrawler/mods/copy.py
+-rw-rw-rw-   0        0        0     1047 2023-07-14 09:58:51.000000 comiccrawler-2024.4.2/comiccrawler/mods/danbooru.py
+-rw-rw-rw-   0        0        0     2751 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/deviantart.py
+-rw-rw-rw-   0        0        0     1986 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/dm5.py
+-rw-rw-rw-   0        0        0     2033 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/dmzj.py
+-rw-rw-rw-   0        0        0     1070 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/dmzj_m.py
+-rw-rw-rw-   0        0        0     1121 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/dmzj_www.py
+-rw-rw-rw-   0        0        0     2647 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/eight.py
+-rw-rw-rw-   0        0        0     2338 2021-11-15 12:30:12.000000 comiccrawler-2024.4.2/comiccrawler/mods/exh.py
+-rw-rw-rw-   0        0        0     1841 2023-03-21 06:51:55.000000 comiccrawler-2024.4.2/comiccrawler/mods/facebook.py
+-rw-rw-rw-   0        0        0     2000 2023-11-13 12:18:43.000000 comiccrawler-2024.4.2/comiccrawler/mods/fanbox.py
+-rw-rw-rw-   0        0        0     1972 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/mods/fantia.py
+-rw-rw-rw-   0        0        0     4186 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/flickr.py
+-rw-rw-rw-   0        0        0     1668 2021-08-24 08:48:41.000000 comiccrawler-2024.4.2/comiccrawler/mods/gelbooru.py
+-rw-rw-rw-   0        0        0     1205 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/gufeng.py
+-rw-rw-rw-   0        0        0     2113 2024-04-02 15:09:12.000000 comiccrawler-2024.4.2/comiccrawler/mods/hhxiee.py
+-rw-rw-rw-   0        0        0     1330 2024-04-02 15:09:12.000000 comiccrawler-2024.4.2/comiccrawler/mods/iibq.py
+-rw-rw-rw-   0        0        0      617 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/imgbox.py
+-rw-rw-rw-   0        0        0     4820 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/mods/instagram.py
+-rw-rw-rw-   0        0        0     1210 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/mods/kemono.py
+-rw-rw-rw-   0        0        0     1139 2020-09-02 04:45:21.000000 comiccrawler-2024.4.2/comiccrawler/mods/konachan.py
+-rw-rw-rw-   0        0        0     3072 2023-07-14 09:58:51.000000 comiccrawler-2024.4.2/comiccrawler/mods/linevoom.py
+-rw-rw-rw-   0        0        0     2358 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/manhuabei_m.py
+-rw-rw-rw-   0        0        0     2157 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/manhuadui.py
+-rw-rw-rw-   0        0        0      751 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/manhuaren.py
+-rw-rw-rw-   0        0        0     1205 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/mh160.py
+-rw-rw-rw-   0        0        0     1842 2020-08-31 08:55:09.000000 comiccrawler-2024.4.2/comiccrawler/mods/nico.py
+-rw-rw-rw-   0        0        0     1597 2020-08-14 04:59:34.000000 comiccrawler-2024.4.2/comiccrawler/mods/nijie.py
+-rw-rw-rw-   0        0        0     2237 2024-03-17 17:30:14.000000 comiccrawler-2024.4.2/comiccrawler/mods/oh.py
+-rw-rw-rw-   0        0        0     1028 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/pixabay.py
+-rw-rw-rw-   0        0        0     8075 2021-08-24 09:08:27.000000 comiccrawler-2024.4.2/comiccrawler/mods/pixiv.py
+-rw-rw-rw-   0        0        0     1664 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/qq.py
+-rw-rw-rw-   0        0        0     1738 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/mods/sankaku.py
+-rw-rw-rw-   0        0        0     1826 2020-09-02 04:32:13.000000 comiccrawler-2024.4.2/comiccrawler/mods/sankaku_beta.py
+-rw-rw-rw-   0        0        0     3987 2024-04-02 15:09:12.000000 comiccrawler-2024.4.2/comiccrawler/mods/seemh.py
+-rw-rw-rw-   0        0        0     1067 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/senmanga.py
+-rw-rw-rw-   0        0        0     2079 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/setnmh.py
+-rw-rw-rw-   0        0        0      962 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/sfacg.py
+-rw-rw-rw-   0        0        0     1395 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/toho.py
+-rw-rw-rw-   0        0        0      813 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/tsundora.py
+-rw-rw-rw-   0        0        0      803 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/tuchong.py
+-rw-rw-rw-   0        0        0     2595 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/tumblr.py
+-rw-rw-rw-   0        0        0     7434 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/mods/twitter.py
+-rw-rw-rw-   0        0        0     1690 2020-08-31 10:59:29.000000 comiccrawler-2024.4.2/comiccrawler/mods/weibo.py
+-rw-rw-rw-   0        0        0     1162 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/wix.py
+-rw-rw-rw-   0        0        0     1470 2023-10-11 03:22:38.000000 comiccrawler-2024.4.2/comiccrawler/mods/xznj120.py
+-rw-rw-rw-   0        0        0     1186 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/yandere.py
+-rw-rw-rw-   0        0        0      703 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/yoedge.py
+-rw-rw-rw-   0        0        0      869 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/mods/youhui.py
+-rw-rw-rw-   0        0        0     1679 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/module_grabber.py
+-rw-rw-rw-   0        0        0      348 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/profile.py
+-rw-rw-rw-   0        0        0       93 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/safeprint.py
+-rw-rw-rw-   0        0        0     1688 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/save_path.py
+-rw-rw-rw-   0        0        0     1606 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/session_manager.py
+-rw-rw-rw-   0        0        0      694 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/comiccrawler/url.py
+-rw-rw-rw-   0        0        0     2133 2024-03-25 06:11:21.000000 comiccrawler-2024.4.2/comiccrawler/util.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:09.342157 comiccrawler-2024.4.2/comiccrawler.egg-info/
+-rw-rw-rw-   0        0        0    41269 2024-04-02 15:12:06.000000 comiccrawler-2024.4.2/comiccrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2817 2024-04-02 15:12:07.000000 comiccrawler-2024.4.2/comiccrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 15:12:06.000000 comiccrawler-2024.4.2/comiccrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-02 15:12:06.000000 comiccrawler-2024.4.2/comiccrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-02 15:12:06.000000 comiccrawler-2024.4.2/comiccrawler.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      226 2024-04-02 15:12:07.000000 comiccrawler-2024.4.2/comiccrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-02 15:12:07.000000 comiccrawler-2024.4.2/comiccrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1235 2024-04-02 15:12:09.429154 comiccrawler-2024.4.2/setup.cfg
+-rw-rw-rw-   0        0        0       55 2020-06-03 06:54:45.000000 comiccrawler-2024.4.2/setup.py
```

### Comparing `comiccrawler-2024.4.10/PKG-INFO` & `comiccrawler-2024.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comiccrawler
-Version: 2024.4.10
+Version: 2024.4.2
 Summary: An image crawler, including multiple modules and GUI.
 Home-page: https://github.com/eight04/ComicCrawler
 Author: eight
 Author-email: eight04@gmail.com
 License: MIT
 Keywords: image,crawler
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,14 @@
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Requires-Dist: belfrywidgets~=1.0
-Requires-Dist: bidict~=0.23.1
 Requires-Dist: brotli~=1.1
 Requires-Dist: deno-vm~=0.6.0
 Requires-Dist: desktop3~=0.5.3
 Requires-Dist: docopt~=0.6.2
 Requires-Dist: enlighten~=1.12
 Requires-Dist: puremagic~=1.21
 Requires-Dist: pycryptodomex~=3.20
@@ -429,22 +428,14 @@
 -  Support pool in Sankaku.
 -  Add module.get_episode_id to make the module decide how to compare episodes.
 -  Use HEAD to grab final URL before requesting the image?
 
 Changelog
 ---------
 
-- 2024.4.10
-
-  - Fix: limit retry delay to 10 minutes at most.
-  - Fix: failed handling http 206 response.
-  - Fix: username may conatain dash in fanbox.
-  - Add: ``max_errors`` setting.
-  - Add: ability to run multiple crawlers. One for each host.
-
 - 2024.4.2
 
   - Fix: wrong protocol in seemh.
   - Fix: failed downloading webp images.
 
 - 2024.3.25
```

### Comparing `comiccrawler-2024.4.10/README.rst` & `comiccrawler-2024.4.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -393,22 +393,14 @@
 -  Support pool in Sankaku.
 -  Add module.get_episode_id to make the module decide how to compare episodes.
 -  Use HEAD to grab final URL before requesting the image?
 
 Changelog
 ---------
 
-- 2024.4.10
-
-  - Fix: limit retry delay to 10 minutes at most.
-  - Fix: failed handling http 206 response.
-  - Fix: username may conatain dash in fanbox.
-  - Add: ``max_errors`` setting.
-  - Add: ability to run multiple crawlers. One for each host.
-
 - 2024.4.2
 
   - Fix: wrong protocol in seemh.
   - Fix: failed downloading webp images.
 
 - 2024.3.25
```

### Comparing `comiccrawler-2024.4.10/comiccrawler/analyzer.py` & `comiccrawler-2024.4.2/comiccrawler/analyzer.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/batch_analyzer.py` & `comiccrawler-2024.4.2/comiccrawler/batch_analyzer.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/cli.py` & `comiccrawler-2024.4.2/comiccrawler/cli.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/config.py` & `comiccrawler-2024.4.2/comiccrawler/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 		"autosave": "5",
 		"errorlog": "false",
 		"lastcheckupdate": "0",
 		"selectall": "true",
 		"mission_conflict_action": "update",
 		"browser": "",
 		"browser_profile": "",
-		"max_errors": "10"
 	}
 	def __init__(self, path):
 		self.path = expanduser(path)
 		self.config = CaseSensitiveConfigParser(interpolation=None)
 		self.load()
 		
 	def load(self):
```

### Comparing `comiccrawler-2024.4.10/comiccrawler/crawler.py` & `comiccrawler-2024.4.2/comiccrawler/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 		mission_ch.pub("MISSION_PROPERTY_CHANGED", crawler.mission)
 		debug_log("D_REST")
 		crawler.rest()
 		debug_log("D_NEXT_IMAGE")
 		crawler.next_image()
 
 	def download_error(er, count):
-		t = min(5 * 2 ** count, 600)
+		t = 5 * 2 ** count
 		print(f"wait {t} seconds...")
 		if is_http(er, code=429):
 			# retry doesn't work with 429 error
 			sleep(t)
 			raise er
 		crawler.handle_error(er)
 		sleep(t)
```

### Comparing `comiccrawler-2024.4.10/comiccrawler/download_manager.py` & `comiccrawler-2024.4.2/comiccrawler/download_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 #! python3
 
 """Download Manager"""
 
-from collections import deque, defaultdict
+from collections import deque
 import re
 import subprocess # nosec
 import shlex
 import sys
 import traceback
 from threading import Lock
-from types import ModuleType
 
 from os.path import join as path_join
 from time import time
 
 from worker import Worker, current, await_, create_worker, async_
-from bidict import bidict
 
 from .analyzer import Analyzer
 from .safeprint import print
 from .batch_analyzer import BatchAnalyzer
 from .config import setting
 from .mission import create_mission
 from .crawler import download
@@ -55,40 +53,38 @@
 			return self.obj.copy()
 
 class DownloadManager:
 	"""Create a download manager used in GUI. Manage threads."""
 
 	def __init__(self):
 		"""Construct."""
-		self.lock = Lock()
-		self.crawlers: bidict[ModuleType, Worker] = bidict()
-		self.mod_errors: dict[ModuleType, int] = defaultdict(int)
+		self.download_thread = None
 		self.analyze_threads = ThreadSafeSet()
 		self.library_thread = None
 		self.library_err_count = None
 		self.batch_analyzer = None
-
+		self.continued_failure = 0
+		
 		thread = current()
-		self.thread = thread
 		
 		download_ch.sub(thread)
-
+		
 		@thread.listen("DOWNLOAD_ERROR")
 		def _(event):
 			_err, mission = event.data
 			mission_manager.drop("view", mission)
-			self.mod_errors[mission.module] += 1
+			self.continued_failure += 1
 
 		@thread.listen("DOWNLOAD_FINISHED")
 		def _(event):
 			"""After download, execute command."""
-			with self.lock:
-				if event.target not in self.crawlers.values():
-					return
-				self.mod_errors[event.data.module] = 0
+			self.continued_failure = 0
+			
+			if event.target is not self.download_thread:
+				return
 				
 			cmd = event.data.module.config.get("runafterdownload")
 			default_cmd = setting.get("runafterdownload")
 			
 			commands = []
 			
 			if cmd:
@@ -115,76 +111,54 @@
 
 			async_(run_command)
 						
 		@thread.listen("DOWNLOAD_FINISHED")
 		@thread.listen("DOWNLOAD_ERROR")
 		def _(event):
 			"""After download, continue next mission"""
-			with self.lock:
-				mod = self.crawlers.inverse.pop(event.target, None)
-				if not mod:
-					return
-
-			max_errors = int(mod.config.get("max_errors", 3))
-			if self.mod_errors[mod] >= max_errors:
-				print(f"{mod.name} 失敗 {max_errors} 次，停止下載")
-				self.mod_errors[mod] = 0
+			if event.target is not self.download_thread:
 				return
-
-			self.start_download_mod(mod)
-
+			self.download_thread = None
+			if self.continued_failure >= len(mission_manager.get_all("view", lambda m: m.state != "FINISHED")):
+				print(f"連續失敗 {self.continued_failure} 次，停止下載")
+				return
+			self.start_download(continued=True)
+				
 		@thread.listen("DOWNLOAD_INVALID")
 		def _(event):
 			"""Something bad happened"""
-			with self.lock:
-				mod = self.crawlers.inverse.pop(event.target, None)
-				if mod:
-					print(f"{mod.name} 停止下載")
+			if event.target is self.download_thread:
+				self.download_thread = None
+				print("停止下載")
 
-	def start_download(self):
+	def start_download(self, continued=False):
 		"""Start downloading."""
-		self.start_download_all()
-
-	def start_download_all(self):
-		missions = mission_manager.get_all("view", lambda m: m.state in ("ANALYZED", "PAUSE", "ERROR", "UPDATE"))
-		if not missions:
-			print("所有任務已下載完成")
+		if self.download_thread:
 			return
 
-		for mission in missions:
-			self.start_download_mod(mission.module)
-
-	def start_download_mod(self, mod):
-		"""Start downloading from a specific mod."""
-		mission = mission_manager.get("view", lambda m: m.module == mod and m.state in ("ANALYZED", "PAUSE", "ERROR", "UPDATE"))
-		if not mission:
-			return
-
-		with self.lock:
-			if mod in self.crawlers:
-				return
-
+		if not continued:
+			self.continued_failure = 0
+			
+		mission = mission_manager.get("view", lambda m: m.state in ("ANALYZED", "PAUSE", "ERROR", "UPDATE"))
+		if mission:
+			print("Start download " + mission.title)
 			def do_download():
 				debug_log("do_download")
 				with load_episodes(mission):
 					download(mission, profile(mission.module.config["savepath"]))
-
-			self.crawlers[mod] = Worker(do_download).start()
+					
+			self.download_thread = Worker(do_download).start()
+		else:
+			print("所有任務已下載完成")
 
 	def stop_download(self):
 		"""Stop downloading."""
-		with self.lock:
-			if not self.crawlers:
-				return
-
-			for crawler in self.crawlers.values():
-				crawler.stop()
-
-			# FIXME: shouldn't we wait for thread stop?
-			self.crawlers.clear()
+		if self.download_thread:
+			self.download_thread.stop()
+			self.download_thread = None
 			print("Stop downloading")
 			
 	def start_analyze(self, mission, on_finished=None):
 		"""Start analyzing"""
 		if mission.state not in ("ANALYZE_INIT", "INIT"):
 			print(
 				"Invalid state to analyze: {state}".format(state=mission.state))
@@ -309,11 +283,10 @@
 	def stop_check_update(self):
 		"""Stop checking update"""
 		if self.library_thread:
 			self.library_thread.stop()
 			self.library_thread = None
 
 	def is_downloading(self):
-		with self.lock:
-			return bool(self.crawlers)
+		return self.download_thread is not None
 		
 download_manager = DownloadManager()
```

### Comparing `comiccrawler-2024.4.10/comiccrawler/episode.py` & `comiccrawler-2024.4.2/comiccrawler/episode.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/episode_loader.py` & `comiccrawler-2024.4.2/comiccrawler/episode_loader.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/error.py` & `comiccrawler-2024.4.2/comiccrawler/error.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/grabber.py` & `comiccrawler-2024.4.2/comiccrawler/grabber.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! python3
 
 from contextlib import contextmanager
 from email.message import EmailMessage
 from pathlib import Path
 from pprint import pformat
 from threading import Lock
-from urllib.parse import quote, urlsplit, urlunsplit, urlparse
+from urllib.parse import quote, urlsplit, urlunsplit
 import re
 import socket
 import time
 
 import enlighten
 import requests
 import puremagic
@@ -87,45 +87,47 @@
 		content_write(profile("grabber.log"), content, append=True)
 
 def grabber(url, header=None, *, referer=None, cookie=None,
 			retry=False, done=None, proxy=None, **kwargs):
 	"""Request url, return text or bytes of the content."""
 	s = session_manager.get(url)
 
+	if header:
+		s.headers.update(header)
+
 	if referer:
 		s.headers['referer'] = quote_unicode(referer)
 
 	if cookie:
 		quote_unicode_dict(cookie)
 		requests.utils.add_dict_to_cookiejar(s.cookies, cookie)
 
 	if isinstance(proxy, str):
 		proxies = {'http': proxy, 'https': proxy}
 	else:
 		proxies = proxy
 
-	r = await_(do_request, s, url, proxies, retry, headers=header, **kwargs)
+	r = await_(do_request, s, url, proxies, retry, **kwargs)
 
 	if done:
 		done(s, r)
 
 	return r
 
 RETRYABLE_HTTP_CODES = (423, 429, 503)
-SUCCESS_CODES = (200, 206)
 
 def do_request(s, url, proxies, retry, **kwargs):
 	sleep_time = 5
 	while True:
 		with get_request_lock(url):
 			r = s.request(kwargs.pop("method", "GET"), url, timeout=(22, 60),
 				 proxies=proxies, **kwargs)
 		grabber_log(url, r.url, r.status_code, r.request.headers, r.headers)
 
-		if r.status_code in SUCCESS_CODES:
+		if r.status_code == 200:
 			content_length = r.headers.get("Content-Length")
 			if not kwargs.get("stream", False) and content_length and int(content_length) != r.raw.tell():
 				raise ValueError(
 					"incomplete response. Content-Length: {content_length}, got: {actual}"
 					.format(content_length=content_length, actual=r.raw.tell())
 					)
 			break
@@ -258,23 +260,21 @@
 			header = {}
 		header["Range"] = f"bytes={loaded}-"
 	r = grabber(*args, header=header, **kwargs)
 	if on_opened:
 		on_opened(r)
 	if r.status_code == 200:
 		loaded = 0
-	total = int(r.headers.get("Content-Length", "0")) + loaded or None
+	total = int(r.headers.get("Content-Length", "0")) or None
 	content_list = []
 	try:
 		@await_
 		def _():
 			nonlocal loaded
-			u = urlparse(r.url)
-			with pb_manager.counter(total=total, unit="b", leave=False, desc=u.hostname) as counter:
-				counter.update(loaded)
+			with pb_manager.counter(total=total, unit="b", leave=False) as counter:
 				if tempfile:
 					Path(tempfile).parent.mkdir(parents=True, exist_ok=True)
 					mode = "ab" if loaded else "wb"
 					with open(tempfile, mode=mode) as f:
 						for chunk in iter_content(r):
 							f.write(chunk)
 							counter.update(len(chunk))
```

### Comparing `comiccrawler-2024.4.10/comiccrawler/gui/core.py` & `comiccrawler-2024.4.2/comiccrawler/gui/core.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/gui/dialog.py` & `comiccrawler-2024.4.2/comiccrawler/gui/dialog.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/gui/main_window.py` & `comiccrawler-2024.4.2/comiccrawler/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/gui/select_episodes.py` & `comiccrawler-2024.4.2/comiccrawler/gui/select_episodes.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/gui/table.py` & `comiccrawler-2024.4.2/comiccrawler/gui/table.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/image.py` & `comiccrawler-2024.4.2/comiccrawler/image.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/io.py` & `comiccrawler-2024.4.2/comiccrawler/io.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mission.py` & `comiccrawler-2024.4.2/comiccrawler/mission.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mission_manager.py` & `comiccrawler-2024.4.2/comiccrawler/mission_manager.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/_177pic.py` & `comiccrawler-2024.4.2/comiccrawler/mods/_177pic.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/_99.py` & `comiccrawler-2024.4.2/comiccrawler/mods/_99.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/__init__.py` & `comiccrawler-2024.4.2/comiccrawler/mods/__init__.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/aacomic.py` & `comiccrawler-2024.4.2/comiccrawler/mods/aacomic.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/acgn.py` & `comiccrawler-2024.4.2/comiccrawler/mods/acgn.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/artstation.py` & `comiccrawler-2024.4.2/comiccrawler/mods/artstation.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/bilibili.py` & `comiccrawler-2024.4.2/comiccrawler/mods/bilibili.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/bilibili_manga.py` & `comiccrawler-2024.4.2/comiccrawler/mods/bilibili_manga.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/buka.py` & `comiccrawler-2024.4.2/comiccrawler/mods/buka.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/cartoonmad.py` & `comiccrawler-2024.4.2/comiccrawler/mods/cartoonmad.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/chuixue.py` & `comiccrawler-2024.4.2/comiccrawler/mods/chuixue.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/copy.py` & `comiccrawler-2024.4.2/comiccrawler/mods/copy.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/danbooru.py` & `comiccrawler-2024.4.2/comiccrawler/mods/danbooru.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/deviantart.py` & `comiccrawler-2024.4.2/comiccrawler/mods/deviantart.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/dm5.py` & `comiccrawler-2024.4.2/comiccrawler/mods/dm5.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/dmzj.py` & `comiccrawler-2024.4.2/comiccrawler/mods/dmzj.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/dmzj_m.py` & `comiccrawler-2024.4.2/comiccrawler/mods/dmzj_m.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/dmzj_www.py` & `comiccrawler-2024.4.2/comiccrawler/mods/dmzj_www.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/eight.py` & `comiccrawler-2024.4.2/comiccrawler/mods/eight.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/exh.py` & `comiccrawler-2024.4.2/comiccrawler/mods/exh.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/facebook.py` & `comiccrawler-2024.4.2/comiccrawler/mods/facebook.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/fanbox.py` & `comiccrawler-2024.4.2/comiccrawler/mods/fanbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # pin_entry_cache = {}
 
 def get_title(html, url):
 	name = re.search('<title>投稿一覽｜([^<]+)｜pixivFANBOX</title>', html).group(1)
 	return f"[fanbox] {(name)}"
 	
 def get_episodes(html, url):
-	if match := re.search(r'https://([\w-]+)\.fanbox\.cc/posts', url):
+	if match := re.search(r'https://(\w+)\.fanbox\.cc/posts', url):
 		author = match.group(1)
 		next_page_cache[url] = f"https://api.fanbox.cc/post.paginateCreator?creatorId={author}"
 		raise SkipPageError
 
 	if match := re.search(r'https://api\.fanbox\.cc/post\.paginateCreator\?creatorId=(\w+)', url):
 		author = match.group(1)
 		pages = json.loads(html)["body"]
@@ -48,15 +48,15 @@
 				title=f"{post['id']} - {(post['title'])}"
 				))
 		return result[::-1]
 
 	raise TypeError(f"Unknown URL: {url}")
 
 def get_images(html, url):
-	if match := re.search(r'https://([\w-]+)\.fanbox\.cc/posts/(\d+)', url):
+	if match := re.search(r'https://(\w+)\.fanbox\.cc/posts/(\d+)', url):
 		# author = match.group(1)
 		post_id = match.group(2)
 		next_page_cache[url] = f"https://api.fanbox.cc/post.info?postId={post_id}"
 		raise SkipPageError
 
 	if match := re.search(r'https://api\.fanbox\.cc/post\.info\?postId=(\d+)', url):
 		result = json.loads(html)
```

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/fantia.py` & `comiccrawler-2024.4.2/comiccrawler/mods/fantia.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/flickr.py` & `comiccrawler-2024.4.2/comiccrawler/mods/flickr.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/gelbooru.py` & `comiccrawler-2024.4.2/comiccrawler/mods/gelbooru.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/gufeng.py` & `comiccrawler-2024.4.2/comiccrawler/mods/gufeng.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/hhxiee.py` & `comiccrawler-2024.4.2/comiccrawler/mods/hhxiee.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/iibq.py` & `comiccrawler-2024.4.2/comiccrawler/mods/iibq.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/imgbox.py` & `comiccrawler-2024.4.2/comiccrawler/mods/imgbox.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/instagram.py` & `comiccrawler-2024.4.2/comiccrawler/mods/instagram.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/kemono.py` & `comiccrawler-2024.4.2/comiccrawler/mods/kemono.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/konachan.py` & `comiccrawler-2024.4.2/comiccrawler/mods/konachan.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/linevoom.py` & `comiccrawler-2024.4.2/comiccrawler/mods/linevoom.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/manhuabei_m.py` & `comiccrawler-2024.4.2/comiccrawler/mods/manhuabei_m.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/manhuadui.py` & `comiccrawler-2024.4.2/comiccrawler/mods/manhuadui.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/manhuaren.py` & `comiccrawler-2024.4.2/comiccrawler/mods/manhuaren.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/mh160.py` & `comiccrawler-2024.4.2/comiccrawler/mods/mh160.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/nico.py` & `comiccrawler-2024.4.2/comiccrawler/mods/nico.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/nijie.py` & `comiccrawler-2024.4.2/comiccrawler/mods/nijie.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/oh.py` & `comiccrawler-2024.4.2/comiccrawler/mods/oh.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/pixabay.py` & `comiccrawler-2024.4.2/comiccrawler/mods/pixabay.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/pixiv.py` & `comiccrawler-2024.4.2/comiccrawler/mods/pixiv.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/qq.py` & `comiccrawler-2024.4.2/comiccrawler/mods/qq.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/sankaku.py` & `comiccrawler-2024.4.2/comiccrawler/mods/sankaku.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/sankaku_beta.py` & `comiccrawler-2024.4.2/comiccrawler/mods/sankaku_beta.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/seemh.py` & `comiccrawler-2024.4.2/comiccrawler/mods/seemh.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/senmanga.py` & `comiccrawler-2024.4.2/comiccrawler/mods/senmanga.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/setnmh.py` & `comiccrawler-2024.4.2/comiccrawler/mods/setnmh.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/sfacg.py` & `comiccrawler-2024.4.2/comiccrawler/mods/sfacg.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/toho.py` & `comiccrawler-2024.4.2/comiccrawler/mods/toho.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/tsundora.py` & `comiccrawler-2024.4.2/comiccrawler/mods/tsundora.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/tuchong.py` & `comiccrawler-2024.4.2/comiccrawler/mods/tuchong.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/tumblr.py` & `comiccrawler-2024.4.2/comiccrawler/mods/tumblr.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/twitter.py` & `comiccrawler-2024.4.2/comiccrawler/mods/twitter.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/weibo.py` & `comiccrawler-2024.4.2/comiccrawler/mods/weibo.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/wix.py` & `comiccrawler-2024.4.2/comiccrawler/mods/wix.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/xznj120.py` & `comiccrawler-2024.4.2/comiccrawler/mods/xznj120.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/yandere.py` & `comiccrawler-2024.4.2/comiccrawler/mods/yandere.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/yoedge.py` & `comiccrawler-2024.4.2/comiccrawler/mods/yoedge.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/mods/youhui.py` & `comiccrawler-2024.4.2/comiccrawler/mods/youhui.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/module_grabber.py` & `comiccrawler-2024.4.2/comiccrawler/module_grabber.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/save_path.py` & `comiccrawler-2024.4.2/comiccrawler/save_path.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/session_manager.py` & `comiccrawler-2024.4.2/comiccrawler/session_manager.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/url.py` & `comiccrawler-2024.4.2/comiccrawler/url.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler/util.py` & `comiccrawler-2024.4.2/comiccrawler/util.py`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/comiccrawler.egg-info/PKG-INFO` & `comiccrawler-2024.4.2/comiccrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comiccrawler
-Version: 2024.4.10
+Version: 2024.4.2
 Summary: An image crawler, including multiple modules and GUI.
 Home-page: https://github.com/eight04/ComicCrawler
 Author: eight
 Author-email: eight04@gmail.com
 License: MIT
 Keywords: image,crawler
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,14 @@
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Requires-Dist: belfrywidgets~=1.0
-Requires-Dist: bidict~=0.23.1
 Requires-Dist: brotli~=1.1
 Requires-Dist: deno-vm~=0.6.0
 Requires-Dist: desktop3~=0.5.3
 Requires-Dist: docopt~=0.6.2
 Requires-Dist: enlighten~=1.12
 Requires-Dist: puremagic~=1.21
 Requires-Dist: pycryptodomex~=3.20
@@ -429,22 +428,14 @@
 -  Support pool in Sankaku.
 -  Add module.get_episode_id to make the module decide how to compare episodes.
 -  Use HEAD to grab final URL before requesting the image?
 
 Changelog
 ---------
 
-- 2024.4.10
-
-  - Fix: limit retry delay to 10 minutes at most.
-  - Fix: failed handling http 206 response.
-  - Fix: username may conatain dash in fanbox.
-  - Add: ``max_errors`` setting.
-  - Add: ability to run multiple crawlers. One for each host.
-
 - 2024.4.2
 
   - Fix: wrong protocol in seemh.
   - Fix: failed downloading webp images.
 
 - 2024.3.25
```

### Comparing `comiccrawler-2024.4.10/comiccrawler.egg-info/SOURCES.txt` & `comiccrawler-2024.4.2/comiccrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comiccrawler-2024.4.10/setup.cfg` & `comiccrawler-2024.4.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6d 6963 6372 6177 6c65 720d   = comiccrawler.
 00000020: 0a76 6572 7369 6f6e 203d 2032 3032 342e  .version = 2024.
-00000030: 342e 3130 0d0a 6465 7363 7269 7074 696f  4.10..descriptio
-00000040: 6e20 3d20 416e 2069 6d61 6765 2063 7261  n = An image cra
-00000050: 776c 6572 2c20 696e 636c 7564 696e 6720  wler, including 
-00000060: 6d75 6c74 6970 6c65 206d 6f64 756c 6573  multiple modules
-00000070: 2061 6e64 2047 5549 2e0d 0a61 7574 686f   and GUI...autho
-00000080: 7220 3d20 6569 6768 740d 0a61 7574 686f  r = eight..autho
-00000090: 725f 656d 6169 6c20 3d20 6569 6768 7430  r_email = eight0
-000000a0: 3440 676d 6169 6c2e 636f 6d0d 0a63 6c61  4@gmail.com..cla
-000000b0: 7373 6966 6965 7273 203d 200d 0a09 4465  ssifiers = ...De
-000000c0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-000000d0: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-000000e0: 6f6e 2f53 7461 626c 650d 0a09 456e 7669  on/Stable...Envi
-000000f0: 726f 6e6d 656e 7420 3a3a 2043 6f6e 736f  ronment :: Conso
-00000100: 6c65 0d0a 0945 6e76 6972 6f6e 6d65 6e74  le...Environment
-00000110: 203a 3a20 5769 6e33 3220 284d 5320 5769   :: Win32 (MS Wi
-00000120: 6e64 6f77 7329 0d0a 0949 6e74 656e 6465  ndows)...Intende
-00000130: 6420 4175 6469 656e 6365 203a 3a20 456e  d Audience :: En
-00000140: 6420 5573 6572 732f 4465 736b 746f 700d  d Users/Desktop.
-00000150: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000160: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000170: 204c 6963 656e 7365 0d0a 094e 6174 7572   License...Natur
-00000180: 616c 204c 616e 6775 6167 6520 3a3a 2043  al Language :: C
-00000190: 6869 6e65 7365 2028 5472 6164 6974 696f  hinese (Traditio
-000001a0: 6e61 6c29 0d0a 094f 7065 7261 7469 6e67  nal)...Operating
-000001b0: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
-000001c0: 736f 6674 203a 3a20 5769 6e64 6f77 7320  soft :: Windows 
-000001d0: 3a3a 2057 696e 646f 7773 2037 0d0a 0950  :: Windows 7...P
-000001e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000200: 2033 2e36 0d0a 0950 726f 6772 616d 6d69   3.6...Programmi
-00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000220: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0954  ython :: 3.8...T
-00000230: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
-00000240: 0d0a 6b65 7977 6f72 6473 203d 2069 6d61  ..keywords = ima
-00000250: 6765 2c20 6372 6177 6c65 720d 0a6c 6963  ge, crawler..lic
-00000260: 656e 7365 203d 204d 4954 0d0a 6c6f 6e67  ense = MIT..long
-00000270: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000280: 696c 653a 2052 4541 444d 452e 7273 740d  ile: README.rst.
-00000290: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-000002a0: 6974 6875 622e 636f 6d2f 6569 6768 7430  ithub.com/eight0
-000002b0: 342f 436f 6d69 6343 7261 776c 6572 0d0a  4/ComicCrawler..
-000002c0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a7a 6970  ..[options]..zip
-000002d0: 5f73 6166 6520 3d20 4661 6c73 650d 0a70  _safe = False..p
-000002e0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000002f0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000300: 7320 3d20 0d0a 0962 656c 6672 7977 6964  s = ...belfrywid
-00000310: 6765 7473 7e3d 312e 300d 0a09 6269 6469  gets~=1.0...bidi
-00000320: 6374 7e3d 302e 3233 2e31 0d0a 0962 726f  ct~=0.23.1...bro
-00000330: 746c 697e 3d31 2e31 0d0a 0964 656e 6f2d  tli~=1.1...deno-
-00000340: 766d 7e3d 302e 362e 300d 0a09 6465 736b  vm~=0.6.0...desk
-00000350: 746f 7033 7e3d 302e 352e 330d 0a09 646f  top3~=0.5.3...do
-00000360: 636f 7074 7e3d 302e 362e 320d 0a09 656e  copt~=0.6.2...en
-00000370: 6c69 6768 7465 6e7e 3d31 2e31 320d 0a09  lighten~=1.12...
-00000380: 7075 7265 6d61 6769 637e 3d31 2e32 310d  puremagic~=1.21.
-00000390: 0a09 7079 6372 7970 746f 646f 6d65 787e  ..pycryptodomex~
-000003a0: 3d33 2e32 300d 0a09 7079 7468 7265 6164  =3.20...pythread
-000003b0: 776f 726b 6572 7e3d 302e 3130 2e30 0d0a  worker~=0.10.0..
-000003c0: 0972 6571 7565 7374 737e 3d32 2e33 310d  .requests~=2.31.
-000003d0: 0a09 7361 6665 7072 696e 747e 3d30 2e32  ..safeprint~=0.2
-000003e0: 2e30 0d0a 0975 6e63 7572 6c7e 3d30 2e30  .0...uncurl~=0.0
-000003f0: 2e31 310d 0a09 7572 6c6c 6962 337e 3d32  .11...urllib3~=2
-00000400: 2e32 0d0a 0979 742d 646c 707e 3d32 3032  .2...yt-dlp~=202
-00000410: 342e 330d 0a70 7974 686f 6e5f 7265 7175  4.3..python_requ
-00000420: 6972 6573 203d 203e 3d33 2e31 300d 0a0d  ires = >=3.10...
-00000430: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-00000440: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
-00000450: 5f73 6372 6970 7473 203d 200d 0a09 636f  _scripts = ...co
-00000460: 6d69 6363 7261 776c 6572 203d 2063 6f6d  miccrawler = com
-00000470: 6963 6372 6177 6c65 722e 636c 693a 636f  iccrawler.cli:co
-00000480: 6e73 6f6c 655f 696e 6974 0d0a 0d0a 5b76  nsole_init....[v
-00000490: 7069 705d 0d0a 636f 6d6d 616e 645f 6661  pip]..command_fa
-000004a0: 6c6c 6261 636b 203d 2070 7974 686f 6e20  llback = python 
-000004b0: 6375 7465 2e70 790d 0a0d 0a5b 6567 675f  cute.py....[egg_
-000004c0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000004d0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000004e0: 300d 0a0d 0a                             0....
+00000030: 342e 320d 0a64 6573 6372 6970 7469 6f6e  4.2..description
+00000040: 203d 2041 6e20 696d 6167 6520 6372 6177   = An image craw
+00000050: 6c65 722c 2069 6e63 6c75 6469 6e67 206d  ler, including m
+00000060: 756c 7469 706c 6520 6d6f 6475 6c65 7320  ultiple modules 
+00000070: 616e 6420 4755 492e 0d0a 6175 7468 6f72  and GUI...author
+00000080: 203d 2065 6967 6874 0d0a 6175 7468 6f72   = eight..author
+00000090: 5f65 6d61 696c 203d 2065 6967 6874 3034  _email = eight04
+000000a0: 4067 6d61 696c 2e63 6f6d 0d0a 636c 6173  @gmail.com..clas
+000000b0: 7369 6669 6572 7320 3d20 0d0a 0944 6576  sifiers = ...Dev
+000000c0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+000000d0: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
+000000e0: 6e2f 5374 6162 6c65 0d0a 0945 6e76 6972  n/Stable...Envir
+000000f0: 6f6e 6d65 6e74 203a 3a20 436f 6e73 6f6c  onment :: Consol
+00000100: 650d 0a09 456e 7669 726f 6e6d 656e 7420  e...Environment 
+00000110: 3a3a 2057 696e 3332 2028 4d53 2057 696e  :: Win32 (MS Win
+00000120: 646f 7773 290d 0a09 496e 7465 6e64 6564  dows)...Intended
+00000130: 2041 7564 6965 6e63 6520 3a3a 2045 6e64   Audience :: End
+00000140: 2055 7365 7273 2f44 6573 6b74 6f70 0d0a   Users/Desktop..
+00000150: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000160: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000170: 4c69 6365 6e73 650d 0a09 4e61 7475 7261  License...Natura
+00000180: 6c20 4c61 6e67 7561 6765 203a 3a20 4368  l Language :: Ch
+00000190: 696e 6573 6520 2854 7261 6469 7469 6f6e  inese (Tradition
+000001a0: 616c 290d 0a09 4f70 6572 6174 696e 6720  al)...Operating 
+000001b0: 5379 7374 656d 203a 3a20 4d69 6372 6f73  System :: Micros
+000001c0: 6f66 7420 3a3a 2057 696e 646f 7773 203a  oft :: Windows :
+000001d0: 3a20 5769 6e64 6f77 7320 370d 0a09 5072  : Windows 7...Pr
+000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000200: 332e 360d 0a09 5072 6f67 7261 6d6d 696e  3.6...Programmin
+00000210: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000220: 7468 6f6e 203a 3a20 332e 380d 0a09 546f  thon :: 3.8...To
+00000230: 7069 6320 3a3a 2049 6e74 6572 6e65 740d  pic :: Internet.
+00000240: 0a6b 6579 776f 7264 7320 3d20 696d 6167  .keywords = imag
+00000250: 652c 2063 7261 776c 6572 0d0a 6c69 6365  e, crawler..lice
+00000260: 6e73 6520 3d20 4d49 540d 0a6c 6f6e 675f  nse = MIT..long_
+00000270: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+00000280: 6c65 3a20 5245 4144 4d45 2e72 7374 0d0a  le: README.rst..
+00000290: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+000002a0: 7468 7562 2e63 6f6d 2f65 6967 6874 3034  thub.com/eight04
+000002b0: 2f43 6f6d 6963 4372 6177 6c65 720d 0a0d  /ComicCrawler...
+000002c0: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
+000002d0: 7361 6665 203d 2046 616c 7365 0d0a 7061  safe = False..pa
+000002e0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+000002f0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000300: 203d 200d 0a09 6265 6c66 7279 7769 6467   = ...belfrywidg
+00000310: 6574 737e 3d31 2e30 0d0a 0962 726f 746c  ets~=1.0...brotl
+00000320: 697e 3d31 2e31 0d0a 0964 656e 6f2d 766d  i~=1.1...deno-vm
+00000330: 7e3d 302e 362e 300d 0a09 6465 736b 746f  ~=0.6.0...deskto
+00000340: 7033 7e3d 302e 352e 330d 0a09 646f 636f  p3~=0.5.3...doco
+00000350: 7074 7e3d 302e 362e 320d 0a09 656e 6c69  pt~=0.6.2...enli
+00000360: 6768 7465 6e7e 3d31 2e31 320d 0a09 7075  ghten~=1.12...pu
+00000370: 7265 6d61 6769 637e 3d31 2e32 310d 0a09  remagic~=1.21...
+00000380: 7079 6372 7970 746f 646f 6d65 787e 3d33  pycryptodomex~=3
+00000390: 2e32 300d 0a09 7079 7468 7265 6164 776f  .20...pythreadwo
+000003a0: 726b 6572 7e3d 302e 3130 2e30 0d0a 0972  rker~=0.10.0...r
+000003b0: 6571 7565 7374 737e 3d32 2e33 310d 0a09  equests~=2.31...
+000003c0: 7361 6665 7072 696e 747e 3d30 2e32 2e30  safeprint~=0.2.0
+000003d0: 0d0a 0975 6e63 7572 6c7e 3d30 2e30 2e31  ...uncurl~=0.0.1
+000003e0: 310d 0a09 7572 6c6c 6962 337e 3d32 2e32  1...urllib3~=2.2
+000003f0: 0d0a 0979 742d 646c 707e 3d32 3032 342e  ...yt-dlp~=2024.
+00000400: 330d 0a70 7974 686f 6e5f 7265 7175 6972  3..python_requir
+00000410: 6573 203d 203e 3d33 2e31 300d 0a0d 0a5b  es = >=3.10....[
+00000420: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
+00000430: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
+00000440: 6372 6970 7473 203d 200d 0a09 636f 6d69  cripts = ...comi
+00000450: 6363 7261 776c 6572 203d 2063 6f6d 6963  ccrawler = comic
+00000460: 6372 6177 6c65 722e 636c 693a 636f 6e73  crawler.cli:cons
+00000470: 6f6c 655f 696e 6974 0d0a 0d0a 5b76 7069  ole_init....[vpi
+00000480: 705d 0d0a 636f 6d6d 616e 645f 6661 6c6c  p]..command_fall
+00000490: 6261 636b 203d 2070 7974 686f 6e20 6375  back = python cu
+000004a0: 7465 2e70 790d 0a0d 0a5b 6567 675f 696e  te.py....[egg_in
+000004b0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+000004c0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000004d0: 0a0d 0a                                  ...
```

