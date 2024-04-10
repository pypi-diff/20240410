# Comparing `tmp/ml_runlog-1.9.tar.gz` & `tmp/ml_runlog-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_runlog-1.9.tar", last modified: Tue Apr  9 06:00:46 2024, max compression
+gzip compressed data, was "ml_runlog-2.0.tar", last modified: Wed Apr 10 02:33:36 2024, max compression
```

## Comparing `ml_runlog-1.9.tar` & `ml_runlog-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 06:00:46.948664 ml_runlog-1.9/
--rw-rw-r--   0 anag      (1000) anag      (1000)    35149 2024-04-09 05:52:10.000000 ml_runlog-1.9/LICENSE
--rw-rw-r--   0 anag      (1000) anag      (1000)      254 2024-04-09 06:00:46.948664 ml_runlog-1.9/PKG-INFO
--rw-rw-r--   0 anag      (1000) anag      (1000)     1827 2024-04-09 03:18:50.000000 ml_runlog-1.9/README.md
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 06:00:46.948664 ml_runlog-1.9/ml_runlog/
--rw-rw-r--   0 anag      (1000) anag      (1000)     2072 2024-04-09 05:50:10.000000 ml_runlog-1.9/ml_runlog/__init__.py
--rw-rw-r--   0 anag      (1000) anag      (1000)      880 2024-04-09 03:18:50.000000 ml_runlog-1.9/ml_runlog/main.py
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 06:00:46.948664 ml_runlog-1.9/ml_runlog.egg-info/
--rw-rw-r--   0 anag      (1000) anag      (1000)      254 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/PKG-INFO
--rw-rw-r--   0 anag      (1000) anag      (1000)      262 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/SOURCES.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/dependency_links.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/not-zip-safe
--rw-rw-r--   0 anag      (1000) anag      (1000)       17 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/requires.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)       10 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/top_level.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)       38 2024-04-09 06:00:46.948664 ml_runlog-1.9/setup.cfg
--rw-rw-r--   0 anag      (1000) anag      (1000)      421 2024-04-09 05:55:02.000000 ml_runlog-1.9/setup.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 02:33:36.393025 ml_runlog-2.0/
+-rw-rw-r--   0 anag      (1000) anag      (1000)    35149 2024-04-09 05:52:10.000000 ml_runlog-2.0/LICENSE
+-rw-r--r--   0 anag      (1000) anag      (1000)      398 2024-04-10 02:33:36.393025 ml_runlog-2.0/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)     1827 2024-04-09 03:18:50.000000 ml_runlog-2.0/README.md
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 02:33:36.393025 ml_runlog-2.0/ml_runlog/
+-rw-rw-r--   0 anag      (1000) anag      (1000)       78 2024-04-10 01:21:01.000000 ml_runlog-2.0/ml_runlog/__init__.py
+-rw-rw-r--   0 anag      (1000) anag      (1000)     2511 2024-04-10 02:22:59.000000 ml_runlog-2.0/ml_runlog/main.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 02:33:36.393025 ml_runlog-2.0/ml_runlog.egg-info/
+-rw-r--r--   0 anag      (1000) anag      (1000)      398 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)      262 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 06:00:46.000000 ml_runlog-2.0/ml_runlog.egg-info/not-zip-safe
+-rw-rw-r--   0 anag      (1000) anag      (1000)       17 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/requires.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       10 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/top_level.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       38 2024-04-10 02:33:36.393025 ml_runlog-2.0/setup.cfg
+-rw-rw-r--   0 anag      (1000) anag      (1000)      518 2024-04-10 02:32:26.000000 ml_runlog-2.0/setup.py
```

### Comparing `ml_runlog-1.9/LICENSE` & `ml_runlog-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_runlog-1.9/README.md` & `ml_runlog-2.0/README.md`

 * *Files identical despite different names*

