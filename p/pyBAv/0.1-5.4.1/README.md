# Comparing `tmp/pyBAv-0.1.tar.gz` & `tmp/pyBAv-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBAv-0.1.tar", last modified: Wed Apr 10 16:47:22 2024, max compression
+gzip compressed data, was "pyBAv-5.4.1.tar", last modified: Wed Apr 10 16:42:24 2024, max compression
```

## Comparing `pyBAv-0.1.tar` & `pyBAv-5.4.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 16:47:22.837554 pyBAv-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-10 16:47:22.829623 pyBAv-0.1/BAv2/
--rw-rw-rw-   0        0        0    15212 2024-04-10 16:39:20.000000 pyBAv-0.1/BAv2/BAv2.py
--rw-rw-rw-   0        0        0      310 2024-04-10 16:16:56.000000 pyBAv-0.1/BAv2/__init__.py
--rw-rw-rw-   0        0        0      696 2024-04-10 16:47:22.835457 pyBAv-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4570 2024-04-10 08:56:15.000000 pyBAv-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 16:47:22.835457 pyBAv-0.1/pyBAv.egg-info/
--rw-rw-rw-   0        0        0      696 2024-04-10 16:47:22.000000 pyBAv-0.1/pyBAv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-10 16:47:22.000000 pyBAv-0.1/pyBAv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 16:47:22.000000 pyBAv-0.1/pyBAv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 16:47:22.000000 pyBAv-0.1/pyBAv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 16:47:22.837554 pyBAv-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-04-10 16:47:17.000000 pyBAv-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:42:24.767145 pyBAv-5.4.1/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:42:24.762132 pyBAv-5.4.1/BAv2/
+-rw-rw-rw-   0        0        0    15212 2024-04-10 16:39:20.000000 pyBAv-5.4.1/BAv2/BAv2.py
+-rw-rw-rw-   0        0        0      310 2024-04-10 16:16:56.000000 pyBAv-5.4.1/BAv2/__init__.py
+-rw-rw-rw-   0        0        0      878 2024-04-10 16:42:24.766134 pyBAv-5.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4570 2024-04-10 08:56:15.000000 pyBAv-5.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 16:42:24.766134 pyBAv-5.4.1/pyBAv.egg-info/
+-rw-rw-rw-   0        0        0      878 2024-04-10 16:42:24.000000 pyBAv-5.4.1/pyBAv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-10 16:42:24.000000 pyBAv-5.4.1/pyBAv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:42:24.000000 pyBAv-5.4.1/pyBAv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 16:42:24.000000 pyBAv-5.4.1/pyBAv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 16:42:24.000000 pyBAv-5.4.1/pyBAv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:42:24.767145 pyBAv-5.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1345 2024-04-10 16:42:21.000000 pyBAv-5.4.1/setup.py
```

### Comparing `pyBAv-0.1/BAv2/BAv2.py` & `pyBAv-5.4.1/BAv2/BAv2.py`

 * *Files identical despite different names*

### Comparing `pyBAv-0.1/README.md` & `pyBAv-5.4.1/README.md`

 * *Files identical despite different names*

