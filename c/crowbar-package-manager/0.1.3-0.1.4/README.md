# Comparing `tmp/crowbar_package_manager-0.1.3.tar.gz` & `tmp/crowbar_package_manager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowbar_package_manager-0.1.3.tar", last modified: Tue Apr  9 20:04:38 2024, max compression
+gzip compressed data, was "crowbar_package_manager-0.1.4.tar", last modified: Tue Apr  9 23:19:40 2024, max compression
```

## Comparing `crowbar_package_manager-0.1.3.tar` & `crowbar_package_manager-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 20:04:38.312005 crowbar_package_manager-0.1.3/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 20:04:38.311865 crowbar_package_manager-0.1.3/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)       33 2024-04-06 18:48:23.000000 crowbar_package_manager-0.1.3/README.md
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 20:04:38.310598 crowbar_package_manager-0.1.3/crowbar/
--rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.3/crowbar/__init__.py
--rw-r--r--   0 coryfitz   (501) staff       (20)     4497 2024-04-09 19:45:07.000000 crowbar_package_manager-0.1.3/crowbar/crowbar.py
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 20:04:38.311501 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/
--rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/entry_points.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-09 20:04:38.000000 crowbar_package_manager-0.1.3/crowbar_package_manager.egg-info/top_level.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-09 20:04:38.312053 crowbar_package_manager-0.1.3/setup.cfg
--rw-r--r--   0 coryfitz   (501) staff       (20)      364 2024-04-09 20:01:14.000000 crowbar_package_manager-0.1.3/setup.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:19:40.144009 crowbar_package_manager-0.1.4/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 23:19:40.143896 crowbar_package_manager-0.1.4/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)       33 2024-04-06 18:48:23.000000 crowbar_package_manager-0.1.4/README.md
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:19:40.143050 crowbar_package_manager-0.1.4/crowbar/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.4/crowbar/__init__.py
+-rw-r--r--   0 coryfitz   (501) staff       (20)     7210 2024-04-09 23:19:15.000000 crowbar_package_manager-0.1.4/crowbar/crowbar.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-09 23:19:40.143732 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       67 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/entry_points.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-09 23:19:40.000000 crowbar_package_manager-0.1.4/crowbar_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-09 23:19:40.144055 crowbar_package_manager-0.1.4/setup.cfg
+-rw-r--r--   0 coryfitz   (501) staff       (20)      364 2024-04-09 23:08:49.000000 crowbar_package_manager-0.1.4/setup.py
```
