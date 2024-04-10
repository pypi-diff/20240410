# Comparing `tmp/suno_songs-0.4.1.tar.gz` & `tmp/suno_songs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suno_songs-0.4.1.tar", last modified: Wed Apr 10 02:51:26 2024, max compression
+gzip compressed data, was "suno_songs-0.5.0.tar", last modified: Wed Apr 10 13:18:52 2024, max compression
```

## Comparing `suno_songs-0.4.1.tar` & `suno_songs-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 02:51:26.359289 suno_songs-0.4.1/
--rw-r--r--   0 hyi        (502) staff       (20)    35149 2024-03-23 03:18:29.000000 suno_songs-0.4.1/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-04-10 02:51:26.358612 suno_songs-0.4.1/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     1580 2024-03-29 13:04:45.000000 suno_songs-0.4.1/README.md
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-10 02:51:26.359341 suno_songs-0.4.1/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1168 2024-04-10 02:51:19.000000 suno_songs-0.4.1/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 02:51:26.354919 suno_songs-0.4.1/suno/
--rw-r--r--   0 hyi        (502) staff       (20)       27 2024-03-23 03:43:01.000000 suno_songs-0.4.1/suno/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       62 2024-03-23 03:21:52.000000 suno_songs-0.4.1/suno/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)    11346 2024-04-10 02:51:12.000000 suno_songs-0.4.1/suno/suno.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 02:51:26.357885 suno_songs-0.4.1/suno_songs.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      279 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       40 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)       53 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        5 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/top_level.txt
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 13:18:52.172396 suno_songs-0.5.0/
+-rw-r--r--   0 hyi        (502) staff       (20)    35149 2024-03-23 03:18:29.000000 suno_songs-0.5.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-04-10 13:18:52.170109 suno_songs-0.5.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     1580 2024-03-29 13:04:45.000000 suno_songs-0.5.0/README.md
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-10 13:18:52.172639 suno_songs-0.5.0/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1168 2024-04-10 13:18:40.000000 suno_songs-0.5.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 13:18:52.162567 suno_songs-0.5.0/suno/
+-rw-r--r--   0 hyi        (502) staff       (20)       27 2024-03-23 03:43:01.000000 suno_songs-0.5.0/suno/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       62 2024-03-23 03:21:52.000000 suno_songs-0.5.0/suno/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11811 2024-04-10 13:13:57.000000 suno_songs-0.5.0/suno/suno.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 13:18:52.168567 suno_songs-0.5.0/suno_songs.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-04-10 13:18:52.000000 suno_songs-0.5.0/suno_songs.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      279 2024-04-10 13:18:52.000000 suno_songs-0.5.0/suno_songs.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-10 13:18:52.000000 suno_songs-0.5.0/suno_songs.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       40 2024-04-10 13:18:52.000000 suno_songs-0.5.0/suno_songs.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       53 2024-04-10 13:18:52.000000 suno_songs-0.5.0/suno_songs.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        5 2024-04-10 13:18:52.000000 suno_songs-0.5.0/suno_songs.egg-info/top_level.txt
```

### Comparing `suno_songs-0.4.1/LICENSE` & `suno_songs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suno_songs-0.4.1/PKG-INFO` & `suno_songs-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suno_songs
-Version: 0.4.1
+Version: 0.5.0
 Summary: High quality songs generation by suno.ai. Reverse engineered API.
 Home-page: https://github.com/yihong0618/SunoSongsCreator
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 Project-URL: Bug Report, https://github.com/yihong0618/SunoSongsCreator/issues/new
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `suno_songs-0.4.1/README.md` & `suno_songs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `suno_songs-0.4.1/setup.py` & `suno_songs-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="suno_songs",
-    version="0.4.1",
+    version="0.5.0",
     author="yihong0618",
     author_email="zouzou0208@gmail.com",
     description="High quality songs generation by suno.ai. Reverse engineered API.",
     url="https://github.com/yihong0618/SunoSongsCreator",
     project_urls={
         "Bug Report": "https://github.com/yihong0618/SunoSongsCreator/issues/new",
     },
```

### Comparing `suno_songs-0.4.1/suno/suno.py` & `suno_songs-0.5.0/suno/suno.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,14 +138,15 @@
             not mt
         ):  # Remove checking for title because custom songs have no title if not specified
             return "", ""
         lyrics = re.sub(r"\[.*?\]", "", mt.get("prompt"))
         return song_name, lyrics
 
     def _fetch_songs_metadata(self, ids):
+        self.song_info_dict["song_url_list"] = []
         id1, id2 = ids[:2]
         url = f"https://studio-api.suno.ai/api/feed/?ids={id1}%2C{id2}"
         response = self.session.get(url, impersonate=browser_version)
         data = response.json()
         if type(data) == dict:
             if data.get("detail", "") == "Unauthorized":
                 song_name, lyric = self._parse_lyrics(self.now_data[0])
@@ -159,33 +160,36 @@
                 # Done here
                 return True
             else:
                 data = [data]
         # renew now data
         self.now_data = data
         try:
