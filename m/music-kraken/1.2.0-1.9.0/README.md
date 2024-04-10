# Comparing `tmp/music_kraken-1.2.0.tar.gz` & `tmp/music_kraken-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music_kraken-1.2.0.tar", last modified: Thu Nov 24 11:37:27 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `music_kraken-1.2.0.tar` & `music_kraken-1.9.0.tar`

### file list

```diff
@@ -1,52 +1,7 @@
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.226579 music_kraken-1.2.0/
--rw-rw-r--   0 lars      (1000) lars      (1000)    34523 2022-10-17 11:31:10.000000 music_kraken-1.2.0/LICENSE
--rw-rw-r--   0 lars      (1000) lars      (1000)    14518 2022-11-24 11:37:27.226579 music_kraken-1.2.0/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)    13953 2022-11-24 11:07:32.000000 music_kraken-1.2.0/README.md
--rw-rw-r--   0 lars      (1000) lars      (1000)      743 2022-11-24 11:35:31.000000 music_kraken-1.2.0/pyproject.toml
--rw-rw-r--   0 lars      (1000) lars      (1000)       38 2022-11-24 11:37:27.226579 music_kraken-1.2.0/setup.cfg
--rw-rw-r--   0 lars      (1000) lars      (1000)     1327 2022-11-23 08:11:35.000000 music_kraken-1.2.0/setup.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.218579 music_kraken-1.2.0/src/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.222579 music_kraken-1.2.0/src/music_kraken/
--rw-rw-r--   0 lars      (1000) lars      (1000)     3831 2022-11-23 22:49:35.000000 music_kraken-1.2.0/src/music_kraken/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      321 2022-11-16 11:34:05.000000 music_kraken-1.2.0/src/music_kraken/__main__.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.222579 music_kraken-1.2.0/src/music_kraken/audio_source/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2022-11-16 08:49:42.000000 music_kraken-1.2.0/src/music_kraken/audio_source/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3126 2022-11-22 22:39:43.000000 music_kraken-1.2.0/src/music_kraken/audio_source/fetch_audio.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     2427 2022-11-24 11:25:43.000000 music_kraken-1.2.0/src/music_kraken/audio_source/fetch_source.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.222579 music_kraken-1.2.0/src/music_kraken/audio_source/sources/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2022-11-16 08:51:41.000000 music_kraken-1.2.0/src/music_kraken/audio_source/sources/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1972 2022-11-16 08:58:37.000000 music_kraken-1.2.0/src/music_kraken/audio_source/sources/local_files.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     6471 2022-11-22 12:47:48.000000 music_kraken-1.2.0/src/music_kraken/audio_source/sources/musify.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      679 2022-11-22 12:50:07.000000 music_kraken-1.2.0/src/music_kraken/audio_source/sources/source.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3000 2022-11-22 22:39:43.000000 music_kraken-1.2.0/src/music_kraken/audio_source/sources/youtube.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.222579 music_kraken-1.2.0/src/music_kraken/database/
--rw-rw-r--   0 lars      (1000) lars      (1000)    10230 2022-11-22 08:17:44.000000 music_kraken-1.2.0/src/music_kraken/database/database.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3635 2022-11-23 10:32:27.000000 music_kraken-1.2.0/src/music_kraken/database/song.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      388 2022-11-22 13:47:20.000000 music_kraken-1.2.0/src/music_kraken/database/temp_database.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.222579 music_kraken-1.2.0/src/music_kraken/lyrics/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2022-11-15 06:47:53.000000 music_kraken-1.2.0/src/music_kraken/lyrics/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     7570 2022-11-15 06:47:53.000000 music_kraken-1.2.0/src/music_kraken/lyrics/genius.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3132 2022-11-22 22:39:43.000000 music_kraken-1.2.0/src/music_kraken/lyrics/lyrics.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.226579 music_kraken-1.2.0/src/music_kraken/metadata/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2022-11-15 06:47:53.000000 music_kraken-1.2.0/src/music_kraken/metadata/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    13852 2022-11-22 13:55:56.000000 music_kraken-1.2.0/src/music_kraken/metadata/metadata_fetch.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    15375 2022-11-22 10:06:30.000000 music_kraken-1.2.0/src/music_kraken/metadata/metadata_search.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.226579 music_kraken-1.2.0/src/music_kraken/tagging/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2022-11-15 06:47:53.000000 music_kraken-1.2.0/src/music_kraken/tagging/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)       60 2022-11-15 06:47:53.000000 music_kraken-1.2.0/src/music_kraken/tagging/song.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.226579 music_kraken-1.2.0/src/music_kraken/target/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2022-11-16 09:01:28.000000 music_kraken-1.2.0/src/music_kraken/target/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1594 2022-11-22 13:58:10.000000 music_kraken-1.2.0/src/music_kraken/target/set_target.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.226579 music_kraken-1.2.0/src/music_kraken/utils/
--rw-rw-r--   0 lars      (1000) lars      (1000)       95 2022-11-22 10:06:30.000000 music_kraken-1.2.0/src/music_kraken/utils/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)       93 2022-11-22 10:06:30.000000 music_kraken-1.2.0/src/music_kraken/utils/functions.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      803 2022-11-15 06:47:53.000000 music_kraken-1.2.0/src/music_kraken/utils/object_handeling.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1280 2022-11-23 22:49:35.000000 music_kraken-1.2.0/src/music_kraken/utils/phonetic_compares.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1602 2022-11-23 07:51:10.000000 music_kraken-1.2.0/src/music_kraken/utils/shared.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2022-11-24 11:37:27.222579 music_kraken-1.2.0/src/music_kraken.egg-info/
--rw-rw-r--   0 lars      (1000) lars      (1000)    14518 2022-11-24 11:37:27.000000 music_kraken-1.2.0/src/music_kraken.egg-info/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     1403 2022-11-24 11:37:27.000000 music_kraken-1.2.0/src/music_kraken.egg-info/SOURCES.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)        1 2022-11-24 11:37:27.000000 music_kraken-1.2.0/src/music_kraken.egg-info/dependency_links.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       50 2022-11-24 11:37:27.000000 music_kraken-1.2.0/src/music_kraken.egg-info/entry_points.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)      138 2022-11-24 11:37:27.000000 music_kraken-1.2.0/src/music_kraken.egg-info/requires.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       13 2022-11-24 11:37:27.000000 music_kraken-1.2.0/src/music_kraken.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 music_kraken-1.9.0/music_kraken/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 music_kraken-1.9.0/music_kraken/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 music_kraken-1.9.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-1.9.0/LICENSE
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 music_kraken-1.9.0/README.md
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 music_kraken-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 music_kraken-1.9.0/PKG-INFO
```

### Comparing `music_kraken-1.2.0/LICENSE` & `music_kraken-1.9.0/LICENSE`

 * *Files identical despite different names*

