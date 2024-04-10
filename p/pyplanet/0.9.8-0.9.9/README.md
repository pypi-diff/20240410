# Comparing `tmp/pyplanet-0.9.8.tar.gz` & `tmp/pyplanet-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyplanet-0.9.8.tar", last modified: Sun Feb 21 14:32:43 2021, max compression
+gzip compressed data, was "dist/pyplanet-0.9.9.tar", last modified: Sun Feb 21 15:04:23 2021, max compression
```

## Comparing `pyplanet-0.9.8.tar` & `pyplanet-0.9.9.tar`

### file list

```diff
@@ -1,638 +1,638 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.723178 pyplanet-0.9.8/
--rw-r--r--   0 tom       (1000) tom       (1000)    38392 2021-02-21 14:21:45.000000 pyplanet-0.9.8/CHANGELOG.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)    35140 2017-03-12 16:16:19.000000 pyplanet-0.9.8/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2020-04-06 13:57:12.000000 pyplanet-0.9.8/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     3912 2021-02-21 14:32:43.723178 pyplanet-0.9.8/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2413 2020-04-06 13:57:12.000000 pyplanet-0.9.8/README.rst
--rwxrwxr-x   0 tom       (1000) tom       (1000)      210 2017-04-22 17:09:14.000000 pyplanet-0.9.8/cli.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.635179 pyplanet-0.9.8/docs/
--rw-r--r--   0 tom       (1000) tom       (1000)     1623 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/Makefile
--rw-rw-r--   0 tom       (1000) tom       (1000)      921 2017-04-29 13:20:04.000000 pyplanet-0.9.8/docs/make.bat
--rw-rw-r--   0 tom       (1000) tom       (1000)      877 2017-07-02 11:50:04.000000 pyplanet-0.9.8/docs/pyplanet.spec
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.635179 pyplanet-0.9.8/docs/scripts/
--rwxrwxr-x   0 tom       (1000) tom       (1000)     4190 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/scripts/setup.sh
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.635179 pyplanet-0.9.8/docs/source/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.635179 pyplanet-0.9.8/docs/source/_static/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-16 10:38:41.000000 pyplanet-0.9.8/docs/source/_static/.gitkeep
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.635179 pyplanet-0.9.8/docs/source/_static/apps/
--rw-rw-r--   0 tom       (1000) tom       (1000)   114128 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/_static/apps/architecture.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    45786 2017-04-19 15:57:17.000000 pyplanet-0.9.8/docs/source/_static/apps/lifecycle.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    63399 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/_static/architecture-overview.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.635179 pyplanet-0.9.8/docs/source/_static/intro/
--rw-rw-r--   0 tom       (1000) tom       (1000)   181899 2017-06-18 09:32:36.000000 pyplanet-0.9.8/docs/source/_static/intro/python-windows-1.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.639179 pyplanet-0.9.8/docs/source/_static/logo/
--rw-rw-r--   0 tom       (1000) tom       (1000)    81672 2017-04-17 10:50:12.000000 pyplanet-0.9.8/docs/source/_static/logo/pyplanet-sm.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    20820 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/_static/logo/pyplanet-xs.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.639179 pyplanet-0.9.8/docs/source/_static/screenshots/
--rw-rw-r--   0 tom       (1000) tom       (1000)   558555 2017-06-18 09:32:36.000000 pyplanet-0.9.8/docs/source/_static/screenshots/tm_1.jpg
--rw-rw-r--   0 tom       (1000) tom       (1000)   476757 2017-06-18 09:32:36.000000 pyplanet-0.9.8/docs/source/_static/screenshots/tm_2.jpg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.639179 pyplanet-0.9.8/docs/source/_templates/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-16 10:38:41.000000 pyplanet-0.9.8/docs/source/_templates/.gitkeep
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.643179 pyplanet-0.9.8/docs/source/api/
--rw-rw-r--   0 tom       (1000) tom       (1000)      151 2017-05-02 19:48:32.000000 pyplanet-0.9.8/docs/source/api/apps.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)     1059 2017-05-14 16:44:01.000000 pyplanet-0.9.8/docs/source/api/contrib_chat.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      170 2017-06-18 12:03:39.000000 pyplanet-0.9.8/docs/source/api/contrib_command.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      299 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/api/contrib_converter.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      154 2017-04-27 20:26:23.000000 pyplanet-0.9.8/docs/source/api/contrib_map.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      173 2017-05-02 19:22:00.000000 pyplanet-0.9.8/docs/source/api/contrib_mode.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      182 2017-04-27 20:25:38.000000 pyplanet-0.9.8/docs/source/api/contrib_permission.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      166 2017-06-18 12:01:53.000000 pyplanet-0.9.8/docs/source/api/contrib_player.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      252 2017-04-27 20:23:26.000000 pyplanet-0.9.8/docs/source/api/contrib_setting.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      419 2017-05-02 20:11:29.000000 pyplanet-0.9.8/docs/source/api/core_events.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      123 2017-04-22 20:23:59.000000 pyplanet-0.9.8/docs/source/api/core_exceptions.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      111 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/api/core_game.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)       99 2017-05-02 19:50:41.000000 pyplanet-0.9.8/docs/source/api/core_instance.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      471 2017-05-02 19:58:19.000000 pyplanet-0.9.8/docs/source/api/core_storage.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      439 2017-05-16 15:35:51.000000 pyplanet-0.9.8/docs/source/api/core_ui.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      241 2017-05-02 19:28:51.000000 pyplanet-0.9.8/docs/source/api/god.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      379 2017-05-14 16:44:01.000000 pyplanet-0.9.8/docs/source/api/index.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      324 2017-05-02 19:21:14.000000 pyplanet-0.9.8/docs/source/api/utils.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      416 2017-04-28 20:39:49.000000 pyplanet-0.9.8/docs/source/api/views.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.647179 pyplanet-0.9.8/docs/source/apps/
--rw-rw-r--   0 tom       (1000) tom       (1000)      418 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/apps/access_instance.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)       81 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/apps/architecture.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      909 2017-05-14 16:44:01.000000 pyplanet-0.9.8/docs/source/apps/chat.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      553 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/apps/context.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.651178 pyplanet-0.9.8/docs/source/apps/contrib/
--rw-r--r--   0 tom       (1000) tom       (1000)    10474 2020-09-10 12:09:46.000000 pyplanet-0.9.8/docs/source/apps/contrib/admin.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1759 2020-04-07 13:11:02.000000 pyplanet-0.9.8/docs/source/apps/contrib/ads.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1192 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/best_cps.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      628 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/clock.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     2529 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/currentcps.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1895 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/dedimania.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      911 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/dynamic_points.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      453 2021-02-21 14:06:12.000000 pyplanet-0.9.8/docs/source/apps/contrib/dynatime.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1345 2020-04-06 17:58:52.000000 pyplanet-0.9.8/docs/source/apps/contrib/funcmd.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1390 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/jukebox.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      980 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/karma.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1481 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/live_rankings.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1359 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/local_records.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      616 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/mapinfo.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1597 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/apps/contrib/music_server.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     2040 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/mx.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      717 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/players.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     2055 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/queue.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      876 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/sector_times.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1174 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/transactions.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1341 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/contrib/voting.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.651178 pyplanet-0.9.8/docs/source/apps/core/
--rw-r--r--   0 tom       (1000) tom       (1000)      316 2020-04-06 19:33:25.000000 pyplanet-0.9.8/docs/source/apps/core/pyplanet.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1422 2020-04-20 13:07:29.000000 pyplanet-0.9.8/docs/source/apps/core/statistics.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)     2495 2017-05-13 20:24:08.000000 pyplanet-0.9.8/docs/source/apps/create.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      535 2017-05-14 16:44:01.000000 pyplanet-0.9.8/docs/source/apps/gbx.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      608 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/apps/index.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)     2147 2017-09-15 11:31:54.000000 pyplanet-0.9.8/docs/source/apps/lifecycle.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)     1330 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/apps/migrations.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)     3571 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/apps/models.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     5011 2020-07-01 14:23:35.000000 pyplanet-0.9.8/docs/source/apps/ui.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.651178 pyplanet-0.9.8/docs/source/architecture/
--rw-rw-r--   0 tom       (1000) tom       (1000)      179 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/architecture/apps.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      471 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/architecture/core.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      105 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/architecture/index.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)       34 2017-04-27 10:56:10.000000 pyplanet-0.9.8/docs/source/changelog.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     5725 2021-02-21 14:32:28.000000 pyplanet-0.9.8/docs/source/conf.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.651178 pyplanet-0.9.8/docs/source/convert/
--rw-r--r--   0 tom       (1000) tom       (1000)     3466 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/convert/index.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.651178 pyplanet-0.9.8/docs/source/howto/
--rw-r--r--   0 tom       (1000) tom       (1000)     1201 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/howto/dbcollate.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     1199 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/howto/dbindex.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      119 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/howto/index.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     4492 2021-02-21 14:06:12.000000 pyplanet-0.9.8/docs/source/index.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.651178 pyplanet-0.9.8/docs/source/intro/
--rw-r--r--   0 tom       (1000) tom       (1000)    14870 2020-09-10 12:09:46.000000 pyplanet-0.9.8/docs/source/intro/configuration.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      192 2020-03-04 20:58:05.000000 pyplanet-0.9.8/docs/source/intro/index.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     4772 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/intro/installation-linux.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     2003 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/intro/installation-simple.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     3615 2020-09-10 12:09:46.000000 pyplanet-0.9.8/docs/source/intro/installation-windows.rst
--rw-r--r--   0 tom       (1000) tom       (1000)      645 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/intro/requirements.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     9102 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/intro/starting.rst
--rw-r--r--   0 tom       (1000) tom       (1000)     3696 2020-04-06 13:57:12.000000 pyplanet-0.9.8/docs/source/intro/upgrading.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.651178 pyplanet-0.9.8/docs/source/notebooks/
--rw-rw-r--   0 tom       (1000) tom       (1000)     2786 2017-05-03 17:20:03.000000 pyplanet-0.9.8/docs/source/notebooks/set-rounds-points.ipynb
--rw-rw-r--   0 tom       (1000) tom       (1000)     3315 2017-06-18 12:18:14.000000 pyplanet-0.9.8/docs/source/privacy.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.655179 pyplanet-0.9.8/docs/source/signals/
--rw-rw-r--   0 tom       (1000) tom       (1000)       84 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/signals/index.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      479 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/signals/maniaplanet.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)      372 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/signals/shootmania.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)       92 2017-05-11 08:35:33.000000 pyplanet-0.9.8/docs/source/signals/trackmania.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)     1616 2020-04-06 16:39:24.000000 pyplanet-0.9.8/docs/source/support.rst
--rw-rw-r--   0 tom       (1000) tom       (1000)       40 2017-04-27 20:13:27.000000 pyplanet-0.9.8/docs/source/todo.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.655179 pyplanet-0.9.8/pyplanet/
--rw-r--r--   0 tom       (1000) tom       (1000)      175 2021-02-21 14:32:28.000000 pyplanet-0.9.8/pyplanet/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      191 2017-04-22 16:46:20.000000 pyplanet-0.9.8/pyplanet/__main__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.655179 pyplanet-0.9.8/pyplanet/apps/
--rw-rw-r--   0 tom       (1000) tom       (1000)       86 2017-03-17 11:22:13.000000 pyplanet-0.9.8/pyplanet/apps/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6032 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8795 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/config.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.655179 pyplanet-0.9.8/pyplanet/apps/contrib/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-15 15:01:44.000000 pyplanet-0.9.8/pyplanet/apps/contrib/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.655179 pyplanet-0.9.8/pyplanet/apps/contrib/admin/
--rw-r--r--   0 tom       (1000) tom       (1000)     1151 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       53 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/app.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2970 2020-09-10 12:09:46.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/flow.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13757 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/map.py
--rw-r--r--   0 tom       (1000) tom       (1000)      722 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/mapbrowser.py
--rw-r--r--   0 tom       (1000) tom       (1000)    22849 2020-09-10 12:09:46.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/player.py
--rw-r--r--   0 tom       (1000) tom       (1000)      666 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/pyplanet.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9035 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/server.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.623179 pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.655179 pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/setting/
--rw-r--r--   0 tom       (1000) tom       (1000)      840 2020-03-02 20:01:38.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/setting/edit.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     3571 2020-04-09 17:20:41.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/setting/edit.xml
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/toolbar/
--rw-r--r--   0 tom       (1000) tom       (1000)     1431 2020-04-06 19:33:25.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     2686 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1898 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/toolbar.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-23 17:12:13.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2231 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/mapbrowser.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4111 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/players.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6761 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/setting.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2263 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/toolbar.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/ads/
--rw-r--r--   0 tom       (1000) tom       (1000)     8403 2020-07-08 14:53:42.000000 pyplanet-0.9.8/pyplanet/apps/contrib/ads/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/ads/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      315 2020-04-07 11:12:16.000000 pyplanet-0.9.8/pyplanet/apps/contrib/ads/templates/discord_logo.xml
--rw-r--r--   0 tom       (1000) tom       (1000)      349 2020-04-07 11:12:16.000000 pyplanet-0.9.8/pyplanet/apps/contrib/ads/templates/paypal_logo.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1230 2020-04-07 11:12:16.000000 pyplanet-0.9.8/pyplanet/apps/contrib/ads/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/
--rw-r--r--   0 tom       (1000) tom       (1000)     2445 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1326 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/templates/widget_top.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     2630 2020-05-23 19:36:09.000000 pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/clock/
--rw-r--r--   0 tom       (1000) tom       (1000)     1134 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/apps/contrib/clock/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/clock/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      490 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/clock/templates/clock.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)      329 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/clock/templates/clock.xml
--rw-r--r--   0 tom       (1000) tom       (1000)      329 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/clock/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/
--rw-r--r--   0 tom       (1000) tom       (1000)     7273 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       72 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/app.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.659179 pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1095 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/templates/cpwidget.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     2949 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/
--rw-r--r--   0 tom       (1000) tom       (1000)    22291 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    11816 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/api.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       69 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/app.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      540 2017-05-23 17:12:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/exceptions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8158 2020-05-23 19:36:09.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/dynamic_points/
--rw-r--r--   0 tom       (1000) tom       (1000)     4436 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dynamic_points/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/dynatime/
--rw-r--r--   0 tom       (1000) tom       (1000)     2793 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/dynatime/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/
--rw-r--r--   0 tom       (1000) tom       (1000)     4481 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      886 2020-04-06 17:58:52.000000 pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     2236 2020-04-09 17:20:41.000000 pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1268 2020-05-13 09:00:23.000000 pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2003 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/info/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/info/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1505 2020-04-07 15:49:35.000000 pyplanet-0.9.8/pyplanet/apps/contrib/info/templates/mapinfo.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1674 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/info/templates/mapinfo.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1796 2020-03-02 20:01:38.000000 pyplanet-0.9.8/pyplanet/apps/contrib/info/templates/serverinfo.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     2784 2020-07-08 14:53:42.000000 pyplanet-0.9.8/pyplanet/apps/contrib/info/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/
--rw-r--r--   0 tom       (1000) tom       (1000)     8382 2020-09-10 12:09:46.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       61 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/app.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8615 2020-05-09 12:23:13.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/folders.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)      385 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/migrations/000_remove_unique_folder_name.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.663179 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/models/
--rw-r--r--   0 tom       (1000) tom       (1000)      113 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/models/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      791 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/models/mapfolder.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1964 2020-05-09 12:23:13.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/templates/folder_add.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1269 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/templates/folder_create.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     2557 2020-05-09 12:23:13.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/templates/folder_create.xml
--rw-r--r--   0 tom       (1000) tom       (1000)    20920 2021-02-05 09:55:19.000000 pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/karma/
--rw-r--r--   0 tom       (1000) tom       (1000)     9178 2020-09-10 12:09:46.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       53 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/app.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/karma/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)      400 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/migrations/000_add_expanded_score.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/karma/models/
--rw-rw-r--   0 tom       (1000) tom       (1000)       50 2017-04-19 19:57:23.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/models/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      586 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/models/karma.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5515 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/mxkarma.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6559 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/mxkarmaapi.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/karma/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1616 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/templates/karma.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     3262 2020-05-23 19:36:09.000000 pyplanet-0.9.8/pyplanet/apps/contrib/karma/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/
--rw-r--r--   0 tom       (1000) tom       (1000)    10866 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1643 2020-04-09 13:05:21.000000 pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/templates/widget.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     5938 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/
--rw-r--r--   0 tom       (1000) tom       (1000)    11802 2021-02-05 09:55:19.000000 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       81 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/app.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/migrations/
--rw-rw-r--   0 tom       (1000) tom       (1000)      320 2017-05-12 22:59:05.000000 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/migrations/000_make_player_map_unique.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/models/
--rw-rw-r--   0 tom       (1000) tom       (1000)       69 2017-04-19 19:35:22.000000 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/models/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      704 2017-05-12 22:59:05.000000 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/models/local_record.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10517 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/local_records/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.667178 pyplanet-0.9.8/pyplanet/apps/contrib/music_server/
--rw-r--r--   0 tom       (1000) tom       (1000)     6695 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/music_server/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2401 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/music_server/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.671178 pyplanet-0.9.8/pyplanet/apps/contrib/mx/
--rw-r--r--   0 tom       (1000) tom       (1000)    10491 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/mx/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8926 2021-02-21 14:29:02.000000 pyplanet-0.9.8/pyplanet/apps/contrib/mx/api.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       41 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/mx/app.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      157 2017-05-12 22:59:05.000000 pyplanet-0.9.8/pyplanet/apps/contrib/mx/exceptions.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.671178 pyplanet-0.9.8/pyplanet/apps/contrib/mx/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      743 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/mx/templates/search.xml
--rw-r--r--   0 tom       (1000) tom       (1000)    15000 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/mx/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.671178 pyplanet-0.9.8/pyplanet/apps/contrib/players/
--rw-r--r--   0 tom       (1000) tom       (1000)     3361 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/apps/contrib/players/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       61 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/players/app.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1098 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/contrib/players/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.671178 pyplanet-0.9.8/pyplanet/apps/contrib/queue/
--rw-r--r--   0 tom       (1000) tom       (1000)     8665 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/queue/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       93 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/queue/exception.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3563 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/queue/list.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.671178 pyplanet-0.9.8/pyplanet/apps/contrib/queue/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1370 2020-04-06 19:33:25.000000 pyplanet-0.9.8/pyplanet/apps/contrib/queue/templates/queue.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1200 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/queue/templates/queue.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1184 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/queue/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.671178 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/
--rw-r--r--   0 tom       (1000) tom       (1000)     2611 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.671178 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     5706 2020-07-01 14:23:26.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/cp_diff.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1638 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/cp_diff.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     6235 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/cp_diff_next.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1556 2020-04-07 13:11:02.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/gear_indicator.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)      440 2020-04-07 13:11:02.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/gear_indicator.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     7003 2020-07-01 14:23:26.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/sector_times.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1961 2020-09-10 12:09:46.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/sector_times.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     7247 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/sector_times_next.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     4402 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/contrib/transactions/
--rw-r--r--   0 tom       (1000) tom       (1000)     7734 2020-05-18 12:23:53.000000 pyplanet-0.9.8/pyplanet/apps/contrib/transactions/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       81 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/apps/contrib/transactions/app.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/contrib/transactions/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     1545 2020-04-07 16:46:26.000000 pyplanet-0.9.8/pyplanet/apps/contrib/transactions/templates/donation_toolbar.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1338 2020-05-18 12:47:06.000000 pyplanet-0.9.8/pyplanet/apps/contrib/transactions/view.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/contrib/voting/
--rw-r--r--   0 tom       (1000) tom       (1000)    25811 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/voting/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/contrib/voting/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      884 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/voting/templates/voting.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1181 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/voting/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1760 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/contrib/voting/vote.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/core/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:52:55.000000 pyplanet-0.9.8/pyplanet/apps/core/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:15:23.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      541 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/app.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/
--rw-rw-r--   0 tom       (1000) tom       (1000)       48 2017-04-23 09:43:28.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12372 2017-05-14 17:32:42.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/flow.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3582 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/map.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3949 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/other.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8029 2020-07-01 11:02:17.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/player.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1175 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/ui.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)      624 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/migrations/000_add_player_donations_time_stats.py
--rw-r--r--   0 tom       (1000) tom       (1000)      412 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/migrations/001_add_maps_mx_id_column.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.675178 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/models/
--rw-rw-r--   0 tom       (1000) tom       (1000)       82 2017-03-26 15:38:36.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/models/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4156 2020-04-09 13:32:25.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/models/map.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5111 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/models/player.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-26 15:37:58.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9257 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/app.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1054 2020-04-09 17:20:41.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/dev.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/migrations/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-17 15:21:00.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/migrations/.gitkeep
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/models/
--rw-rw-r--   0 tom       (1000) tom       (1000)       99 2017-04-24 18:10:58.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/models/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      613 2017-05-12 22:59:05.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/models/perms.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2041 2017-05-12 22:59:05.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/models/setting.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1089 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/setting.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/call/
--rw-r--r--   0 tom       (1000) tom       (1000)     4394 2020-04-09 17:20:41.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/call/call.xml
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/command/
--rw-r--r--   0 tom       (1000) tom       (1000)     2318 2020-04-09 17:20:41.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/command/details.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     2221 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/controller.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1443 2020-05-13 08:54:05.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/controller.xml
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/setting/
--rw-rw-r--   0 tom       (1000) tom       (1000)      840 2017-04-27 17:56:40.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/setting/edit.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     4321 2020-04-09 17:20:41.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/setting/edit.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     3121 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/toolbar.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     3421 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/toolbar.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1467 2020-04-06 19:33:25.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/toolbar.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-26 15:28:10.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7113 2020-04-09 17:20:41.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/call.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3538 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/command.py
--rw-r--r--   0 tom       (1000) tom       (1000)      850 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/controller.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6262 2020-04-07 12:06:21.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/setting.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1043 2020-09-10 12:09:46.000000 pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/toolbar.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.679179 pyplanet-0.9.8/pyplanet/apps/core/shootmania/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:15:23.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      222 2017-05-18 16:38:48.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/app.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.683179 pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/
--rw-rw-r--   0 tom       (1000) tom       (1000)       47 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17223 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/base.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1692 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/elite.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2245 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/joust.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1844 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/royal.py
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-14 16:44:01.000000 pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/siege.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.683179 pyplanet-0.9.8/pyplanet/apps/core/statistics/
--rw-r--r--   0 tom       (1000) tom       (1000)      872 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       79 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/app.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      615 2017-05-03 16:25:53.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1166 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/mp.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4941 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/processor.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.683179 pyplanet-0.9.8/pyplanet/apps/core/statistics/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)     2591 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/templates/dashboard.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     2319 2020-10-16 14:05:49.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/tm.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.683179 pyplanet-0.9.8/pyplanet/apps/core/statistics/views/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/views/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      290 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/views/base.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1901 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/views/dashboard.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3019 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/views/players.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2243 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/views/records.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9410 2020-04-20 13:07:29.000000 pyplanet-0.9.8/pyplanet/apps/core/statistics/views/score.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.683179 pyplanet-0.9.8/pyplanet/apps/core/trackmania/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:15:23.000000 pyplanet-0.9.8/pyplanet/apps/core/trackmania/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      746 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/core/trackmania/app.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14142 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/apps/core/trackmania/callbacks.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.683179 pyplanet-0.9.8/pyplanet/bin/
--rwxrwxr-x   0 tom       (1000) tom       (1000)      128 2017-04-22 17:09:27.000000 pyplanet-0.9.8/pyplanet/bin/pyplanet
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/conf/
--rw-r--r--   0 tom       (1000) tom       (1000)     2680 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/conf/app_template/
--rw-rw-r--   0 tom       (1000) tom       (1000)      387 2020-04-05 20:40:52.000000 pyplanet-0.9.8/pyplanet/conf/app_template/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       32 2017-04-22 18:15:29.000000 pyplanet-0.9.8/pyplanet/conf/app_template/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/conf/backends/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/backends/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2210 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/backends/base.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1649 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/backends/file.py
--rw-r--r--   0 tom       (1000) tom       (1000)      962 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/backends/json.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1598 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/backends/python.py
--rw-r--r--   0 tom       (1000) tom       (1000)      937 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/backends/yaml.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5731 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/default_settings.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/conf/project_template/
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1258 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/project_template/manage.py
--rw-r--r--   0 tom       (1000) tom       (1000)       79 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/project_template/requirements.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/conf/project_template/settings/
--rw-r--r--   0 tom       (1000) tom       (1000)      447 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/project_template/settings/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1959 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/project_template/settings/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2980 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/conf/project_template/settings/base.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/contrib/
--rw-rw-r--   0 tom       (1000) tom       (1000)      339 2017-04-26 14:11:32.000000 pyplanet-0.9.8/pyplanet/contrib/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/contrib/chat/
--rw-rw-r--   0 tom       (1000) tom       (1000)      213 2017-05-14 16:44:01.000000 pyplanet-0.9.8/pyplanet/contrib/chat/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       40 2017-05-14 16:44:01.000000 pyplanet-0.9.8/pyplanet/contrib/chat/exceptions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1720 2017-05-14 16:44:01.000000 pyplanet-0.9.8/pyplanet/contrib/chat/manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4764 2017-06-18 09:32:36.000000 pyplanet-0.9.8/pyplanet/contrib/chat/query.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.687178 pyplanet-0.9.8/pyplanet/contrib/command/
--rw-rw-r--   0 tom       (1000) tom       (1000)      256 2017-04-23 20:32:27.000000 pyplanet-0.9.8/pyplanet/contrib/command/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7587 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/command/command.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      363 2017-03-25 20:46:30.000000 pyplanet-0.9.8/pyplanet/contrib/command/exceptions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3943 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/command/manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4034 2017-05-11 08:58:44.000000 pyplanet-0.9.8/pyplanet/contrib/command/params.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.691178 pyplanet-0.9.8/pyplanet/contrib/converter/
--rw-r--r--   0 tom       (1000) tom       (1000)      677 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/converter/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1716 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/converter/base.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5443 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/converter/expansion.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5741 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/converter/maniacontrol.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7162 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/converter/uaseco.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6164 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/contrib/converter/xaseco2.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.691178 pyplanet-0.9.8/pyplanet/contrib/map/
--rw-rw-r--   0 tom       (1000) tom       (1000)      146 2017-04-23 20:35:30.000000 pyplanet-0.9.8/pyplanet/contrib/map/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/map/exceptions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17241 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/contrib/map/manager.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.691178 pyplanet-0.9.8/pyplanet/contrib/mode/
--rw-rw-r--   0 tom       (1000) tom       (1000)      212 2017-05-02 19:10:15.000000 pyplanet-0.9.8/pyplanet/contrib/mode/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-01 18:42:05.000000 pyplanet-0.9.8/pyplanet/contrib/mode/exceptions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6054 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/contrib/mode/manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      600 2017-05-02 19:10:15.000000 pyplanet-0.9.8/pyplanet/contrib/mode/signals.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.691178 pyplanet-0.9.8/pyplanet/contrib/permission/
--rw-rw-r--   0 tom       (1000) tom       (1000)      169 2017-03-26 15:03:53.000000 pyplanet-0.9.8/pyplanet/contrib/permission/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-26 15:03:59.000000 pyplanet-0.9.8/pyplanet/contrib/permission/exceptions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2768 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/contrib/permission/manager.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.691178 pyplanet-0.9.8/pyplanet/contrib/player/
--rw-rw-r--   0 tom       (1000) tom       (1000)      157 2017-03-23 16:31:59.000000 pyplanet-0.9.8/pyplanet/contrib/player/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       94 2017-04-23 20:33:28.000000 pyplanet-0.9.8/pyplanet/contrib/player/exceptions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13902 2020-09-10 12:09:46.000000 pyplanet-0.9.8/pyplanet/contrib/player/manager.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.691178 pyplanet-0.9.8/pyplanet/contrib/setting/
--rw-rw-r--   0 tom       (1000) tom       (1000)      212 2017-05-01 18:42:05.000000 pyplanet-0.9.8/pyplanet/contrib/setting/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      284 2017-05-12 23:28:22.000000 pyplanet-0.9.8/pyplanet/contrib/setting/core_settings.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      286 2017-04-27 20:23:24.000000 pyplanet-0.9.8/pyplanet/contrib/setting/exceptions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8244 2020-04-07 11:35:40.000000 pyplanet-0.9.8/pyplanet/contrib/setting/manager.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7335 2020-04-07 13:11:02.000000 pyplanet-0.9.8/pyplanet/contrib/setting/setting.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.695178 pyplanet-0.9.8/pyplanet/core/
--rw-rw-r--   0 tom       (1000) tom       (1000)      173 2017-05-14 16:44:01.000000 pyplanet-0.9.8/pyplanet/core/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.695178 pyplanet-0.9.8/pyplanet/core/checks/
--rw-rw-r--   0 tom       (1000) tom       (1000)      347 2020-04-07 09:09:12.000000 pyplanet-0.9.8/pyplanet/core/checks/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1937 2017-05-01 13:35:06.000000 pyplanet-0.9.8/pyplanet/core/checks/messages.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1582 2020-04-07 09:39:40.000000 pyplanet-0.9.8/pyplanet/core/checks/registry.py
--rw-r--r--   0 tom       (1000) tom       (1000)      823 2020-03-02 20:01:38.000000 pyplanet-0.9.8/pyplanet/core/controller.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.695178 pyplanet-0.9.8/pyplanet/core/db/
--rw-rw-r--   0 tom       (1000) tom       (1000)      226 2017-04-09 19:02:44.000000 pyplanet-0.9.8/pyplanet/core/db/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3169 2017-06-18 09:32:36.000000 pyplanet-0.9.8/pyplanet/core/db/database.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4274 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/db/migrator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3948 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/core/db/model.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.695178 pyplanet-0.9.8/pyplanet/core/db/models/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-17 13:40:22.000000 pyplanet-0.9.8/pyplanet/core/db/models/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      166 2017-03-17 13:41:04.000000 pyplanet-0.9.8/pyplanet/core/db/models/migration.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2036 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/core/db/registry.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.695178 pyplanet-0.9.8/pyplanet/core/events/
--rw-rw-r--   0 tom       (1000) tom       (1000)      242 2017-04-26 14:11:32.000000 pyplanet-0.9.8/pyplanet/core/events/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2070 2017-05-23 17:12:13.000000 pyplanet-0.9.8/pyplanet/core/events/callback.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10041 2017-05-23 17:12:13.000000 pyplanet-0.9.8/pyplanet/core/events/dispatcher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6932 2018-03-11 13:38:21.000000 pyplanet-0.9.8/pyplanet/core/events/manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      593 2017-03-25 19:00:05.000000 pyplanet-0.9.8/pyplanet/core/exceptions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/core/game.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.695178 pyplanet-0.9.8/pyplanet/core/gbx/
--rw-rw-r--   0 tom       (1000) tom       (1000)       83 2017-05-14 16:44:01.000000 pyplanet-0.9.8/pyplanet/core/gbx/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9013 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/core/gbx/client.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3225 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/core/gbx/query.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10697 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/gbx/remote.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7545 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/core/instance.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.699178 pyplanet-0.9.8/pyplanet/core/management/
--rw-r--r--   0 tom       (1000) tom       (1000)     9058 2020-04-07 09:39:40.000000 pyplanet-0.9.8/pyplanet/core/management/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    15492 2020-04-07 09:16:40.000000 pyplanet-0.9.8/pyplanet/core/management/base.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2017-04-22 15:18:33.000000 pyplanet-0.9.8/pyplanet/core/management/color.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.699178 pyplanet-0.9.8/pyplanet/core/management/commands/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-22 14:56:11.000000 pyplanet-0.9.8/pyplanet/core/management/commands/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2189 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/management/commands/db_convert.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      906 2017-05-13 20:24:08.000000 pyplanet-0.9.8/pyplanet/core/management/commands/init_app.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      863 2017-06-18 09:32:36.000000 pyplanet-0.9.8/pyplanet/core/management/commands/init_project.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3723 2020-04-07 09:13:25.000000 pyplanet-0.9.8/pyplanet/core/management/commands/start.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1785 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/management/commands/upgrade.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1599 2017-04-26 14:38:04.000000 pyplanet-0.9.8/pyplanet/core/management/management.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5555 2017-06-18 09:32:36.000000 pyplanet-0.9.8/pyplanet/core/management/templates.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1344 2017-05-12 23:28:22.000000 pyplanet-0.9.8/pyplanet/core/signals.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.699178 pyplanet-0.9.8/pyplanet/core/storage/
--rw-rw-r--   0 tom       (1000) tom       (1000)      107 2017-04-15 11:03:27.000000 pyplanet-0.9.8/pyplanet/core/storage/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.699178 pyplanet-0.9.8/pyplanet/core/storage/drivers/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-09 19:46:06.000000 pyplanet-0.9.8/pyplanet/core/storage/drivers/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.699178 pyplanet-0.9.8/pyplanet/core/storage/drivers/asyncssh/
--rw-r--r--   0 tom       (1000) tom       (1000)     5676 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/storage/drivers/asyncssh/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.699178 pyplanet-0.9.8/pyplanet/core/storage/drivers/local/
--rw-r--r--   0 tom       (1000) tom       (1000)     2653 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/storage/drivers/local/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       67 2017-04-29 13:42:23.000000 pyplanet-0.9.8/pyplanet/core/storage/exceptions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2400 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/storage/interface.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3977 2020-01-26 17:49:37.000000 pyplanet-0.9.8/pyplanet/core/storage/storage.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.703179 pyplanet-0.9.8/pyplanet/core/ui/
--rw-r--r--   0 tom       (1000) tom       (1000)     8387 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/core/ui/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.703179 pyplanet-0.9.8/pyplanet/core/ui/components/
--rw-rw-r--   0 tom       (1000) tom       (1000)      114 2017-04-28 20:32:19.000000 pyplanet-0.9.8/pyplanet/core/ui/components/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8082 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/core/ui/components/manialink.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      421 2017-05-16 15:35:51.000000 pyplanet-0.9.8/pyplanet/core/ui/exceptions.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.703179 pyplanet-0.9.8/pyplanet/core/ui/filters/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-15 11:40:44.000000 pyplanet-0.9.8/pyplanet/core/ui/filters/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      913 2017-04-28 20:26:16.000000 pyplanet-0.9.8/pyplanet/core/ui/loader.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1410 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/core/ui/template.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7714 2021-02-21 14:06:12.000000 pyplanet-0.9.8/pyplanet/core/ui/ui_properties.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.703179 pyplanet-0.9.8/pyplanet/god/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-13 20:00:09.000000 pyplanet-0.9.8/pyplanet/god/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3283 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/god/pool.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3272 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/god/process.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.703179 pyplanet-0.9.8/pyplanet/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-12 18:25:07.000000 pyplanet-0.9.8/pyplanet/utils/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2167 2020-07-06 18:00:34.000000 pyplanet-0.9.8/pyplanet/utils/analytics.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      675 2017-04-19 16:19:15.000000 pyplanet-0.9.8/pyplanet/utils/codeutils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      131 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/utils/functional.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8159 2020-07-06 18:00:34.000000 pyplanet-0.9.8/pyplanet/utils/gbxparser.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      374 2017-03-25 16:53:08.000000 pyplanet-0.9.8/pyplanet/utils/livereload.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4035 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/utils/log.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      865 2017-04-27 18:55:11.000000 pyplanet-0.9.8/pyplanet/utils/memleak.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4244 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/utils/pip.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.703179 pyplanet-0.9.8/pyplanet/utils/pip_test_pkg/
--rw-r--r--   0 tom       (1000) tom       (1000)     1600 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/utils/pip_test_pkg/setup.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2489 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/utils/releases.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9238 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/utils/semver.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3565 2017-05-11 08:35:33.000000 pyplanet-0.9.8/pyplanet/utils/style.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6369 2017-04-22 14:39:05.000000 pyplanet-0.9.8/pyplanet/utils/termcolors.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1090 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/utils/times.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      599 2017-04-26 14:42:19.000000 pyplanet-0.9.8/pyplanet/utils/toposort.py
--rw-r--r--   0 tom       (1000) tom       (1000)      472 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/utils/zone.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.707178 pyplanet-0.9.8/pyplanet/views/
--rw-rw-r--   0 tom       (1000) tom       (1000)       98 2017-04-22 19:25:36.000000 pyplanet-0.9.8/pyplanet/views/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      184 2017-04-22 19:48:52.000000 pyplanet-0.9.8/pyplanet/views/base.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.707178 pyplanet-0.9.8/pyplanet/views/generics/
--rw-rw-r--   0 tom       (1000) tom       (1000)      199 2017-06-18 09:32:36.000000 pyplanet-0.9.8/pyplanet/views/generics/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8893 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/views/generics/alert.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14069 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/views/generics/list.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3000 2020-04-07 16:46:26.000000 pyplanet-0.9.8/pyplanet/views/generics/widget.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5805 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/views/template.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.631179 pyplanet-0.9.8/pyplanet/views/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.707178 pyplanet-0.9.8/pyplanet/views/templates/generics/
--rw-r--r--   0 tom       (1000) tom       (1000)     1701 2020-01-17 13:07:25.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/alert.xml
--rw-r--r--   0 tom       (1000) tom       (1000)      379 2020-01-17 13:07:25.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/list.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     7988 2020-10-16 14:18:04.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/list.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     1928 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/prompt.xml
--rw-r--r--   0 tom       (1000) tom       (1000)      961 2020-01-17 13:07:25.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/timeswidget.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     4536 2020-05-13 08:57:07.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/widget.Script.Txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1389 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/widget.xml
--rw-r--r--   0 tom       (1000) tom       (1000)     2421 2020-07-01 14:23:35.000000 pyplanet-0.9.8/pyplanet/views/templates/generics/widget_next.Script.Txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.707178 pyplanet-0.9.8/pyplanet/views/templates/libs/
--rw-r--r--   0 tom       (1000) tom       (1000)      736 2020-03-02 20:01:38.000000 pyplanet-0.9.8/pyplanet/views/templates/libs/TimeUtils.Script.Txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.655179 pyplanet-0.9.8/pyplanet.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     3912 2021-02-21 14:32:42.000000 pyplanet-0.9.8/pyplanet.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)    18867 2021-02-21 14:32:43.000000 pyplanet-0.9.8/pyplanet.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-02-21 14:32:42.000000 pyplanet-0.9.8/pyplanet.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       81 2021-02-21 14:32:42.000000 pyplanet-0.9.8/pyplanet.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-02-21 14:32:39.000000 pyplanet-0.9.8/pyplanet.egg-info/not-zip-safe
--rw-r--r--   0 tom       (1000) tom       (1000)      379 2021-02-21 14:32:42.000000 pyplanet-0.9.8/pyplanet.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2021-02-21 14:32:42.000000 pyplanet-0.9.8/pyplanet.egg-info/top_level.txt
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1037 2020-04-06 13:57:12.000000 pyplanet-0.9.8/pyplanet.py
--rw-r--r--   0 tom       (1000) tom       (1000)      246 2020-04-06 13:57:12.000000 pyplanet-0.9.8/requirements-dev.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      434 2020-04-06 13:57:12.000000 pyplanet-0.9.8/requirements.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       80 2021-02-21 14:32:43.723178 pyplanet-0.9.8/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     2404 2020-04-06 13:57:12.000000 pyplanet-0.9.8/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.707178 pyplanet-0.9.8/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)      293 2017-04-19 15:38:58.000000 pyplanet-0.9.8/tests/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.631179 pyplanet-0.9.8/tests/_files/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.711178 pyplanet-0.9.8/tests/_files/maps/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-30 15:23:26.000000 pyplanet-0.9.8/tests/_files/maps/.gitkeep
--rw-rw-r--   0 tom       (1000) tom       (1000)   263043 2017-03-30 16:47:30.000000 pyplanet-0.9.8/tests/_files/maps/canyon-mp4-1.gbx
--rw-rw-r--   0 tom       (1000) tom       (1000)   455963 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/_files/maps/canyon-mp4-2.gbx
--rw-rw-r--   0 tom       (1000) tom       (1000)   468177 2017-04-09 15:15:12.000000 pyplanet-0.9.8/tests/_files/maps/greyroad.gbx
--rw-rw-r--   0 tom       (1000) tom       (1000)   604744 2017-03-30 16:47:52.000000 pyplanet-0.9.8/tests/_files/maps/royal-mp4-1.gbx
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.715178 pyplanet-0.9.8/tests/_scripts/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.631179 pyplanet-0.9.8/tests/_scripts/appveyor/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.715178 pyplanet-0.9.8/tests/_scripts/appveyor/dedicated/
--rw-r--r--   0 tom       (1000) tom       (1000)     3898 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/dedicated/dedicated_cfg.txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1532 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/dedicated/matchsettings_1.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.715178 pyplanet-0.9.8/tests/_scripts/appveyor/settings/
--rw-r--r--   0 tom       (1000) tom       (1000)      271 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/settings/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      573 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/settings/apps.json
--rw-r--r--   0 tom       (1000) tom       (1000)     1301 2020-05-13 09:46:44.000000 pyplanet-0.9.8/tests/_scripts/appveyor/settings/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      493 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/settings/apps.yaml
--rw-r--r--   0 tom       (1000) tom       (1000)      736 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/settings/base.json
--rw-r--r--   0 tom       (1000) tom       (1000)     2254 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/settings/base.py
--rw-r--r--   0 tom       (1000) tom       (1000)      530 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor/settings/base.yaml
--rw-r--r--   0 tom       (1000) tom       (1000)       93 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor_config.ps1
--rw-r--r--   0 tom       (1000) tom       (1000)     4103 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor_init.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1598 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/appveyor_with_compiler.cmd
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.631179 pyplanet-0.9.8/tests/_scripts/travis/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.715178 pyplanet-0.9.8/tests/_scripts/travis/dedicated/
--rw-r--r--   0 tom       (1000) tom       (1000)     3898 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis/dedicated/dedicated_cfg.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1532 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/_scripts/travis/dedicated/matchsettings_1.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/_scripts/travis/settings/
--rw-rw-r--   0 tom       (1000) tom       (1000)      271 2017-03-14 14:13:30.000000 pyplanet-0.9.8/tests/_scripts/travis/settings/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      573 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis/settings/apps.json
--rw-r--r--   0 tom       (1000) tom       (1000)     1301 2020-05-13 09:46:44.000000 pyplanet-0.9.8/tests/_scripts/travis/settings/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      493 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis/settings/apps.yaml
--rw-r--r--   0 tom       (1000) tom       (1000)      725 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis/settings/base.json
--rw-r--r--   0 tom       (1000) tom       (1000)     2243 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis/settings/base.py
--rw-r--r--   0 tom       (1000) tom       (1000)      519 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis/settings/base.yaml
--rwxrwxr-x   0 tom       (1000) tom       (1000)      227 2017-04-22 23:23:40.000000 pyplanet-0.9.8/tests/_scripts/travis_config.sh
--rwxr-xr-x   0 tom       (1000) tom       (1000)      340 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis_coverage.sh
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1251 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis_dedicated_setup.sh
--rwxr-xr-x   0 tom       (1000) tom       (1000)      837 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/_scripts/travis_dedicated_start.sh
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/apps/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-19 15:28:37.000000 pyplanet-0.9.8/tests/apps/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/apps/migration_test/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2017-05-13 20:24:08.000000 pyplanet-0.9.8/tests/apps/migration_test/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       85 2017-05-13 20:24:08.000000 pyplanet-0.9.8/tests/apps/migration_test/app.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/apps/migration_test/migrations/
--rw-rw-r--   0 tom       (1000) tom       (1000)      327 2017-04-19 17:22:41.000000 pyplanet-0.9.8/tests/apps/migration_test/migrations/000_sample_field.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      272 2017-04-19 15:14:46.000000 pyplanet-0.9.8/tests/apps/migration_test/migrations/001_remove_player_field.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      284 2017-04-19 15:14:35.000000 pyplanet-0.9.8/tests/apps/migration_test/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/apps/new_import_style/
--rw-rw-r--   0 tom       (1000) tom       (1000)       84 2017-05-13 20:24:08.000000 pyplanet-0.9.8/tests/apps/new_import_style/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/integration/
--rw-rw-r--   0 tom       (1000) tom       (1000)      446 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/integration/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/integration/contrib/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/integration/contrib/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1265 2017-05-23 17:12:08.000000 pyplanet-0.9.8/tests/integration/contrib/test_map.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      830 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/integration/contrib/test_player.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3208 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/integration/test_gbx.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      619 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/integration/test_instance.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.719178 pyplanet-0.9.8/tests/unit/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-26 14:25:28.000000 pyplanet-0.9.8/tests/unit/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.723178 pyplanet-0.9.8/tests/unit/contrib/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/unit/contrib/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2646 2017-05-14 16:44:01.000000 pyplanet-0.9.8/tests/unit/contrib/test_chat.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2182 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/unit/contrib/test_commands.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2277 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/unit/contrib/test_permissions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2228 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/unit/contrib/test_settings.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.723178 pyplanet-0.9.8/tests/unit/storage/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-30 12:34:12.000000 pyplanet-0.9.8/tests/unit/storage/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1493 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/unit/storage/test_local_driver.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      511 2017-04-30 12:34:12.000000 pyplanet-0.9.8/tests/unit/storage/test_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2017-09-15 11:31:54.000000 pyplanet-0.9.8/tests/unit/test_callbacks.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1083 2020-04-06 13:57:12.000000 pyplanet-0.9.8/tests/unit/test_conf.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1816 2017-05-11 08:35:33.000000 pyplanet-0.9.8/tests/unit/test_database.py
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-26 18:33:10.000000 pyplanet-0.9.8/tests/unit/test_db_migrator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3105 2017-09-15 11:31:54.000000 pyplanet-0.9.8/tests/unit/test_signals.py
--rw-r--r--   0 tom       (1000) tom       (1000)      823 2020-01-17 15:14:28.000000 pyplanet-0.9.8/tests/unit/test_ui_template.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1147 2017-04-30 12:34:12.000000 pyplanet-0.9.8/tests/unit/test_views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 14:32:43.723178 pyplanet-0.9.8/tests/unit/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-30 14:48:30.000000 pyplanet-0.9.8/tests/unit/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2508 2017-04-26 17:33:09.000000 pyplanet-0.9.8/tests/unit/utils/test_gbxparser.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2017-05-30 14:28:01.000000 pyplanet-0.9.8/tests/unit/utils/test_style.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      447 2017-03-30 15:21:11.000000 pyplanet-0.9.8/tests/unit/utils/test_times.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      602 2017-04-30 12:34:12.000000 pyplanet-0.9.8/tests/unit/utils/test_toposort.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.164791 pyplanet-0.9.9/
+-rw-r--r--   0 tom       (1000) tom       (1000)    38455 2021-02-21 15:03:15.000000 pyplanet-0.9.9/CHANGELOG.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35140 2017-03-12 16:16:19.000000 pyplanet-0.9.9/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2020-04-06 13:57:12.000000 pyplanet-0.9.9/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     3912 2021-02-21 15:04:23.164791 pyplanet-0.9.9/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2413 2020-04-06 13:57:12.000000 pyplanet-0.9.9/README.rst
+-rwxrwxr-x   0 tom       (1000) tom       (1000)      210 2017-04-22 17:09:14.000000 pyplanet-0.9.9/cli.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.048792 pyplanet-0.9.9/docs/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1623 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/Makefile
+-rw-rw-r--   0 tom       (1000) tom       (1000)      921 2017-04-29 13:20:04.000000 pyplanet-0.9.9/docs/make.bat
+-rw-rw-r--   0 tom       (1000) tom       (1000)      877 2017-07-02 11:50:04.000000 pyplanet-0.9.9/docs/pyplanet.spec
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.048792 pyplanet-0.9.9/docs/scripts/
+-rwxrwxr-x   0 tom       (1000) tom       (1000)     4190 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/scripts/setup.sh
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.052791 pyplanet-0.9.9/docs/source/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.052791 pyplanet-0.9.9/docs/source/_static/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-16 10:38:41.000000 pyplanet-0.9.9/docs/source/_static/.gitkeep
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.056791 pyplanet-0.9.9/docs/source/_static/apps/
+-rw-rw-r--   0 tom       (1000) tom       (1000)   114128 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/_static/apps/architecture.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    45786 2017-04-19 15:57:17.000000 pyplanet-0.9.9/docs/source/_static/apps/lifecycle.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    63399 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/_static/architecture-overview.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.056791 pyplanet-0.9.9/docs/source/_static/intro/
+-rw-rw-r--   0 tom       (1000) tom       (1000)   181899 2017-06-18 09:32:36.000000 pyplanet-0.9.9/docs/source/_static/intro/python-windows-1.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.056791 pyplanet-0.9.9/docs/source/_static/logo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    81672 2017-04-17 10:50:12.000000 pyplanet-0.9.9/docs/source/_static/logo/pyplanet-sm.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20820 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/_static/logo/pyplanet-xs.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.060792 pyplanet-0.9.9/docs/source/_static/screenshots/
+-rw-rw-r--   0 tom       (1000) tom       (1000)   558555 2017-06-18 09:32:36.000000 pyplanet-0.9.9/docs/source/_static/screenshots/tm_1.jpg
+-rw-rw-r--   0 tom       (1000) tom       (1000)   476757 2017-06-18 09:32:36.000000 pyplanet-0.9.9/docs/source/_static/screenshots/tm_2.jpg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.064792 pyplanet-0.9.9/docs/source/_templates/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-16 10:38:41.000000 pyplanet-0.9.9/docs/source/_templates/.gitkeep
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.068791 pyplanet-0.9.9/docs/source/api/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      151 2017-05-02 19:48:32.000000 pyplanet-0.9.9/docs/source/api/apps.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1059 2017-05-14 16:44:01.000000 pyplanet-0.9.9/docs/source/api/contrib_chat.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      170 2017-06-18 12:03:39.000000 pyplanet-0.9.9/docs/source/api/contrib_command.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      299 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/api/contrib_converter.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      154 2017-04-27 20:26:23.000000 pyplanet-0.9.9/docs/source/api/contrib_map.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      173 2017-05-02 19:22:00.000000 pyplanet-0.9.9/docs/source/api/contrib_mode.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      182 2017-04-27 20:25:38.000000 pyplanet-0.9.9/docs/source/api/contrib_permission.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      166 2017-06-18 12:01:53.000000 pyplanet-0.9.9/docs/source/api/contrib_player.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      252 2017-04-27 20:23:26.000000 pyplanet-0.9.9/docs/source/api/contrib_setting.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      419 2017-05-02 20:11:29.000000 pyplanet-0.9.9/docs/source/api/core_events.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      123 2017-04-22 20:23:59.000000 pyplanet-0.9.9/docs/source/api/core_exceptions.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      111 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/api/core_game.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)       99 2017-05-02 19:50:41.000000 pyplanet-0.9.9/docs/source/api/core_instance.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      471 2017-05-02 19:58:19.000000 pyplanet-0.9.9/docs/source/api/core_storage.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      439 2017-05-16 15:35:51.000000 pyplanet-0.9.9/docs/source/api/core_ui.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      241 2017-05-02 19:28:51.000000 pyplanet-0.9.9/docs/source/api/god.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      379 2017-05-14 16:44:01.000000 pyplanet-0.9.9/docs/source/api/index.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      324 2017-05-02 19:21:14.000000 pyplanet-0.9.9/docs/source/api/utils.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      416 2017-04-28 20:39:49.000000 pyplanet-0.9.9/docs/source/api/views.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.068791 pyplanet-0.9.9/docs/source/apps/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      418 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/apps/access_instance.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)       81 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/apps/architecture.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      909 2017-05-14 16:44:01.000000 pyplanet-0.9.9/docs/source/apps/chat.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      553 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/apps/context.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.076791 pyplanet-0.9.9/docs/source/apps/contrib/
+-rw-r--r--   0 tom       (1000) tom       (1000)    10474 2020-09-10 12:09:46.000000 pyplanet-0.9.9/docs/source/apps/contrib/admin.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1759 2020-04-07 13:11:02.000000 pyplanet-0.9.9/docs/source/apps/contrib/ads.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1192 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/best_cps.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      628 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/clock.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     2529 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/currentcps.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1895 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/dedimania.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      911 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/dynamic_points.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      453 2021-02-21 14:06:12.000000 pyplanet-0.9.9/docs/source/apps/contrib/dynatime.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1345 2020-04-06 17:58:52.000000 pyplanet-0.9.9/docs/source/apps/contrib/funcmd.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1390 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/jukebox.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      980 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/karma.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1481 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/live_rankings.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1359 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/local_records.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      616 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/mapinfo.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1597 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/apps/contrib/music_server.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     2040 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/mx.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      717 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/players.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     2055 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/queue.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      876 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/sector_times.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1174 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/transactions.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1341 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/contrib/voting.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.076791 pyplanet-0.9.9/docs/source/apps/core/
+-rw-r--r--   0 tom       (1000) tom       (1000)      316 2020-04-06 19:33:25.000000 pyplanet-0.9.9/docs/source/apps/core/pyplanet.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1422 2020-04-20 13:07:29.000000 pyplanet-0.9.9/docs/source/apps/core/statistics.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2495 2017-05-13 20:24:08.000000 pyplanet-0.9.9/docs/source/apps/create.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      535 2017-05-14 16:44:01.000000 pyplanet-0.9.9/docs/source/apps/gbx.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      608 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/apps/index.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2147 2017-09-15 11:31:54.000000 pyplanet-0.9.9/docs/source/apps/lifecycle.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1330 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/apps/migrations.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3571 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/apps/models.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     5011 2020-07-01 14:23:35.000000 pyplanet-0.9.9/docs/source/apps/ui.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.076791 pyplanet-0.9.9/docs/source/architecture/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      179 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/architecture/apps.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      471 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/architecture/core.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      105 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/architecture/index.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)       34 2017-04-27 10:56:10.000000 pyplanet-0.9.9/docs/source/changelog.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     5725 2021-02-21 15:03:21.000000 pyplanet-0.9.9/docs/source/conf.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.076791 pyplanet-0.9.9/docs/source/convert/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3466 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/convert/index.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.076791 pyplanet-0.9.9/docs/source/howto/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1201 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/howto/dbcollate.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     1199 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/howto/dbindex.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      119 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/howto/index.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     4492 2021-02-21 14:06:12.000000 pyplanet-0.9.9/docs/source/index.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.080791 pyplanet-0.9.9/docs/source/intro/
+-rw-r--r--   0 tom       (1000) tom       (1000)    14870 2020-09-10 12:09:46.000000 pyplanet-0.9.9/docs/source/intro/configuration.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      192 2020-03-04 20:58:05.000000 pyplanet-0.9.9/docs/source/intro/index.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     4772 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/intro/installation-linux.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     2003 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/intro/installation-simple.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     3615 2020-09-10 12:09:46.000000 pyplanet-0.9.9/docs/source/intro/installation-windows.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)      645 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/intro/requirements.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     9102 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/intro/starting.rst
+-rw-r--r--   0 tom       (1000) tom       (1000)     3696 2020-04-06 13:57:12.000000 pyplanet-0.9.9/docs/source/intro/upgrading.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.080791 pyplanet-0.9.9/docs/source/notebooks/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2786 2017-05-03 17:20:03.000000 pyplanet-0.9.9/docs/source/notebooks/set-rounds-points.ipynb
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3315 2017-06-18 12:18:14.000000 pyplanet-0.9.9/docs/source/privacy.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.080791 pyplanet-0.9.9/docs/source/signals/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       84 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/signals/index.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      479 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/signals/maniaplanet.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)      372 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/signals/shootmania.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)       92 2017-05-11 08:35:33.000000 pyplanet-0.9.9/docs/source/signals/trackmania.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1616 2020-04-06 16:39:24.000000 pyplanet-0.9.9/docs/source/support.rst
+-rw-rw-r--   0 tom       (1000) tom       (1000)       40 2017-04-27 20:13:27.000000 pyplanet-0.9.9/docs/source/todo.rst
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.080791 pyplanet-0.9.9/pyplanet/
+-rw-r--r--   0 tom       (1000) tom       (1000)      175 2021-02-21 15:03:21.000000 pyplanet-0.9.9/pyplanet/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      191 2017-04-22 16:46:20.000000 pyplanet-0.9.9/pyplanet/__main__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.084791 pyplanet-0.9.9/pyplanet/apps/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       86 2017-03-17 11:22:13.000000 pyplanet-0.9.9/pyplanet/apps/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6032 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8795 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/config.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.084791 pyplanet-0.9.9/pyplanet/apps/contrib/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-15 15:01:44.000000 pyplanet-0.9.9/pyplanet/apps/contrib/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.084791 pyplanet-0.9.9/pyplanet/apps/contrib/admin/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1151 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       53 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/app.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2970 2020-09-10 12:09:46.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/flow.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    13757 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/map.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      722 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/mapbrowser.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    22849 2020-09-10 12:09:46.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/player.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      666 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/pyplanet.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9035 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/server.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.036792 pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.084791 pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/setting/
+-rw-r--r--   0 tom       (1000) tom       (1000)      840 2020-03-02 20:01:38.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/setting/edit.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     3571 2020-04-09 17:20:41.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/setting/edit.xml
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.084791 pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/toolbar/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1431 2020-04-06 19:33:25.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     2686 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1898 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/toolbar.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.084791 pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-23 17:12:13.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2231 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/mapbrowser.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4111 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/players.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6761 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/setting.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2263 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/toolbar.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/ads/
+-rw-r--r--   0 tom       (1000) tom       (1000)     8403 2020-07-08 14:53:42.000000 pyplanet-0.9.9/pyplanet/apps/contrib/ads/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/ads/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      315 2020-04-07 11:12:16.000000 pyplanet-0.9.9/pyplanet/apps/contrib/ads/templates/discord_logo.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)      349 2020-04-07 11:12:16.000000 pyplanet-0.9.9/pyplanet/apps/contrib/ads/templates/paypal_logo.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1230 2020-04-07 11:12:16.000000 pyplanet-0.9.9/pyplanet/apps/contrib/ads/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2445 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1326 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/templates/widget_top.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     2630 2020-05-23 19:36:09.000000 pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/clock/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1134 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/apps/contrib/clock/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/clock/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      490 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/clock/templates/clock.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      329 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/clock/templates/clock.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)      329 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/clock/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7273 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       72 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/app.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1095 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/templates/cpwidget.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     2949 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/
+-rw-r--r--   0 tom       (1000) tom       (1000)    22281 2021-02-21 15:03:15.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    11816 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/api.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       69 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/app.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      540 2017-05-23 17:12:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8158 2020-05-23 19:36:09.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.088791 pyplanet-0.9.9/pyplanet/apps/contrib/dynamic_points/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4436 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dynamic_points/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/dynatime/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2793 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/dynatime/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4481 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      886 2020-04-06 17:58:52.000000 pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     2236 2020-04-09 17:20:41.000000 pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1268 2020-05-13 09:00:23.000000 pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2003 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/info/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/info/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1505 2020-04-07 15:49:35.000000 pyplanet-0.9.9/pyplanet/apps/contrib/info/templates/mapinfo.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1674 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/info/templates/mapinfo.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1796 2020-03-02 20:01:38.000000 pyplanet-0.9.9/pyplanet/apps/contrib/info/templates/serverinfo.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     2784 2020-07-08 14:53:42.000000 pyplanet-0.9.9/pyplanet/apps/contrib/info/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/
+-rw-r--r--   0 tom       (1000) tom       (1000)     8382 2020-09-10 12:09:46.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       61 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/app.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8615 2020-05-09 12:23:13.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/folders.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)      385 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/migrations/000_remove_unique_folder_name.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/models/
+-rw-r--r--   0 tom       (1000) tom       (1000)      113 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/models/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      791 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/models/mapfolder.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.092791 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1964 2020-05-09 12:23:13.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/templates/folder_add.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1269 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/templates/folder_create.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     2557 2020-05-09 12:23:13.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/templates/folder_create.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)    20920 2021-02-05 09:55:19.000000 pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/karma/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9178 2020-09-10 12:09:46.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       53 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/app.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/karma/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)      400 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/migrations/000_add_expanded_score.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/karma/models/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       50 2017-04-19 19:57:23.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/models/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      586 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/models/karma.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5515 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/mxkarma.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6559 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/mxkarmaapi.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/karma/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1616 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/templates/karma.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     3262 2020-05-23 19:36:09.000000 pyplanet-0.9.9/pyplanet/apps/contrib/karma/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/
+-rw-r--r--   0 tom       (1000) tom       (1000)    10866 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1643 2020-04-09 13:05:21.000000 pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/templates/widget.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     5938 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/
+-rw-r--r--   0 tom       (1000) tom       (1000)    11802 2021-02-05 09:55:19.000000 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       81 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/app.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/migrations/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      320 2017-05-12 22:59:05.000000 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/migrations/000_make_player_map_unique.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/models/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       69 2017-04-19 19:35:22.000000 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/models/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      704 2017-05-12 22:59:05.000000 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/models/local_record.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10517 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/local_records/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.096791 pyplanet-0.9.9/pyplanet/apps/contrib/music_server/
+-rw-r--r--   0 tom       (1000) tom       (1000)     6695 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/music_server/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2401 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/music_server/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.100791 pyplanet-0.9.9/pyplanet/apps/contrib/mx/
+-rw-r--r--   0 tom       (1000) tom       (1000)    10491 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/mx/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8926 2021-02-21 14:34:55.000000 pyplanet-0.9.9/pyplanet/apps/contrib/mx/api.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       41 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/mx/app.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      157 2017-05-12 22:59:05.000000 pyplanet-0.9.9/pyplanet/apps/contrib/mx/exceptions.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.100791 pyplanet-0.9.9/pyplanet/apps/contrib/mx/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      743 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/mx/templates/search.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)    15000 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/mx/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.100791 pyplanet-0.9.9/pyplanet/apps/contrib/players/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3361 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/apps/contrib/players/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       61 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/players/app.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1098 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/contrib/players/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.100791 pyplanet-0.9.9/pyplanet/apps/contrib/queue/
+-rw-r--r--   0 tom       (1000) tom       (1000)     8665 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/queue/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       93 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/queue/exception.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3563 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/queue/list.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.100791 pyplanet-0.9.9/pyplanet/apps/contrib/queue/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1370 2020-04-06 19:33:25.000000 pyplanet-0.9.9/pyplanet/apps/contrib/queue/templates/queue.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1200 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/queue/templates/queue.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1184 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/queue/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.100791 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2611 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.104791 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5706 2020-07-01 14:23:26.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/cp_diff.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1638 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/cp_diff.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     6235 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/cp_diff_next.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1556 2020-04-07 13:11:02.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/gear_indicator.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      440 2020-04-07 13:11:02.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/gear_indicator.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     7003 2020-07-01 14:23:26.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/sector_times.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1961 2020-09-10 12:09:46.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/sector_times.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     7247 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/sector_times_next.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     4402 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.104791 pyplanet-0.9.9/pyplanet/apps/contrib/transactions/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7734 2020-05-18 12:23:53.000000 pyplanet-0.9.9/pyplanet/apps/contrib/transactions/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       81 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/apps/contrib/transactions/app.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.104791 pyplanet-0.9.9/pyplanet/apps/contrib/transactions/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1545 2020-04-07 16:46:26.000000 pyplanet-0.9.9/pyplanet/apps/contrib/transactions/templates/donation_toolbar.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1338 2020-05-18 12:47:06.000000 pyplanet-0.9.9/pyplanet/apps/contrib/transactions/view.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.104791 pyplanet-0.9.9/pyplanet/apps/contrib/voting/
+-rw-r--r--   0 tom       (1000) tom       (1000)    25811 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/voting/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.104791 pyplanet-0.9.9/pyplanet/apps/contrib/voting/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      884 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/voting/templates/voting.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1181 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/voting/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1760 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/contrib/voting/vote.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.104791 pyplanet-0.9.9/pyplanet/apps/core/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:52:55.000000 pyplanet-0.9.9/pyplanet/apps/core/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.104791 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:15:23.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      541 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/app.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       48 2017-04-23 09:43:28.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12372 2017-05-14 17:32:42.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/flow.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3582 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/map.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3949 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/other.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8029 2020-07-01 11:02:17.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/player.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1175 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/ui.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)      624 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/migrations/000_add_player_donations_time_stats.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      412 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/migrations/001_add_maps_mx_id_column.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/models/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       82 2017-03-26 15:38:36.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/models/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4156 2020-04-09 13:32:25.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/models/map.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5111 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/models/player.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-26 15:37:58.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9257 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/app.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1054 2020-04-09 17:20:41.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/dev.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/migrations/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-17 15:21:00.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/migrations/.gitkeep
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/models/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       99 2017-04-24 18:10:58.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/models/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      613 2017-05-12 22:59:05.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/models/perms.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2041 2017-05-12 22:59:05.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/models/setting.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1089 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/setting.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/call/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4394 2020-04-09 17:20:41.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/call/call.xml
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/command/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2318 2020-04-09 17:20:41.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/command/details.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     2221 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/controller.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1443 2020-05-13 08:54:05.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/controller.xml
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.108791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/setting/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      840 2017-04-27 17:56:40.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/setting/edit.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     4321 2020-04-09 17:20:41.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/setting/edit.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     3121 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/toolbar.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     3421 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/toolbar.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1467 2020-04-06 19:33:25.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/toolbar.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.112791 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-26 15:28:10.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7113 2020-04-09 17:20:41.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/call.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3538 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/command.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      850 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/controller.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6262 2020-04-07 12:06:21.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/setting.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1043 2020-09-10 12:09:46.000000 pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/toolbar.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.112791 pyplanet-0.9.9/pyplanet/apps/core/shootmania/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:15:23.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      222 2017-05-18 16:38:48.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/app.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.112791 pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       47 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17223 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/base.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1692 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/elite.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2245 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/joust.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1844 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/royal.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-14 16:44:01.000000 pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/siege.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.112791 pyplanet-0.9.9/pyplanet/apps/core/statistics/
+-rw-r--r--   0 tom       (1000) tom       (1000)      872 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       79 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/app.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      615 2017-05-03 16:25:53.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1166 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/mp.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4941 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/processor.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.112791 pyplanet-0.9.9/pyplanet/apps/core/statistics/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2591 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/templates/dashboard.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     2319 2020-10-16 14:05:49.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/tm.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.116791 pyplanet-0.9.9/pyplanet/apps/core/statistics/views/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/views/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      290 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/views/base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1901 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/views/dashboard.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3019 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/views/players.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2243 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/views/records.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9410 2020-04-20 13:07:29.000000 pyplanet-0.9.9/pyplanet/apps/core/statistics/views/score.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.116791 pyplanet-0.9.9/pyplanet/apps/core/trackmania/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-14 16:15:23.000000 pyplanet-0.9.9/pyplanet/apps/core/trackmania/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      746 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/core/trackmania/app.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14142 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/apps/core/trackmania/callbacks.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.116791 pyplanet-0.9.9/pyplanet/bin/
+-rwxrwxr-x   0 tom       (1000) tom       (1000)      128 2017-04-22 17:09:27.000000 pyplanet-0.9.9/pyplanet/bin/pyplanet
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.116791 pyplanet-0.9.9/pyplanet/conf/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2680 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.116791 pyplanet-0.9.9/pyplanet/conf/app_template/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      387 2020-04-05 20:40:52.000000 pyplanet-0.9.9/pyplanet/conf/app_template/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       32 2017-04-22 18:15:29.000000 pyplanet-0.9.9/pyplanet/conf/app_template/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.120791 pyplanet-0.9.9/pyplanet/conf/backends/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/backends/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2210 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/backends/base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1649 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/backends/file.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      962 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/backends/json.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1598 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/backends/python.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      937 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/backends/yaml.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5731 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/default_settings.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.120791 pyplanet-0.9.9/pyplanet/conf/project_template/
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1258 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/project_template/manage.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       79 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/project_template/requirements.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.120791 pyplanet-0.9.9/pyplanet/conf/project_template/settings/
+-rw-r--r--   0 tom       (1000) tom       (1000)      447 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/project_template/settings/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1959 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/project_template/settings/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2980 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/conf/project_template/settings/base.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.120791 pyplanet-0.9.9/pyplanet/contrib/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      339 2017-04-26 14:11:32.000000 pyplanet-0.9.9/pyplanet/contrib/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.120791 pyplanet-0.9.9/pyplanet/contrib/chat/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      213 2017-05-14 16:44:01.000000 pyplanet-0.9.9/pyplanet/contrib/chat/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       40 2017-05-14 16:44:01.000000 pyplanet-0.9.9/pyplanet/contrib/chat/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1720 2017-05-14 16:44:01.000000 pyplanet-0.9.9/pyplanet/contrib/chat/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4764 2017-06-18 09:32:36.000000 pyplanet-0.9.9/pyplanet/contrib/chat/query.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.124791 pyplanet-0.9.9/pyplanet/contrib/command/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      256 2017-04-23 20:32:27.000000 pyplanet-0.9.9/pyplanet/contrib/command/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7587 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/command/command.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      363 2017-03-25 20:46:30.000000 pyplanet-0.9.9/pyplanet/contrib/command/exceptions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3943 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/command/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4034 2017-05-11 08:58:44.000000 pyplanet-0.9.9/pyplanet/contrib/command/params.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.124791 pyplanet-0.9.9/pyplanet/contrib/converter/
+-rw-r--r--   0 tom       (1000) tom       (1000)      677 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/converter/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1716 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/converter/base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5443 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/converter/expansion.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5741 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/converter/maniacontrol.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7162 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/converter/uaseco.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6164 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/contrib/converter/xaseco2.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.124791 pyplanet-0.9.9/pyplanet/contrib/map/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      146 2017-04-23 20:35:30.000000 pyplanet-0.9.9/pyplanet/contrib/map/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/map/exceptions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17241 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/contrib/map/manager.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.124791 pyplanet-0.9.9/pyplanet/contrib/mode/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      212 2017-05-02 19:10:15.000000 pyplanet-0.9.9/pyplanet/contrib/mode/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-01 18:42:05.000000 pyplanet-0.9.9/pyplanet/contrib/mode/exceptions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6054 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/contrib/mode/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      600 2017-05-02 19:10:15.000000 pyplanet-0.9.9/pyplanet/contrib/mode/signals.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.124791 pyplanet-0.9.9/pyplanet/contrib/permission/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      169 2017-03-26 15:03:53.000000 pyplanet-0.9.9/pyplanet/contrib/permission/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-26 15:03:59.000000 pyplanet-0.9.9/pyplanet/contrib/permission/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2768 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/contrib/permission/manager.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.124791 pyplanet-0.9.9/pyplanet/contrib/player/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      157 2017-03-23 16:31:59.000000 pyplanet-0.9.9/pyplanet/contrib/player/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       94 2017-04-23 20:33:28.000000 pyplanet-0.9.9/pyplanet/contrib/player/exceptions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    13902 2020-09-10 12:09:46.000000 pyplanet-0.9.9/pyplanet/contrib/player/manager.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.128791 pyplanet-0.9.9/pyplanet/contrib/setting/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      212 2017-05-01 18:42:05.000000 pyplanet-0.9.9/pyplanet/contrib/setting/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      284 2017-05-12 23:28:22.000000 pyplanet-0.9.9/pyplanet/contrib/setting/core_settings.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      286 2017-04-27 20:23:24.000000 pyplanet-0.9.9/pyplanet/contrib/setting/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8244 2020-04-07 11:35:40.000000 pyplanet-0.9.9/pyplanet/contrib/setting/manager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7335 2020-04-07 13:11:02.000000 pyplanet-0.9.9/pyplanet/contrib/setting/setting.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.128791 pyplanet-0.9.9/pyplanet/core/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      173 2017-05-14 16:44:01.000000 pyplanet-0.9.9/pyplanet/core/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.128791 pyplanet-0.9.9/pyplanet/core/checks/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      347 2020-04-07 09:09:12.000000 pyplanet-0.9.9/pyplanet/core/checks/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1937 2017-05-01 13:35:06.000000 pyplanet-0.9.9/pyplanet/core/checks/messages.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1582 2020-04-07 09:39:40.000000 pyplanet-0.9.9/pyplanet/core/checks/registry.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      823 2020-03-02 20:01:38.000000 pyplanet-0.9.9/pyplanet/core/controller.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.128791 pyplanet-0.9.9/pyplanet/core/db/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      226 2017-04-09 19:02:44.000000 pyplanet-0.9.9/pyplanet/core/db/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3169 2017-06-18 09:32:36.000000 pyplanet-0.9.9/pyplanet/core/db/database.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4274 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/db/migrator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3948 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/core/db/model.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.128791 pyplanet-0.9.9/pyplanet/core/db/models/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-17 13:40:22.000000 pyplanet-0.9.9/pyplanet/core/db/models/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      166 2017-03-17 13:41:04.000000 pyplanet-0.9.9/pyplanet/core/db/models/migration.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2036 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/core/db/registry.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.128791 pyplanet-0.9.9/pyplanet/core/events/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      242 2017-04-26 14:11:32.000000 pyplanet-0.9.9/pyplanet/core/events/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2070 2017-05-23 17:12:13.000000 pyplanet-0.9.9/pyplanet/core/events/callback.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10041 2017-05-23 17:12:13.000000 pyplanet-0.9.9/pyplanet/core/events/dispatcher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6932 2018-03-11 13:38:21.000000 pyplanet-0.9.9/pyplanet/core/events/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      593 2017-03-25 19:00:05.000000 pyplanet-0.9.9/pyplanet/core/exceptions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/core/game.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.132791 pyplanet-0.9.9/pyplanet/core/gbx/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       83 2017-05-14 16:44:01.000000 pyplanet-0.9.9/pyplanet/core/gbx/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9013 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/core/gbx/client.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3225 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/core/gbx/query.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10697 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/gbx/remote.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7545 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/core/instance.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.132791 pyplanet-0.9.9/pyplanet/core/management/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9058 2020-04-07 09:39:40.000000 pyplanet-0.9.9/pyplanet/core/management/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    15492 2020-04-07 09:16:40.000000 pyplanet-0.9.9/pyplanet/core/management/base.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2017-04-22 15:18:33.000000 pyplanet-0.9.9/pyplanet/core/management/color.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.132791 pyplanet-0.9.9/pyplanet/core/management/commands/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-22 14:56:11.000000 pyplanet-0.9.9/pyplanet/core/management/commands/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2189 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/management/commands/db_convert.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      906 2017-05-13 20:24:08.000000 pyplanet-0.9.9/pyplanet/core/management/commands/init_app.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      863 2017-06-18 09:32:36.000000 pyplanet-0.9.9/pyplanet/core/management/commands/init_project.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3723 2020-04-07 09:13:25.000000 pyplanet-0.9.9/pyplanet/core/management/commands/start.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1785 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/management/commands/upgrade.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1599 2017-04-26 14:38:04.000000 pyplanet-0.9.9/pyplanet/core/management/management.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5555 2017-06-18 09:32:36.000000 pyplanet-0.9.9/pyplanet/core/management/templates.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1344 2017-05-12 23:28:22.000000 pyplanet-0.9.9/pyplanet/core/signals.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.132791 pyplanet-0.9.9/pyplanet/core/storage/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      107 2017-04-15 11:03:27.000000 pyplanet-0.9.9/pyplanet/core/storage/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.132791 pyplanet-0.9.9/pyplanet/core/storage/drivers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-09 19:46:06.000000 pyplanet-0.9.9/pyplanet/core/storage/drivers/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.132791 pyplanet-0.9.9/pyplanet/core/storage/drivers/asyncssh/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5676 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/storage/drivers/asyncssh/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.132791 pyplanet-0.9.9/pyplanet/core/storage/drivers/local/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2653 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/storage/drivers/local/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       67 2017-04-29 13:42:23.000000 pyplanet-0.9.9/pyplanet/core/storage/exceptions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2400 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/storage/interface.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3977 2020-01-26 17:49:37.000000 pyplanet-0.9.9/pyplanet/core/storage/storage.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.136791 pyplanet-0.9.9/pyplanet/core/ui/
+-rw-r--r--   0 tom       (1000) tom       (1000)     8387 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/core/ui/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.136791 pyplanet-0.9.9/pyplanet/core/ui/components/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      114 2017-04-28 20:32:19.000000 pyplanet-0.9.9/pyplanet/core/ui/components/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8082 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/core/ui/components/manialink.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      421 2017-05-16 15:35:51.000000 pyplanet-0.9.9/pyplanet/core/ui/exceptions.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.136791 pyplanet-0.9.9/pyplanet/core/ui/filters/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-15 11:40:44.000000 pyplanet-0.9.9/pyplanet/core/ui/filters/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      913 2017-04-28 20:26:16.000000 pyplanet-0.9.9/pyplanet/core/ui/loader.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1410 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/core/ui/template.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7714 2021-02-21 14:06:12.000000 pyplanet-0.9.9/pyplanet/core/ui/ui_properties.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.136791 pyplanet-0.9.9/pyplanet/god/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-13 20:00:09.000000 pyplanet-0.9.9/pyplanet/god/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3283 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/god/pool.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3272 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/god/process.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.140791 pyplanet-0.9.9/pyplanet/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-12 18:25:07.000000 pyplanet-0.9.9/pyplanet/utils/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2167 2020-07-06 18:00:34.000000 pyplanet-0.9.9/pyplanet/utils/analytics.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      675 2017-04-19 16:19:15.000000 pyplanet-0.9.9/pyplanet/utils/codeutils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      131 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/utils/functional.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8159 2020-07-06 18:00:34.000000 pyplanet-0.9.9/pyplanet/utils/gbxparser.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      374 2017-03-25 16:53:08.000000 pyplanet-0.9.9/pyplanet/utils/livereload.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4035 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/utils/log.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      865 2017-04-27 18:55:11.000000 pyplanet-0.9.9/pyplanet/utils/memleak.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4244 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/utils/pip.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.140791 pyplanet-0.9.9/pyplanet/utils/pip_test_pkg/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1600 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/utils/pip_test_pkg/setup.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2489 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/utils/releases.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9238 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/utils/semver.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3565 2017-05-11 08:35:33.000000 pyplanet-0.9.9/pyplanet/utils/style.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6369 2017-04-22 14:39:05.000000 pyplanet-0.9.9/pyplanet/utils/termcolors.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1090 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/utils/times.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      599 2017-04-26 14:42:19.000000 pyplanet-0.9.9/pyplanet/utils/toposort.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      472 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/utils/zone.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.140791 pyplanet-0.9.9/pyplanet/views/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       98 2017-04-22 19:25:36.000000 pyplanet-0.9.9/pyplanet/views/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      184 2017-04-22 19:48:52.000000 pyplanet-0.9.9/pyplanet/views/base.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.140791 pyplanet-0.9.9/pyplanet/views/generics/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      199 2017-06-18 09:32:36.000000 pyplanet-0.9.9/pyplanet/views/generics/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8893 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/views/generics/alert.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14069 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/views/generics/list.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3000 2020-04-07 16:46:26.000000 pyplanet-0.9.9/pyplanet/views/generics/widget.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5805 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/views/template.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.044792 pyplanet-0.9.9/pyplanet/views/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.140791 pyplanet-0.9.9/pyplanet/views/templates/generics/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1701 2020-01-17 13:07:25.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/alert.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)      379 2020-01-17 13:07:25.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/list.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     7988 2020-10-16 14:18:04.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/list.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1928 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/prompt.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)      961 2020-01-17 13:07:25.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/timeswidget.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     4536 2020-05-13 08:57:07.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/widget.Script.Txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1389 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/widget.xml
+-rw-r--r--   0 tom       (1000) tom       (1000)     2421 2020-07-01 14:23:35.000000 pyplanet-0.9.9/pyplanet/views/templates/generics/widget_next.Script.Txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.140791 pyplanet-0.9.9/pyplanet/views/templates/libs/
+-rw-r--r--   0 tom       (1000) tom       (1000)      736 2020-03-02 20:01:38.000000 pyplanet-0.9.9/pyplanet/views/templates/libs/TimeUtils.Script.Txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.080791 pyplanet-0.9.9/pyplanet.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3912 2021-02-21 15:04:20.000000 pyplanet-0.9.9/pyplanet.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)    18867 2021-02-21 15:04:22.000000 pyplanet-0.9.9/pyplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-02-21 15:04:20.000000 pyplanet-0.9.9/pyplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       81 2021-02-21 15:04:20.000000 pyplanet-0.9.9/pyplanet.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-02-21 15:04:20.000000 pyplanet-0.9.9/pyplanet.egg-info/not-zip-safe
+-rw-r--r--   0 tom       (1000) tom       (1000)      379 2021-02-21 15:04:20.000000 pyplanet-0.9.9/pyplanet.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        9 2021-02-21 15:04:20.000000 pyplanet-0.9.9/pyplanet.egg-info/top_level.txt
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1037 2020-04-06 13:57:12.000000 pyplanet-0.9.9/pyplanet.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      246 2020-04-06 13:57:12.000000 pyplanet-0.9.9/requirements-dev.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      434 2020-04-06 13:57:12.000000 pyplanet-0.9.9/requirements.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       80 2021-02-21 15:04:23.164791 pyplanet-0.9.9/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     2404 2020-04-06 13:57:12.000000 pyplanet-0.9.9/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.140791 pyplanet-0.9.9/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      293 2017-04-19 15:38:58.000000 pyplanet-0.9.9/tests/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.044792 pyplanet-0.9.9/tests/_files/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.152791 pyplanet-0.9.9/tests/_files/maps/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-30 15:23:26.000000 pyplanet-0.9.9/tests/_files/maps/.gitkeep
+-rw-rw-r--   0 tom       (1000) tom       (1000)   263043 2017-03-30 16:47:30.000000 pyplanet-0.9.9/tests/_files/maps/canyon-mp4-1.gbx
+-rw-rw-r--   0 tom       (1000) tom       (1000)   455963 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/_files/maps/canyon-mp4-2.gbx
+-rw-rw-r--   0 tom       (1000) tom       (1000)   468177 2017-04-09 15:15:12.000000 pyplanet-0.9.9/tests/_files/maps/greyroad.gbx
+-rw-rw-r--   0 tom       (1000) tom       (1000)   604744 2017-03-30 16:47:52.000000 pyplanet-0.9.9/tests/_files/maps/royal-mp4-1.gbx
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.156791 pyplanet-0.9.9/tests/_scripts/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.044792 pyplanet-0.9.9/tests/_scripts/appveyor/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.156791 pyplanet-0.9.9/tests/_scripts/appveyor/dedicated/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3898 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/dedicated/dedicated_cfg.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1532 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/dedicated/matchsettings_1.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.156791 pyplanet-0.9.9/tests/_scripts/appveyor/settings/
+-rw-r--r--   0 tom       (1000) tom       (1000)      271 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/settings/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      573 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/settings/apps.json
+-rw-r--r--   0 tom       (1000) tom       (1000)     1301 2020-05-13 09:46:44.000000 pyplanet-0.9.9/tests/_scripts/appveyor/settings/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      493 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/settings/apps.yaml
+-rw-r--r--   0 tom       (1000) tom       (1000)      736 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/settings/base.json
+-rw-r--r--   0 tom       (1000) tom       (1000)     2254 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/settings/base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      530 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor/settings/base.yaml
+-rw-r--r--   0 tom       (1000) tom       (1000)       93 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor_config.ps1
+-rw-r--r--   0 tom       (1000) tom       (1000)     4103 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor_init.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1598 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/appveyor_with_compiler.cmd
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.044792 pyplanet-0.9.9/tests/_scripts/travis/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.156791 pyplanet-0.9.9/tests/_scripts/travis/dedicated/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3898 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis/dedicated/dedicated_cfg.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1532 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/_scripts/travis/dedicated/matchsettings_1.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.156791 pyplanet-0.9.9/tests/_scripts/travis/settings/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      271 2017-03-14 14:13:30.000000 pyplanet-0.9.9/tests/_scripts/travis/settings/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      573 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis/settings/apps.json
+-rw-r--r--   0 tom       (1000) tom       (1000)     1301 2020-05-13 09:46:44.000000 pyplanet-0.9.9/tests/_scripts/travis/settings/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      493 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis/settings/apps.yaml
+-rw-r--r--   0 tom       (1000) tom       (1000)      725 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis/settings/base.json
+-rw-r--r--   0 tom       (1000) tom       (1000)     2243 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis/settings/base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      519 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis/settings/base.yaml
+-rwxrwxr-x   0 tom       (1000) tom       (1000)      227 2017-04-22 23:23:40.000000 pyplanet-0.9.9/tests/_scripts/travis_config.sh
+-rwxr-xr-x   0 tom       (1000) tom       (1000)      340 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis_coverage.sh
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1251 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis_dedicated_setup.sh
+-rwxr-xr-x   0 tom       (1000) tom       (1000)      837 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/_scripts/travis_dedicated_start.sh
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.156791 pyplanet-0.9.9/tests/apps/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-19 15:28:37.000000 pyplanet-0.9.9/tests/apps/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.160791 pyplanet-0.9.9/tests/apps/migration_test/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2017-05-13 20:24:08.000000 pyplanet-0.9.9/tests/apps/migration_test/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       85 2017-05-13 20:24:08.000000 pyplanet-0.9.9/tests/apps/migration_test/app.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.160791 pyplanet-0.9.9/tests/apps/migration_test/migrations/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      327 2017-04-19 17:22:41.000000 pyplanet-0.9.9/tests/apps/migration_test/migrations/000_sample_field.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      272 2017-04-19 15:14:46.000000 pyplanet-0.9.9/tests/apps/migration_test/migrations/001_remove_player_field.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      284 2017-04-19 15:14:35.000000 pyplanet-0.9.9/tests/apps/migration_test/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.160791 pyplanet-0.9.9/tests/apps/new_import_style/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       84 2017-05-13 20:24:08.000000 pyplanet-0.9.9/tests/apps/new_import_style/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.160791 pyplanet-0.9.9/tests/integration/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      446 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/integration/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.160791 pyplanet-0.9.9/tests/integration/contrib/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/integration/contrib/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1265 2017-05-23 17:12:08.000000 pyplanet-0.9.9/tests/integration/contrib/test_map.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      830 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/integration/contrib/test_player.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3208 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/integration/test_gbx.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      619 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/integration/test_instance.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.160791 pyplanet-0.9.9/tests/unit/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-26 14:25:28.000000 pyplanet-0.9.9/tests/unit/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.164791 pyplanet-0.9.9/tests/unit/contrib/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/unit/contrib/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2646 2017-05-14 16:44:01.000000 pyplanet-0.9.9/tests/unit/contrib/test_chat.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2182 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/unit/contrib/test_commands.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2277 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/unit/contrib/test_permissions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2228 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/unit/contrib/test_settings.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.164791 pyplanet-0.9.9/tests/unit/storage/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-30 12:34:12.000000 pyplanet-0.9.9/tests/unit/storage/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1493 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/unit/storage/test_local_driver.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      511 2017-04-30 12:34:12.000000 pyplanet-0.9.9/tests/unit/storage/test_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2017-09-15 11:31:54.000000 pyplanet-0.9.9/tests/unit/test_callbacks.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1083 2020-04-06 13:57:12.000000 pyplanet-0.9.9/tests/unit/test_conf.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1816 2017-05-11 08:35:33.000000 pyplanet-0.9.9/tests/unit/test_database.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-04-26 18:33:10.000000 pyplanet-0.9.9/tests/unit/test_db_migrator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3105 2017-09-15 11:31:54.000000 pyplanet-0.9.9/tests/unit/test_signals.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      823 2020-01-17 15:14:28.000000 pyplanet-0.9.9/tests/unit/test_ui_template.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1147 2017-04-30 12:34:12.000000 pyplanet-0.9.9/tests/unit/test_views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-02-21 15:04:23.164791 pyplanet-0.9.9/tests/unit/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2017-03-30 14:48:30.000000 pyplanet-0.9.9/tests/unit/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2508 2017-04-26 17:33:09.000000 pyplanet-0.9.9/tests/unit/utils/test_gbxparser.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2017-05-30 14:28:01.000000 pyplanet-0.9.9/tests/unit/utils/test_style.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      447 2017-03-30 15:21:11.000000 pyplanet-0.9.9/tests/unit/utils/test_times.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      602 2017-04-30 12:34:12.000000 pyplanet-0.9.9/tests/unit/utils/test_toposort.py
```

### Comparing `pyplanet-0.9.8/CHANGELOG.rst` & `pyplanet-0.9.9/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Changelog
 =========
 
