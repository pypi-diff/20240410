# Comparing `tmp/crowbar_package_manager-0.1.2.tar.gz` & `tmp/crowbar_package_manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowbar_package_manager-0.1.2.tar", last modified: Mon Apr  8 19:19:54 2024, max compression
+gzip compressed data, was "crowbar_package_manager-0.1.3.tar", last modified: Tue Apr  9 20:04:38 2024, max compression
```

## Comparing `crowbar_package_manager-0.1.2.tar` & `crowbar_package_manager-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 19:19:54.887535 crowbar_package_manager-0.1.2/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-08 19:19:54.887423 crowbar_package_manager-0.1.2/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)       33 2024-04-06 18:48:23.000000 crowbar_package_manager-0.1.2/README.md
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 19:19:54.886530 crowbar_package_manager-0.1.2/crowbar/
--rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.2/crowbar/__init__.py
--rw-r--r--   0 coryfitz   (501) staff       (20)     3186 2024-04-08 19:13:49.000000 crowbar_package_manager-0.1.2/crowbar/crowbar.py
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-08 19:19:54.887256 crowbar_package_manager-0.1.2/crowbar_package_manager.egg-info/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-08 19:19:54.000000 crowbar_package_manager-0.1.2/crowbar_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-08 19:19:54.000000 crowbar_package_manager-0.1.2/crowbar_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-08 19:19:54.000000 crowbar_package_manager-0.1.2/crowbar_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-08 19:19:54.000000 crowbar_package_manager-0.1.2/crowbar_package_manager.egg-info/entry_points.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-08 19:19:54.000000 crowbar_package_manager-0.1.2/crowbar_package_manager.egg-info/top_level.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-08 19:19:54.887578 crowbar_package_manager-0.1.2/setup.cfg
--rw-r--r--   0 coryfitz   (501) staff       (20)      364 2024-04-08 18:58:41.000000 crowbar_package_manager-0.1.2/setup.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 20:04:38.312005 crowbar_package_manager-0.1.3/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 20:04:38.311865 crowbar_package_manager-0.1.3/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)       33 2024-04-06 18:48:23.000000 crowbar_package_manager-0.1.3/README.md
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 20:04:38.310598 crowbar_package_manager-0.1.3/crowbar/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.3/crowbar/__init__.py
+-rw-r--r--   0 coryfitz   (501) staff       (20)     4497 2024-04-09 19:45:07.000000 crowbar_package_manager-0.1.3/crowbar/crowbar.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 20:04:38.311501 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/entry_points.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-09 20:04:38.312053 crowbar_package_manager-0.1.3/setup.cfg
+-rw-r--r--   0 coryfitz   (501) staff       (20)      364 2024-04-09 20:01:14.000000 crowbar_package_manager-0.1.3/setup.py
```

