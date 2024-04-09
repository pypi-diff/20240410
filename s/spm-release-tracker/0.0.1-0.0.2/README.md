# Comparing `tmp/spm_release_tracker-0.0.1.tar.gz` & `tmp/spm_release_tracker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spm_release_tracker-0.0.1.tar", last modified: Tue Apr  9 23:17:28 2024, max compression
+gzip compressed data, was "spm_release_tracker-0.0.2.tar", last modified: Tue Apr  9 23:30:57 2024, max compression
```

## Comparing `spm_release_tracker-0.0.1.tar` & `spm_release_tracker-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:17:28.395783 spm_release_tracker-0.0.1/
--rw-r--r--   0 hugovanderlei   (501) staff       (20)     1071 2024-04-02 20:08:10.000000 spm_release_tracker-0.0.1/LICENSE
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-09 23:17:28.395589 spm_release_tracker-0.0.1/PKG-INFO
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       21 2024-04-02 20:08:10.000000 spm_release_tracker-0.0.1/README.md
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       38 2024-04-09 23:17:28.395821 spm_release_tracker-0.0.1/setup.cfg
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      354 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.1/setup.py
-drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:17:28.393958 spm_release_tracker-0.0.1/spm_release_tracker/
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       90 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.1/spm_release_tracker/__init__.py
--rw-r--r--   0 hugovanderlei   (501) staff       (20)     7467 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.1/spm_release_tracker/spm_release_tracker.py
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       22 2024-04-09 21:34:17.000000 spm_release_tracker-0.0.1/spm_release_tracker/version.py
-drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:17:28.395355 spm_release_tracker-0.0.1/spm_release_tracker.egg-info/
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-09 23:17:28.000000 spm_release_tracker-0.0.1/spm_release_tracker.egg-info/PKG-INFO
--rw-r--r--   0 hugovanderlei   (501) staff       (20)      392 2024-04-09 23:17:28.000000 spm_release_tracker-0.0.1/spm_release_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)        1 2024-04-09 23:17:28.000000 spm_release_tracker-0.0.1/spm_release_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       57 2024-04-09 23:17:28.000000 spm_release_tracker-0.0.1/spm_release_tracker.egg-info/entry_points.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       43 2024-04-09 23:17:28.000000 spm_release_tracker-0.0.1/spm_release_tracker.egg-info/requires.txt
--rw-r--r--   0 hugovanderlei   (501) staff       (20)       20 2024-04-09 23:17:28.000000 spm_release_tracker-0.0.1/spm_release_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:30:57.457300 spm_release_tracker-0.0.2/
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)     1071 2024-04-02 20:08:10.000000 spm_release_tracker-0.0.2/LICENSE
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-09 23:30:57.457095 spm_release_tracker-0.0.2/PKG-INFO
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       21 2024-04-02 20:08:10.000000 spm_release_tracker-0.0.2/README.md
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       38 2024-04-09 23:30:57.457343 spm_release_tracker-0.0.2/setup.cfg
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      378 2024-04-09 23:29:12.000000 spm_release_tracker-0.0.2/setup.py
+drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:30:57.455978 spm_release_tracker-0.0.2/spm_release_tracker/
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       90 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.2/spm_release_tracker/__init__.py
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)     7467 2024-04-09 20:58:00.000000 spm_release_tracker-0.0.2/spm_release_tracker/spm_release_tracker.py
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       22 2024-04-09 23:30:52.000000 spm_release_tracker-0.0.2/spm_release_tracker/version.py
+drwxr-xr-x   0 hugovanderlei   (501) staff       (20)        0 2024-04-09 23:30:57.456887 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      203 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)      392 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)        1 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       57 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       43 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/requires.txt
+-rw-r--r--   0 hugovanderlei   (501) staff       (20)       20 2024-04-09 23:30:57.000000 spm_release_tracker-0.0.2/spm_release_tracker.egg-info/top_level.txt
```

### Comparing `spm_release_tracker-0.0.1/LICENSE` & `spm_release_tracker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spm_release_tracker-0.0.1/spm_release_tracker/spm_release_tracker.py` & `spm_release_tracker-0.0.2/spm_release_tracker/spm_release_tracker.py`

 * *Files identical despite different names*

