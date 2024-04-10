# Comparing `tmp/characterai-1.0.0.tar.gz` & `tmp/characterai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "characterai-1.0.0.tar", last modified: Wed Apr 10 08:32:59 2024, max compression
+gzip compressed data, was "characterai-1.0.1.tar", last modified: Wed Apr 10 08:43:44 2024, max compression
```

## Comparing `characterai-1.0.0.tar` & `characterai-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.814230 characterai-1.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     3698 2024-04-10 08:32:59.814230 characterai-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-04-10 08:17:58.000000 characterai-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.346184 characterai-1.0.0/characterai/
--rw-------   0 runner    (1000) runner    (1000)      391 2024-04-10 08:18:20.000000 characterai-1.0.0/characterai/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.414190 characterai-1.0.0/characterai/aiocai/
--rw-------   0 runner    (1000) runner    (1000)      263 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1655 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.522201 characterai-1.0.0/characterai/aiocai/methods/
--rw-------   0 runner    (1000) runner    (1000)      289 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6864 2024-04-10 08:29:27.000000 characterai-1.0.0/characterai/aiocai/methods/account.py
--rw-------   0 runner    (1000) runner    (1000)     9183 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/characters.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6658 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/chat1.py
--rw-------   0 runner    (1000) runner    (1000)    12061 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/chat2.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/chats.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2376 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/other.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1430 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/recent.py
--rw-------   0 runner    (1000) runner    (1000)      815 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/users.py
--rw-------   0 runner    (1000) runner    (1000)     4029 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/aiocai/methods/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3561 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/auth.py
--rw-------   0 runner    (1000) runner    (1000)      194 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/errors.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.526201 characterai-1.0.0/characterai/pycai/
--rw-------   0 runner    (1000) runner    (1000)      243 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1462 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.626211 characterai-1.0.0/characterai/pycai/methods/
--rw-------   0 runner    (1000) runner    (1000)      289 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     6608 2024-04-10 08:29:37.000000 characterai-1.0.0/characterai/pycai/methods/account.py
--rw-------   0 runner    (1000) runner    (1000)     8601 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/characters.py
--rw-------   0 runner    (1000) runner    (1000)     6460 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/chat1.py
--rw-------   0 runner    (1000) runner    (1000)    11629 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/chat2.py
--rw-------   0 runner    (1000) runner    (1000)     1581 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/chats.py
--rw-------   0 runner    (1000) runner    (1000)     2328 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/other.py
--rw-------   0 runner    (1000) runner    (1000)     1394 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/recent.py
--rw-------   0 runner    (1000) runner    (1000)      803 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/users.py
--rw-------   0 runner    (1000) runner    (1000)     3900 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/pycai/methods/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.734222 characterai-1.0.0/characterai/types/
--rw-------   0 runner    (1000) runner    (1000)        0 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/types/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6909 2024-04-10 08:29:07.000000 characterai-1.0.0/characterai/types/account.py
--rw-------   0 runner    (1000) runner    (1000)     8248 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/types/character.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11231 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/types/chat1.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4745 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/types/chat2.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4190 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/types/other.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2598 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/types/recent.py
--rw-------   0 runner    (1000) runner    (1000)     1302 2024-04-10 08:17:45.000000 characterai-1.0.0/characterai/types/user.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:32:59.734222 characterai-1.0.0/characterai.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3698 2024-04-10 08:32:58.000000 characterai-1.0.0/characterai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1334 2024-04-10 08:32:58.000000 characterai-1.0.0/characterai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 08:32:58.000000 characterai-1.0.0/characterai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       30 2024-04-10 08:32:58.000000 characterai-1.0.0/characterai.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 08:32:58.000000 characterai-1.0.0/characterai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-10 08:32:59.814230 characterai-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      873 2024-04-10 08:30:18.000000 characterai-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.821424 characterai-1.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3602 2024-04-10 08:43:44.821424 characterai-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3000 2024-04-10 08:42:38.000000 characterai-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.745416 characterai-1.0.1/characterai/
+-rw-------   0 runner    (1000) runner    (1000)      391 2024-04-10 08:18:20.000000 characterai-1.0.1/characterai/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.749417 characterai-1.0.1/characterai/aiocai/
+-rw-------   0 runner    (1000) runner    (1000)      263 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1655 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.813423 characterai-1.0.1/characterai/aiocai/methods/
+-rw-------   0 runner    (1000) runner    (1000)      289 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6864 2024-04-10 08:29:27.000000 characterai-1.0.1/characterai/aiocai/methods/account.py
+-rw-------   0 runner    (1000) runner    (1000)     9183 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/characters.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6658 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/chat1.py
+-rw-------   0 runner    (1000) runner    (1000)    12061 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/chat2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/chats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2376 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/other.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1430 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/recent.py
+-rw-------   0 runner    (1000) runner    (1000)      815 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/users.py
+-rw-------   0 runner    (1000) runner    (1000)     4029 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/aiocai/methods/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3561 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/auth.py
+-rw-------   0 runner    (1000) runner    (1000)      194 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/errors.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.813423 characterai-1.0.1/characterai/pycai/
+-rw-------   0 runner    (1000) runner    (1000)      243 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1462 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.817423 characterai-1.0.1/characterai/pycai/methods/
+-rw-------   0 runner    (1000) runner    (1000)      289 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     6608 2024-04-10 08:29:37.000000 characterai-1.0.1/characterai/pycai/methods/account.py
+-rw-------   0 runner    (1000) runner    (1000)     8601 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/characters.py
+-rw-------   0 runner    (1000) runner    (1000)     6460 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/chat1.py
+-rw-------   0 runner    (1000) runner    (1000)    11629 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/chat2.py
+-rw-------   0 runner    (1000) runner    (1000)     1581 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/chats.py
+-rw-------   0 runner    (1000) runner    (1000)     2328 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/other.py
+-rw-------   0 runner    (1000) runner    (1000)     1394 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/recent.py
+-rw-------   0 runner    (1000) runner    (1000)      803 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/users.py
+-rw-------   0 runner    (1000) runner    (1000)     3900 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/pycai/methods/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.821424 characterai-1.0.1/characterai/types/
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6909 2024-04-10 08:29:07.000000 characterai-1.0.1/characterai/types/account.py
+-rw-------   0 runner    (1000) runner    (1000)     8248 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/types/character.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11231 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/types/chat1.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4745 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/types/chat2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4190 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/types/other.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2598 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/types/recent.py
+-rw-------   0 runner    (1000) runner    (1000)     1302 2024-04-10 08:17:45.000000 characterai-1.0.1/characterai/types/user.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 08:43:44.821424 characterai-1.0.1/characterai.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3602 2024-04-10 08:43:44.000000 characterai-1.0.1/characterai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1334 2024-04-10 08:43:44.000000 characterai-1.0.1/characterai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 08:43:44.000000 characterai-1.0.1/characterai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       30 2024-04-10 08:43:44.000000 characterai-1.0.1/characterai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 08:43:44.000000 characterai-1.0.1/characterai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-10 08:43:44.909432 characterai-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      873 2024-04-10 08:43:39.000000 characterai-1.0.1/setup.py
```

### Comparing `characterai-1.0.0/PKG-INFO` & `characterai-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unofficial API for Character AI for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: MIT
 Project-URL: Community, https://discord.gg/ZHJe3tXQkf
 Project-URL: Source, https://github.com/kramcat/characterai
 Project-URL: Documentation, https://docs.kram.cat