-0.9.6 + 0.9.7 + 0.9.8 (21 February 2021)
-----------------------------------------
+0.9.6 + 0.9.7 + 0.9.8 + 0.9.9 (21 February 2021)
+------------------------------------------------
 
 Core
 ~~~~
 
 * Improvement: Add support for UI properties in TM2020.
 * Improvement: Add support for Echo callback.
 * Improvement: Add support for several new TM2020 callbacks.
@@ -28,14 +28,15 @@
 
 * Bugfix: Fix for TeamMode where the quad is fully colored.
 * Bugfix: Fix for fun commands usage in wrong games and when muted.
 * Bugfix: Fix retrieval of current players/spectators in Dedimania API update loop
 * Bugfix: Fixing issues with retrieving dedimania records when switching modes.
 * Bugfix: Resolve typos in several locations.
 * Bugfix: Resolve issues with MX on MP.
+* Bugfix: Resolve issues with dedimania on MP.
 
 
 0.9.5 (28 October 2020)
 -----------------------
 
 Core
 ~~~~
```

### Comparing `pyplanet-0.9.8/LICENSE` & `pyplanet-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/PKG-INFO` & `pyplanet-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyplanet
-Version: 0.9.8
+Version: 0.9.9
 Summary: Maniaplanet Server Controller
 Home-page: http://pypla.net/
 Author: Tom Valk
 Author-email: tomvalk@lt-box.info
 License: GNU General Public License v3 (GPLv3)
 Description: PyPlanet
         ========
