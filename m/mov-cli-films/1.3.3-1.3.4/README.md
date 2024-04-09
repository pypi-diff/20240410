# Comparing `tmp/mov-cli-films-1.3.3.tar.gz` & `tmp/mov-cli-films-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-films-1.3.3.tar", last modified: Wed Apr  3 18:26:32 2024, max compression
+gzip compressed data, was "mov-cli-films-1.3.4.tar", last modified: Tue Apr  9 02:09:56 2024, max compression
```

## Comparing `mov-cli-films-1.3.3.tar` & `mov-cli-films-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.271755 mov-cli-films-1.3.3/
--rw-rw-rw-   0        0        0     1085 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/LICENSE
--rw-rw-rw-   0        0        0     3004 2024-04-03 18:26:32.269758 mov-cli-films-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      607 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.226746 mov-cli-films-1.3.3/mov_cli_films/
--rw-rw-rw-   0        0        0      406 2024-04-03 17:37:24.000000 mov-cli-films-1.3.3/mov_cli_films/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.249749 mov-cli-films-1.3.3/mov_cli_films/vidsrcme/
--rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcme/__init__.py
--rw-rw-rw-   0        0        0     3307 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcme/scraper.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.263752 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/
--rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.266754 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/
--rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/__init__.py
--rw-rw-rw-   0        0        0     4140 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/vidplay.py
--rw-rw-rw-   0        0        0     4531 2024-04-03 18:25:52.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/scraper.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.268756 mov-cli-films-1.3.3/mov_cli_films.egg-info/
--rw-rw-rw-   0        0        0     3004 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1378 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 18:26:32.271755 mov-cli-films-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 02:09:56.072482 mov-cli-films-1.3.4/
+-rw-rw-rw-   0        0        0     1085 2024-04-03 14:45:08.000000 mov-cli-films-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0     2996 2024-04-09 02:09:56.071485 mov-cli-films-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2024-04-08 22:16:54.000000 mov-cli-films-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 02:09:56.038574 mov-cli-films-1.3.4/mov_cli_films/
+-rw-rw-rw-   0        0        0      527 2024-04-09 02:08:32.000000 mov-cli-films-1.3.4/mov_cli_films/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:09:56.065501 mov-cli-films-1.3.4/mov_cli_films/vidsrcme/
+-rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.4/mov_cli_films/vidsrcme/__init__.py
+-rw-rw-rw-   0        0        0     4446 2024-04-09 02:08:13.000000 mov-cli-films-1.3.4/mov_cli_films/vidsrcme/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:09:56.067496 mov-cli-films-1.3.4/mov_cli_films/vidsrcto/
+-rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.4/mov_cli_films/vidsrcto/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:09:56.069491 mov-cli-films-1.3.4/mov_cli_films/vidsrcto/ext/
+-rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.4/mov_cli_films/vidsrcto/ext/__init__.py
+-rw-rw-rw-   0        0        0     4140 2024-04-03 14:45:08.000000 mov-cli-films-1.3.4/mov_cli_films/vidsrcto/ext/vidplay.py
+-rw-rw-rw-   0        0        0     4531 2024-04-03 18:25:52.000000 mov-cli-films-1.3.4/mov_cli_films/vidsrcto/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:09:56.070488 mov-cli-films-1.3.4/mov_cli_films.egg-info/
+-rw-rw-rw-   0        0        0     2996 2024-04-09 02:09:56.000000 mov-cli-films-1.3.4/mov_cli_films.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-04-09 02:09:56.000000 mov-cli-films-1.3.4/mov_cli_films.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 02:09:56.000000 mov-cli-films-1.3.4/mov_cli_films.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-09 02:09:56.000000 mov-cli-films-1.3.4/mov_cli_films.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 02:09:56.000000 mov-cli-films-1.3.4/mov_cli_films.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1376 2024-04-03 18:27:12.000000 mov-cli-films-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 02:09:56.072482 mov-cli-films-1.3.4/setup.cfg
```

### Comparing `mov-cli-films-1.3.3/LICENSE` & `mov-cli-films-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-films-1.3.3/PKG-INFO` & `mov-cli-films-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-films
-Version: 1.3.3
+Version: 1.3.4
 Summary: A mov-cli v4 plugin for watching Films and Shows.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-films
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-films/issues
+Project-URL: GitHub, https://github.com/JDALab/mov-cli-films
+Project-URL: BugTracker, https://github.com/JDALab/mov-cli-films/issues
 Keywords: amazing mov-cli plugin
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -52,16 +52,16 @@
   # mov-cli-films 
   <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
 
 </div>
 