-            for d in data:
-                # only get one url for now TODO: See if possible for both urls
-                # and early return
-                if audio_url := d.get("audio_url"):
+            if all(d.get("audio_url") for d in data):
+                for d in data:
                     song_name, lyric = self._parse_lyrics(d)
                     self.song_info_dict["song_name"] = song_name
                     self.song_info_dict["lyric"] = lyric
-                    self.song_info_dict["song_url"] = audio_url
-                    return True
-            return False
+                    self.song_info_dict["song_url_list"].append(d.get("audio_url"))
+                    # for support old api
+                    self.song_info_dict["song_url"] = d.get("audio_url")
+                return True
         except Exception as e:
             print(e)
             # since we only get the music_id is ok
             # so we can make the id here and sleep some time
             print("Will sleep 30s and get the music url")
             time.sleep(30)
             song_name, lyric = self._parse_lyrics(self.now_data[0])
             self.song_info_dict["song_name"] = song_name
             self.song_info_dict["lyric"] = lyric
+            self.song_info_dict["song_url_list"] = [
+                f"https://audiopipe.suno.ai/?item_id={id1}",
+                f"https://audiopipe.suno.ai/?item_id={id2}",
+            ]
             self.song_info_dict["song_url"] = (
                 f"https://audiopipe.suno.ai/?item_id={id1}"
             )
             # Done here
             return True
 
     def get_songs(
@@ -243,63 +247,67 @@
             if not song_info:
                 print(".", end="", flush=True)
             else:
                 break
         # keep the song info dict as old api
         return self.song_info_dict
 
+    def _download_suno_song(self, link: str, song_id: str, output_dir: str) -> None:
+        song_name = self.song_info_dict["song_name"]
+        lyric = self.song_info_dict["lyric"]
+        response = rget(link, allow_redirects=False, stream=True)
+        if response.status_code != 200:
+            raise Exception("Could not download song")
+        # save response to file
+        print(f"Downloading song... {song_id}")
+        with open(os.path.join(output_dir, f"suno_{song_id}.mp3"), "wb") as output_file:
+            for chunk in response.iter_content(chunk_size=1024):
+                # If the chunk is not empty, write it to the file.
+                if chunk:
+                    output_file.write(chunk)
+        if not song_name:
+            song_name = "Untitled"
+        with open(
+            os.path.join(output_dir, f"{song_name.replace(' ', '_')}.lrc"),
+            "w",
+            encoding="utf-8",
+        ) as lyric_file:
+            lyric_file.write(f"{song_name}\n\n{lyric}")
+
     def save_songs(
         self,
         prompt: str,
         output_dir: str = "./output",
         tags: Union[str, None] = None,
         title: Union[str, None] = None,
         make_instrumental: bool = False,
         is_custom: bool = False,
     ) -> None:
-        mp3_index = 0
         try:
             self.get_songs(
                 prompt,
                 tags=tags,
                 title=title,
                 is_custom=is_custom,
                 make_instrumental=make_instrumental,
             )  # make the info dict
-            song_name = self.song_info_dict["song_name"]
-            lyric = self.song_info_dict["lyric"]
-            link = self.song_info_dict["song_url"]
+            link_list = self.song_info_dict["song_url_list"]
         except Exception as e:
             print(e)
             raise
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
         print()
-        while os.path.exists(os.path.join(output_dir, f"suno_{mp3_index}.mp3")):
-            mp3_index += 1
-        print(link)
-        response = rget(link, allow_redirects=False, stream=True)
-        if response.status_code != 200:
-            raise Exception("Could not download song")
-        # save response to file
-        with open(
-            os.path.join(output_dir, f"suno_{mp3_index + 1}.mp3"), "wb"
-        ) as output_file:
-            for chunk in response.iter_content(chunk_size=1024):
-                # If the chunk is not empty, write it to the file.
-                if chunk:
-                    output_file.write(chunk)
-        if not song_name:
-            song_name = "Untitled"
-        with open(
-            os.path.join(output_dir, f"{song_name.replace(' ', '_')}.lrc"),
-            "w",
-            encoding="utf-8",
-        ) as lyric_file:
-            lyric_file.write(f"{song_name}\n\n{lyric}")
+        print(link_list)
+        for link in link_list:
+            if link.endswith(".mp3"):
+                mp3_id = link.split("/")[-1][:-4]
+            else:
+                mp3_id = link.split("=")[-1]
+            self._download_suno_song(link, mp3_id, output_dir)
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-U", help="Auth cookie from browser", type=str, default="")
     parser.add_argument(
         "--prompt",
```

### Comparing `suno_songs-0.4.1/suno_songs.egg-info/PKG-INFO` & `suno_songs-0.5.0/suno_songs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suno_songs
-Version: 0.4.1
+Version: 0.5.0
 Summary: High quality songs generation by suno.ai. Reverse engineered API.
 Home-page: https://github.com/yihong0618/SunoSongsCreator
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 Project-URL: Bug Report, https://github.com/yihong0618/SunoSongsCreator/issues/new
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

