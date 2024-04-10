# Comparing `tmp/ilovetea-0.1.0.tar.gz` & `tmp/ilovetea-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilovetea-0.1.0.tar", last modified: Wed Apr 10 02:55:08 2024, max compression
+gzip compressed data, was "ilovetea-0.1.1.tar", last modified: Wed Apr 10 03:33:54 2024, max compression
```

## Comparing `ilovetea-0.1.0.tar` & `ilovetea-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:55:08.078139 ilovetea-0.1.0/
--rw-rw-rw-   0        0        0      398 2024-04-10 02:55:08.077169 ilovetea-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       41 2024-04-10 02:32:10.000000 ilovetea-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 02:55:08.072139 ilovetea-0.1.0/ilovetea.egg-info/
--rw-rw-rw-   0        0        0      398 2024-04-10 02:55:07.000000 ilovetea-0.1.0/ilovetea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-04-10 02:55:08.000000 ilovetea-0.1.0/ilovetea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:55:07.000000 ilovetea-0.1.0/ilovetea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:55:07.000000 ilovetea-0.1.0/ilovetea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:55:08.080138 ilovetea-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      394 2024-04-10 02:54:43.000000 ilovetea-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:33:54.913366 ilovetea-0.1.1/
+-rw-rw-rw-   0        0        0    35802 2024-04-10 03:09:07.000000 ilovetea-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      421 2024-04-10 03:33:54.911365 ilovetea-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2024-04-10 02:32:10.000000 ilovetea-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 03:33:54.902367 ilovetea-0.1.1/ilovetea.egg-info/
+-rw-rw-rw-   0        0        0      421 2024-04-10 03:33:54.000000 ilovetea-0.1.1/ilovetea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2024-04-10 03:33:54.000000 ilovetea-0.1.1/ilovetea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:33:54.000000 ilovetea-0.1.1/ilovetea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:33:54.000000 ilovetea-0.1.1/ilovetea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:33:54.935885 ilovetea-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      394 2024-04-10 03:31:32.000000 ilovetea-0.1.1/setup.py
```

