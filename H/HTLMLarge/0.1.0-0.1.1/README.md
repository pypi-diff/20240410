# Comparing `tmp/HTLMLarge-0.1.0.tar.gz` & `tmp/HTLMLarge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTLMLarge-0.1.0.tar", last modified: Wed Apr 10 07:59:55 2024, max compression
+gzip compressed data, was "HTLMLarge-0.1.1.tar", last modified: Wed Apr 10 08:08:34 2024, max compression
```

## Comparing `HTLMLarge-0.1.0.tar` & `HTLMLarge-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 07:59:55.345105 HTLMLarge-0.1.0/
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 07:59:55.344193 HTLMLarge-0.1.0/HTLMLarge.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)       53 2024-04-10 07:59:55.000000 HTLMLarge-0.1.0/HTLMLarge.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      232 2024-04-10 07:59:55.000000 HTLMLarge-0.1.0/HTLMLarge.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-10 07:59:55.000000 HTLMLarge-0.1.0/HTLMLarge.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        9 2024-04-10 07:59:55.000000 HTLMLarge-0.1.0/HTLMLarge.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       15 2024-04-10 07:59:55.000000 HTLMLarge-0.1.0/HTLMLarge.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       53 2024-04-10 07:59:55.344853 HTLMLarge-0.1.0/PKG-INFO
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 07:59:55.344507 HTLMLarge-0.1.0/rtra_connector/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-10 07:52:46.000000 HTLMLarge-0.1.0/rtra_connector/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)     1648 2024-04-10 07:53:10.000000 HTLMLarge-0.1.0/rtra_connector/rtra_connector.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-10 07:59:55.345156 HTLMLarge-0.1.0/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      177 2024-04-10 07:59:27.000000 HTLMLarge-0.1.0/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 08:08:34.782476 HTLMLarge-0.1.1/
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 08:08:34.778806 HTLMLarge-0.1.1/HTLMLarge.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       53 2024-04-10 08:08:34.000000 HTLMLarge-0.1.1/HTLMLarge.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      228 2024-04-10 08:08:34.000000 HTLMLarge-0.1.1/HTLMLarge.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-10 08:08:34.000000 HTLMLarge-0.1.1/HTLMLarge.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        9 2024-04-10 08:08:34.000000 HTLMLarge-0.1.1/HTLMLarge.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       15 2024-04-10 08:08:34.000000 HTLMLarge-0.1.1/HTLMLarge.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       53 2024-04-10 08:08:34.779403 HTLMLarge-0.1.1/PKG-INFO
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 08:08:34.779052 HTLMLarge-0.1.1/rtra_connector/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-10 07:52:46.000000 HTLMLarge-0.1.1/rtra_connector/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     1648 2024-04-10 07:53:10.000000 HTLMLarge-0.1.1/rtra_connector/htlmupward.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-10 08:08:34.782656 HTLMLarge-0.1.1/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      177 2024-04-10 08:08:19.000000 HTLMLarge-0.1.1/setup.py
```

### Comparing `HTLMLarge-0.1.0/rtra_connector/rtra_connector.py` & `HTLMLarge-0.1.1/rtra_connector/htlmupward.py`

 * *Files identical despite different names*

