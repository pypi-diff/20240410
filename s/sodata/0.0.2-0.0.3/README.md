# Comparing `tmp/sodata-0.0.2.tar.gz` & `tmp/sodata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sodata-0.0.2.tar", last modified: Wed Apr 10 05:22:05 2024, max compression
+gzip compressed data, was "sodata-0.0.3.tar", last modified: Wed Apr 10 06:38:07 2024, max compression
```

## Comparing `sodata-0.0.2.tar` & `sodata-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 05:22:05.351116 sodata-0.0.2/
--rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 05:22:05.351116 sodata-0.0.2/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.2/README.md
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-10 05:22:05.351116 sodata-0.0.2/setup.cfg
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      343 2024-04-10 05:22:02.000000 sodata-0.0.2/setup.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 05:22:05.351116 sodata-0.0.2/sodata/
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       46 2024-04-09 13:11:40.000000 sodata-0.0.2/sodata/_init_.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      139 2024-04-09 12:56:22.000000 sodata-0.0.2/sodata/chunk_split.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     1959 2024-04-10 05:11:02.000000 sodata-0.0.2/sodata/file_process.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      141 2024-04-09 12:56:22.000000 sodata-0.0.2/sodata/text_clean.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 05:22:05.351116 sodata-0.0.2/sodata.egg-info/
--rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 05:22:05.000000 sodata-0.0.2/sodata.egg-info/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      250 2024-04-10 05:22:05.000000 sodata-0.0.2/sodata.egg-info/SOURCES.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-10 05:22:05.000000 sodata-0.0.2/sodata.egg-info/dependency_links.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       19 2024-04-10 05:22:05.000000 sodata-0.0.2/sodata.egg-info/requires.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-10 05:22:05.000000 sodata-0.0.2/sodata.egg-info/top_level.txt
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:38:07.780614 sodata-0.0.3/
+-rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 06:38:07.780614 sodata-0.0.3/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.3/README.md
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-10 06:38:07.780614 sodata-0.0.3/setup.cfg
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      343 2024-04-10 06:38:05.000000 sodata-0.0.3/setup.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:38:07.780614 sodata-0.0.3/sodata/
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      129 2024-04-10 06:25:35.000000 sodata-0.0.3/sodata/__init__.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      139 2024-04-09 12:56:22.000000 sodata-0.0.3/sodata/chunk_split.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     1959 2024-04-10 05:11:02.000000 sodata-0.0.3/sodata/file_process.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      141 2024-04-09 12:56:22.000000 sodata-0.0.3/sodata/text_clean.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-10 06:38:07.780614 sodata-0.0.3/sodata.egg-info/
+-rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      229 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      252 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       19 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/requires.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-10 06:38:07.000000 sodata-0.0.3/sodata.egg-info/top_level.txt
```

### Comparing `sodata-0.0.2/sodata/file_process.py` & `sodata-0.0.3/sodata/file_process.py`

 * *Files identical despite different names*

