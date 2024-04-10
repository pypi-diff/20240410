# Comparing `tmp/mov-cli-films-1.3.5.tar.gz` & `tmp/mov-cli-films-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-films-1.3.5.tar", last modified: Tue Apr  9 23:52:05 2024, max compression
+gzip compressed data, was "mov-cli-films-1.3.6.tar", last modified: Wed Apr 10 00:51:17 2024, max compression
```

## Comparing `mov-cli-films-1.3.5.tar` & `mov-cli-films-1.3.6.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:34:31.000000 mov-cli-films-1.3.5/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2915 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      569 2024-04-09 23:47:16.000000 mov-cli-films-1.3.5/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/mov_cli_films/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      507 2024-04-09 23:51:22.000000 mov-cli-films-1.3.5/mov_cli_films/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/mov_cli_films/vidsrcme/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 20:16:52.000000 mov-cli-films-1.3.5/mov_cli_films/vidsrcme/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4390 2024-04-09 23:50:40.000000 mov-cli-films-1.3.5/mov_cli_films/vidsrcme/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/mov_cli_films/vidsrcto/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-09 16:43:29.000000 mov-cli-films-1.3.5/mov_cli_films/vidsrcto/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/mov_cli_films/vidsrcto/ext/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-27 21:59:37.000000 mov-cli-films-1.3.5/mov_cli_films/vidsrcto/ext/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4019 2024-03-27 21:59:49.000000 mov-cli-films-1.3.5/mov_cli_films/vidsrcto/ext/vidplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4508 2024-04-09 23:50:24.000000 mov-cli-films-1.3.5/mov_cli_films/vidsrcto/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/mov_cli_films.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2915 2024-04-09 23:52:04.000000 mov-cli-films-1.3.5/mov_cli_films.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      457 2024-04-09 23:52:05.000000 mov-cli-films-1.3.5/mov_cli_films.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-09 23:52:04.000000 mov-cli-films-1.3.5/mov_cli_films.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-04-09 23:52:04.000000 mov-cli-films-1.3.5/mov_cli_films.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-09 23:52:04.000000 mov-cli-films-1.3.5/mov_cli_films.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1326 2024-04-03 21:05:40.000000 mov-cli-films-1.3.5/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-09 23:52:05.004075 mov-cli-films-1.3.5/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 00:51:17.857077 mov-cli-films-1.3.6/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:34:31.000000 mov-cli-films-1.3.6/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2915 2024-04-10 00:51:17.857077 mov-cli-films-1.3.6/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      569 2024-04-09 23:47:16.000000 mov-cli-films-1.3.6/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 00:51:17.853744 mov-cli-films-1.3.6/mov_cli_films/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      568 2024-04-10 00:50:30.000000 mov-cli-films-1.3.6/mov_cli_films/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 00:51:17.853744 mov-cli-films-1.3.6/mov_cli_films/vadapav/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-04-10 00:49:50.000000 mov-cli-films-1.3.6/mov_cli_films/vadapav/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6450 2024-04-10 00:50:07.000000 mov-cli-films-1.3.6/mov_cli_films/vadapav/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 00:51:17.857077 mov-cli-films-1.3.6/mov_cli_films/vidsrcme/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 20:16:52.000000 mov-cli-films-1.3.6/mov_cli_films/vidsrcme/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4364 2024-04-10 00:48:41.000000 mov-cli-films-1.3.6/mov_cli_films/vidsrcme/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 00:51:17.857077 mov-cli-films-1.3.6/mov_cli_films/vidsrcto/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-09 16:43:29.000000 mov-cli-films-1.3.6/mov_cli_films/vidsrcto/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 00:51:17.857077 mov-cli-films-1.3.6/mov_cli_films/vidsrcto/ext/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-27 21:59:37.000000 mov-cli-films-1.3.6/mov_cli_films/vidsrcto/ext/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4019 2024-03-27 21:59:49.000000 mov-cli-films-1.3.6/mov_cli_films/vidsrcto/ext/vidplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4508 2024-04-10 00:47:28.000000 mov-cli-films-1.3.6/mov_cli_films/vidsrcto/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 00:51:17.857077 mov-cli-films-1.3.6/mov_cli_films.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2915 2024-04-10 00:51:17.000000 mov-cli-films-1.3.6/mov_cli_films.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      524 2024-04-10 00:51:17.000000 mov-cli-films-1.3.6/mov_cli_films.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-10 00:51:17.000000 mov-cli-films-1.3.6/mov_cli_films.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-04-10 00:51:17.000000 mov-cli-films-1.3.6/mov_cli_films.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-10 00:51:17.000000 mov-cli-films-1.3.6/mov_cli_films.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1326 2024-04-03 21:05:40.000000 mov-cli-films-1.3.6/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-10 00:51:17.857077 mov-cli-films-1.3.6/setup.cfg
```

### Comparing `mov-cli-films-1.3.5/LICENSE` & `mov-cli-films-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-films-1.3.5/PKG-INFO` & `mov-cli-films-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-films
-Version: 1.3.5
+Version: 1.3.6
 Summary: A mov-cli v4 plugin for watching Films and Shows.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-films-1.3.5/README.md` & `mov-cli-films-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mov-cli-films-1.3.5/mov_cli_films/vidsrcme/scraper.py` & `mov-cli-films-1.3.6/mov_cli_films/vidsrcme/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     from mov_cli import Config
     from httpx import Response
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
 import re
 
-from mov_cli import utils
 from mov_cli.scraper import Scraper
 from mov_cli import Multi, Single, Metadata, MetadataType
 from mov_cli.utils.scraper import TheMovieDB
 from mov_cli.utils import EpisodeSelector
 
 import base64
```

### Comparing `mov-cli-films-1.3.5/mov_cli_films/vidsrcto/ext/vidplay.py` & `mov-cli-films-1.3.6/mov_cli_films/vidsrcto/ext/vidplay.py`

 * *Files identical despite different names*

### Comparing `mov-cli-films-1.3.5/mov_cli_films/vidsrcto/scraper.py` & `mov-cli-films-1.3.6/mov_cli_films/vidsrcto/scraper.py`

 * *Files identical despite different names*

### Comparing `mov-cli-films-1.3.5/mov_cli_films.egg-info/PKG-INFO` & `mov-cli-films-1.3.6/mov_cli_films.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-films
-Version: 1.3.5
+Version: 1.3.6
 Summary: A mov-cli v4 plugin for watching Films and Shows.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-films-1.3.5/pyproject.toml` & `mov-cli-films-1.3.6/pyproject.toml`

 * *Files identical despite different names*

