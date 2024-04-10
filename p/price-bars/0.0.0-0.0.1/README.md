# Comparing `tmp/price-bars-0.0.0.tar.gz` & `tmp/price-bars-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "price-bars-0.0.0.tar", last modified: Sun Apr  7 22:54:13 2024, max compression
+gzip compressed data, was "price-bars-0.0.1.tar", last modified: Wed Apr 10 20:17:55 2024, max compression
```

## Comparing `price-bars-0.0.0.tar` & `price-bars-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rory      (1000) rory      (1000)        0 2024-04-07 22:54:13.016639 price-bars-0.0.0/
--rw-r--r--   0 rory      (1000) rory      (1000)      380 2024-04-07 22:54:13.016639 price-bars-0.0.0/PKG-INFO
--rw-rw-r--   0 rory      (1000) rory      (1000)        0 2024-03-26 21:56:27.000000 price-bars-0.0.0/README.md
-drwxrwxr-x   0 rory      (1000) rory      (1000)        0 2024-04-07 22:54:13.016639 price-bars-0.0.0/bars/
--rw-rw-r--   0 rory      (1000) rory      (1000)        0 2024-03-26 22:04:09.000000 price-bars-0.0.0/bars/__init__.py
--rw-rw-r--   0 rory      (1000) rory      (1000)       71 2024-04-07 20:09:51.000000 price-bars-0.0.0/bars/domain.py
--rw-rw-r--   0 rory      (1000) rory      (1000)     2587 2024-04-07 20:09:51.000000 price-bars-0.0.0/bars/repository.py
-drwxrwxr-x   0 rory      (1000) rory      (1000)        0 2024-04-07 22:54:13.016639 price-bars-0.0.0/price_bars.egg-info/
--rw-r--r--   0 rory      (1000) rory      (1000)      380 2024-04-07 22:54:13.000000 price-bars-0.0.0/price_bars.egg-info/PKG-INFO
--rw-rw-r--   0 rory      (1000) rory      (1000)      244 2024-04-07 22:54:13.000000 price-bars-0.0.0/price_bars.egg-info/SOURCES.txt
--rw-rw-r--   0 rory      (1000) rory      (1000)        1 2024-04-07 22:54:13.000000 price-bars-0.0.0/price_bars.egg-info/dependency_links.txt
--rw-rw-r--   0 rory      (1000) rory      (1000)       53 2024-04-07 22:54:13.000000 price-bars-0.0.0/price_bars.egg-info/requires.txt
--rw-rw-r--   0 rory      (1000) rory      (1000)        5 2024-04-07 22:54:13.000000 price-bars-0.0.0/price_bars.egg-info/top_level.txt
--rw-rw-r--   0 rory      (1000) rory      (1000)      403 2024-04-07 22:54:05.000000 price-bars-0.0.0/pyproject.toml
--rw-rw-r--   0 rory      (1000) rory      (1000)       38 2024-04-07 22:54:13.016639 price-bars-0.0.0/setup.cfg
+drwxrwxr-x   0 rory      (1000) rory      (1000)        0 2024-04-10 20:17:55.638251 price-bars-0.0.1/
+-rw-r--r--   0 rory      (1000) rory      (1000)      413 2024-04-10 20:17:55.638251 price-bars-0.0.1/PKG-INFO
+-rw-rw-r--   0 rory      (1000) rory      (1000)       32 2024-04-07 22:55:01.000000 price-bars-0.0.1/README.md
+drwxrwxr-x   0 rory      (1000) rory      (1000)        0 2024-04-10 20:17:55.638251 price-bars-0.0.1/bars/
+-rw-rw-r--   0 rory      (1000) rory      (1000)        0 2024-03-26 22:04:09.000000 price-bars-0.0.1/bars/__init__.py
+-rw-rw-r--   0 rory      (1000) rory      (1000)       71 2024-04-07 20:09:51.000000 price-bars-0.0.1/bars/domain.py
+-rw-rw-r--   0 rory      (1000) rory      (1000)     2587 2024-04-07 20:09:51.000000 price-bars-0.0.1/bars/repository.py
+drwxrwxr-x   0 rory      (1000) rory      (1000)        0 2024-04-10 20:17:55.638251 price-bars-0.0.1/price_bars.egg-info/
+-rw-r--r--   0 rory      (1000) rory      (1000)      413 2024-04-10 20:17:55.000000 price-bars-0.0.1/price_bars.egg-info/PKG-INFO
+-rw-rw-r--   0 rory      (1000) rory      (1000)      244 2024-04-10 20:17:55.000000 price-bars-0.0.1/price_bars.egg-info/SOURCES.txt
+-rw-rw-r--   0 rory      (1000) rory      (1000)        1 2024-04-10 20:17:55.000000 price-bars-0.0.1/price_bars.egg-info/dependency_links.txt
+-rw-rw-r--   0 rory      (1000) rory      (1000)       53 2024-04-10 20:17:55.000000 price-bars-0.0.1/price_bars.egg-info/requires.txt
+-rw-rw-r--   0 rory      (1000) rory      (1000)        5 2024-04-10 20:17:55.000000 price-bars-0.0.1/price_bars.egg-info/top_level.txt
+-rw-rw-r--   0 rory      (1000) rory      (1000)      403 2024-04-10 20:17:36.000000 price-bars-0.0.1/pyproject.toml
+-rw-rw-r--   0 rory      (1000) rory      (1000)       38 2024-04-10 20:17:55.638251 price-bars-0.0.1/setup.cfg
```

### Comparing `price-bars-0.0.0/bars/repository.py` & `price-bars-0.0.1/bars/repository.py`

 * *Files identical despite different names*

