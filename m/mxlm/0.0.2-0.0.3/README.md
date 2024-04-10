# Comparing `tmp/mxlm-0.0.2.tar.gz` & `tmp/mxlm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxlm-0.0.2.tar", last modified: Sun Apr  7 12:50:58 2024, max compression
+gzip compressed data, was "mxlm-0.0.3.tar", last modified: Tue Apr  9 09:58:35 2024, max compression
```

## Comparing `mxlm-0.0.2.tar` & `mxlm-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-07 12:50:58.875848 mxlm-0.0.2/
--rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.2/MANIFEST.in
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-07 12:50:58.875848 mxlm-0.0.2/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      601 2024-03-30 08:36:12.000000 mxlm-0.0.2/README.md
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-07 12:50:58.875848 mxlm-0.0.2/mxlm/
--rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-07 12:47:58.000000 mxlm-0.0.2/mxlm/__info__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      128 2024-03-29 08:26:32.000000 mxlm-0.0.2/mxlm/__init__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2709 2024-04-07 12:49:51.000000 mxlm-0.0.2/mxlm/chat_api.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2023 2024-04-07 12:48:14.000000 mxlm-0.0.2/mxlm/chatmd_utils.py
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-07 12:50:58.875848 mxlm-0.0.2/mxlm.egg-info/
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      258 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/SOURCES.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/dependency_links.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/requires.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/top_level.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.2/requirements.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-07 12:50:58.875848 mxlm-0.0.2/setup.cfg
--rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.2/setup.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-09 09:58:35.745833 mxlm-0.0.3/
+-rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.3/MANIFEST.in
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-09 09:58:35.741833 mxlm-0.0.3/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      601 2024-03-30 08:36:12.000000 mxlm-0.0.3/README.md
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-09 09:58:35.741833 mxlm-0.0.3/mxlm/
+-rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-09 09:57:04.000000 mxlm-0.0.3/mxlm/__info__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      171 2024-04-09 06:51:51.000000 mxlm-0.0.3/mxlm/__init__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     4794 2024-04-09 09:56:46.000000 mxlm-0.0.3/mxlm/chat_api.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2023 2024-04-07 12:48:14.000000 mxlm-0.0.3/mxlm/chatmd_utils.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-09 09:58:35.741833 mxlm-0.0.3/mxlm.egg-info/
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      258 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/SOURCES.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/dependency_links.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/requires.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/top_level.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.3/requirements.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-09 09:58:35.745833 mxlm-0.0.3/setup.cfg
+-rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.3/setup.py
```

### Comparing `mxlm-0.0.2/README.md` & `mxlm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.2/mxlm/__info__.py` & `mxlm-0.0.3/mxlm/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __description__ = "Language Model Utils"
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `mxlm-0.0.2/mxlm/chatmd_utils.py` & `mxlm-0.0.3/mxlm/chatmd_utils.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.2/setup.py` & `mxlm-0.0.3/setup.py`

 * *Files identical despite different names*

