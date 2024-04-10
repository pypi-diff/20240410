# Comparing `tmp/pluginTest-0.1.tar.gz` & `tmp/pluginTest-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluginTest-0.1.tar", last modified: Thu Apr  4 11:03:30 2024, max compression
+gzip compressed data, was "pluginTest-0.2.1.tar", last modified: Wed Apr 10 07:36:49 2024, max compression
```

## Comparing `pluginTest-0.1.tar` & `pluginTest-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 node      (1000) node      (1000)        0 2024-04-04 11:03:30.330230 pluginTest-0.1/
--rw-r--r--   0 node      (1000) node      (1000)       97 2024-04-04 11:03:30.330230 pluginTest-0.1/PKG-INFO
-drwxr-xr-x   0 node      (1000) node      (1000)        0 2024-04-04 11:03:30.329230 pluginTest-0.1/pluginTest/
--rw-r--r--   0 node      (1000) node      (1000)        0 2024-04-03 13:56:55.000000 pluginTest-0.1/pluginTest/__init__.py
--rw-r--r--   0 node      (1000) node      (1000)      720 2024-04-04 10:57:59.000000 pluginTest-0.1/pluginTest/plugin.py
-drwxr-xr-x   0 node      (1000) node      (1000)        0 2024-04-04 11:03:30.330230 pluginTest-0.1/pluginTest.egg-info/
--rw-r--r--   0 node      (1000) node      (1000)       97 2024-04-04 11:03:30.000000 pluginTest-0.1/pluginTest.egg-info/PKG-INFO
--rw-r--r--   0 node      (1000) node      (1000)      258 2024-04-04 11:03:30.000000 pluginTest-0.1/pluginTest.egg-info/SOURCES.txt
--rw-r--r--   0 node      (1000) node      (1000)        1 2024-04-04 11:03:30.000000 pluginTest-0.1/pluginTest.egg-info/dependency_links.txt
--rw-r--r--   0 node      (1000) node      (1000)       61 2024-04-04 11:03:30.000000 pluginTest-0.1/pluginTest.egg-info/entry_points.txt
--rw-r--r--   0 node      (1000) node      (1000)        7 2024-04-04 11:03:30.000000 pluginTest-0.1/pluginTest.egg-info/requires.txt
--rw-r--r--   0 node      (1000) node      (1000)       11 2024-04-04 11:03:30.000000 pluginTest-0.1/pluginTest.egg-info/top_level.txt
--rw-r--r--   0 node      (1000) node      (1000)       38 2024-04-04 11:03:30.330230 pluginTest-0.1/setup.cfg
--rw-r--r--   0 node      (1000) node      (1000)      322 2024-04-04 10:50:00.000000 pluginTest-0.1/setup.py
+drwxr-xr-x   0 node      (1000) node      (1000)        0 2024-04-10 07:36:49.039919 pluginTest-0.2.1/
+-rw-r--r--   0 node      (1000) node      (1000)       99 2024-04-10 07:36:49.039919 pluginTest-0.2.1/PKG-INFO
+drwxr-xr-x   0 node      (1000) node      (1000)        0 2024-04-10 07:36:49.039919 pluginTest-0.2.1/pluginTest/
+-rw-r--r--   0 node      (1000) node      (1000)        0 2024-04-09 13:46:57.000000 pluginTest-0.2.1/pluginTest/__init__.py
+-rw-r--r--   0 node      (1000) node      (1000)     2112 2024-04-09 13:50:33.000000 pluginTest-0.2.1/pluginTest/plugin.py
+drwxr-xr-x   0 node      (1000) node      (1000)        0 2024-04-10 07:36:49.039919 pluginTest-0.2.1/pluginTest.egg-info/
+-rw-r--r--   0 node      (1000) node      (1000)       99 2024-04-10 07:36:49.000000 pluginTest-0.2.1/pluginTest.egg-info/PKG-INFO
+-rw-r--r--   0 node      (1000) node      (1000)      258 2024-04-10 07:36:49.000000 pluginTest-0.2.1/pluginTest.egg-info/SOURCES.txt
+-rw-r--r--   0 node      (1000) node      (1000)        1 2024-04-10 07:36:49.000000 pluginTest-0.2.1/pluginTest.egg-info/dependency_links.txt
+-rw-r--r--   0 node      (1000) node      (1000)       61 2024-04-10 07:36:49.000000 pluginTest-0.2.1/pluginTest.egg-info/entry_points.txt
+-rw-r--r--   0 node      (1000) node      (1000)        7 2024-04-10 07:36:49.000000 pluginTest-0.2.1/pluginTest.egg-info/requires.txt
+-rw-r--r--   0 node      (1000) node      (1000)       11 2024-04-10 07:36:49.000000 pluginTest-0.2.1/pluginTest.egg-info/top_level.txt
+-rw-r--r--   0 node      (1000) node      (1000)       38 2024-04-10 07:36:49.039919 pluginTest-0.2.1/setup.cfg
+-rw-r--r--   0 node      (1000) node      (1000)      324 2024-04-10 07:35:40.000000 pluginTest-0.2.1/setup.py
```