@@ -37,22 +37,14 @@
 .. |tag4| image:: https://img.shields.io/discord/1120066151515422772?style=flat-square
     :target: https://discord.com/invite/ZHJe3tXQkf
     :alt: Stars
 
 
 Welcome to the documentation for a synchronous/asynchronous unofficial library for CharacterAI using `curl_cffi <https://github.com/yifeikong/curl_cffi>`_
 
-
-💻 Installation
----------------
-
-.. code-block:: bash
-
-    pip install characterai==1.0.0a1
-
 ⚠️ Warning
 ==========
 
 This version of the library is in alpha version, there may be bugs and errors. The library was developed without the participation of Character AI developers or their knowledge. To work with the library you need to know how to work with `asyncio <https://docs.python.org/3/library/asyncio.html>`_
 
 
 🔥 Features
```

### Comparing `characterai-1.0.0/README.rst` & `characterai-1.0.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,14 @@
 .. |tag4| image:: https://img.shields.io/discord/1120066151515422772?style=flat-square
     :target: https://discord.com/invite/ZHJe3tXQkf
     :alt: Stars
 
 
 Welcome to the documentation for a synchronous/asynchronous unofficial library for CharacterAI using `curl_cffi <https://github.com/yifeikong/curl_cffi>`_
 
-
-💻 Installation
----------------
-
-.. code-block:: bash
-
-    pip install characterai==1.0.0a1
-
 ⚠️ Warning
 ==========
 
 This version of the library is in alpha version, there may be bugs and errors. The library was developed without the participation of Character AI developers or their knowledge. To work with the library you need to know how to work with `asyncio <https://docs.python.org/3/library/asyncio.html>`_
 
 
 🔥 Features
