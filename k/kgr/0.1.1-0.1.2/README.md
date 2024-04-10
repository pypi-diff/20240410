# Comparing `tmp/kgr-0.1.1.tar.gz` & `tmp/kgr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.1.1.tar", last modified: Wed Apr 10 15:32:53 2024, max compression
+gzip compressed data, was "kgr-0.1.2.tar", last modified: Wed Apr 10 15:42:16 2024, max compression
```

## Comparing `kgr-0.1.1.tar` & `kgr-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2024-04-10 14:38:49.000000 kgr-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2024-04-10 14:34:29.000000 kgr-0.1.1/README.md
--rw-r--r--   0        0        0      733 2024-04-10 15:32:53.094038 kgr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 14:21:46.000000 kgr-0.1.1/src/kgr/__init__.py
--rw-r--r--   0        0        0     8963 2024-04-10 14:22:03.000000 kgr-0.1.1/src/kgr/main.py
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 kgr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-10 14:38:49.000000 kgr-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-10 14:34:29.000000 kgr-0.1.2/README.md
+-rw-r--r--   0        0        0      729 2024-04-10 15:42:16.827299 kgr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 14:21:46.000000 kgr-0.1.2/src/kgr/__init__.py
+-rw-r--r--   0        0        0     8963 2024-04-10 14:22:03.000000 kgr-0.1.2/src/kgr/main.py
+-rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 kgr-0.1.2/PKG-INFO
```

### Comparing `kgr-0.1.1/LICENSE` & `kgr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.1.1/pyproject.toml` & `kgr-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
@@ -28,10 +28,10 @@
     "Operating System :: OS Independent",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.scripts]
-kgr = "kgr.main:main"
+kgr = "main:main"
 
 [tool]
```

### Comparing `kgr-0.1.1/src/kgr/main.py` & `kgr-0.1.2/src/kgr/main.py`

 * *Files identical despite different names*

### Comparing `kgr-0.1.1/PKG-INFO` & `kgr-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Miltitool for convert data from https://memopzk.org to Google Maps
 Author-Email: Dmitry Luschan <dluschan@gmail.com>
 Maintainer-Email: Dmitry Luschan <dluschan@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

