# Comparing `tmp/ipih-0.19.tar.gz` & `tmp/ipih-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipih-0.19.tar", last modified: Wed Apr 10 02:53:32 2024, max compression
+gzip compressed data, was "ipih-0.20.tar", last modified: Fri Mar 29 00:39:54 2024, max compression
```

## Comparing `ipih-0.19.tar` & `ipih-0.20.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:53:32.372113 ipih-0.19/
--rw-rw-rw-   0        0        0      449 2024-04-10 02:53:32.307796 ipih-0.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:53:31.930673 ipih-0.19/ipih/
--rw-rw-rw-   0        0        0     1317 2024-04-10 02:48:29.000000 ipih-0.19/ipih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:53:32.276546 ipih-0.19/ipih.egg-info/
--rw-rw-rw-   0        0        0      449 2024-04-10 02:53:31.000000 ipih-0.19/ipih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-04-10 02:53:31.000000 ipih-0.19/ipih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:53:31.000000 ipih-0.19/ipih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-04-10 02:53:31.000000 ipih-0.19/ipih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 02:53:31.000000 ipih-0.19/ipih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:53:32.387753 ipih-0.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-29 00:39:54.051152 ipih-0.20/
+-rw-rw-rw-   0        0        0      449 2024-03-29 00:39:54.003227 ipih-0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-03-29 00:39:53.659062 ipih-0.20/ipih/
+-rw-rw-rw-   0        0        0     1317 2024-03-29 00:38:25.000000 ipih-0.20/ipih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-29 00:39:53.971977 ipih-0.20/ipih.egg-info/
+-rw-rw-rw-   0        0        0      449 2024-03-29 00:39:53.000000 ipih-0.20/ipih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-03-29 00:39:53.000000 ipih-0.20/ipih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-29 00:39:53.000000 ipih-0.20/ipih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-03-29 00:39:53.000000 ipih-0.20/ipih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-03-29 00:39:53.000000 ipih-0.20/ipih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-29 00:39:54.051152 ipih-0.20/setup.cfg
```

### Comparing `ipih-0.19/ipih/__init__.py` & `ipih-0.20/ipih/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 import importlib.util
 import platform
 
 
 NAME: str = "ipih"
-VERSION: str = "0.19"
+VERSION: str = "0.20"
 
 ROOT_MODULE_NAME: str = "pih"
 FACADE_FOLDER_NAME: str = "facade"
 BUILD_FOLDER_NAME: str = ".build"
 BUILD_FILES_FOLDER_NAME: str = ".files"
 WINDOWS_SHARE_DOMAIN_NAME: str = ROOT_MODULE_NAME
 WINDOWS_SHARE_DOMAIN_ALIAS: str = "fmv"
```

