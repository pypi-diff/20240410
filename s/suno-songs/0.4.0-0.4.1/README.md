# Comparing `tmp/suno_songs-0.4.0.tar.gz` & `tmp/suno_songs-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suno_songs-0.4.0.tar", last modified: Fri Mar 29 13:14:45 2024, max compression
+gzip compressed data, was "suno_songs-0.4.1.tar", last modified: Wed Apr 10 02:51:26 2024, max compression
```

## Comparing `suno_songs-0.4.0.tar` & `suno_songs-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-03-29 13:14:45.687970 suno_songs-0.4.0/
--rw-r--r--   0 hyi        (502) staff       (20)    35149 2024-03-23 03:18:29.000000 suno_songs-0.4.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-03-29 13:14:45.686758 suno_songs-0.4.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     1580 2024-03-29 13:04:45.000000 suno_songs-0.4.0/README.md
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-03-29 13:14:45.688017 suno_songs-0.4.0/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1168 2024-03-29 13:13:30.000000 suno_songs-0.4.0/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-03-29 13:14:45.674954 suno_songs-0.4.0/suno/
--rw-r--r--   0 hyi        (502) staff       (20)       27 2024-03-23 03:43:01.000000 suno_songs-0.4.0/suno/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       62 2024-03-23 03:21:52.000000 suno_songs-0.4.0/suno/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)    11307 2024-03-29 13:13:15.000000 suno_songs-0.4.0/suno/suno.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-03-29 13:14:45.686258 suno_songs-0.4.0/suno_songs.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-03-29 13:14:45.000000 suno_songs-0.4.0/suno_songs.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      279 2024-03-29 13:14:45.000000 suno_songs-0.4.0/suno_songs.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-03-29 13:14:45.000000 suno_songs-0.4.0/suno_songs.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       40 2024-03-29 13:14:45.000000 suno_songs-0.4.0/suno_songs.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)       53 2024-03-29 13:14:45.000000 suno_songs-0.4.0/suno_songs.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        5 2024-03-29 13:14:45.000000 suno_songs-0.4.0/suno_songs.egg-info/top_level.txt
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 02:51:26.359289 suno_songs-0.4.1/
+-rw-r--r--   0 hyi        (502) staff       (20)    35149 2024-03-23 03:18:29.000000 suno_songs-0.4.1/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-04-10 02:51:26.358612 suno_songs-0.4.1/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     1580 2024-03-29 13:04:45.000000 suno_songs-0.4.1/README.md
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-10 02:51:26.359341 suno_songs-0.4.1/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1168 2024-04-10 02:51:19.000000 suno_songs-0.4.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 02:51:26.354919 suno_songs-0.4.1/suno/
+-rw-r--r--   0 hyi        (502) staff       (20)       27 2024-03-23 03:43:01.000000 suno_songs-0.4.1/suno/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       62 2024-03-23 03:21:52.000000 suno_songs-0.4.1/suno/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11346 2024-04-10 02:51:12.000000 suno_songs-0.4.1/suno/suno.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-10 02:51:26.357885 suno_songs-0.4.1/suno_songs.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)     2465 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      279 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       40 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       53 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        5 2024-04-10 02:51:26.000000 suno_songs-0.4.1/suno_songs.egg-info/top_level.txt
```

### Comparing `suno_songs-0.4.0/LICENSE` & `suno_songs-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `suno_songs-0.4.0/PKG-INFO` & `suno_songs-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suno_songs
-Version: 0.4.0
+Version: 0.4.1
 Summary: High quality songs generation by suno.ai. Reverse engineered API.
 Home-page: https://github.com/yihong0618/SunoSongsCreator
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 Project-URL: Bug Report, https://github.com/yihong0618/SunoSongsCreator/issues/new
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `suno_songs-0.4.0/README.md` & `suno_songs-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `suno_songs-0.4.0/setup.py` & `suno_songs-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="suno_songs",
-    version="0.4.0",
+    version="0.4.1",
     author="yihong0618",
     author_email="zouzou0208@gmail.com",
     description="High quality songs generation by suno.ai. Reverse engineered API.",
     url="https://github.com/yihong0618/SunoSongsCreator",
     project_urls={
         "Bug Report": "https://github.com/yihong0618/SunoSongsCreator/issues/new",
     },
```

### Comparing `suno_songs-0.4.0/suno/suno.py` & `suno_songs-0.4.1/suno/suno.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 from dotenv import load_dotenv, find_dotenv
 
 _ = load_dotenv(find_dotenv())
 
 ua = UserAgent(browsers=["edge"])
 
-get_session_url = "https://clerk.suno.ai/v1/client?_clerk_js_version=4.70.5"
-exchange_token_url = (
-    "https://clerk.suno.ai/v1/client/sessions/{sid}/tokens/api?_clerk_js_version=4.70.0"
+get_session_url = (
+    "https://clerk.suno.com/v1/client/?_clerk_js_version=4.72.0-snapshot.vc141245"
 )
+exchange_token_url = "https://clerk.suno.com/v1/client/sessions/{sid}/tokens/api?_clerk_js_version=4.72.0-snapshot.vc141245"
 
 base_url = "https://studio-api.suno.ai"
 browser_version = "edge101"
 
 HEADERS = {
     "Accept-Encoding": "gzip, deflate, br",
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) \
```

### Comparing `suno_songs-0.4.0/suno_songs.egg-info/PKG-INFO` & `suno_songs-0.4.1/suno_songs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suno_songs
-Version: 0.4.0
+Version: 0.4.1
 Summary: High quality songs generation by suno.ai. Reverse engineered API.
 Home-page: https://github.com/yihong0618/SunoSongsCreator
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 Project-URL: Bug Report, https://github.com/yihong0618/SunoSongsCreator/issues/new
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