```

### Comparing `characterai-1.0.0/characterai/aiocai/client.py` & `characterai-1.0.1/characterai/aiocai/client.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/account.py` & `characterai-1.0.1/characterai/aiocai/methods/account.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/characters.py` & `characterai-1.0.1/characterai/aiocai/methods/characters.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/chat1.py` & `characterai-1.0.1/characterai/aiocai/methods/chat1.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/chat2.py` & `characterai-1.0.1/characterai/aiocai/methods/chat2.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/chats.py` & `characterai-1.0.1/characterai/aiocai/methods/chats.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/other.py` & `characterai-1.0.1/characterai/aiocai/methods/other.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/recent.py` & `characterai-1.0.1/characterai/aiocai/methods/recent.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/users.py` & `characterai-1.0.1/characterai/aiocai/methods/users.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/aiocai/methods/utils.py` & `characterai-1.0.1/characterai/aiocai/methods/utils.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/auth.py` & `characterai-1.0.1/characterai/auth.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/client.py` & `characterai-1.0.1/characterai/pycai/client.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/account.py` & `characterai-1.0.1/characterai/pycai/methods/account.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/characters.py` & `characterai-1.0.1/characterai/pycai/methods/characters.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/chat1.py` & `characterai-1.0.1/characterai/pycai/methods/chat1.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/chat2.py` & `characterai-1.0.1/characterai/pycai/methods/chat2.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/chats.py` & `characterai-1.0.1/characterai/pycai/methods/chats.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/other.py` & `characterai-1.0.1/characterai/pycai/methods/other.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/recent.py` & `characterai-1.0.1/characterai/pycai/methods/recent.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/users.py` & `characterai-1.0.1/characterai/pycai/methods/users.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/pycai/methods/utils.py` & `characterai-1.0.1/characterai/pycai/methods/utils.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/types/account.py` & `characterai-1.0.1/characterai/types/account.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/types/character.py` & `characterai-1.0.1/characterai/types/character.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/types/chat1.py` & `characterai-1.0.1/characterai/types/chat1.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/types/chat2.py` & `characterai-1.0.1/characterai/types/chat2.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/types/other.py` & `characterai-1.0.1/characterai/types/other.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/types/recent.py` & `characterai-1.0.1/characterai/types/recent.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai/types/user.py` & `characterai-1.0.1/characterai/types/user.py`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/characterai.egg-info/PKG-INFO` & `characterai-1.0.1/characterai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unofficial API for Character AI for Python
 Home-page: https://github.com/kramcat/characterai
 Author: kramcat
 License: MIT
 Project-URL: Community, https://discord.gg/ZHJe3tXQkf
 Project-URL: Source, https://github.com/kramcat/characterai
 Project-URL: Documentation, https://docs.kram.cat
@@ -37,22 +37,14 @@
 .. |tag4| image:: https://img.shields.io/discord/1120066151515422772?style=flat-square
     :target: https://discord.com/invite/ZHJe3tXQkf
     :alt: Stars
 
 
 Welcome to the documentation for a synchronous/asynchronous unofficial library for CharacterAI using `curl_cffi <https://github.com/yifeikong/curl_cffi>`_
 
-
-💻 Installation
----------------
-
-.. code-block:: bash
-
-    pip install characterai==1.0.0a1
-
 ⚠️ Warning
 ==========
 
 This version of the library is in alpha version, there may be bugs and errors. The library was developed without the participation of Character AI developers or their knowledge. To work with the library you need to know how to work with `asyncio <https://docs.python.org/3/library/asyncio.html>`_
 
 
 🔥 Features
```

### Comparing `characterai-1.0.0/characterai.egg-info/SOURCES.txt` & `characterai-1.0.1/characterai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `characterai-1.0.0/setup.py` & `characterai-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='characterai',
-    version='1.0.0',
+    version='1.0.1',
     description='An unofficial API for Character AI for Python',
     keywords='ai wrapper api library',
     long_description=readme,
     long_description_content_type='text/x-rst',
     url='https://github.com/kramcat/characterai',
     author='kramcat',
     license='MIT',
```

