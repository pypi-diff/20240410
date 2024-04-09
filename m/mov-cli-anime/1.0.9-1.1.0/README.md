# Comparing `tmp/mov-cli-anime-1.0.9.tar.gz` & `tmp/mov-cli-anime-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-anime-1.0.9.tar", last modified: Mon Apr  8 22:04:12 2024, max compression
+gzip compressed data, was "mov-cli-anime-1.1.0.tar", last modified: Tue Apr  9 23:45:55 2024, max compression
```

## Comparing `mov-cli-anime-1.0.9.tar` & `mov-cli-anime-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.857237 mov-cli-anime-1.0.9/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:26:30.000000 mov-cli-anime-1.0.9/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-04-08 22:01:37.000000 mov-cli-anime-1.0.9/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/mov_cli_anime/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      323 2024-04-08 22:03:38.000000 mov-cli-anime-1.0.9/mov_cli_anime/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/mov_cli_anime/anitaku/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 17:40:35.000000 mov-cli-anime-1.0.9/mov_cli_anime/anitaku/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5244 2024-04-08 22:02:12.000000 mov-cli-anime-1.0.9/mov_cli_anime/anitaku/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 22:04:12.853904 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      309 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-08 22:04:12.000000 mov-cli-anime-1.0.9/mov_cli_anime.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1324 2024-03-23 21:13:23.000000 mov-cli-anime-1.0.9/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-08 22:04:12.857237 mov-cli-anime-1.0.9/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:26:30.000000 mov-cli-anime-1.1.0/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-04-08 22:01:37.000000 mov-cli-anime-1.1.0/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.688726 mov-cli-anime-1.1.0/mov_cli_anime/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      402 2024-04-09 23:41:30.000000 mov-cli-anime-1.1.0/mov_cli_anime/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.688726 mov-cli-anime-1.1.0/mov_cli_anime/anitaku/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 17:40:35.000000 mov-cli-anime-1.1.0/mov_cli_anime/anitaku/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5232 2024-04-09 23:43:21.000000 mov-cli-anime-1.1.0/mov_cli_anime/anitaku/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      309 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1324 2024-03-23 21:13:23.000000 mov-cli-anime-1.1.0/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/setup.cfg
```

### Comparing `mov-cli-anime-1.0.9/LICENSE` & `mov-cli-anime-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-anime-1.0.9/PKG-INFO` & `mov-cli-anime-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-anime
-Version: 1.0.9
+Version: 1.1.0
 Summary: A mov-cli v4 plugin for watching anime.
 Author-email: Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-anime-1.0.9/README.md` & `mov-cli-anime-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mov-cli-anime-1.0.9/mov_cli_anime/anitaku/scraper.py` & `mov-cli-anime-1.1.0/mov_cli_anime/anitaku/scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,67 +2,65 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import List, Optional, Dict, Generator, Any
 
     from mov_cli import Config
     from mov_cli.http_client import HTTPClient
+    from mov_cli.scraper import ScraperOptionsT
 
 import re
 
 from mov_cli import utils
 from mov_cli.scraper import Scraper
-from mov_cli import Series, Movie, Metadata, MetadataType
+from mov_cli import Single, Multi, Metadata, MetadataType
 from mov_cli import ExtraMetadata
 
 __all__ = ("AnitakuScraper",)
 
 class AnitakuScraper(Scraper):
-    def __init__(self, config: Config, http_client: HTTPClient) -> None:
+    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         self.base_url = "https://anitaku.so"
-        super().__init__(config, http_client)
+        super().__init__(config, http_client, options)
 
     def search(self, query: str, limit: int = 20) -> List[Metadata]:
         query = query.replace(' ', '-')
         results = self.__results(query, limit)
         return results
 
-    def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] = None, **kwargs) -> Series | Movie:
-        if episode is None:
-            episode = utils.EpisodeSelector()
-
+    def scrape(self, metadata: Metadata, episode: utils.EpisodeSelector) -> Multi | Single:
         req = self.http_client.get(self.base_url + f"/{metadata.id}-episode-{episode.episode}", redirect = True)
         soup = self.soup(req)
 
         streamwish = soup.find("li", {"class": "streamwish"})
         dood = soup.find("li", {"class": "doodstream"})
 
         if streamwish:
             url = self.__streamwish(streamwish.find("a")["data-video"])
         elif dood:
             url = self.__dood(dood.find("a")["data-video"])
 
         if metadata.type == MetadataType.MOVIE:
-            return Movie(
+            return Single(
                 url,
                 title = metadata.title,
                 referrer = self.base_url,
                 year = metadata.year,
                 subtitles = None
             )
 
-        return Series(
+        return Multi(
             url,
             title = metadata.title,
             referrer = self.base_url,
             episode = episode,
             subtitles = None
         )
 
-    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[int, int]:
+    def scrape_episodes(self, metadata: Metadata) -> Dict[int, int]:
         page = self.http_client.get(f"{self.base_url}/category/{metadata.id}")
         _soup = self.soup(page)
 
         episode_page = _soup.find("ul", {"id": "episode_page"})
         li = episode_page.findAll("li")
         last = int(li[-1].find("a")["ep_end"])
         return {1: last} # TODO: Return multiple seasons.
```

### Comparing `mov-cli-anime-1.0.9/mov_cli_anime.egg-info/PKG-INFO` & `mov-cli-anime-1.1.0/mov_cli_anime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-anime
-Version: 1.0.9
+Version: 1.1.0
 Summary: A mov-cli v4 plugin for watching anime.
 Author-email: Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-anime-1.0.9/pyproject.toml` & `mov-cli-anime-1.1.0/pyproject.toml`

 * *Files identical despite different names*

