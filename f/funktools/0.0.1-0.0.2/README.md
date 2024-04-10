# Comparing `tmp/funktools-0.0.1.tar.gz` & `tmp/funktools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funktools-0.0.1.tar", last modified: Fri Apr  5 00:31:18 2024, max compression
+gzip compressed data, was "funktools-0.0.2.tar", last modified: Wed Apr 10 21:16:54 2024, max compression
```

## Comparing `funktools-0.0.1.tar` & `funktools-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-05 00:31:18.189553 funktools-0.0.1/
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     1070 2023-09-05 02:03:17.000000 funktools-0.0.1/LICENSE
--rw-rw-r--   0 modulo    (1000) modulo    (1000)      317 2024-04-05 00:31:18.189553 funktools-0.0.1/PKG-INFO
--rw-rw-r--   0 modulo    (1000) modulo    (1000)       21 2024-04-04 23:24:51.000000 funktools-0.0.1/README.md
-drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-05 00:31:18.185553 funktools-0.0.1/demo/
--rw-rw-r--   0 modulo    (1000) modulo    (1000)        0 2024-04-04 23:04:39.000000 funktools-0.0.1/demo/__init__.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)      286 2024-04-04 23:15:25.000000 funktools-0.0.1/demo/__main__.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)    11833 2024-04-04 23:24:51.000000 funktools-0.0.1/demo/cli.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     1710 2024-04-04 23:12:42.000000 funktools-0.0.1/demo/throttle.py
-drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-05 00:31:18.185553 funktools-0.0.1/funktools/
--rw-rw-r--   0 modulo    (1000) modulo    (1000)      252 2024-04-04 23:24:51.000000 funktools-0.0.1/funktools/__init__.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)    14907 2024-04-04 23:12:42.000000 funktools-0.0.1/funktools/_base.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)    22778 2024-04-04 23:24:51.000000 funktools-0.0.1/funktools/_cli.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     4813 2024-04-04 23:12:42.000000 funktools-0.0.1/funktools/_log.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     5783 2024-04-04 23:12:42.000000 funktools-0.0.1/funktools/_lru_cache.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     3829 2024-04-04 23:12:42.000000 funktools-0.0.1/funktools/_noop.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     4329 2024-04-04 23:12:42.000000 funktools-0.0.1/funktools/_retry.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     7798 2024-04-04 23:12:42.000000 funktools-0.0.1/funktools/_sqlite_cache.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)    15584 2024-04-04 23:24:51.000000 funktools-0.0.1/funktools/_throttle.py
-drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-05 00:31:18.185553 funktools-0.0.1/funktools.egg-info/
--rw-rw-r--   0 modulo    (1000) modulo    (1000)      317 2024-04-05 00:31:18.000000 funktools-0.0.1/funktools.egg-info/PKG-INFO
--rw-rw-r--   0 modulo    (1000) modulo    (1000)      585 2024-04-05 00:31:18.000000 funktools-0.0.1/funktools.egg-info/SOURCES.txt
--rw-rw-r--   0 modulo    (1000) modulo    (1000)        1 2024-04-05 00:31:18.000000 funktools-0.0.1/funktools.egg-info/dependency_links.txt
--rw-rw-r--   0 modulo    (1000) modulo    (1000)       49 2024-04-05 00:31:18.000000 funktools-0.0.1/funktools.egg-info/requires.txt
--rw-rw-r--   0 modulo    (1000) modulo    (1000)       20 2024-04-05 00:31:18.000000 funktools-0.0.1/funktools.egg-info/top_level.txt
--rw-rw-r--   0 modulo    (1000) modulo    (1000)       38 2024-04-05 00:31:18.189553 funktools-0.0.1/setup.cfg
--rw-rw-r--   0 modulo    (1000) modulo    (1000)      523 2024-04-05 00:14:13.000000 funktools-0.0.1/setup.py
-drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-05 00:31:18.185553 funktools-0.0.1/test/
--rw-rw-r--   0 modulo    (1000) modulo    (1000)        0 2024-04-04 23:04:39.000000 funktools-0.0.1/test/__init__.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     2380 2024-04-04 23:12:42.000000 funktools-0.0.1/test/test_base.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)    16960 2024-04-04 23:24:51.000000 funktools-0.0.1/test/test_cli.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     8326 2024-04-04 23:12:42.000000 funktools-0.0.1/test/test_lru_cache.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)      804 2024-04-04 23:12:42.000000 funktools-0.0.1/test/test_retry.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     4693 2024-04-04 23:12:42.000000 funktools-0.0.1/test/test_sqlite_cache.py
--rw-rw-r--   0 modulo    (1000) modulo    (1000)     2970 2024-04-04 23:12:42.000000 funktools-0.0.1/test/test_throttle.py
+drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-10 21:16:54.148966 funktools-0.0.2/
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     1070 2023-09-05 02:03:17.000000 funktools-0.0.2/LICENSE
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)      399 2024-04-10 21:16:54.148966 funktools-0.0.2/PKG-INFO
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)       21 2024-04-04 23:24:51.000000 funktools-0.0.2/README.md
+drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-10 21:16:54.144966 funktools-0.0.2/demo/
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)        0 2024-04-04 23:04:39.000000 funktools-0.0.2/demo/__init__.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)      286 2024-04-04 23:15:25.000000 funktools-0.0.2/demo/__main__.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)    11833 2024-04-04 23:24:51.000000 funktools-0.0.2/demo/cli.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     1710 2024-04-04 23:12:42.000000 funktools-0.0.2/demo/throttle.py
+drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-10 21:16:54.148966 funktools-0.0.2/funktools/
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     1287 2024-04-10 21:15:42.000000 funktools-0.0.2/funktools/__init__.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)    14907 2024-04-10 21:15:34.000000 funktools-0.0.2/funktools/_base.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)    22778 2024-04-04 23:24:51.000000 funktools-0.0.2/funktools/_cli.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     4813 2024-04-10 21:15:34.000000 funktools-0.0.2/funktools/_log.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     5783 2024-04-10 21:15:34.000000 funktools-0.0.2/funktools/_lru_cache.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     3829 2024-04-04 23:12:42.000000 funktools-0.0.2/funktools/_noop.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     4329 2024-04-04 23:12:42.000000 funktools-0.0.2/funktools/_retry.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     7798 2024-04-04 23:12:42.000000 funktools-0.0.2/funktools/_sqlite_cache.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     7382 2024-04-10 21:15:42.000000 funktools-0.0.2/funktools/_template.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)    15584 2024-04-04 23:24:51.000000 funktools-0.0.2/funktools/_throttle.py
+drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-10 21:16:54.148966 funktools-0.0.2/funktools.egg-info/
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)      399 2024-04-10 21:16:54.000000 funktools-0.0.2/funktools.egg-info/PKG-INFO
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)      630 2024-04-10 21:16:54.000000 funktools-0.0.2/funktools.egg-info/SOURCES.txt
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)        1 2024-04-10 21:16:54.000000 funktools-0.0.2/funktools.egg-info/dependency_links.txt
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)      222 2024-04-10 21:16:54.000000 funktools-0.0.2/funktools.egg-info/requires.txt
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)       20 2024-04-10 21:16:54.000000 funktools-0.0.2/funktools.egg-info/top_level.txt
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)       38 2024-04-10 21:16:54.148966 funktools-0.0.2/setup.cfg
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)      767 2024-04-10 21:15:42.000000 funktools-0.0.2/setup.py
+drwxrwxr-x   0 modulo    (1000) modulo    (1000)        0 2024-04-10 21:16:54.148966 funktools-0.0.2/test/
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)        0 2024-04-04 23:04:39.000000 funktools-0.0.2/test/__init__.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     2380 2024-04-04 23:12:42.000000 funktools-0.0.2/test/test_base.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)    16960 2024-04-04 23:24:51.000000 funktools-0.0.2/test/test_cli.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     8326 2024-04-04 23:12:42.000000 funktools-0.0.2/test/test_lru_cache.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)      804 2024-04-04 23:12:42.000000 funktools-0.0.2/test/test_retry.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     4693 2024-04-04 23:12:42.000000 funktools-0.0.2/test/test_sqlite_cache.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     2839 2024-04-10 21:15:42.000000 funktools-0.0.2/test/test_template.py
+-rw-rw-r--   0 modulo    (1000) modulo    (1000)     2970 2024-04-04 23:12:42.000000 funktools-0.0.2/test/test_throttle.py
```

### Comparing `funktools-0.0.1/LICENSE` & `funktools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/demo/cli.py` & `funktools-0.0.2/demo/cli.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/demo/throttle.py` & `funktools-0.0.2/demo/throttle.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_base.py` & `funktools-0.0.2/funktools/_base.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_cli.py` & `funktools-0.0.2/funktools/_cli.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_log.py` & `funktools-0.0.2/funktools/_log.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_lru_cache.py` & `funktools-0.0.2/funktools/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_noop.py` & `funktools-0.0.2/funktools/_noop.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_retry.py` & `funktools-0.0.2/funktools/_retry.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_sqlite_cache.py` & `funktools-0.0.2/funktools/_sqlite_cache.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools/_throttle.py` & `funktools-0.0.2/funktools/_throttle.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/funktools.egg-info/SOURCES.txt` & `funktools-0.0.2/funktools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 funktools/_base.py
 funktools/_cli.py
 funktools/_log.py
 funktools/_lru_cache.py
 funktools/_noop.py
 funktools/_retry.py
 funktools/_sqlite_cache.py
+funktools/_template.py
 funktools/_throttle.py
 funktools.egg-info/PKG-INFO
 funktools.egg-info/SOURCES.txt
 funktools.egg-info/dependency_links.txt
 funktools.egg-info/requires.txt
 funktools.egg-info/top_level.txt
 test/__init__.py
 test/test_base.py
 test/test_cli.py
 test/test_lru_cache.py
 test/test_retry.py
 test/test_sqlite_cache.py
+test/test_template.py
 test/test_throttle.py
```

### Comparing `funktools-0.0.1/test/test_base.py` & `funktools-0.0.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/test/test_cli.py` & `funktools-0.0.2/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/test/test_lru_cache.py` & `funktools-0.0.2/test/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/test/test_retry.py` & `funktools-0.0.2/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/test/test_sqlite_cache.py` & `funktools-0.0.2/test/test_sqlite_cache.py`

 * *Files identical despite different names*

### Comparing `funktools-0.0.1/test/test_throttle.py` & `funktools-0.0.2/test/test_throttle.py`

 * *Files identical despite different names*

