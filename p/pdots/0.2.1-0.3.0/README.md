# Comparing `tmp/pdots-0.2.1.tar.gz` & `tmp/pdots-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdots-0.2.1.tar", max compression
+gzip compressed data, was "pdots-0.3.0.tar", max compression
```

## Comparing `pdots-0.2.1.tar` & `pdots-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      105 2024-02-07 09:30:51.517230 pdots-0.2.1/README.md
--rw-r--r--   0        0        0      791 2024-02-07 09:58:01.267155 pdots-0.2.1/pdots.py
--rw-r--r--   0        0        0      266 2024-02-07 09:58:01.267381 pdots-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      531 2024-02-07 09:58:02.803961 pdots-0.2.1/setup.py
--rw-r--r--   0        0        0      440 2024-02-07 09:58:02.804066 pdots-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      105 2024-02-07 09:30:51.517230 pdots-0.3.0/README.md
+-rw-r--r--   0        0        0      865 2024-04-10 08:48:52.923377 pdots-0.3.0/pdots.py
+-rw-r--r--   0        0        0      266 2024-04-10 08:48:52.923567 pdots-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      531 2024-04-10 08:48:59.573235 pdots-0.3.0/setup.py
+-rw-r--r--   0        0        0      440 2024-04-10 08:48:59.573340 pdots-0.3.0/PKG-INFO
```

### Comparing `pdots-0.2.1/setup.py` & `pdots-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['pdots']
 setup_kwargs = {
     'name': 'pdots',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Progress dots',
     'long_description': 'A simple, infinite progress indicator, as in: there is progress going on (and not: how far along are we)\n',
     'author': 'L3viathan',
     'author_email': 'git@l3vi.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

