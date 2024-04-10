# Comparing `tmp/characterai-0.8.0.tar.gz` & `tmp/characterai-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "characterai-0.8.0.tar", last modified: Thu Oct  5 20:43:29 2023, max compression
+gzip compressed data, was "characterai-1.0.1a1.tar", last modified: Wed Apr 10 07:58:18 2024, max compression
```

## Comparing `characterai-0.8.0.tar` & `characterai-1.0.1a1.tar`

### file list

```diff
@@ -1,17 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-10-05 20:43:29.735922 characterai-0.8.0/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     2093 2023-10-05 20:43:29.733921 characterai-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-10-05 20:36:42.000000 characterai-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-05 20:43:29.651861 characterai-0.8.0/characterai/
--rw-rw-rw-   0        0        0       90 2023-08-15 13:48:38.000000 characterai-0.8.0/characterai/__init__.py
--rw-rw-rw-   0        0        0    18337 2023-10-05 20:42:35.000000 characterai-0.8.0/characterai/characterai.py
--rw-rw-rw-   0        0        0      213 2023-10-05 20:42:47.000000 characterai-0.8.0/characterai/errors.py
--rw-rw-rw-   0        0        0    26135 2023-10-05 20:42:27.000000 characterai-0.8.0/characterai/pyasynccai.py
-drwxrwxrwx   0        0        0        0 2023-10-05 20:43:29.729920 characterai-0.8.0/characterai.egg-info/
--rw-rw-rw-   0        0        0     2093 2023-10-05 20:43:28.000000 characterai-0.8.0/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-10-05 20:43:29.000000 characterai-0.8.0/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-05 20:43:28.000000 characterai-0.8.0/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-10-05 20:43:28.000000 characterai-0.8.0/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-05 20:43:28.000000 characterai-0.8.0/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-05 20:43:29.736922 characterai-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-10-05 20:35:31.000000 characterai-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.937956 characterai-1.0.1a1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3731 2024-04-10 07:58:18.937956 characterai-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-04-10 06:52:36.000000 characterai-1.0.1a1/README.rst
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.837946 characterai-1.0.1a1/characterai/
+-rw-------   0 runner    (1000) runner    (1000)      391 2024-04-07 22:04:22.000000 characterai-1.0.1a1/characterai/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.837946 characterai-1.0.1a1/characterai/aiocai/
+-rw-------   0 runner    (1000) runner    (1000)      263 2024-04-07 21:51:49.000000 characterai-1.0.1a1/characterai/aiocai/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1655 2024-04-08 11:25:08.000000 characterai-1.0.1a1/characterai/aiocai/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.845947 characterai-1.0.1a1/characterai/aiocai/methods/
+-rw-------   0 runner    (1000) runner    (1000)      289 2024-04-02 08:55:21.000000 characterai-1.0.1a1/characterai/aiocai/methods/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6711 2024-04-08 13:44:06.000000 characterai-1.0.1a1/characterai/aiocai/methods/account.py
+-rw-------   0 runner    (1000) runner    (1000)     9183 2024-04-09 07:45:55.000000 characterai-1.0.1a1/characterai/aiocai/methods/characters.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6658 2024-04-09 08:29:08.000000 characterai-1.0.1a1/characterai/aiocai/methods/chat1.py
+-rw-------   0 runner    (1000) runner    (1000)    12061 2024-04-09 08:24:30.000000 characterai-1.0.1a1/characterai/aiocai/methods/chat2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-09 08:01:54.000000 characterai-1.0.1a1/characterai/aiocai/methods/chats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2376 2024-04-09 08:02:31.000000 characterai-1.0.1a1/characterai/aiocai/methods/other.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1430 2024-04-09 07:48:23.000000 characterai-1.0.1a1/characterai/aiocai/methods/recent.py
+-rw-------   0 runner    (1000) runner    (1000)      815 2024-04-09 08:02:45.000000 characterai-1.0.1a1/characterai/aiocai/methods/users.py
+-rw-------   0 runner    (1000) runner    (1000)     4029 2024-04-08 18:23:06.000000 characterai-1.0.1a1/characterai/aiocai/methods/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3561 2024-03-21 15:41:40.000000 characterai-1.0.1a1/characterai/auth.py
+-rw-------   0 runner    (1000) runner    (1000)      194 2024-04-07 20:51:55.000000 characterai-1.0.1a1/characterai/errors.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.845947 characterai-1.0.1a1/characterai/pycai/
+-rw-------   0 runner    (1000) runner    (1000)      243 2024-04-07 21:57:33.000000 characterai-1.0.1a1/characterai/pycai/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1462 2024-04-08 11:16:16.000000 characterai-1.0.1a1/characterai/pycai/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.929955 characterai-1.0.1a1/characterai/pycai/methods/
+-rw-------   0 runner    (1000) runner    (1000)      289 2024-04-07 21:54:03.000000 characterai-1.0.1a1/characterai/pycai/methods/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     6455 2024-04-09 20:25:28.000000 characterai-1.0.1a1/characterai/pycai/methods/account.py
+-rw-------   0 runner    (1000) runner    (1000)     8601 2024-04-09 20:31:10.000000 characterai-1.0.1a1/characterai/pycai/methods/characters.py
+-rw-------   0 runner    (1000) runner    (1000)     6460 2024-04-09 20:28:57.000000 characterai-1.0.1a1/characterai/pycai/methods/chat1.py
+-rw-------   0 runner    (1000) runner    (1000)    11629 2024-04-09 20:30:23.000000 characterai-1.0.1a1/characterai/pycai/methods/chat2.py
+-rw-------   0 runner    (1000) runner    (1000)     1581 2024-04-09 20:31:50.000000 characterai-1.0.1a1/characterai/pycai/methods/chats.py
+-rw-------   0 runner    (1000) runner    (1000)     2328 2024-04-09 20:32:28.000000 characterai-1.0.1a1/characterai/pycai/methods/other.py
+-rw-------   0 runner    (1000) runner    (1000)     1394 2024-04-09 20:32:51.000000 characterai-1.0.1a1/characterai/pycai/methods/recent.py
+-rw-------   0 runner    (1000) runner    (1000)      803 2024-04-09 20:33:03.000000 characterai-1.0.1a1/characterai/pycai/methods/users.py
+-rw-------   0 runner    (1000) runner    (1000)     3900 2024-04-07 22:04:41.000000 characterai-1.0.1a1/characterai/pycai/methods/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.933956 characterai-1.0.1a1/characterai/types/
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-03-15 10:35:14.000000 characterai-1.0.1a1/characterai/types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6619 2024-04-09 19:40:37.000000 characterai-1.0.1a1/characterai/types/account.py
+-rw-------   0 runner    (1000) runner    (1000)     8248 2024-04-09 20:23:40.000000 characterai-1.0.1a1/characterai/types/character.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11231 2024-04-09 20:17:22.000000 characterai-1.0.1a1/characterai/types/chat1.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4745 2024-04-09 20:00:46.000000 characterai-1.0.1a1/characterai/types/chat2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4190 2024-04-09 19:55:40.000000 characterai-1.0.1a1/characterai/types/other.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2598 2024-04-09 19:51:12.000000 characterai-1.0.1a1/characterai/types/recent.py
+-rw-------   0 runner    (1000) runner    (1000)     1302 2024-04-09 19:44:03.000000 characterai-1.0.1a1/characterai/types/user.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 07:58:18.933956 characterai-1.0.1a1/characterai.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3731 2024-04-10 07:58:18.000000 characterai-1.0.1a1/characterai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1349 2024-04-10 07:58:18.000000 characterai-1.0.1a1/characterai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 07:58:18.000000 characterai-1.0.1a1/characterai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       50 2024-04-10 07:58:18.000000 characterai-1.0.1a1/characterai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 07:58:18.000000 characterai-1.0.1a1/characterai.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      644 2024-03-17 10:18:21.000000 characterai-1.0.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-10 07:58:18.937956 characterai-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      955 2024-04-10 07:58:00.000000 characterai-1.0.1a1/setup.py
```

