# Comparing `tmp/characterai-1.0.2a1.tar.gz` & `tmp/characterai-1.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "characterai-1.0.2a1.tar", last modified: Wed Apr 10 08:03:16 2024, max compression
+gzip compressed data, was "characterai-1.0.4a1.tar", last modified: Wed Apr 10 08:18:30 2024, max compression
```

## Comparing `characterai-1.0.2a1.tar` & `characterai-1.0.4a1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.532425 characterai-1.0.2a1/
--rw-r--r--   0 runner    (1000) runner    (1000)     3700 2024-04-10 08:03:16.532425 characterai-1.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-04-10 06:52:36.000000 characterai-1.0.2a1/README.rst
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.368408 characterai-1.0.2a1/characterai/
--rw-------   0 runner    (1000) runner    (1000)      391 2024-04-07 22:04:22.000000 characterai-1.0.2a1/characterai/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.424414 characterai-1.0.2a1/characterai/aiocai/
--rw-------   0 runner    (1000) runner    (1000)      263 2024-04-07 21:51:49.000000 characterai-1.0.2a1/characterai/aiocai/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1655 2024-04-08 11:25:08.000000 characterai-1.0.2a1/characterai/aiocai/client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.432414 characterai-1.0.2a1/characterai/aiocai/methods/
--rw-------   0 runner    (1000) runner    (1000)      289 2024-04-02 08:55:21.000000 characterai-1.0.2a1/characterai/aiocai/methods/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6711 2024-04-08 13:44:06.000000 characterai-1.0.2a1/characterai/aiocai/methods/account.py
--rw-------   0 runner    (1000) runner    (1000)     9183 2024-04-09 07:45:55.000000 characterai-1.0.2a1/characterai/aiocai/methods/characters.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6658 2024-04-09 08:29:08.000000 characterai-1.0.2a1/characterai/aiocai/methods/chat1.py
--rw-------   0 runner    (1000) runner    (1000)    12061 2024-04-09 08:24:30.000000 characterai-1.0.2a1/characterai/aiocai/methods/chat2.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-09 08:01:54.000000 characterai-1.0.2a1/characterai/aiocai/methods/chats.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2376 2024-04-09 08:02:31.000000 characterai-1.0.2a1/characterai/aiocai/methods/other.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1430 2024-04-09 07:48:23.000000 characterai-1.0.2a1/characterai/aiocai/methods/recent.py
--rw-------   0 runner    (1000) runner    (1000)      815 2024-04-09 08:02:45.000000 characterai-1.0.2a1/characterai/aiocai/methods/users.py
--rw-------   0 runner    (1000) runner    (1000)     4029 2024-04-08 18:23:06.000000 characterai-1.0.2a1/characterai/aiocai/methods/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3561 2024-03-21 15:41:40.000000 characterai-1.0.2a1/characterai/auth.py
--rw-------   0 runner    (1000) runner    (1000)      194 2024-04-07 20:51:55.000000 characterai-1.0.2a1/characterai/errors.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.432414 characterai-1.0.2a1/characterai/pycai/
--rw-------   0 runner    (1000) runner    (1000)      243 2024-04-07 21:57:33.000000 characterai-1.0.2a1/characterai/pycai/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1462 2024-04-08 11:16:16.000000 characterai-1.0.2a1/characterai/pycai/client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.524424 characterai-1.0.2a1/characterai/pycai/methods/
--rw-------   0 runner    (1000) runner    (1000)      289 2024-04-07 21:54:03.000000 characterai-1.0.2a1/characterai/pycai/methods/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     6455 2024-04-09 20:25:28.000000 characterai-1.0.2a1/characterai/pycai/methods/account.py
--rw-------   0 runner    (1000) runner    (1000)     8601 2024-04-09 20:31:10.000000 characterai-1.0.2a1/characterai/pycai/methods/characters.py
--rw-------   0 runner    (1000) runner    (1000)     6460 2024-04-09 20:28:57.000000 characterai-1.0.2a1/characterai/pycai/methods/chat1.py
--rw-------   0 runner    (1000) runner    (1000)    11629 2024-04-09 20:30:23.000000 characterai-1.0.2a1/characterai/pycai/methods/chat2.py
--rw-------   0 runner    (1000) runner    (1000)     1581 2024-04-09 20:31:50.000000 characterai-1.0.2a1/characterai/pycai/methods/chats.py
--rw-------   0 runner    (1000) runner    (1000)     2328 2024-04-09 20:32:28.000000 characterai-1.0.2a1/characterai/pycai/methods/other.py
--rw-------   0 runner    (1000) runner    (1000)     1394 2024-04-09 20:32:51.000000 characterai-1.0.2a1/characterai/pycai/methods/recent.py
--rw-------   0 runner    (1000) runner    (1000)      803 2024-04-09 20:33:03.000000 characterai-1.0.2a1/characterai/pycai/methods/users.py
--rw-------   0 runner    (1000) runner    (1000)     3900 2024-04-07 22:04:41.000000 characterai-1.0.2a1/characterai/pycai/methods/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.528424 characterai-1.0.2a1/characterai/types/
--rw-------   0 runner    (1000) runner    (1000)        0 2024-03-15 10:35:14.000000 characterai-1.0.2a1/characterai/types/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6619 2024-04-09 19:40:37.000000 characterai-1.0.2a1/characterai/types/account.py
--rw-------   0 runner    (1000) runner    (1000)     8248 2024-04-09 20:23:40.000000 characterai-1.0.2a1/characterai/types/character.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11231 2024-04-09 20:17:22.000000 characterai-1.0.2a1/characterai/types/chat1.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4745 2024-04-09 20:00:46.000000 characterai-1.0.2a1/characterai/types/chat2.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4190 2024-04-09 19:55:40.000000 characterai-1.0.2a1/characterai/types/other.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2598 2024-04-09 19:51:12.000000 characterai-1.0.2a1/characterai/types/recent.py
--rw-------   0 runner    (1000) runner    (1000)     1302 2024-04-09 19:44:03.000000 characterai-1.0.2a1/characterai/types/user.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:03:16.528424 characterai-1.0.2a1/characterai.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3700 2024-04-10 08:03:16.000000 characterai-1.0.2a1/characterai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1349 2024-04-10 08:03:16.000000 characterai-1.0.2a1/characterai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 08:03:16.000000 characterai-1.0.2a1/characterai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       30 2024-04-10 08:03:16.000000 characterai-1.0.2a1/characterai.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 08:03:16.000000 characterai-1.0.2a1/characterai.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      644 2024-03-17 10:18:21.000000 characterai-1.0.2a1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-10 08:03:16.532425 characterai-1.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      876 2024-04-10 08:03:02.000000 characterai-1.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:30.045951 characterai-1.0.4a1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3700 2024-04-10 08:18:30.041951 characterai-1.0.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-04-10 08:17:58.000000 characterai-1.0.4a1/README.rst
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:29.973944 characterai-1.0.4a1/characterai/
+-rw-------   0 runner    (1000) runner    (1000)      391 2024-04-10 08:18:20.000000 characterai-1.0.4a1/characterai/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:30.025949 characterai-1.0.4a1/characterai/aiocai/
+-rw-------   0 runner    (1000) runner    (1000)      263 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1655 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:30.029950 characterai-1.0.4a1/characterai/aiocai/methods/
+-rw-------   0 runner    (1000) runner    (1000)      289 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6711 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/account.py
+-rw-------   0 runner    (1000) runner    (1000)     9183 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/characters.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6658 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/chat1.py
+-rw-------   0 runner    (1000) runner    (1000)    12061 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/chat2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/chats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2376 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/other.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1430 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/recent.py
+-rw-------   0 runner    (1000) runner    (1000)      815 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/users.py
+-rw-------   0 runner    (1000) runner    (1000)     4029 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/aiocai/methods/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3561 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/auth.py
+-rw-------   0 runner    (1000) runner    (1000)      194 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/errors.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:30.033950 characterai-1.0.4a1/characterai/pycai/
+-rw-------   0 runner    (1000) runner    (1000)      243 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1462 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:30.037950 characterai-1.0.4a1/characterai/pycai/methods/
+-rw-------   0 runner    (1000) runner    (1000)      289 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     6455 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/account.py
+-rw-------   0 runner    (1000) runner    (1000)     8601 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/characters.py
+-rw-------   0 runner    (1000) runner    (1000)     6460 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/chat1.py
+-rw-------   0 runner    (1000) runner    (1000)    11629 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/chat2.py
+-rw-------   0 runner    (1000) runner    (1000)     1581 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/chats.py
+-rw-------   0 runner    (1000) runner    (1000)     2328 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/other.py
+-rw-------   0 runner    (1000) runner    (1000)     1394 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/recent.py
+-rw-------   0 runner    (1000) runner    (1000)      803 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/users.py
+-rw-------   0 runner    (1000) runner    (1000)     3900 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/pycai/methods/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:30.041951 characterai-1.0.4a1/characterai/types/
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6619 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/account.py
+-rw-------   0 runner    (1000) runner    (1000)     8248 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/character.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11231 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/chat1.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4745 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/chat2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4190 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/other.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2598 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/recent.py
+-rw-------   0 runner    (1000) runner    (1000)     1302 2024-04-10 08:17:45.000000 characterai-1.0.4a1/characterai/types/user.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:18:30.041951 characterai-1.0.4a1/characterai.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3700 2024-04-10 08:18:29.000000 characterai-1.0.4a1/characterai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1334 2024-04-10 08:18:29.000000 characterai-1.0.4a1/characterai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 08:18:29.000000 characterai-1.0.4a1/characterai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       30 2024-04-10 08:18:29.000000 characterai-1.0.4a1/characterai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 08:18:29.000000 characterai-1.0.4a1/characterai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-10 08:18:30.045951 characterai-1.0.4a1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      876 2024-04-10 08:18:13.000000 characterai-1.0.4a1/setup.py
```

### Comparing `characterai-1.0.2a1/PKG-INFO` & `characterai-1.0.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 1.0.2a1
+Version: 1.0.4a1
 Summary: An unofficial API for Character AI for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: MIT
 Project-URL: Community, https://discord.gg/ZHJe3tXQkf
 Project-URL: Source, https://github.com/kramcat/characterai
 Project-URL: Documentation, https://docs.kram.cat
