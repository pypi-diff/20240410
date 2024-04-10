# Comparing `tmp/crowbar_package_manager-0.1.4.tar.gz` & `tmp/crowbar_package_manager-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowbar_package_manager-0.1.4.tar", last modified: Tue Apr  9 23:19:40 2024, max compression
+gzip compressed data, was "crowbar_package_manager-0.1.5.tar", last modified: Tue Apr  9 23:49:55 2024, max compression
```

## Comparing `crowbar_package_manager-0.1.4.tar` & `crowbar_package_manager-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:19:40.144009 crowbar_package_manager-0.1.4/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 23:19:40.143896 crowbar_package_manager-0.1.4/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)       33 2024-04-06 18:48:23.000000 crowbar_package_manager-0.1.4/README.md
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:19:40.143050 crowbar_package_manager-0.1.4/crowbar/
--rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.4/crowbar/__init__.py
--rw-r--r--   0 coryfitz   (501) staff       (20)     7210 2024-04-09 23:19:15.000000 crowbar_package_manager-0.1.4/crowbar/crowbar.py
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:19:40.143732 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/entry_points.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/top_level.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-09 23:19:40.144055 crowbar_package_manager-0.1.4/setup.cfg
--rw-r--r--   0 coryfitz   (501) staff       (20)      364 2024-04-09 23:08:49.000000 crowbar_package_manager-0.1.4/setup.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:49:55.481610 crowbar_package_manager-0.1.5/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1005 2024-04-09 23:49:55.481500 crowbar_package_manager-0.1.5/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      896 2024-04-09 23:41:35.000000 crowbar_package_manager-0.1.5/README.md
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:49:55.480510 crowbar_package_manager-0.1.5/crowbar/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.5/crowbar/__init__.py
+-rw-r--r--   0 coryfitz   (501) staff       (20)     7210 2024-04-09 23:19:15.000000 crowbar_package_manager-0.1.5/crowbar/crowbar.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:49:55.481329 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1005 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/entry_points.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-09 23:49:55.000000 crowbar_package_manager-0.1.5/crowbar_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-09 23:49:55.481655 crowbar_package_manager-0.1.5/setup.cfg
+-rw-r--r--   0 coryfitz   (501) staff       (20)      571 2024-04-09 23:49:38.000000 crowbar_package_manager-0.1.5/setup.py
```

### Comparing `crowbar_package_manager-0.1.4/crowbar/crowbar.py` & `crowbar_package_manager-0.1.5/crowbar/crowbar.py`

 * *Files identical despite different names*