```

### Comparing `pyplanet-0.9.8/README.rst` & `pyplanet-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/Makefile` & `pyplanet-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/make.bat` & `pyplanet-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/pyplanet.spec` & `pyplanet-0.9.9/docs/pyplanet.spec`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/scripts/setup.sh` & `pyplanet-0.9.9/docs/scripts/setup.sh`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/apps/architecture.png` & `pyplanet-0.9.9/docs/source/_static/apps/architecture.png`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/apps/lifecycle.png` & `pyplanet-0.9.9/docs/source/_static/apps/lifecycle.png`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/architecture-overview.png` & `pyplanet-0.9.9/docs/source/_static/architecture-overview.png`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/intro/python-windows-1.png` & `pyplanet-0.9.9/docs/source/_static/intro/python-windows-1.png`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/logo/pyplanet-sm.png` & `pyplanet-0.9.9/docs/source/_static/logo/pyplanet-sm.png`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/logo/pyplanet-xs.png` & `pyplanet-0.9.9/docs/source/_static/logo/pyplanet-xs.png`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/screenshots/tm_1.jpg` & `pyplanet-0.9.9/docs/source/_static/screenshots/tm_1.jpg`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/_static/screenshots/tm_2.jpg` & `pyplanet-0.9.9/docs/source/_static/screenshots/tm_2.jpg`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/api/contrib_chat.rst` & `pyplanet-0.9.9/docs/source/api/contrib_chat.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/chat.rst` & `pyplanet-0.9.9/docs/source/apps/chat.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/context.rst` & `pyplanet-0.9.9/docs/source/apps/context.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/admin.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/admin.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/ads.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/ads.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/best_cps.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/best_cps.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/clock.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/clock.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/currentcps.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/currentcps.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/dedimania.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/dedimania.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/dynamic_points.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/dynamic_points.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/funcmd.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/funcmd.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/jukebox.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/jukebox.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/karma.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/karma.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/live_rankings.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/live_rankings.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/local_records.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/local_records.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/mapinfo.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/mapinfo.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/music_server.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/music_server.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/mx.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/mx.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/players.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/players.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/queue.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/queue.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/sector_times.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/sector_times.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/transactions.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/transactions.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/contrib/voting.rst` & `pyplanet-0.9.9/docs/source/apps/contrib/voting.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/core/statistics.rst` & `pyplanet-0.9.9/docs/source/apps/core/statistics.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/create.rst` & `pyplanet-0.9.9/docs/source/apps/create.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/gbx.rst` & `pyplanet-0.9.9/docs/source/apps/gbx.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/index.rst` & `pyplanet-0.9.9/docs/source/apps/index.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/lifecycle.rst` & `pyplanet-0.9.9/docs/source/apps/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/migrations.rst` & `pyplanet-0.9.9/docs/source/apps/migrations.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/models.rst` & `pyplanet-0.9.9/docs/source/apps/models.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/apps/ui.rst` & `pyplanet-0.9.9/docs/source/apps/ui.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/conf.py` & `pyplanet-0.9.9/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 author = 'Tom Valk'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.9.8'
+version = '0.9.9'
 # The full version, including alpha/beta/rc tags.
