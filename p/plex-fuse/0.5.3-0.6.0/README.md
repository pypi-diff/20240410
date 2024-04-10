# Comparing `tmp/plex-fuse-0.5.3.tar.gz` & `tmp/plex-fuse-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-fuse-0.5.3.tar", last modified: Tue Mar 26 22:54:47 2024, max compression
+gzip compressed data, was "plex-fuse-0.6.0.tar", last modified: Wed Apr 10 13:44:37 2024, max compression
```

## Comparing `plex-fuse-0.5.3.tar` & `plex-fuse-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.765309 plex-fuse-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-26 22:54:47.761309 plex-fuse-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.761309 plex-fuse-0.5.3/plex_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-26 22:54:47.000000 plex-fuse-0.5.3/plex_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-26 22:54:47.000000 plex-fuse-0.5.3/plex_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:54:47.000000 plex-fuse-0.5.3/plex_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-26 22:54:47.000000 plex-fuse-0.5.3/plex_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-26 22:54:47.000000 plex-fuse-0.5.3/plex_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 22:54:47.000000 plex-fuse-0.5.3/plex_fuse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.757310 plex-fuse-0.5.3/plexfuse/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.757310 plex-fuse-0.5.3/plexfuse/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/cache/CacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/cache/CachedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/cache/DelayedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/cache/FileCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/cache/HttpCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/cache/UserDictCacheControl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.757310 plex-fuse-0.5.3/plexfuse/control/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/control/ControlListener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.757310 plex-fuse-0.5.3/plexfuse/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/fs/FsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/fs/PlexDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/fs/PlexFS.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/fs/PlexFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/fs/RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/fs/Timestampable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/fs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.761309 plex-fuse-0.5.3/plexfuse/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/plex/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.761309 plex-fuse-0.5.3/plexfuse/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/ChunkedFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/Control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/Playable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/PlexVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.761309 plex-fuse-0.5.3/plexfuse/vfs/entry/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/AttrEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/ControlEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/DirEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/EpisodeEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/FileEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/LibraryEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/MovieEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/PathEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/PlexMatchEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/SeasonEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/SectionEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/plexfuse/vfs/entry/SubtitleEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 22:54:47.765309 plex-fuse-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:54:47.761309 plex-fuse-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/tests/test_RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/tests/test_chunk_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/tests/test_chunk_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/tests/test_file_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/tests/test_file_copy_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-26 22:54:44.000000 plex-fuse-0.5.3/tests/test_socket_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/plex_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.271532 plex-fuse-0.6.0/plexfuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/CacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/CachedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/DelayedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/FileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/HttpCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/UserDictCacheControl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/control/ControlListener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/FsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/PlexDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/PlexFS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/PlexFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/Timestampable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/plex/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/ChunkedFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/Control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/Playable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/PlexVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/plexfuse/vfs/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/AttrEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/ControlEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/ControlSockEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/DirEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/EpisodeEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/FileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/LibraryEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/MovieEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/PathEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/PlexMatchEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/SeasonEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/SectionEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/SubtitleEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_chunk_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_chunk_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_file_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_file_copy_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_socket_control.py
```

### Comparing `plex-fuse-0.5.3/LICENSE` & `plex-fuse-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/PKG-INFO` & `plex-fuse-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.5.3
+Version: 0.6.0
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
@@ -52,15 +52,15 @@
 Requires-Dist: fuse-python
 Requires-Dist: plexapi>=4.15
 Requires-Dist: requests-cache>=1.1
 Requires-Dist: websocket-client>=1.7.0
 
 # Plex FUSE Filesystem
 
-An attempt to create fuse filesystem to access Plex Media Server.
+An attempt to create fuse filesystem to access Plex Media Server files as local files.
 
 ## Development
 
 This project is in very early development.
 
 Currently implemented:
 - [x] Listing of root directory
@@ -94,24 +94,33 @@
 - [ ] Add docker volume driver
 - [ ] Add cache management (max size?)
 - [ ] Add cache purge option (special file?)
 - [ ] Detect need to refresh cache (add event listener)
 - [ ] Handling of "artist" library type
 - [x] Add "status" and "reload" control channels
 
+## Requirements
+
+1. Python >= 3.11
+1. fuse, macfuse, osxfuse or [fuse-t] depending on your OS
+
+[fuse-t]: https://github.com/macos-fuse-t/fuse-t
+
+## Installation
+
+1. Install [pipx]
+1. Install `plex-fuse`: `pipx install plex-fuse`
+
+[pipx]: https://pipx.pypa.io/stable/installation
+
 ## Usage
 