```

### Comparing `characterai-1.0.2a1/README.rst` & `characterai-1.0.4a1/README.rst`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/client.py` & `characterai-1.0.4a1/characterai/aiocai/client.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/account.py` & `characterai-1.0.4a1/characterai/aiocai/methods/account.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/characters.py` & `characterai-1.0.4a1/characterai/aiocai/methods/characters.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/chat1.py` & `characterai-1.0.4a1/characterai/aiocai/methods/chat1.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/chat2.py` & `characterai-1.0.4a1/characterai/aiocai/methods/chat2.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/chats.py` & `characterai-1.0.4a1/characterai/aiocai/methods/chats.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/other.py` & `characterai-1.0.4a1/characterai/aiocai/methods/other.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/recent.py` & `characterai-1.0.4a1/characterai/aiocai/methods/recent.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/users.py` & `characterai-1.0.4a1/characterai/aiocai/methods/users.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/aiocai/methods/utils.py` & `characterai-1.0.4a1/characterai/aiocai/methods/utils.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/auth.py` & `characterai-1.0.4a1/characterai/auth.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/client.py` & `characterai-1.0.4a1/characterai/pycai/client.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/account.py` & `characterai-1.0.4a1/characterai/pycai/methods/account.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/characters.py` & `characterai-1.0.4a1/characterai/pycai/methods/characters.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/chat1.py` & `characterai-1.0.4a1/characterai/pycai/methods/chat1.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/chat2.py` & `characterai-1.0.4a1/characterai/pycai/methods/chat2.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/chats.py` & `characterai-1.0.4a1/characterai/pycai/methods/chats.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/other.py` & `characterai-1.0.4a1/characterai/pycai/methods/other.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/recent.py` & `characterai-1.0.4a1/characterai/pycai/methods/recent.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/users.py` & `characterai-1.0.4a1/characterai/pycai/methods/users.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/pycai/methods/utils.py` & `characterai-1.0.4a1/characterai/pycai/methods/utils.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/types/account.py` & `characterai-1.0.4a1/characterai/types/account.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/types/character.py` & `characterai-1.0.4a1/characterai/types/character.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/types/chat1.py` & `characterai-1.0.4a1/characterai/types/chat1.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/types/chat2.py` & `characterai-1.0.4a1/characterai/types/chat2.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/types/other.py` & `characterai-1.0.4a1/characterai/types/other.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/types/recent.py` & `characterai-1.0.4a1/characterai/types/recent.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai/types/user.py` & `characterai-1.0.4a1/characterai/types/user.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.2a1/characterai.egg-info/PKG-INFO` & `characterai-1.0.4a1/characterai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 1.0.2a1
+Version: 1.0.4a1
 Summary: An unofficial API for Character AI for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: MIT
 Project-URL: Community, https://discord.gg/ZHJe3tXQkf
 Project-URL: Source, https://github.com/kramcat/characterai
 Project-URL: Documentation, https://docs.kram.cat
```

### Comparing `characterai-1.0.2a1/characterai.egg-info/SOURCES.txt` & `characterai-1.0.4a1/characterai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.rst
-pyproject.toml
 setup.py
 characterai/__init__.py
 characterai/auth.py
 characterai/errors.py
 characterai.egg-info/PKG-INFO
 characterai.egg-info/SOURCES.txt
 characterai.egg-info/dependency_links.txt
```

### Comparing `characterai-1.0.2a1/setup.py` & `characterai-1.0.4a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='characterai',
-    version='1.0.2-a1',
+    version='1.0.4-a1',
     description='An unofficial API for Character AI for Python',
     keywords='ai wrapper api library',
     long_description=readme,
     long_description_content_type='text/x-rst',
     url='https://github.com/kramcat/characterai',
     author='kramcat',
     license='MIT',
```