-release = '0.9.8'
+release = '0.9.9'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `pyplanet-0.9.8/docs/source/convert/index.rst` & `pyplanet-0.9.9/docs/source/convert/index.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/howto/dbcollate.rst` & `pyplanet-0.9.9/docs/source/howto/dbcollate.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/howto/dbindex.rst` & `pyplanet-0.9.9/docs/source/howto/dbindex.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/index.rst` & `pyplanet-0.9.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/intro/configuration.rst` & `pyplanet-0.9.9/docs/source/intro/configuration.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/intro/installation-linux.rst` & `pyplanet-0.9.9/docs/source/intro/installation-linux.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/intro/installation-simple.rst` & `pyplanet-0.9.9/docs/source/intro/installation-simple.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/intro/installation-windows.rst` & `pyplanet-0.9.9/docs/source/intro/installation-windows.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/intro/requirements.rst` & `pyplanet-0.9.9/docs/source/intro/requirements.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/intro/starting.rst` & `pyplanet-0.9.9/docs/source/intro/starting.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/intro/upgrading.rst` & `pyplanet-0.9.9/docs/source/intro/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/notebooks/set-rounds-points.ipynb` & `pyplanet-0.9.9/docs/source/notebooks/set-rounds-points.ipynb`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/privacy.rst` & `pyplanet-0.9.9/docs/source/privacy.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/docs/source/support.rst` & `pyplanet-0.9.9/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/apps.py` & `pyplanet-0.9.9/pyplanet/apps/apps.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/config.py` & `pyplanet-0.9.9/pyplanet/apps/config.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/flow.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/flow.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/map.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/map.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/mapbrowser.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/mapbrowser.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/player.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/player.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/pyplanet.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/pyplanet.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/server.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/server.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/setting/edit.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/setting/edit.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/setting/edit.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/setting/edit.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/templates/toolbar/toolbar.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/toolbar.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/mapbrowser.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/mapbrowser.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/players.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/players.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/setting.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/setting.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/admin/views/toolbar.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/admin/views/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/ads/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/ads/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/ads/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/ads/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/templates/widget_top.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/templates/widget_top.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/best_cps/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/best_cps/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/clock/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/clock/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/templates/cpwidget.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/templates/cpwidget.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/currentcps/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/currentcps/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 		# Load initial data.
 		if not self.widget:
 			self.widget = DedimaniaRecordsWidget(self)
 
 		# Load settings + initiate api.
 		if self.instance.game.game == "tm":
 			await self.reload_settings()