-1. Install Python >= 3.11
-1. Install fuse, macfuse, osxfuse, [fuse-t](https://github.com/macos-fuse-t/fuse-t) depending on your OS
-1. Install [pipenv](https://pipenv.pypa.io/en/latest/installation.html)
-1. Clone this project: `git clone https://github.com/glensc/plex-fuse`
-1. Change to `plex-fuse` directory
-1. Install project dependencies `pipenv install`
+1. Check [requirements](#requirements) and [installation](#installation)
 1. Create [config.ini](#plex-config) for `python-plexapi`
-1. Mount the configured PMS somewhere, i.e `plex-server`: `mkdir plex-server; pipenv run python -m plexfuse plex-server -f`
+1. Mount the configured PMS somewhere, i.e `plex-server`: `mkdir plex-server; plex-fuse plex-server -f`
 1. Access the `plex-server` directory from another terminal
 1. `umount` or `fusermount -u` the directory to remove the `plex-server` mount
 
 ## Plex Config
 
 Create Plex [configuration] file:
```

### Comparing `plex-fuse-0.5.3/README.md` & `plex-fuse-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Plex FUSE Filesystem
 
-An attempt to create fuse filesystem to access Plex Media Server.
+An attempt to create fuse filesystem to access Plex Media Server files as local files.
 
 ## Development
 
 This project is in very early development.
 
 Currently implemented:
 - [x] Listing of root directory
@@ -38,24 +38,33 @@
 - [ ] Add docker volume driver
 - [ ] Add cache management (max size?)
 - [ ] Add cache purge option (special file?)
 - [ ] Detect need to refresh cache (add event listener)
 - [ ] Handling of "artist" library type
 - [x] Add "status" and "reload" control channels
 
+## Requirements
+
+1. Python >= 3.11
+1. fuse, macfuse, osxfuse or [fuse-t] depending on your OS
+
+[fuse-t]: https://github.com/macos-fuse-t/fuse-t
+
+## Installation
+
+1. Install [pipx]
+1. Install `plex-fuse`: `pipx install plex-fuse`
+
+[pipx]: https://pipx.pypa.io/stable/installation
+
 ## Usage
 
-1. Install Python >= 3.11
-1. Install fuse, macfuse, osxfuse, [fuse-t](https://github.com/macos-fuse-t/fuse-t) depending on your OS
-1. Install [pipenv](https://pipenv.pypa.io/en/latest/installation.html)
-1. Clone this project: `git clone https://github.com/glensc/plex-fuse`
-1. Change to `plex-fuse` directory
-1. Install project dependencies `pipenv install`
+1. Check [requirements](#requirements) and [installation](#installation)
 1. Create [config.ini](#plex-config) for `python-plexapi`
-1. Mount the configured PMS somewhere, i.e `plex-server`: `mkdir plex-server; pipenv run python -m plexfuse plex-server -f`
+1. Mount the configured PMS somewhere, i.e `plex-server`: `mkdir plex-server; plex-fuse plex-server -f`
 1. Access the `plex-server` directory from another terminal
 1. `umount` or `fusermount -u` the directory to remove the `plex-server` mount
 
 ## Plex Config
 
 Create Plex [configuration] file:
```

### Comparing `plex-fuse-0.5.3/plex_fuse.egg-info/PKG-INFO` & `plex-fuse-0.6.0/plex_fuse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.5.3
+Version: 0.6.0
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
@@ -52,15 +52,15 @@
 Requires-Dist: fuse-python
 Requires-Dist: plexapi>=4.15
 Requires-Dist: requests-cache>=1.1
 Requires-Dist: websocket-client>=1.7.0
 
 # Plex FUSE Filesystem
 
-An attempt to create fuse filesystem to access Plex Media Server.
+An attempt to create fuse filesystem to access Plex Media Server files as local files.
 
 ## Development
 
 This project is in very early development.
 
 Currently implemented:
 - [x] Listing of root directory
@@ -94,24 +94,33 @@
 - [ ] Add docker volume driver
 - [ ] Add cache management (max size?)
 - [ ] Add cache purge option (special file?)
 - [ ] Detect need to refresh cache (add event listener)
 - [ ] Handling of "artist" library type
 - [x] Add "status" and "reload" control channels
 
+## Requirements
+
+1. Python >= 3.11
+1. fuse, macfuse, osxfuse or [fuse-t] depending on your OS
+
+[fuse-t]: https://github.com/macos-fuse-t/fuse-t
+
+## Installation
+
+1. Install [pipx]
+1. Install `plex-fuse`: `pipx install plex-fuse`
+
+[pipx]: https://pipx.pypa.io/stable/installation
+
 ## Usage
 
-1. Install Python >= 3.11
-1. Install fuse, macfuse, osxfuse, [fuse-t](https://github.com/macos-fuse-t/fuse-t) depending on your OS
-1. Install [pipenv](https://pipenv.pypa.io/en/latest/installation.html)
-1. Clone this project: `git clone https://github.com/glensc/plex-fuse`
-1. Change to `plex-fuse` directory
-1. Install project dependencies `pipenv install`
+1. Check [requirements](#requirements) and [installation](#installation)
 1. Create [config.ini](#plex-config) for `python-plexapi`
-1. Mount the configured PMS somewhere, i.e `plex-server`: `mkdir plex-server; pipenv run python -m plexfuse plex-server -f`
+1. Mount the configured PMS somewhere, i.e `plex-server`: `mkdir plex-server; plex-fuse plex-server -f`
 1. Access the `plex-server` directory from another terminal
 1. `umount` or `fusermount -u` the directory to remove the `plex-server` mount
 
 ## Plex Config
 
 Create Plex [configuration] file:
```

### Comparing `plex-fuse-0.5.3/plex_fuse.egg-info/SOURCES.txt` & `plex-fuse-0.6.0/plex_fuse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 plexfuse/plex/types.py
 plexfuse/vfs/ChunkedFile.py
 plexfuse/vfs/Control.py
 plexfuse/vfs/Playable.py
 plexfuse/vfs/PlexVFS.py
 plexfuse/vfs/entry/AttrEntry.py
 plexfuse/vfs/entry/ControlEntry.py
+plexfuse/vfs/entry/ControlSockEntry.py
 plexfuse/vfs/entry/DirEntry.py
 plexfuse/vfs/entry/EpisodeEntry.py
 plexfuse/vfs/entry/FileEntry.py
 plexfuse/vfs/entry/LibraryEntry.py
 plexfuse/vfs/entry/MovieEntry.py
 plexfuse/vfs/entry/PathEntry.py
 plexfuse/vfs/entry/PlexMatchEntry.py
```

### Comparing `plex-fuse-0.5.3/plexfuse/cache/CacheControl.py` & `plex-fuse-0.6.0/plexfuse/cache/CacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/cache/CachedPropertyCacheControl.py` & `plex-fuse-0.6.0/plexfuse/cache/CachedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/cache/DelayedPropertyCacheControl.py` & `plex-fuse-0.6.0/plexfuse/cache/DelayedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/cache/FileCache.py` & `plex-fuse-0.6.0/plexfuse/cache/FileCache.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/cache/HttpCache.py` & `plex-fuse-0.6.0/plexfuse/cache/HttpCache.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/cache/UserDictCacheControl.py` & `plex-fuse-0.6.0/plexfuse/cache/UserDictCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/control/ControlListener.py` & `plex-fuse-0.6.0/plexfuse/control/ControlListener.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/fs/RefCountedDict.py` & `plex-fuse-0.6.0/plexfuse/fs/RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/fs/main.py` & `plex-fuse-0.6.0/plexfuse/fs/main.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/plex/Monitor.py` & `plex-fuse-0.6.0/plexfuse/plex/Monitor.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/plex/PlexApi.py` & `plex-fuse-0.6.0/plexfuse/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/ChunkedFile.py` & `plex-fuse-0.6.0/plexfuse/vfs/ChunkedFile.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/Control.py` & `plex-fuse-0.6.0/plexfuse/vfs/Control.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,31 +6,43 @@
 from plexfuse.cache.CacheControl import CacheControl
 from plexfuse.cache.CachedPropertyCacheControl import \
     CachedPropertyCacheControl
 from plexfuse.cache.DelayedPropertyCacheControl import \
     DelayedPropertyCacheControl
 from plexfuse.cache.UserDictCacheControl import UserDictCacheControl
 from plexfuse.vfs.entry.ControlEntry import ControlEntry
+from plexfuse.vfs.entry.ControlSockEntry import ControlSockEntry
 from plexfuse.vfs.entry.DirEntry import DirEntry
 
 if TYPE_CHECKING:
     from plexfuse.fs.PlexFS import PlexFS
     from plexfuse.plex.PlexApi import PlexApi
     from plexfuse.vfs.PlexVFS import PlexVFS
 
 
 class Control:
-    def __init__(self, plex: PlexApi, plexfs: PlexFS, plexvfs: PlexVFS):
+    CONTROL_DIR = "control"
+    CONTROL_SOCK = "control.sock"
+
+    def __init__(self, plex: PlexApi, plexfs: PlexFS, plexvfs: PlexVFS, control_path: str = None):
         self.plex = plex
         self.plexfs = plexfs
         self.plexvfs = plexvfs
+        self.control_path = control_path
 
     @property
     def root(self):
-        return ["control"]
+        entries = [
+            self.CONTROL_DIR,
+        ]
+
+        if self.control_path:
+            entries.append(self.CONTROL_SOCK)
+
+        return entries
 
     @property
     def commands(self):
         return ["reload", "status"]
 
     @cached_property
     def cc_plexfs(self):
@@ -61,15 +73,18 @@
         yield from self.cc_library.cache_info()
 
     def action(self, action: str):
         method = getattr(self, action)
         return "\n".join(method()).encode() + b"\n"
 
     def handle(self, pc: int, pe: list[str]):
-        if pc == 1 and pe[0] in self.root:
+        if pc == 1 and pe[0] == self.CONTROL_SOCK:
+            return ControlSockEntry(pe[0], self.control_path)
+
+        if pc == 1 and pe[0] == self.CONTROL_DIR:
             return DirEntry(self.commands)
 
-        if pc != 2 or pe[0] != self.root[0]:
+        if pc != 2 or pe[0] != self.CONTROL_DIR:
             return
 
         if pe[1] in self.commands:
             return ControlEntry(pe[1], getattr(self, pe[1]))
```

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/Playable.py` & `plex-fuse-0.6.0/plexfuse/vfs/Playable.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/PlexVFS.py` & `plex-fuse-0.6.0/plexfuse/vfs/PlexVFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from collections import UserDict
 from typing import TYPE_CHECKING
 
 from plexfuse.vfs.ChunkedFile import ChunkedFile
 from plexfuse.vfs.Control import Control
 from plexfuse.vfs.entry.DirEntry import DirEntry
 from plexfuse.vfs.entry.FileEntry import FileEntry
-from plexfuse.vfs.entry.SubtitleEntry import SubtitleEntry
 from plexfuse.vfs.entry.PlexMatchEntry import PlexMatchEntry
+from plexfuse.vfs.entry.SubtitleEntry import SubtitleEntry
 
 if TYPE_CHECKING:
     from plexfuse.fs.PlexFS import PlexFS
     from plexfuse.plex.PlexApi import PlexApi
 
 
 class PlexVFS(UserDict):
     SUBTITLE_EXT = (".srt", ".vtt")
 
-    def __init__(self, plex: PlexApi, plexfs: PlexFS):
+    def __init__(self, plex: PlexApi, plexfs: PlexFS, control_path: str = None):
         super().__init__()
         self.plex = plex
         self.reader = ChunkedFile(plex)
-        self.control = Control(plex, plexfs, self)
+        self.control = Control(plex, plexfs, self, control_path)
 
     def __missing__(self, path: str):
         entry = self.resolve(path)
         if entry is None:
             raise KeyError(path)
 
         self[path] = entry
```

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/entry/ControlEntry.py` & `plex-fuse-0.6.0/plexfuse/vfs/entry/ControlEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/entry/FileEntry.py` & `plex-fuse-0.6.0/plexfuse/vfs/entry/FileEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/entry/LibraryEntry.py` & `plex-fuse-0.6.0/plexfuse/vfs/entry/LibraryEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/entry/PlexMatchEntry.py` & `plex-fuse-0.6.0/plexfuse/vfs/entry/PlexMatchEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/entry/SectionEntry.py` & `plex-fuse-0.6.0/plexfuse/vfs/entry/SectionEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/plexfuse/vfs/entry/SubtitleEntry.py` & `plex-fuse-0.6.0/plexfuse/vfs/entry/SubtitleEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/pyproject.toml` & `plex-fuse-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/tests/test_RefCountedDict.py` & `plex-fuse-0.6.0/tests/test_RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/tests/test_chunk_calc.py` & `plex-fuse-0.6.0/tests/test_chunk_calc.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/tests/test_chunk_read.py` & `plex-fuse-0.6.0/tests/test_chunk_read.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/tests/test_file_copy_partial.py` & `plex-fuse-0.6.0/tests/test_file_copy_partial.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.5.3/tests/test_socket_control.py` & `plex-fuse-0.6.0/tests/test_socket_control.py`

 * *Files identical despite different names*

