# Comparing `tmp/ml_runlog-2.0.tar.gz` & `tmp/ml_runlog-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_runlog-2.0.tar", last modified: Wed Apr 10 02:33:36 2024, max compression
+gzip compressed data, was "ml_runlog-2.1.tar", last modified: Wed Apr 10 03:46:10 2024, max compression
```

## Comparing `ml_runlog-2.0.tar` & `ml_runlog-2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 02:33:36.393025 ml_runlog-2.0/
--rw-rw-r--   0 anag      (1000) anag      (1000)    35149 2024-04-09 05:52:10.000000 ml_runlog-2.0/LICENSE
--rw-r--r--   0 anag      (1000) anag      (1000)      398 2024-04-10 02:33:36.393025 ml_runlog-2.0/PKG-INFO
--rw-rw-r--   0 anag      (1000) anag      (1000)     1827 2024-04-09 03:18:50.000000 ml_runlog-2.0/README.md
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 02:33:36.393025 ml_runlog-2.0/ml_runlog/
--rw-rw-r--   0 anag      (1000) anag      (1000)       78 2024-04-10 01:21:01.000000 ml_runlog-2.0/ml_runlog/__init__.py
--rw-rw-r--   0 anag      (1000) anag      (1000)     2511 2024-04-10 02:22:59.000000 ml_runlog-2.0/ml_runlog/main.py
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 02:33:36.393025 ml_runlog-2.0/ml_runlog.egg-info/
--rw-r--r--   0 anag      (1000) anag      (1000)      398 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/PKG-INFO
--rw-rw-r--   0 anag      (1000) anag      (1000)      262 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/SOURCES.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/dependency_links.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 06:00:46.000000 ml_runlog-2.0/ml_runlog.egg-info/not-zip-safe
--rw-rw-r--   0 anag      (1000) anag      (1000)       17 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/requires.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)       10 2024-04-10 02:33:36.000000 ml_runlog-2.0/ml_runlog.egg-info/top_level.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)       38 2024-04-10 02:33:36.393025 ml_runlog-2.0/setup.cfg
--rw-rw-r--   0 anag      (1000) anag      (1000)      518 2024-04-10 02:32:26.000000 ml_runlog-2.0/setup.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 03:46:10.788205 ml_runlog-2.1/
+-rw-rw-r--   0 anag      (1000) anag      (1000)    35149 2024-04-09 05:52:10.000000 ml_runlog-2.1/LICENSE
+-rw-r--r--   0 anag      (1000) anag      (1000)      398 2024-04-10 03:46:10.788205 ml_runlog-2.1/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)     1827 2024-04-09 03:18:50.000000 ml_runlog-2.1/README.md
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 03:46:10.788205 ml_runlog-2.1/ml_runlog/
+-rw-rw-r--   0 anag      (1000) anag      (1000)       78 2024-04-10 01:21:01.000000 ml_runlog-2.1/ml_runlog/__init__.py
+-rw-rw-r--   0 anag      (1000) anag      (1000)     3091 2024-04-10 03:31:48.000000 ml_runlog-2.1/ml_runlog/main.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-10 03:46:10.788205 ml_runlog-2.1/ml_runlog.egg-info/
+-rw-r--r--   0 anag      (1000) anag      (1000)      398 2024-04-10 03:46:10.000000 ml_runlog-2.1/ml_runlog.egg-info/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)      262 2024-04-10 03:46:10.000000 ml_runlog-2.1/ml_runlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-10 03:46:10.000000 ml_runlog-2.1/ml_runlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 06:00:46.000000 ml_runlog-2.1/ml_runlog.egg-info/not-zip-safe
+-rw-rw-r--   0 anag      (1000) anag      (1000)       17 2024-04-10 03:46:10.000000 ml_runlog-2.1/ml_runlog.egg-info/requires.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       10 2024-04-10 03:46:10.000000 ml_runlog-2.1/ml_runlog.egg-info/top_level.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       38 2024-04-10 03:46:10.788205 ml_runlog-2.1/setup.cfg
+-rw-rw-r--   0 anag      (1000) anag      (1000)      518 2024-04-10 03:46:01.000000 ml_runlog-2.1/setup.py
```

### Comparing `ml_runlog-2.0/LICENSE` & `ml_runlog-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_runlog-2.0/README.md` & `ml_runlog-2.1/README.md`

 * *Files identical despite different names*

### Comparing `ml_runlog-2.0/setup.py` & `ml_runlog-2.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='ml_runlog',
-      version='2.0',
+      version='2.1',
       description='Simple script to log experiments to Google Sheets. Version 2.0 is cleaner, has a class based structure and supports logging multiple rows at once.',
       url='https://github.com/anag004/ml-runlog',
       author='Ananye Agarwal',
       author_email='ananayagarwal@gmail.com',
       license='MIT',
       packages=['ml_runlog'],
       install_requires=[
```

