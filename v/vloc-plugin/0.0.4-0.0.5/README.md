# Comparing `tmp/vloc_plugin-0.0.4.tar.gz` & `tmp/vloc_plugin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc_plugin-0.0.4.tar", last modified: Tue Apr  9 06:42:41 2024, max compression
+gzip compressed data, was "vloc_plugin-0.0.5.tar", last modified: Tue Apr  9 08:00:11 2024, max compression
```

## Comparing `vloc_plugin-0.0.4.tar` & `vloc_plugin-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.258962 vloc_plugin-0.0.4/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.4/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 06:42:41.258775 vloc_plugin-0.0.4/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.4/README.md
--rw-r--r--   0 byron      (501) staff       (20)      479 2024-04-09 06:42:04.000000 vloc_plugin-0.0.4/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 06:42:41.259001 vloc_plugin-0.0.4/setup.cfg
--rw-------   0 byron      (501) staff       (20)      583 2024-04-08 09:39:30.000000 vloc_plugin-0.0.4/setup.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.257599 vloc_plugin-0.0.4/vloc/
--rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:40:26.000000 vloc_plugin-0.0.4/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.257957 vloc_plugin-0.0.4/vloc/plugin/
--rw-r--r--   0 byron      (501) staff       (20)     1439 2024-04-09 02:44:26.000000 vloc_plugin-0.0.4/vloc/plugin/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-09 02:39:51.000000 vloc_plugin-0.0.4/vloc/plugin/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)      299 2024-04-09 03:13:08.000000 vloc_plugin-0.0.4/vloc/plugin/catalog.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.258611 vloc_plugin-0.0.4/vloc_plugin.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      273 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:00:11.915556 vloc_plugin-0.0.5/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.5/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      388 2024-04-09 08:00:11.915329 vloc_plugin-0.0.5/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.5/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      479 2024-04-09 07:59:29.000000 vloc_plugin-0.0.5/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 08:00:11.915602 vloc_plugin-0.0.5/setup.cfg
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:00:11.913693 vloc_plugin-0.0.5/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:40:26.000000 vloc_plugin-0.0.5/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:00:11.914231 vloc_plugin-0.0.5/vloc/plugin/
+-rw-r--r--   0 byron      (501) staff       (20)     1439 2024-04-09 07:58:36.000000 vloc_plugin-0.0.5/vloc/plugin/__info__.py
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-09 02:39:51.000000 vloc_plugin-0.0.5/vloc/plugin/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)      368 2024-04-09 07:51:05.000000 vloc_plugin-0.0.5/vloc/plugin/catalog.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:00:11.915132 vloc_plugin-0.0.5/vloc_plugin.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      388 2024-04-09 08:00:11.000000 vloc_plugin-0.0.5/vloc_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      264 2024-04-09 08:00:11.000000 vloc_plugin-0.0.5/vloc_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 08:00:11.000000 vloc_plugin-0.0.5/vloc_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 08:00:11.000000 vloc_plugin-0.0.5/vloc_plugin.egg-info/top_level.txt
```

### Comparing `vloc_plugin-0.0.4/LICENSE.txt` & `vloc_plugin-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc_plugin-0.0.4/vloc/plugin/__info__.py` & `vloc_plugin-0.0.5/vloc/plugin/__info__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from importlib.util import find_spec
 from dataclasses import dataclass
 import re
 import cv2
 import pytesseract
 from vloc.config.catalog import VL
 from vloc.exception.catalog import OcrException
-if find_spec('vloc_plugin_selenium'):
+if find_spec('vloc.plugin.selenium'):
     from vloc.plugin.selenium.__info__ import Action as SeleniumAction
 
 
 @dataclass
 class DetectInfo:
     x: int
     y: int
```