-> [!Warning]
-> WIP and written at 3 am 💀
+> [!NOTE]
+> Searching for maintainers
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-films
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mov-cli-films-1.3.3/README.md` & `mov-cli-films-1.3.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,16 @@
   # mov-cli-films 
   <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
 
 </div>
 
-> [!Warning]
-> WIP and written at 3 am 💀
+> [!NOTE]
+> Searching for maintainers
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-films
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mov-cli-films-1.3.3/mov_cli_films/vidsrcme/scraper.py` & `mov-cli-films-1.3.4/mov_cli_films/vidsrcme/scraper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,133 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Dict, Iterable
 
 if TYPE_CHECKING:
     from typing import Dict, Literal, Optional
 
     from mov_cli import Config
+    from httpx import Response
     from mov_cli.http_client import HTTPClient
 
 import re
 
 from mov_cli import utils
 from mov_cli.scraper import Scraper
-from mov_cli import Series, Movie, Metadata, MetadataType
+from mov_cli import Multi, Single, Metadata, MetadataType
 from mov_cli.utils.scraper import TheMovieDB
+from mov_cli.utils import EpisodeSelector
+
 import base64
 
 
 __all__ = ("VidSrcMeScraper",)
 
 class VidSrcMeScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient) -> None:
         self.base_url = "https://vidsrc.net"
         self.tmdb = TheMovieDB(http_client)
+
+        self.MAX_TRIES = 10
         super().__init__(config, http_client)
 
     def search(self, query: str, limit: int = 10) -> Iterable[Metadata]:
