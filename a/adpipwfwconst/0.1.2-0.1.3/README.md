# Comparing `tmp/adpipwfwconst-0.1.2.tar.gz` & `tmp/adpipwfwconst-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipwfwconst-0.1.2.tar", last modified: Sun Apr  7 20:08:53 2024, max compression
+gzip compressed data, was "adpipwfwconst-0.1.3.tar", last modified: Wed Apr 10 17:04:54 2024, max compression
```

## Comparing `adpipwfwconst-0.1.2.tar` & `adpipwfwconst-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 20:08:53.582561 adpipwfwconst-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-07 20:08:29.000000 adpipwfwconst-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-07 20:08:53.582561 adpipwfwconst-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 20:08:29.000000 adpipwfwconst-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 20:08:53.578560 adpipwfwconst-0.1.2/adpipwfwconst/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 20:08:29.000000 adpipwfwconst-0.1.2/adpipwfwconst/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2024-04-07 20:08:29.000000 adpipwfwconst-0.1.2/adpipwfwconst/adpipwfwconst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 20:08:53.582561 adpipwfwconst-0.1.2/adpipwfwconst.egg-info/
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-07 20:08:53.000000 adpipwfwconst-0.1.2/adpipwfwconst.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2024-04-07 20:08:53.000000 adpipwfwconst-0.1.2/adpipwfwconst.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 20:08:53.000000 adpipwfwconst-0.1.2/adpipwfwconst.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-07 20:08:53.000000 adpipwfwconst-0.1.2/adpipwfwconst.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 20:08:53.582561 adpipwfwconst-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      408 2024-04-07 20:08:29.000000 adpipwfwconst-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:04:54.234398 adpipwfwconst-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-10 17:04:01.000000 adpipwfwconst-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-10 17:04:54.234398 adpipwfwconst-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 17:04:01.000000 adpipwfwconst-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:04:54.234398 adpipwfwconst-0.1.3/adpipwfwconst/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:04:01.000000 adpipwfwconst-0.1.3/adpipwfwconst/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-04-10 17:04:01.000000 adpipwfwconst-0.1.3/adpipwfwconst/adpipwfwconst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:04:54.234398 adpipwfwconst-0.1.3/adpipwfwconst.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-10 17:04:54.000000 adpipwfwconst-0.1.3/adpipwfwconst.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-10 17:04:54.000000 adpipwfwconst-0.1.3/adpipwfwconst.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:04:54.000000 adpipwfwconst-0.1.3/adpipwfwconst.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-10 17:04:54.000000 adpipwfwconst-0.1.3/adpipwfwconst.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 17:04:54.234398 adpipwfwconst-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      408 2024-04-10 17:04:01.000000 adpipwfwconst-0.1.3/setup.py
```

### Comparing `adpipwfwconst-0.1.2/LICENSE` & `adpipwfwconst-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adpipwfwconst-0.1.2/adpipwfwconst/adpipwfwconst.py` & `adpipwfwconst-0.1.3/adpipwfwconst/adpipwfwconst.py`

 * *Files identical despite different names*

