# Comparing `tmp/llmreader-0.2.6.tar.gz` & `tmp/llmreader-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreader-0.2.6.tar", last modified: Wed Apr 10 03:21:00 2024, max compression
+gzip compressed data, was "llmreader-0.2.7.tar", last modified: Wed Apr 10 03:23:11 2024, max compression
```

## Comparing `llmreader-0.2.6.tar` & `llmreader-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-10 03:21:00.180841 llmreader-0.2.6/
--rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.6/LICENSE
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-10 03:21:00.180695 llmreader-0.2.6/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.6/README.md
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-10 03:21:00.179599 llmreader-0.2.6/llmreader/
--rw-r--r--   0 ethanhou   (501) staff       (20)       54 2024-04-04 02:21:26.000000 llmreader-0.2.6/llmreader/__init__.py
--rw-r--r--   0 ethanhou   (501) staff       (20)     4717 2024-04-10 03:20:31.000000 llmreader-0.2.6/llmreader/inject.py
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-10 03:21:00.180476 llmreader-0.2.6/llmreader.egg-info/
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-10 03:21:00.000000 llmreader-0.2.6/llmreader.egg-info/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)      232 2024-04-10 03:21:00.000000 llmreader-0.2.6/llmreader.egg-info/SOURCES.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-10 03:21:00.000000 llmreader-0.2.6/llmreader.egg-info/dependency_links.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        7 2024-04-10 03:21:00.000000 llmreader-0.2.6/llmreader.egg-info/requires.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)       10 2024-04-10 03:21:00.000000 llmreader-0.2.6/llmreader.egg-info/top_level.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-10 03:21:00.180902 llmreader-0.2.6/setup.cfg
--rw-r--r--   0 ethanhou   (501) staff       (20)      532 2024-04-10 00:53:46.000000 llmreader-0.2.6/setup.py
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-10 03:23:11.527003 llmreader-0.2.7/
+-rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.7/LICENSE
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-10 03:23:11.526873 llmreader-0.2.7/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.7/README.md
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-10 03:23:11.525895 llmreader-0.2.7/llmreader/
+-rw-r--r--   0 ethanhou   (501) staff       (20)       53 2024-04-10 03:23:01.000000 llmreader-0.2.7/llmreader/__init__.py
+-rw-r--r--   0 ethanhou   (501) staff       (20)     4717 2024-04-10 03:20:31.000000 llmreader-0.2.7/llmreader/inject.py
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-10 03:23:11.526699 llmreader-0.2.7/llmreader.egg-info/
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-10 03:23:11.000000 llmreader-0.2.7/llmreader.egg-info/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)      232 2024-04-10 03:23:11.000000 llmreader-0.2.7/llmreader.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-10 03:23:11.000000 llmreader-0.2.7/llmreader.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        7 2024-04-10 03:23:11.000000 llmreader-0.2.7/llmreader.egg-info/requires.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)       10 2024-04-10 03:23:11.000000 llmreader-0.2.7/llmreader.egg-info/top_level.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-10 03:23:11.527053 llmreader-0.2.7/setup.cfg
+-rw-r--r--   0 ethanhou   (501) staff       (20)      532 2024-04-10 03:23:05.000000 llmreader-0.2.7/setup.py
```

### Comparing `llmreader-0.2.6/LICENSE` & `llmreader-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llmreader-0.2.6/llmreader/inject.py` & `llmreader-0.2.7/llmreader/inject.py`

 * *Files identical despite different names*

### Comparing `llmreader-0.2.6/setup.py` & `llmreader-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="llmreader",
-    version="0.2.6",
+    version="0.2.7",
     description="Intercept OpenAI inputs",
     author="Ethan Hou",
     author_email="ethanfhou10@gmail.com",
     packages=find_packages(),
     install_requires=[
         'openai'
     ],
```