-			return
 
 		# Register signals
 		self.context.signals.listen(mp_signals.map.map_begin, self.map_begin)
 		self.context.signals.listen(mp_signals.map.map_start, self.map_start)
 		self.context.signals.listen(mp_signals.map.map_end, self.map_end)
 
 		self.context.signals.listen(mp_signals.flow.podium_start, self.podium_start)
```

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/api.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/api.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/exceptions.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/dedimania/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/dedimania/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/dynamic_points/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/dynamic_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/dynatime/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/dynatime/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/templates/emoji_toolbar.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/funcmd/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/funcmd/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/info/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/info/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/info/templates/mapinfo.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/info/templates/mapinfo.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/info/templates/mapinfo.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/info/templates/mapinfo.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/info/templates/serverinfo.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/info/templates/serverinfo.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/info/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/info/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/folders.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/folders.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/models/mapfolder.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/models/mapfolder.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/templates/folder_add.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/templates/folder_add.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/templates/folder_create.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/templates/folder_create.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/templates/folder_create.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/templates/folder_create.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/jukebox/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/jukebox/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/karma/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/karma/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/karma/models/karma.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/karma/models/karma.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/karma/mxkarma.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/karma/mxkarma.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/karma/mxkarmaapi.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/karma/mxkarmaapi.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/karma/templates/karma.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/karma/templates/karma.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/karma/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/karma/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/templates/widget.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/templates/widget.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/live_rankings/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/live_rankings/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/local_records/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/local_records/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/local_records/models/local_record.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/local_records/models/local_record.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/local_records/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/local_records/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/music_server/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/music_server/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/music_server/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/music_server/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/mx/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/mx/api.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/mx/api.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/mx/templates/search.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/mx/templates/search.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/mx/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/mx/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/players/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/players/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/players/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/players/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/queue/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/queue/list.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/queue/list.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/queue/templates/queue.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/queue/templates/queue.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/queue/templates/queue.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/queue/templates/queue.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/queue/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/queue/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/cp_diff.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/cp_diff.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/cp_diff.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/cp_diff.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/cp_diff_next.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/cp_diff_next.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/gear_indicator.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/gear_indicator.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/sector_times.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/sector_times.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/sector_times.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/sector_times.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/templates/sector_times_next.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/templates/sector_times_next.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/sector_times/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/sector_times/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/transactions/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/transactions/templates/donation_toolbar.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/transactions/templates/donation_toolbar.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/transactions/view.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/transactions/view.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/voting/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/voting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/voting/templates/voting.xml` & `pyplanet-0.9.9/pyplanet/apps/contrib/voting/templates/voting.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/voting/views.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/voting/views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/contrib/voting/vote.py` & `pyplanet-0.9.9/pyplanet/apps/contrib/voting/vote.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/app.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/app.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/flow.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/flow.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/map.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/map.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/other.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/other.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/player.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/player.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/callbacks/ui.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/callbacks/ui.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/migrations/000_add_player_donations_time_stats.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/migrations/000_add_player_donations_time_stats.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/models/map.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/models/map.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/maniaplanet/models/player.py` & `pyplanet-0.9.9/pyplanet/apps/core/maniaplanet/models/player.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/app.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/app.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/dev.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/dev.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/models/perms.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/models/perms.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/models/setting.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/models/setting.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/setting.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/setting.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/call/call.xml` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/call/call.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/command/details.xml` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/command/details.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/controller.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/controller.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/controller.xml` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/controller.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/setting/edit.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/setting/edit.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/setting/edit.xml` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/setting/edit.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/toolbar.Script.Txt` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/toolbar.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/templates/toolbar.xml` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/templates/toolbar.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/toolbar.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/call.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/call.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/command.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/command.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/controller.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/controller.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/setting.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/setting.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/pyplanet/views/toolbar.py` & `pyplanet-0.9.9/pyplanet/apps/core/pyplanet/views/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/base.py` & `pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/elite.py` & `pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/elite.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/joust.py` & `pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/joust.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/shootmania/callbacks/royal.py` & `pyplanet-0.9.9/pyplanet/apps/core/shootmania/callbacks/royal.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/__init__.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/models.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/models.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/mp.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/mp.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/processor.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/processor.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/templates/dashboard.xml` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/templates/dashboard.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/tm.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/tm.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/views/dashboard.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/views/players.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/views/players.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/views/records.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/views/records.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/statistics/views/score.py` & `pyplanet-0.9.9/pyplanet/apps/core/statistics/views/score.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/trackmania/app.py` & `pyplanet-0.9.9/pyplanet/apps/core/trackmania/app.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/apps/core/trackmania/callbacks.py` & `pyplanet-0.9.9/pyplanet/apps/core/trackmania/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/__init__.py` & `pyplanet-0.9.9/pyplanet/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/backends/base.py` & `pyplanet-0.9.9/pyplanet/conf/backends/base.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/backends/file.py` & `pyplanet-0.9.9/pyplanet/conf/backends/file.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/backends/json.py` & `pyplanet-0.9.9/pyplanet/conf/backends/json.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/backends/python.py` & `pyplanet-0.9.9/pyplanet/conf/backends/python.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/backends/yaml.py` & `pyplanet-0.9.9/pyplanet/conf/backends/yaml.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/default_settings.py` & `pyplanet-0.9.9/pyplanet/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/project_template/manage.py` & `pyplanet-0.9.9/pyplanet/conf/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/project_template/settings/apps.py` & `pyplanet-0.9.9/pyplanet/conf/project_template/settings/apps.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/conf/project_template/settings/base.py` & `pyplanet-0.9.9/pyplanet/conf/project_template/settings/base.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/chat/manager.py` & `pyplanet-0.9.9/pyplanet/contrib/chat/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/chat/query.py` & `pyplanet-0.9.9/pyplanet/contrib/chat/query.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/command/command.py` & `pyplanet-0.9.9/pyplanet/contrib/command/command.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/command/manager.py` & `pyplanet-0.9.9/pyplanet/contrib/command/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/command/params.py` & `pyplanet-0.9.9/pyplanet/contrib/command/params.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/converter/__init__.py` & `pyplanet-0.9.9/pyplanet/contrib/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/converter/base.py` & `pyplanet-0.9.9/pyplanet/contrib/converter/base.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/converter/expansion.py` & `pyplanet-0.9.9/pyplanet/contrib/converter/expansion.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/converter/maniacontrol.py` & `pyplanet-0.9.9/pyplanet/contrib/converter/maniacontrol.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/converter/uaseco.py` & `pyplanet-0.9.9/pyplanet/contrib/converter/uaseco.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/converter/xaseco2.py` & `pyplanet-0.9.9/pyplanet/contrib/converter/xaseco2.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/map/manager.py` & `pyplanet-0.9.9/pyplanet/contrib/map/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/mode/manager.py` & `pyplanet-0.9.9/pyplanet/contrib/mode/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/mode/signals.py` & `pyplanet-0.9.9/pyplanet/contrib/mode/signals.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/permission/manager.py` & `pyplanet-0.9.9/pyplanet/contrib/permission/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/player/manager.py` & `pyplanet-0.9.9/pyplanet/contrib/player/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/setting/manager.py` & `pyplanet-0.9.9/pyplanet/contrib/setting/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/contrib/setting/setting.py` & `pyplanet-0.9.9/pyplanet/contrib/setting/setting.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/checks/messages.py` & `pyplanet-0.9.9/pyplanet/core/checks/messages.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/checks/registry.py` & `pyplanet-0.9.9/pyplanet/core/checks/registry.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/controller.py` & `pyplanet-0.9.9/pyplanet/core/controller.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/db/database.py` & `pyplanet-0.9.9/pyplanet/core/db/database.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/db/migrator.py` & `pyplanet-0.9.9/pyplanet/core/db/migrator.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/db/model.py` & `pyplanet-0.9.9/pyplanet/core/db/model.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/db/registry.py` & `pyplanet-0.9.9/pyplanet/core/db/registry.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/events/callback.py` & `pyplanet-0.9.9/pyplanet/core/events/callback.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/events/dispatcher.py` & `pyplanet-0.9.9/pyplanet/core/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/events/manager.py` & `pyplanet-0.9.9/pyplanet/core/events/manager.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/exceptions.py` & `pyplanet-0.9.9/pyplanet/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/game.py` & `pyplanet-0.9.9/pyplanet/core/game.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/gbx/client.py` & `pyplanet-0.9.9/pyplanet/core/gbx/client.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/gbx/query.py` & `pyplanet-0.9.9/pyplanet/core/gbx/query.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/gbx/remote.py` & `pyplanet-0.9.9/pyplanet/core/gbx/remote.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/instance.py` & `pyplanet-0.9.9/pyplanet/core/instance.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/__init__.py` & `pyplanet-0.9.9/pyplanet/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/base.py` & `pyplanet-0.9.9/pyplanet/core/management/base.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/color.py` & `pyplanet-0.9.9/pyplanet/core/management/color.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/commands/db_convert.py` & `pyplanet-0.9.9/pyplanet/core/management/commands/db_convert.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/commands/init_app.py` & `pyplanet-0.9.9/pyplanet/core/management/commands/init_app.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/commands/init_project.py` & `pyplanet-0.9.9/pyplanet/core/management/commands/init_project.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/commands/start.py` & `pyplanet-0.9.9/pyplanet/core/management/commands/start.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/commands/upgrade.py` & `pyplanet-0.9.9/pyplanet/core/management/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/management.py` & `pyplanet-0.9.9/pyplanet/core/management/management.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/management/templates.py` & `pyplanet-0.9.9/pyplanet/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/signals.py` & `pyplanet-0.9.9/pyplanet/core/signals.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/storage/drivers/asyncssh/__init__.py` & `pyplanet-0.9.9/pyplanet/core/storage/drivers/asyncssh/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/storage/drivers/local/__init__.py` & `pyplanet-0.9.9/pyplanet/core/storage/drivers/local/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/storage/interface.py` & `pyplanet-0.9.9/pyplanet/core/storage/interface.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/storage/storage.py` & `pyplanet-0.9.9/pyplanet/core/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/ui/__init__.py` & `pyplanet-0.9.9/pyplanet/core/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/ui/components/manialink.py` & `pyplanet-0.9.9/pyplanet/core/ui/components/manialink.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/ui/loader.py` & `pyplanet-0.9.9/pyplanet/core/ui/loader.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/ui/template.py` & `pyplanet-0.9.9/pyplanet/core/ui/template.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/core/ui/ui_properties.py` & `pyplanet-0.9.9/pyplanet/core/ui/ui_properties.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/god/pool.py` & `pyplanet-0.9.9/pyplanet/god/pool.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/god/process.py` & `pyplanet-0.9.9/pyplanet/god/process.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/analytics.py` & `pyplanet-0.9.9/pyplanet/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/codeutils.py` & `pyplanet-0.9.9/pyplanet/utils/codeutils.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/gbxparser.py` & `pyplanet-0.9.9/pyplanet/utils/gbxparser.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/log.py` & `pyplanet-0.9.9/pyplanet/utils/log.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/memleak.py` & `pyplanet-0.9.9/pyplanet/utils/memleak.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/pip.py` & `pyplanet-0.9.9/pyplanet/utils/pip.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/pip_test_pkg/setup.py` & `pyplanet-0.9.9/pyplanet/utils/pip_test_pkg/setup.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/releases.py` & `pyplanet-0.9.9/pyplanet/utils/releases.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/semver.py` & `pyplanet-0.9.9/pyplanet/utils/semver.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/style.py` & `pyplanet-0.9.9/pyplanet/utils/style.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/termcolors.py` & `pyplanet-0.9.9/pyplanet/utils/termcolors.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/times.py` & `pyplanet-0.9.9/pyplanet/utils/times.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/utils/toposort.py` & `pyplanet-0.9.9/pyplanet/utils/toposort.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/generics/alert.py` & `pyplanet-0.9.9/pyplanet/views/generics/alert.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/generics/list.py` & `pyplanet-0.9.9/pyplanet/views/generics/list.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/generics/widget.py` & `pyplanet-0.9.9/pyplanet/views/generics/widget.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/template.py` & `pyplanet-0.9.9/pyplanet/views/template.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/generics/alert.xml` & `pyplanet-0.9.9/pyplanet/views/templates/generics/alert.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/generics/list.xml` & `pyplanet-0.9.9/pyplanet/views/templates/generics/list.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/generics/prompt.xml` & `pyplanet-0.9.9/pyplanet/views/templates/generics/prompt.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/generics/timeswidget.xml` & `pyplanet-0.9.9/pyplanet/views/templates/generics/timeswidget.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/generics/widget.Script.Txt` & `pyplanet-0.9.9/pyplanet/views/templates/generics/widget.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/generics/widget.xml` & `pyplanet-0.9.9/pyplanet/views/templates/generics/widget.xml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/generics/widget_next.Script.Txt` & `pyplanet-0.9.9/pyplanet/views/templates/generics/widget_next.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet/views/templates/libs/TimeUtils.Script.Txt` & `pyplanet-0.9.9/pyplanet/views/templates/libs/TimeUtils.Script.Txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet.egg-info/PKG-INFO` & `pyplanet-0.9.9/pyplanet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyplanet
-Version: 0.9.8
+Version: 0.9.9
 Summary: Maniaplanet Server Controller
 Home-page: http://pypla.net/
 Author: Tom Valk
 Author-email: tomvalk@lt-box.info
 License: GNU General Public License v3 (GPLv3)
 Description: PyPlanet
         ========
