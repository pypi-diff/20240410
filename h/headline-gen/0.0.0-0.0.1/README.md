# Comparing `tmp/headline-gen-0.0.0.tar.gz` & `tmp/headline-gen-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline-gen-0.0.0.tar", last modified: Wed Apr 10 03:49:53 2024, max compression
+gzip compressed data, was "headline-gen-0.0.1.tar", last modified: Wed Apr 10 03:59:44 2024, max compression
```

## Comparing `headline-gen-0.0.0.tar` & `headline-gen-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:53.126676 headline-gen-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      150 2024-04-10 03:49:53.126676 headline-gen-0.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:53.124676 headline-gen-0.0.0/headline-gen/
--rw-r--r--   0 root         (0) root         (0)     2410 2024-04-10 03:13:37.000000 headline-gen-0.0.0/headline-gen/Compression.py
--rw-r--r--   0 root         (0) root         (0)      909 2024-04-10 03:13:37.000000 headline-gen-0.0.0/headline-gen/Control.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-04-10 03:13:37.000000 headline-gen-0.0.0/headline-gen/KEA.py
--rw-r--r--   0 root         (0) root         (0)     4099 2024-04-10 03:13:37.000000 headline-gen-0.0.0/headline-gen/LeadingSentences.py
--rw-r--r--   0 root         (0) root         (0)     3176 2024-04-10 03:13:37.000000 headline-gen-0.0.0/headline-gen/PostProcess.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-10 03:13:37.000000 headline-gen-0.0.0/headline-gen/Ranking.py
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 03:34:36.000000 headline-gen-0.0.0/headline-gen/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:49:53.126676 headline-gen-0.0.0/headline_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      150 2024-04-10 03:49:52.000000 headline-gen-0.0.0/headline_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-10 03:49:53.000000 headline-gen-0.0.0/headline_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:49:52.000000 headline-gen-0.0.0/headline_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-10 03:49:52.000000 headline-gen-0.0.0/headline_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 03:49:52.000000 headline-gen-0.0.0/headline_gen.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:49:53.126676 headline-gen-0.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      348 2024-04-10 03:49:38.000000 headline-gen-0.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:59:44.612163 headline-gen-0.0.1/
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-10 03:59:44.611163 headline-gen-0.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:59:44.610163 headline-gen-0.0.1/headline_gen/
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-10 03:58:31.000000 headline-gen-0.0.1/headline_gen/Compression.py
+-rw-r--r--   0 root         (0) root         (0)      909 2024-04-10 03:58:31.000000 headline-gen-0.0.1/headline_gen/Control.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-10 03:58:31.000000 headline-gen-0.0.1/headline_gen/KEA.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2024-04-10 03:58:31.000000 headline-gen-0.0.1/headline_gen/LeadingSentences.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2024-04-10 03:58:31.000000 headline-gen-0.0.1/headline_gen/PostProcess.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-10 03:58:31.000000 headline-gen-0.0.1/headline_gen/Ranking.py
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 03:58:31.000000 headline-gen-0.0.1/headline_gen/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 03:59:44.611163 headline-gen-0.0.1/headline_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-10 03:59:44.000000 headline-gen-0.0.1/headline_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-10 03:59:44.000000 headline-gen-0.0.1/headline_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 03:59:44.000000 headline-gen-0.0.1/headline_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-10 03:59:44.000000 headline-gen-0.0.1/headline_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 03:59:44.000000 headline-gen-0.0.1/headline_gen.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 03:59:44.612163 headline-gen-0.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      348 2024-04-10 03:59:37.000000 headline-gen-0.0.1/setup.py
```

### Comparing `headline-gen-0.0.0/headline-gen/Compression.py` & `headline-gen-0.0.1/headline_gen/Compression.py`

 * *Files identical despite different names*

### Comparing `headline-gen-0.0.0/headline-gen/Control.py` & `headline-gen-0.0.1/headline_gen/Control.py`

 * *Files identical despite different names*

### Comparing `headline-gen-0.0.0/headline-gen/LeadingSentences.py` & `headline-gen-0.0.1/headline_gen/LeadingSentences.py`

 * *Files identical despite different names*

### Comparing `headline-gen-0.0.0/headline-gen/PostProcess.py` & `headline-gen-0.0.1/headline_gen/PostProcess.py`

 * *Files identical despite different names*

