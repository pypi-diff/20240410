# Comparing `tmp/mov-cli-test-1.1.0.tar.gz` & `tmp/mov-cli-test-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-test-1.1.0.tar", last modified: Tue Mar 26 18:21:41 2024, max compression
+gzip compressed data, was "mov-cli-test-1.1.1.tar", last modified: Mon Apr  8 23:38:44 2024, max compression
```

## Comparing `mov-cli-test-1.1.0.tar` & `mov-cli-test-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-26 18:21:41.150911 mov-cli-test-1.1.0/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1062 2024-03-02 20:16:40.000000 mov-cli-test-1.1.0/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-03-26 18:21:41.150911 mov-cli-test-1.1.0/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      532 2024-03-26 18:16:37.000000 mov-cli-test-1.1.0/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-26 18:21:41.147578 mov-cli-test-1.1.0/mov_cli_test/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      313 2024-03-26 18:16:51.000000 mov-cli-test-1.1.0/mov_cli_test/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4275 2024-03-26 18:20:06.000000 mov-cli-test-1.1.0/mov_cli_test/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-26 18:21:41.147578 mov-cli-test-1.1.0/mov_cli_test.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-03-26 18:21:41.000000 mov-cli-test-1.1.0/mov_cli_test.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      260 2024-03-26 18:21:41.000000 mov-cli-test-1.1.0/mov_cli_test.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-03-26 18:21:41.000000 mov-cli-test-1.1.0/mov_cli_test.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      114 2024-03-26 18:21:41.000000 mov-cli-test-1.1.0/mov_cli_test.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       13 2024-03-26 18:21:41.000000 mov-cli-test-1.1.0/mov_cli_test.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1395 2024-03-26 17:26:10.000000 mov-cli-test-1.1.0/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-03-26 18:21:41.150911 mov-cli-test-1.1.0/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 23:38:44.376108 mov-cli-test-1.1.1/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1062 2024-03-02 20:16:40.000000 mov-cli-test-1.1.1/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-08 23:38:44.376108 mov-cli-test-1.1.1/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      532 2024-03-26 18:16:37.000000 mov-cli-test-1.1.1/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 23:38:44.376108 mov-cli-test-1.1.1/mov_cli_test/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      350 2024-04-08 23:38:17.000000 mov-cli-test-1.1.1/mov_cli_test/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4275 2024-03-26 18:20:06.000000 mov-cli-test-1.1.1/mov_cli_test/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-08 23:38:44.376108 mov-cli-test-1.1.1/mov_cli_test.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-08 23:38:44.000000 mov-cli-test-1.1.1/mov_cli_test.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      260 2024-04-08 23:38:44.000000 mov-cli-test-1.1.1/mov_cli_test.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-08 23:38:44.000000 mov-cli-test-1.1.1/mov_cli_test.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      114 2024-04-08 23:38:44.000000 mov-cli-test-1.1.1/mov_cli_test.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       13 2024-04-08 23:38:44.000000 mov-cli-test-1.1.1/mov_cli_test.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1395 2024-03-26 17:26:10.000000 mov-cli-test-1.1.1/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-08 23:38:44.376108 mov-cli-test-1.1.1/setup.cfg
```

### Comparing `mov-cli-test-1.1.0/LICENSE` & `mov-cli-test-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-test-1.1.0/PKG-INFO` & `mov-cli-test-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.0
+Version: 1.1.1
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-test-1.1.0/README.md` & `mov-cli-test-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mov-cli-test-1.1.0/mov_cli_test/scraper.py` & `mov-cli-test-1.1.1/mov_cli_test/scraper.py`

 * *Files identical despite different names*

### Comparing `mov-cli-test-1.1.0/mov_cli_test.egg-info/PKG-INFO` & `mov-cli-test-1.1.1/mov_cli_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.0
+Version: 1.1.1
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-test-1.1.0/pyproject.toml` & `mov-cli-test-1.1.1/pyproject.toml`

 * *Files identical despite different names*

