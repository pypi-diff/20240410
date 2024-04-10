# Comparing `tmp/socketman-0.2.2.tar.gz` & `tmp/socketman-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketman-0.2.2.tar", last modified: Sat Mar  2 13:05:17 2024, max compression
+gzip compressed data, was "socketman-0.4.0.tar", last modified: Wed Apr 10 18:21:21 2024, max compression
```

## Comparing `socketman-0.2.2.tar` & `socketman-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-03-02 13:05:17.107845 socketman-0.2.2/
--rw-r--r--   0 zlols     (1000) zlols     (1000)     1062 2024-03-02 09:19:03.000000 socketman-0.2.2/LICENSE
--rw-r--r--   0 zlols     (1000) zlols     (1000)     1948 2024-03-02 13:05:17.107845 socketman-0.2.2/PKG-INFO
--rw-r--r--   0 zlols     (1000) zlols     (1000)     1522 2024-03-02 13:04:11.000000 socketman-0.2.2/README.md
--rw-r--r--   0 zlols     (1000) zlols     (1000)       38 2024-03-02 13:05:17.107845 socketman-0.2.2/setup.cfg
--rw-r--r--   0 zlols     (1000) zlols     (1000)      890 2024-03-02 13:02:31.000000 socketman-0.2.2/setup.py
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-03-02 13:05:17.105845 socketman-0.2.2/socketman/
--rw-r--r--   0 zlols     (1000) zlols     (1000)      156 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/__init__.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)      950 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/test.py
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-03-02 13:05:17.106845 socketman-0.2.2/socketman/utils/
--rw-r--r--   0 zlols     (1000) zlols     (1000)        0 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/utils/__init__.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)      554 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/utils/infowrap.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     1070 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/utils/iptools.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     5532 2024-03-02 09:19:45.000000 socketman-0.2.2/socketman/utils/packing.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     4665 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/v2.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     8763 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/v3.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)       98 2024-03-02 13:04:53.000000 socketman-0.2.2/socketman/version.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     7393 2024-03-02 09:19:03.000000 socketman-0.2.2/socketman/websocketthread.py
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-03-02 13:05:17.106845 socketman-0.2.2/socketman.egg-info/
--rw-r--r--   0 zlols     (1000) zlols     (1000)     1948 2024-03-02 13:05:17.000000 socketman-0.2.2/socketman.egg-info/PKG-INFO
--rw-r--r--   0 zlols     (1000) zlols     (1000)      422 2024-03-02 13:05:17.000000 socketman-0.2.2/socketman.egg-info/SOURCES.txt
--rw-r--r--   0 zlols     (1000) zlols     (1000)        1 2024-03-02 13:05:17.000000 socketman-0.2.2/socketman.egg-info/dependency_links.txt
--rw-r--r--   0 zlols     (1000) zlols     (1000)       11 2024-03-02 13:05:17.000000 socketman-0.2.2/socketman.egg-info/requires.txt
--rw-r--r--   0 zlols     (1000) zlols     (1000)       10 2024-03-02 13:05:17.000000 socketman-0.2.2/socketman.egg-info/top_level.txt
+drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:21:21.184961 socketman-0.4.0/
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     1062 2024-03-02 09:19:03.000000 socketman-0.4.0/LICENSE
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     1268 2024-04-10 18:21:21.184961 socketman-0.4.0/PKG-INFO
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      868 2024-04-10 18:15:52.000000 socketman-0.4.0/README.md
+-rw-r--r--   0 zlols     (1000) zlols     (1000)       38 2024-04-10 18:21:21.184961 socketman-0.4.0/setup.cfg
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      890 2024-03-02 13:02:31.000000 socketman-0.4.0/setup.py
+drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:21:21.183961 socketman-0.4.0/socketman/
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     1720 2024-04-10 17:50:33.000000 socketman-0.4.0/socketman/__init__.py
+drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:21:21.184961 socketman-0.4.0/socketman/manager/
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      244 2024-04-09 18:24:10.000000 socketman-0.4.0/socketman/manager/__init__.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     6411 2024-04-10 17:06:53.000000 socketman-0.4.0/socketman/manager/__main__.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     2687 2024-04-09 18:30:10.000000 socketman-0.4.0/socketman/manager/client.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     1301 2024-04-08 17:39:13.000000 socketman-0.4.0/socketman/manager/common.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     4124 2024-04-10 17:54:52.000000 socketman-0.4.0/socketman/objsocket.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     2287 2024-03-30 09:22:41.000000 socketman-0.4.0/socketman/serialization.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)       98 2024-04-10 18:17:31.000000 socketman-0.4.0/socketman/version.py
+drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:21:21.184961 socketman-0.4.0/socketman.egg-info/
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     1268 2024-04-10 18:21:21.000000 socketman-0.4.0/socketman.egg-info/PKG-INFO
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      399 2024-04-10 18:21:21.000000 socketman-0.4.0/socketman.egg-info/SOURCES.txt
+-rw-r--r--   0 zlols     (1000) zlols     (1000)        1 2024-04-10 18:21:21.000000 socketman-0.4.0/socketman.egg-info/dependency_links.txt
+-rw-r--r--   0 zlols     (1000) zlols     (1000)       11 2024-04-10 18:21:21.000000 socketman-0.4.0/socketman.egg-info/requires.txt
+-rw-r--r--   0 zlols     (1000) zlols     (1000)       10 2024-04-10 18:21:21.000000 socketman-0.4.0/socketman.egg-info/top_level.txt
```

### Comparing `socketman-0.2.2/LICENSE` & `socketman-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketman-0.2.2/setup.py` & `socketman-0.4.0/setup.py`

 * *Files identical despite different names*