-        return self.tmdb.search(query, limit)
+        for search_result in self.tmdb.search(query, limit):
+            embed_response = self.__get_embed(search_result, EpisodeSelector())
+
+            if embed_response.status_code == 404: # don't include media that isn't available on the provider.
+                continue
+
+            yield search_result
 
     def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
         return self.tmdb.scrape_episodes(metadata)
 
     def __deobfstr(self, hash, index):
         result = ""
         for i in range(0, len(hash), 2):
             j = hash[i:i+2]
             result += chr(int(j, 16) ^ ord(index[i // 2 % len(index)]))
         return result
 
-    def __extraction(self, script):
-        file_section = re.findall(r"file:\"#9(.*?)\"", script)[0]
+    def __get_url(self, prourl: str):
+        url = None
+        
+        for _ in range(self.MAX_TRIES):
+            prorcp = self.http_client.get(prourl, headers={"Referer": "https://vidsrc.stream/"})
+
+            if prorcp.status_code == 503:
+                continue
+            
+            hls_url = re.search(r'file:"([^"]*)"', prorcp.text).group(1)
+            hls_url = re.sub(r'\/\/\S+?=', '', hls_url)[2:]     
+            hls_url = re.sub(r"\/@#@\/[^=\/]+==", "", hls_url)
+
+            hls_url = hls_url.replace('_', '/').replace('-', '+')
+
+            try:
+                hls_url = bytearray(base64.b64decode(hls_url))
+                hls_url = hls_url.decode('utf-8')
+            except UnicodeDecodeError:
+                hls_url = None
 
-        based64 = re.sub('/@#@\\S+?=?=', '', file_section)
+            if hls_url is not None:
+                url = hls_url
+                break
 
-        decoded_video = base64.b64decode(based64)
+        return url
 
-        return decoded_video.decode()
+    def __get_embed(self, metadata: Metadata, episode: EpisodeSelector) -> Response:
+        media_type = "tv" if metadata.type == MetadataType.SERIES else "movie"
 
-    def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] | None = None) -> Series | Movie:
-        if episode is None:
-            episode = utils.EpisodeSelector()
+        url = f"{self.base_url}/embed/{media_type}/{metadata.id}"
 
-        type = "movie" if metadata.type == MetadataType.MOVIE else "tv"
+        if metadata.type == MetadataType.SERIES:
+            url += f"/{episode.season}/{episode.episode}"
 
-        url_const = f"{self.base_url}/embed/{type}/{metadata.id}"
+        return self.http_client.get(url)
 
-        if metadata.type == MetadataType.SERIES:
-            url_const += f"/{episode.season}-{episode.episode}" 
+    def scrape(self, metadata: Metadata, episode: Optional[EpisodeSelector] | None = None) -> Multi | Single:        
+        for _ in range(self.MAX_TRIES):
+            vidsrc = self.__get_embed(metadata, EpisodeSelector())
 
-        vidsrc = self.http_client.get(url_const)
+            if vidsrc.status_code != 503:
+                break
+
+        print(self.soup(vidsrc).prettify())
 
         iframeurl = "https:" + self.soup(vidsrc).select("iframe#player_iframe")[0]["src"]
 
-        doc = self.http_client.get(iframeurl, headers={"Referer": vidsrc})
+        for _ in range(self.MAX_TRIES):
+            doc = self.http_client.get(iframeurl, headers={"Referer": vidsrc})
+
+            if doc.status_code != 503:
+                break
 
         doc = self.soup(doc)
 
         index = doc.select("body")[0]["data-i"]
         hash = doc.select("div#hidden")[0]["data-h"]
 
         srcrcp = "https:" + self.__deobfstr(hash, index).replace("vidsrc.stream", "vidsrc.net")
 
-        prourl = self.http_client.get(srcrcp, headers={"Referer": "https://vidsrc.stream/"}).headers["Location"]
-
-        prorcp = self.http_client.get(prourl, headers={"Referer": "https://vidsrc.stream/"})
-
-        prorcp = self.soup(prorcp)
-
-        scripts = prorcp.findAll("script")
+        for _ in range(self.MAX_TRIES):
+            prourl = self.http_client.get(srcrcp, headers={"Referer": "https://vidsrc.stream/"}).headers.get("Location", None)
 
-        for script in scripts:
-            if "Playerjs" in script.text:
-                player = script.text
+            if prourl is not None:
                 break
 
-        url = self.__extraction(player)
+        url = self.__get_url(prourl)
 
         if metadata.type == MetadataType.MOVIE:
-            return Movie(
+            return Single(
                 url = url,
                 title = metadata.title,
                 referrer = "https://vidsrc.stream/",
                 year = metadata.year
             )
 
-        return Series(
+        return Multi(
             url = url,
             title = metadata.title,
             referrer = "https://vidsrc.stream/",
             episode = episode
         )
```

### Comparing `mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/vidplay.py` & `mov-cli-films-1.3.4/mov_cli_films/vidsrcto/ext/vidplay.py`

 * *Files identical despite different names*

### Comparing `mov-cli-films-1.3.3/mov_cli_films/vidsrcto/scraper.py` & `mov-cli-films-1.3.4/mov_cli_films/vidsrcto/scraper.py`

 * *Files identical despite different names*

### Comparing `mov-cli-films-1.3.3/mov_cli_films.egg-info/PKG-INFO` & `mov-cli-films-1.3.4/mov_cli_films.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-films
-Version: 1.3.3
+Version: 1.3.4
 Summary: A mov-cli v4 plugin for watching Films and Shows.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-films
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-films/issues
+Project-URL: GitHub, https://github.com/JDALab/mov-cli-films
+Project-URL: BugTracker, https://github.com/JDALab/mov-cli-films/issues
 Keywords: amazing mov-cli plugin
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -52,16 +52,16 @@
   # mov-cli-films 
   <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
 
 </div>
 
-> [!Warning]
-> WIP and written at 3 am 💀
+> [!NOTE]
+> Searching for maintainers
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-films
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mov-cli-films-1.3.3/pyproject.toml` & `mov-cli-films-1.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 [project.optional-dependencies]
 dev = [
     "ruff",
     "build"
 ]
 
 [project.urls]
-GitHub = "https://github.com/mov-cli/mov-cli-films"
-BugTracker = "https://github.com/mov-cli/mov-cli-films/issues"
+GitHub = "https://github.com/JDALab/mov-cli-films"
+BugTracker = "https://github.com/JDALab/mov-cli-films/issues"
 
 [tool.setuptools.dynamic]
 version = { attr = "mov_cli_films.__version__" }
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