```

### Comparing `pyplanet-0.9.8/pyplanet.egg-info/SOURCES.txt` & `pyplanet-0.9.9/pyplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/pyplanet.py` & `pyplanet-0.9.9/pyplanet.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/setup.py` & `pyplanet-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_files/maps/canyon-mp4-1.gbx` & `pyplanet-0.9.9/tests/_files/maps/canyon-mp4-1.gbx`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_files/maps/canyon-mp4-2.gbx` & `pyplanet-0.9.9/tests/_files/maps/canyon-mp4-2.gbx`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_files/maps/greyroad.gbx` & `pyplanet-0.9.9/tests/_files/maps/greyroad.gbx`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_files/maps/royal-mp4-1.gbx` & `pyplanet-0.9.9/tests/_files/maps/royal-mp4-1.gbx`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor/dedicated/dedicated_cfg.txt` & `pyplanet-0.9.9/tests/_scripts/appveyor/dedicated/dedicated_cfg.txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor/dedicated/matchsettings_1.txt` & `pyplanet-0.9.9/tests/_scripts/appveyor/dedicated/matchsettings_1.txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor/settings/apps.json` & `pyplanet-0.9.9/tests/_scripts/appveyor/settings/apps.json`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor/settings/apps.py` & `pyplanet-0.9.9/tests/_scripts/appveyor/settings/apps.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor/settings/base.json` & `pyplanet-0.9.9/tests/_scripts/appveyor/settings/base.json`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor/settings/base.py` & `pyplanet-0.9.9/tests/_scripts/appveyor/settings/base.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor/settings/base.yaml` & `pyplanet-0.9.9/tests/_scripts/appveyor/settings/base.yaml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor_init.py` & `pyplanet-0.9.9/tests/_scripts/appveyor_init.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/appveyor_with_compiler.cmd` & `pyplanet-0.9.9/tests/_scripts/appveyor_with_compiler.cmd`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis/dedicated/dedicated_cfg.txt` & `pyplanet-0.9.9/tests/_scripts/travis/dedicated/dedicated_cfg.txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis/dedicated/matchsettings_1.txt` & `pyplanet-0.9.9/tests/_scripts/travis/dedicated/matchsettings_1.txt`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis/settings/apps.json` & `pyplanet-0.9.9/tests/_scripts/travis/settings/apps.json`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis/settings/apps.py` & `pyplanet-0.9.9/tests/_scripts/travis/settings/apps.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis/settings/base.json` & `pyplanet-0.9.9/tests/_scripts/travis/settings/base.json`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis/settings/base.py` & `pyplanet-0.9.9/tests/_scripts/travis/settings/base.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis/settings/base.yaml` & `pyplanet-0.9.9/tests/_scripts/travis/settings/base.yaml`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis_dedicated_setup.sh` & `pyplanet-0.9.9/tests/_scripts/travis_dedicated_setup.sh`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/_scripts/travis_dedicated_start.sh` & `pyplanet-0.9.9/tests/_scripts/travis_dedicated_start.sh`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/apps/migration_test/__init__.py` & `pyplanet-0.9.9/tests/apps/migration_test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/integration/contrib/test_map.py` & `pyplanet-0.9.9/tests/integration/contrib/test_map.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/integration/contrib/test_player.py` & `pyplanet-0.9.9/tests/integration/contrib/test_player.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/integration/test_gbx.py` & `pyplanet-0.9.9/tests/integration/test_gbx.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/integration/test_instance.py` & `pyplanet-0.9.9/tests/integration/test_instance.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/contrib/test_chat.py` & `pyplanet-0.9.9/tests/unit/contrib/test_chat.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/contrib/test_commands.py` & `pyplanet-0.9.9/tests/unit/contrib/test_commands.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/contrib/test_permissions.py` & `pyplanet-0.9.9/tests/unit/contrib/test_permissions.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/contrib/test_settings.py` & `pyplanet-0.9.9/tests/unit/contrib/test_settings.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/storage/test_local_driver.py` & `pyplanet-0.9.9/tests/unit/storage/test_local_driver.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/test_callbacks.py` & `pyplanet-0.9.9/tests/unit/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/test_conf.py` & `pyplanet-0.9.9/tests/unit/test_conf.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/test_database.py` & `pyplanet-0.9.9/tests/unit/test_database.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/test_signals.py` & `pyplanet-0.9.9/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/test_ui_template.py` & `pyplanet-0.9.9/tests/unit/test_ui_template.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/test_views.py` & `pyplanet-0.9.9/tests/unit/test_views.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/utils/test_gbxparser.py` & `pyplanet-0.9.9/tests/unit/utils/test_gbxparser.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/utils/test_style.py` & `pyplanet-0.9.9/tests/unit/utils/test_style.py`

 * *Files identical despite different names*

### Comparing `pyplanet-0.9.8/tests/unit/utils/test_toposort.py` & `pyplanet-0.9.9/tests/unit/utils/test_toposort.py`

 * *Files identical despite different names*

