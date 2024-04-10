# Comparing `tmp/vloc-0.1.15.tar.gz` & `tmp/vloc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc-0.1.15.tar", last modified: Tue Apr  9 08:08:13 2024, max compression
+gzip compressed data, was "vloc-0.1.9.tar", last modified: Tue Apr  9 04:08:57 2024, max compression
```

## Comparing `vloc-0.1.15.tar` & `vloc-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,14 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:08:13.026402 vloc-0.1.15/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 03:31:37.000000 vloc-0.1.15/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      493 2024-04-09 08:08:13.026158 vloc-0.1.15/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:32:50.000000 vloc-0.1.15/README.md
--rw-r--r--   0 byron      (501) staff       (20)      585 2024-04-09 08:08:04.000000 vloc-0.1.15/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 08:08:13.026448 vloc-0.1.15/setup.cfg
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:08:13.022694 vloc-0.1.15/vloc/
--rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 04:33:14.000000 vloc-0.1.15/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:08:13.024277 vloc-0.1.15/vloc/config/
--rw-r--r--   0 byron      (501) staff       (20)     2291 2024-04-08 03:52:10.000000 vloc-0.1.15/vloc/config/__config__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:31:37.000000 vloc-0.1.15/vloc/config/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)      801 2024-04-08 03:51:03.000000 vloc-0.1.15/vloc/config/catalog.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:08:13.025077 vloc-0.1.15/vloc/detect/
--rw-r--r--   0 byron      (501) staff       (20)      152 2024-04-08 09:28:17.000000 vloc-0.1.15/vloc/detect/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:31:37.000000 vloc-0.1.15/vloc/detect/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)     6208 2024-04-09 07:34:53.000000 vloc-0.1.15/vloc/detect/catalog.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:08:13.025563 vloc-0.1.15/vloc/exception/
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:31:37.000000 vloc-0.1.15/vloc/exception/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)      211 2024-04-08 03:31:37.000000 vloc-0.1.15/vloc/exception/catalog.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 08:08:13.025895 vloc-0.1.15/vloc.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      493 2024-04-09 08:08:13.000000 vloc-0.1.15/vloc.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      389 2024-04-09 08:08:13.000000 vloc-0.1.15/vloc.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 08:08:13.000000 vloc-0.1.15/vloc.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)       63 2024-04-09 08:08:13.000000 vloc-0.1.15/vloc.egg-info/requires.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 08:08:13.000000 vloc-0.1.15/vloc.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.549106 vloc-0.1.9/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 03:31:37.000000 vloc-0.1.9/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      482 2024-04-09 04:08:57.548887 vloc-0.1.9/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:32:50.000000 vloc-0.1.9/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      625 2024-04-09 04:08:12.000000 vloc-0.1.9/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 04:08:57.549143 vloc-0.1.9/setup.cfg
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.547789 vloc-0.1.9/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 03:59:47.000000 vloc-0.1.9/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.548685 vloc-0.1.9/vloc.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      482 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      192 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)       63 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/requires.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/top_level.txt
```

### Comparing `vloc-0.1.15/LICENSE.txt` & `vloc-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc-0.1.15/pyproject.toml` & `vloc-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.packages.find]
+include = ["vloc"]
 
 [project]
 name = "vloc"
-version = "0.1.15"
+version = "0.1.9"
 urls = { GitHub = "https://github.com/linyeh1129/vloc" }
 authors = [{ name = 'Lin Yeh', email = 'lin_yeh@outlook.com' }]
-description = "An UI antomation tool based by YOLO"
+description = "Plugin functions for vloc"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = "MIT" }
 keywords = ['ui aumomation', 'computer vision']
 classifiers = ['Programming Language :: Python :: 3']
 dependencies = [
     'opencv-python >= 4.9.0.80',
```

