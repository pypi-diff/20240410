# Comparing `tmp/scrachy-0.5.9.tar.gz` & `tmp/scrachy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrachy-0.5.9.tar", last modified: Wed Dec 13 18:00:09 2023, max compression
+gzip compressed data, was "scrachy-0.7.0.tar", last modified: Wed Apr 10 20:07:34 2024, max compression
```

## Comparing `scrachy-0.5.9.tar` & `scrachy-0.7.0.tar`

### file list

```diff
@@ -1,85 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.626565 scrachy-0.5.9/
--rw-rw-rw-   0        0        0     7382 2020-09-17 15:54:11.000000 scrachy-0.5.9/LICENSE.md
--rw-rw-rw-   0        0        0       70 2020-09-19 16:00:35.000000 scrachy-0.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5202 2023-12-13 18:00:09.625562 scrachy-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     3010 2023-11-28 15:58:30.000000 scrachy-0.5.9/README.md
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.563807 scrachy-0.5.9/scrachy/
--rw-rw-rw-   0        0        0      975 2023-12-13 17:55:04.000000 scrachy-0.5.9/scrachy/__init__.py
--rw-rw-rw-   0        0        0     3093 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/addons.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.572181 scrachy-0.5.9/scrachy/cli/
--rw-rw-rw-   0        0        0      812 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/cli/__init__.py
--rw-rw-rw-   0        0        0    14340 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/cli/benchmark.py
--rw-rw-rw-   0        0        0     5521 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/cli/webdriver_server.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.575299 scrachy-0.5.9/scrachy/content/
--rw-rw-rw-   0        0        0     1541 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/content/__init__.py
--rw-rw-rw-   0        0        0     2406 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/content/boilerpipe.py
--rw-rw-rw-   0        0        0     2850 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/content/bs4.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.580549 scrachy-0.5.9/scrachy/db/
--rw-rw-rw-   0        0        0      881 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/db/__init__.py
--rw-rw-rw-   0        0        0     8359 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/db/base.py
--rw-rw-rw-   0        0        0     2995 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/db/engine.py
--rw-rw-rw-   0        0        0     5268 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/db/models.py
--rw-rw-rw-   0        0        0     6483 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/db/repositories.py
--rw-rw-rw-   0        0        0      961 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/exceptions.py
--rw-rw-rw-   0        0        0     5110 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/http_.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.584705 scrachy-0.5.9/scrachy/middleware/
--rw-rw-rw-   0        0        0      814 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/middleware/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/middleware/filter.py
--rw-rw-rw-   0        0        0    23429 2023-12-10 23:07:33.000000 scrachy-0.5.9/scrachy/middleware/httpcache.py
--rw-rw-rw-   0        0        0    12014 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/middleware/selenium.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.585731 scrachy-0.5.9/scrachy/settings/
--rw-rw-rw-   0        0        0     1542 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.591018 scrachy-0.5.9/scrachy/settings/defaults/
--rw-rw-rw-   0        0        0      849 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/settings/defaults/__init__.py
--rw-rw-rw-   0        0        0     1086 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/settings/defaults/filter.py
--rw-rw-rw-   0        0        0     1273 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/settings/defaults/fingerprinter.py
--rw-rw-rw-   0        0        0     1643 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/settings/defaults/policy.py
--rw-rw-rw-   0        0        0     1797 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/settings/defaults/selenium.py
--rw-rw-rw-   0        0        0     7992 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/settings/defaults/storage.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.603571 scrachy-0.5.9/scrachy/utils/
--rw-rw-rw-   0        0        0      845 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/__init__.py
--rw-rw-rw-   0        0        0     1095 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/datetime.py
--rw-rw-rw-   0        0        0     1356 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/db.py
--rw-rw-rw-   0        0        0     2164 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/hash.py
--rw-rw-rw-   0        0        0     1248 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/imports.py
--rw-rw-rw-   0        0        0     2261 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/numeric.py
--rw-rw-rw-   0        0        0     8442 2023-11-28 17:57:57.000000 scrachy-0.5.9/scrachy/utils/request.py
--rw-rw-rw-   0        0        0     5166 2023-12-10 22:31:28.000000 scrachy-0.5.9/scrachy/utils/selenium.py
--rw-rw-rw-   0        0        0     1128 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/settings.py
--rw-rw-rw-   0        0        0     2144 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/sqltypes.py
--rw-rw-rw-   0        0        0     1007 2023-11-28 15:58:30.000000 scrachy-0.5.9/scrachy/utils/strings.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.623465 scrachy-0.5.9/scrachy.egg-info/
--rw-rw-rw-   0        0        0     5202 2023-12-13 18:00:09.000000 scrachy-0.5.9/scrachy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1889 2023-12-13 18:00:09.000000 scrachy-0.5.9/scrachy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-13 18:00:09.000000 scrachy-0.5.9/scrachy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2020-09-19 15:20:56.000000 scrachy-0.5.9/scrachy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      369 2023-12-13 18:00:09.000000 scrachy-0.5.9/scrachy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-12-13 18:00:09.000000 scrachy-0.5.9/scrachy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-13 18:00:09.626565 scrachy-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0     2697 2023-12-13 17:55:04.000000 scrachy-0.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.606707 scrachy-0.5.9/test/
--rw-rw-rw-   0        0        0      780 2020-09-19 00:56:02.000000 scrachy-0.5.9/test/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-11-28 17:53:01.000000 scrachy-0.5.9/test/conftest.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.608832 scrachy-0.5.9/test/integration/
--rw-rw-rw-   0        0        0      780 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/__init__.py
--rw-rw-rw-   0        0        0     1416 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/conftest.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.612027 scrachy-0.5.9/test/integration/db/
--rw-rw-rw-   0        0        0      780 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/db/__init__.py
--rw-rw-rw-   0        0        0      780 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/db/conftest.py
--rw-rw-rw-   0        0        0     3866 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/db/test_repositories.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.619269 scrachy-0.5.9/test/integration/middleware/
--rw-rw-rw-   0        0        0      780 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/conftest.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.619269 scrachy-0.5.9/test/integration/middleware/httpcache/
--rw-rw-rw-   0        0        0      780 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/httpcache/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.620299 scrachy-0.5.9/test/integration/middleware/selenium/
--rw-rw-rw-   0        0        0      780 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/selenium/__init__.py
--rw-rw-rw-   0        0        0     5449 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/test_async_selenium.py
--rw-rw-rw-   0        0        0     4999 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/test_cache_filter.py
--rw-rw-rw-   0        0        0     6575 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/test_selenium.py
--rw-rw-rw-   0        0        0     9042 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/integration/middleware/test_storage.py
-drwxrwxrwx   0        0        0        0 2023-12-13 18:00:09.622408 scrachy-0.5.9/test/unit/
--rw-rw-rw-   0        0        0      780 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/unit/__init__.py
--rw-rw-rw-   0        0        0     5878 2023-11-28 17:57:42.000000 scrachy-0.5.9/test/unit/test_expiration_manager.py
--rw-rw-rw-   0        0        0     2129 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/unit/test_utils.py
--rw-rw-rw-   0        0        0     4470 2023-11-28 15:58:30.000000 scrachy-0.5.9/test/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.621859 scrachy-0.7.0/
+-rw-rw-rw-   0        0        0     7382 2024-01-30 23:58:38.000000 scrachy-0.7.0/LICENSE.md
+-rw-rw-rw-   0        0        0       70 2024-01-30 23:58:38.000000 scrachy-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12495 2024-04-10 20:07:34.621859 scrachy-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3010 2024-01-30 23:58:38.000000 scrachy-0.7.0/README.md
+-rw-rw-rw-   0        0        0     1118 2024-04-10 20:03:28.000000 scrachy-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 20:07:34.622857 scrachy-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.583858 scrachy-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.591325 scrachy-0.7.0/src/scrachy/
+-rw-rw-rw-   0        0        0      975 2024-04-10 20:03:28.000000 scrachy-0.7.0/src/scrachy/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/addons.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.597325 scrachy-0.7.0/src/scrachy/cli/
+-rw-rw-rw-   0        0        0      812 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/cli/__init__.py
+-rw-rw-rw-   0        0        0    14340 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/cli/benchmark.py
+-rw-rw-rw-   0        0        0     6003 2024-01-31 01:26:54.000000 scrachy-0.7.0/src/scrachy/cli/webdriver_server.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.599324 scrachy-0.7.0/src/scrachy/content/
+-rw-rw-rw-   0        0        0     1541 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/content/__init__.py
+-rw-rw-rw-   0        0        0     2406 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/content/boilerpipe.py
+-rw-rw-rw-   0        0        0     2850 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/content/bs4.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.602324 scrachy-0.7.0/src/scrachy/db/
+-rw-rw-rw-   0        0        0      881 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/db/__init__.py
+-rw-rw-rw-   0        0        0     2391 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/db/base.py
+-rw-rw-rw-   0        0        0     2995 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/db/engine.py
+-rw-rw-rw-   0        0        0     5360 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/db/models.py
+-rw-rw-rw-   0        0        0     6518 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/db/repositories.py
+-rw-rw-rw-   0        0        0      961 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/exceptions.py
+-rw-rw-rw-   0        0        0     4027 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/http_.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.605331 scrachy-0.7.0/src/scrachy/middleware/
+-rw-rw-rw-   0        0        0      814 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/middleware/__init__.py
+-rw-rw-rw-   0        0        0     4871 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/middleware/filter.py
+-rw-rw-rw-   0        0        0    24775 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/middleware/httpcache.py
+-rw-rw-rw-   0        0        0    17227 2024-01-31 01:26:54.000000 scrachy-0.7.0/src/scrachy/middleware/selenium.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.605331 scrachy-0.7.0/src/scrachy/settings/
+-rw-rw-rw-   0        0        0     1542 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.611289 scrachy-0.7.0/src/scrachy/settings/defaults/
+-rw-rw-rw-   0        0        0      849 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/settings/defaults/__init__.py
+-rw-rw-rw-   0        0        0     1086 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/settings/defaults/filter.py
+-rw-rw-rw-   0        0        0     1273 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/settings/defaults/fingerprinter.py
+-rw-rw-rw-   0        0        0     1643 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/settings/defaults/policy.py
+-rw-rw-rw-   0        0        0     2825 2024-01-31 01:26:54.000000 scrachy-0.7.0/src/scrachy/settings/defaults/selenium.py
+-rw-rw-rw-   0        0        0     7992 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/settings/defaults/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.618857 scrachy-0.7.0/src/scrachy/utils/
+-rw-rw-rw-   0        0        0      845 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1095 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/datetime.py
+-rw-rw-rw-   0        0        0     1356 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/db.py
+-rw-rw-rw-   0        0        0     2164 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/hash.py
+-rw-rw-rw-   0        0        0     1248 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/imports.py
+-rw-rw-rw-   0        0        0     2261 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/numeric.py
+-rw-rw-rw-   0        0        0     8442 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/request.py
+-rw-rw-rw-   0        0        0    10412 2024-01-31 16:53:30.000000 scrachy-0.7.0/src/scrachy/utils/selenium.py
+-rw-rw-rw-   0        0        0     1128 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/settings.py
+-rw-rw-rw-   0        0        0     3029 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/sqltypes.py
+-rw-rw-rw-   0        0        0     1007 2024-01-30 23:58:38.000000 scrachy-0.7.0/src/scrachy/utils/strings.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:07:34.619858 scrachy-0.7.0/src/scrachy.egg-info/
+-rw-rw-rw-   0        0        0    12495 2024-04-10 20:07:34.000000 scrachy-0.7.0/src/scrachy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1371 2024-04-10 20:07:34.000000 scrachy-0.7.0/src/scrachy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 20:07:34.000000 scrachy-0.7.0/src/scrachy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      334 2024-04-10 20:07:34.000000 scrachy-0.7.0/src/scrachy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 20:07:34.000000 scrachy-0.7.0/src/scrachy.egg-info/top_level.txt
```

### Comparing `scrachy-0.5.9/LICENSE.md` & `scrachy-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/README.md` & `scrachy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/__init__.py` & `scrachy-0.7.0/src/scrachy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 # Python Modules
 import pathlib
 
 # 3rd Party Modules
 
 # Project Modules
 
-__version__ = '0.5.9'
+__version__ = '0.7.0'
 
 PROJECT_ROOT = pathlib.Path(__file__).parent.parent
```

### Comparing `scrachy-0.5.9/scrachy/addons.py` & `scrachy-0.7.0/src/scrachy/addons.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/cli/__init__.py` & `scrachy-0.7.0/src/scrachy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/cli/benchmark.py` & `scrachy-0.7.0/src/scrachy/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/cli/webdriver_server.py` & `scrachy-0.7.0/src/scrachy/cli/webdriver_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,179 @@
-#  Copyright 2023 Reid Swanson.
-#
-#  This file is part of scrachy.
-#
-#  scrachy is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  scrachy is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#   You should have received a copy of the GNU Lesser General Public License
-#   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
-"""
-A simple server that receives pickled ``SeleniumRequests`` from ``stdin`` and
-sends back pickled ``HtmlResponses`` to ``stdout``. It is meant to be used with
-:class:`~scrachy.middleware.selenium.AsyncSeleniumMiddleware`.
-"""
-
-from __future__ import annotations
-
-# Python Modules
-import argparse
-import logging
-import sys
-
-from struct import pack, unpack
-from typing import Optional
-
-# 3rd Party Modules
-import pickle
-
-from scrapy.http import HtmlResponse
-from selenium.common import TimeoutException
-from selenium.webdriver.remote.webdriver import WebDriver
-
-# Project Modules
-from scrachy.http_ import SeleniumRequest
-from scrachy.utils.selenium import BufferIncompleteError, ShutdownRequest, UnhandledError, UnknownMessageType, \
-    initialize_driver, \
-    process_request
-
-log = logging.getLogger('driver_process')
-
-
-Message = (
-    HtmlResponse | pickle.PickleError| SeleniumRequest | ShutdownRequest | TimeoutException | UnhandledError
-    | UnknownMessageType
-)
-
-
-DEFAULT_BUFFER_SIZE = 256
-REQUEST_HEADER_SIZE = 8
-
-
-def strippable(arg: str) -> str:
-    return arg.replace('"', '').strip()
-
-
-def setup_logging(args: argparse.Namespace):
-    if not args.log_file:
-        return
-
-    log_file = args.log_file
-    logging.basicConfig(filename=log_file, level=logging.DEBUG, filemode='w')
-    log.info(f"Logging is setup")
-
-
-def decode_message(buffer: bytearray) -> Optional[Message]:
-    # A message will always have two 4 byte header fields
-    while len(buffer) >= REQUEST_HEADER_SIZE:
-        req_length, msg_length = decode_header(buffer)
-
-        if len(buffer) >= msg_length:
-            # Get the data (minus the msg_length) and strip the padding
-            data_start, data_end = REQUEST_HEADER_SIZE, REQUEST_HEADER_SIZE + req_length
-            data = buffer[data_start:data_end]
-
-            # Deserialize the object
-            obj = pickle.loads(data)
-
-            # Trim off the processed data
-            buffer[:] = buffer[msg_length:]
-
-            return obj
-
-        # The data transmission is not complete
-        raise BufferIncompleteError()
-
-
-def decode_header(buffer: bytearray) -> tuple[int, int]:
-    # The total length of data sent from one call. This should always
-    # be the buffer_size.
-    req_length = unpack('!I', buffer[:4])[0]
-
-    # The length of the actual data.
-    msg_length = unpack('!I', buffer[4:8])[0]
-
-    return req_length, msg_length
-
-
-def send_message(message: Message):
-    data = pickle.dumps(message)
-    res_length = pack('!I', len(data))
-    sys.stdout.buffer.write(res_length + data)
-    sys.stdout.buffer.flush()
-
-
-def message_loop(driver: WebDriver, buffer: bytearray, buffer_size: int):
-    while True:
-        buffer.extend(sys.stdin.buffer.read(buffer_size))
-
-        try:
-            in_message: Optional[Message] = decode_message(buffer)
-
-            if isinstance(in_message, ShutdownRequest):
-                return
-
-            if isinstance(in_message, SeleniumRequest):
-                send_message(process_request(driver, in_message))
-            else:
-                send_message(UnknownMessageType(type(in_message)))
-        except pickle.PickleError as e:
-            send_message(e)
-        except TimeoutException as e:
-            send_message(e)
-        except BufferIncompleteError:
-            pass  # Keep going
-        except Exception as e:
-            send_message(UnhandledError(e))
-
-
-def main(args: argparse.Namespace):
-    setup_logging(args)
-
-    driver = None
-
-    try:
-        buffer = bytearray()
-        driver = initialize_driver(args.driver, args.driver_options, args.driver_extensions)
-        message_loop(driver, buffer, args.buffer_size)
-    except Exception as e:
-        send_message(UnhandledError(e))
-    finally:
-        if driver is not None:
-            driver.quit()
-
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser()
-
-    # It's not entirely clear why, but when the arguments are passed in via the
-    # twisted spawnProcess quotes and extra spaces are added to the arguments.
-    # This is especially problematic for the options, extensions, and log_file.
-    # The `strippable` function removes all quotes from the parsed arguments
-    # and strips any spaces surrounding spaces. It is possible, although
-    # unlikely, this could cause unintended consequences for some
-    # argument names or paths.
-    parser.add_argument('-d', '--driver', choices=['Chrome', 'Firefox'], default='Chrome')
-    parser.add_argument('-o', '--driver-options', type=strippable, action='append', default=[])
-    parser.add_argument('-e', '--driver-extensions', type=strippable, action='append', default=[])
-    parser.add_argument('-b', '--buffer-size', type=int, default=DEFAULT_BUFFER_SIZE)
-    parser.add_argument('-f', '--log-file', type=strippable)
-
-    main(parser.parse_args())
+#  Copyright 2023 Reid Swanson.
+#
+#  This file is part of scrachy.
+#
+#  scrachy is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  scrachy is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#   You should have received a copy of the GNU Lesser General Public License
+#   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
+"""
+A simple server that receives pickled ``SeleniumRequests`` from ``stdin`` and
+sends back pickled ``HtmlResponses`` to ``stdout``. It is meant to be used with
+:class:`~scrachy.middleware.selenium.AsyncSeleniumMiddleware`.
+"""
+
+from __future__ import annotations
+
+# Python Modules
+import argparse
+import logging
+import pickle
+import sys
+
+from struct import pack, unpack
+from typing import Optional
+
+# 3rd Party Modules
+from scrapy.http import HtmlResponse
+from selenium.common import TimeoutException
+from selenium.webdriver.remote.webdriver import WebDriver
+
+# Project Modules
+from scrachy.http_ import SeleniumRequest
+from scrachy.utils.selenium import BufferIncompleteError, ShutdownRequest, UnhandledError, UnknownMessageType, \
+    initialize_driver, \
+    process_request
+
+log = logging.getLogger('driver_process')
+
+
+Message = (
+    HtmlResponse | pickle.PickleError| SeleniumRequest | ShutdownRequest | TimeoutException | UnhandledError
+    | UnknownMessageType
+)
+
+
+DEFAULT_BUFFER_SIZE = 256
+REQUEST_HEADER_SIZE = 8
+
+
+def strippable(arg: str) -> str:
+    return arg.replace('"', '').strip()
+
+
+def setup_logging(args: argparse.Namespace):
+    if not args.log_file:
+        return
+
+    log_file = args.log_file
+    logging.basicConfig(filename=log_file, level=logging.DEBUG, filemode='w')
+    log.info(f"Logging is setup")
+
+
+def decode_message(buffer: bytearray) -> Optional[Message]:
+    # A message will always have two 4 byte header fields
+    while len(buffer) >= REQUEST_HEADER_SIZE:
+        req_length, msg_length = decode_header(buffer)
+
+        if len(buffer) >= msg_length:
+            # Get the data (minus the msg_length) and strip the padding
+            data_start, data_end = REQUEST_HEADER_SIZE, REQUEST_HEADER_SIZE + req_length
+            data = buffer[data_start:data_end]
+
+            # Deserialize the object
+            obj = pickle.loads(data)
+
+            # Trim off the processed data
+            buffer[:] = buffer[msg_length:]
+
+            return obj
+
+        # The data transmission is not complete
+        raise BufferIncompleteError()
+
+
+def decode_header(buffer: bytearray) -> tuple[int, int]:
+    # The total length of data sent from one call. This should always
+    # be the buffer_size.
+    req_length = unpack('!I', buffer[:4])[0]
+
+    # The length of the actual data.
+    msg_length = unpack('!I', buffer[4:8])[0]
+
+    return req_length, msg_length
+
+
+def send_message(message: Message):
+    data = pickle.dumps(message)
+    res_length = pack('!I', len(data))
+    sys.stdout.buffer.write(res_length + data)
+    sys.stdout.buffer.flush()
+
+
+def message_loop(driver: WebDriver, buffer: bytearray, buffer_size: int):
+    while True:
+        buffer.extend(sys.stdin.buffer.read(buffer_size))
+
+        try:
+            in_message: Optional[Message] = decode_message(buffer)
+
+            if isinstance(in_message, ShutdownRequest):
+                return
+
+            if isinstance(in_message, SeleniumRequest):
+                send_message(process_request(driver, in_message))
+            else:
+                send_message(UnknownMessageType(type(in_message)))
+        except pickle.PickleError as e:
+            send_message(e)
+        except TimeoutException as e:
+            send_message(e)
+        except BufferIncompleteError:
+            pass  # Keep going
+        except Exception as e:
+            send_message(UnhandledError(e))
+
+
+def main(args: argparse.Namespace):
+    """
+    The main driver program that starts the message loop.
+
+    :param args:
+    :return:
+    """
+    setup_logging(args)
+
+    driver = None
+
+    try:
+        buffer = bytearray()
+        driver = initialize_driver(
+            args.driver,
+            args.driver_options,
+            args.driver_extensions
+        )
+        message_loop(driver, buffer, args.buffer_size)
+    except Exception as e:
+        send_message(UnhandledError(e))
+    finally:
+        if driver is not None:
+            driver.quit()
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+
+    # It's not entirely clear why, but when the arguments are passed in via the
+    # twisted spawnProcess quotes and extra spaces are added to the arguments.
+    # This is especially problematic for the options, extensions, and log_file.
+    # The `strippable` function removes all quotes from the parsed arguments
+    # and strips any surrounding spaces. It is possible, although unlikely,
+    # this could cause unintended consequences for some argument names or
+    # paths.
+    parser.add_argument('-d', '--driver', choices=['Chrome', 'Firefox'], default='Chrome')
+    parser.add_argument('-o', '--driver-options', type=strippable, action='append', default=[])
+    parser.add_argument('-e', '--driver-extensions', type=strippable, action='append', default=[])
+    parser.add_argument('-w', '--implicit_wait', type=int, default=None)
+    parser.add_argument('-b', '--buffer-size', type=int, default=DEFAULT_BUFFER_SIZE)
+    parser.add_argument('-f', '--log-file', type=strippable)
+    parser.add_argument('-p', '--verify-proxy', action=argparse.BooleanOptionalAction)
+
+    main(parser.parse_args())
```

### Comparing `scrachy-0.5.9/scrachy/content/__init__.py` & `scrachy-0.7.0/src/scrachy/content/__init__.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/content/boilerpipe.py` & `scrachy-0.7.0/src/scrachy/content/boilerpipe.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/content/bs4.py` & `scrachy-0.7.0/src/scrachy/content/bs4.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/db/__init__.py` & `scrachy-0.7.0/src/scrachy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/db/engine.py` & `scrachy-0.7.0/src/scrachy/db/engine.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/db/repositories.py` & `scrachy-0.7.0/src/scrachy/db/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     def _find_standard(self, fingerprint: bytes) -> Response:
         stmt = (
             select(
                 Response
             ).options(
                 load_only(
                     Response.body,
+                    Response.meta,
                     Response.headers,
                     Response.status
                 )
             ).where(
                 Response.fingerprint == fingerprint
             )
         )
```

### Comparing `scrachy-0.5.9/scrachy/exceptions.py` & `scrachy-0.7.0/src/scrachy/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/middleware/__init__.py` & `scrachy-0.7.0/src/scrachy/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/middleware/filter.py` & `scrachy-0.7.0/src/scrachy/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/middleware/httpcache.py` & `scrachy-0.7.0/src/scrachy/middleware/httpcache.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,51 +32,44 @@
 import datetime
 import logging
 import re
 
 from typing import Optional, Any, cast
 
 # 3rd Party Modules
-from scrapy.http import Headers, HtmlResponse, Request, Response, TextResponse, XmlResponse
+from scrapy.http import Headers, Request, Response, TextResponse
 from scrapy.responsetypes import responsetypes
 from scrapy.spiders import Spider
 from scrapy.settings import Settings
 from scrapy.utils.misc import load_object
 from scrapy.utils.python import to_bytes, to_unicode
 from scrapy.utils.request import RequestFingerprinter
 from sqlalchemy import Engine
-from w3lib.http import headers_dict_to_raw
+from w3lib.http import headers_dict_to_raw, headers_raw_to_dict
 
 # Project Modules
 from scrachy.addons import try_import
 from scrachy.content import ContentExtractor
 from scrachy.db.engine import initialize_engine, session_scope
 from scrachy.db.models import Response as CachedResponse, ScrapeHistory
 from scrachy.db.repositories import ResponseRepository, ScrapeHistoryRepository
 from scrachy.exceptions import InvalidSettingError
-from scrachy.http_ import CachedHtmlResponse, CachedTextResponse, CachedXmlResponse
 from scrachy.settings import iter_default_settings
 from scrachy.settings.defaults import filter as default_filter_settings
 from scrachy.settings.defaults import fingerprinter as default_fingerprinter_settings
 from scrachy.settings.defaults import storage as default_storage_settings
 from scrachy.settings.defaults.storage import RetrievalMethod
 from scrachy.utils.datetime import now_tzaware
 from scrachy.utils.imports import get_import_path
 from scrachy.utils.request import DynamicHashRequestFingerprinter, ExpirationManager
 from scrachy.utils.settings import compile_patterns
 
 log = logging.getLogger(__name__)
 
 
-CLASS_ADAPTER = {
-    HtmlResponse: CachedHtmlResponse,
-    TextResponse: CachedTextResponse,
-    XmlResponse: CachedXmlResponse,
-}
-
 
 class BlacklistPolicy:
     """
     A wrapper around another cache control policy, but you can also blacklist
     urls (exclude from caching) via pattern matching using the
     :code:`SCRACHY_POLICY_EXCLUDE_URL_PATTERNS` setting. The patterns must
     either be strings that can be compiled with :meth:`re.compile` or
@@ -85,27 +78,46 @@
     def __init__(self, settings: Settings):
         super().__init__()
 
         self.base_policy = load_object(settings.get('SCRACHY_POLICY_BASE_CLASS'))(settings)
         self.exclude_patterns = compile_patterns(settings.getlist('SCRACHY_POLICY_EXCLUDE_URL_PATTERNS'))
 
     def should_cache_request(self, request: Request) -> bool:
-        return self.base_policy.should_cache_request(request) and not self.is_excluded(request.url)
+        if self.is_excluded(request.url):
+            log.debug(f"Request url is excluded from the cache: {request.url}")
+            return False
+
+        return self.base_policy.should_cache_request(request)
 
     def should_cache_response(self, response: Response, request: Request) -> bool:
-        return self.base_policy.should_cache_response(response, request) and not self.is_excluded(response.url)
+        if self.is_excluded(response.url):
+            log.debug(f"Response url is excluded from the cache: {response.url}")
+            return False
+
+        return self.base_policy.should_cache_response(response, request)
 
     def is_cached_response_fresh(self, response: Response, request: Request) -> bool:
-        return self.base_policy.is_cached_response_fresh(response, request) and not self.is_excluded(response.url)
+        if self.is_excluded(response.url):
+            log.debug(
+                f"Response url is excluded from the cache and should never be fresh: {response.url}"
+            )
+            return False
+
+        return self.base_policy.is_cached_response_fresh(response, request)
 
     def is_excluded(self, url: str) -> bool:
         return any([p.match(url) for p in self.exclude_patterns])
 
 
 class AlchemyCacheStorage:
+    """
+    This class implements a `scrapy cache storage backend
+    <https://docs.scrapy.org/en/latest/topics/downloader-middleware.html#writing-your-own-storage-backend>`_
+    that uses a relational database to store the cached documents.
+    """
     def __init__(self, settings: Settings):
         """
         This class implements a `scrapy cache storage backend
         <https://docs.scrapy.org/en/latest/topics/downloader-middleware.html#writing-your-own-storage-backend>`_
         that uses a relational database to store the cached documents.
 
         :param settings: The Scrapy project middleware.
@@ -142,26 +154,38 @@
 
         :return: The value of the setting or ``None`` if it is not set.
         """
         return self._settings.get(f"SCRACHY_{name}".upper(), default)
 
     @property
     def is_scrapy_fingerprinter(self) -> bool:
+        """
+        Returns ``True`` if we're using the scrapy fingerprinter.
+        """
         return self.fingerprinter_import_path.startswith('scrapy')
 
     @property
     def is_scrachy_fingerprinter(self) -> bool:
+        """
+        Returns ``True`` if we're using the scrachy fingerprinter.
+        """
         return self.fingerprinter_import_path.startswith('scrachy')
 
     @property
     def fingerprinter_import_path(self) -> str:
+        """
+        Get the import path to our fingerprinter.
+        """
         return get_import_path(type(self._fingerprinter))
 
     @property
     def fingerprinter_implementation(self) -> str:
+        """
+        Get the implementation string of the fingerprinter in use.
+        """
         return self._settings.get('REQUEST_FINGERPRINTER_IMPLEMENTATION')
 
     @property
     def fingerprinter_hasher_import_path(self) -> Optional[str]:
         if not self.is_scrachy_fingerprinter:
             return None
 
@@ -311,26 +335,14 @@
         :param engine: Use this engine instead of creating a new one.
         """
         self._fingerprinter = spider.crawler.request_fingerprinter
 
         if self._fingerprinter is None:
             raise ValueError(f"The request fingerprinter has not been initialized")
 
-        # if engine is not None:
-        #     self._engine = engine
-        #     self._dispose_on_close = False  # Don't manage an external engine
-        # else:
-        #     self._create_engine()
-        # if engine is None:
-        #     self._create_engine()
-        #     self._create_tables()
-        #     self._dispose_on_close = True
-        # else:
-        #     self._engine = engine
-        #     self._dispose_on_close = False
         initialize_engine(spider.settings)
 
         self.validate_settings()
 
     def close_spider(self, spider: Optional[Spider] = None):
         """
         Dispose of the SqlAlchemy Engine.
@@ -340,63 +352,67 @@
 
         # self._engine.dispose()
 
     def retrieve_response(
             self,
             spider: Spider,
             request: Request
-    ) -> Optional[CachedTextResponse | CachedXmlResponse | CachedHtmlResponse]:
+    ) -> Optional[Response]:
         """
         Retrieves an item from the cache if it exists, otherwise this returns
         ``None`` to signal downstream processes to continue retrieving the
         page normally. Depending on the value of the
         ``SCRACHY_RESPONSE_RETRIEVAL_METHOD`` setting more or less information
         may be returned in the response.
 
         :param spider: The Scrapy Spider requesting the data.
         :param request: The request describing what information to retrieve.
         :return: If the page is in the cache then this will return a
-                 :class:`~scrachy.http.CachedHtmlResponse`, otherwise it will
+                 :class:`~scrapy.http.Response`, otherwise it will
                  return ``None``.
         """
         cached_response: CachedResponse = self._read_data(spider, request)
 
         # We didn't find anything (or the item is expired)
         if not cached_response:
             return None
 
         # Create a new Response from the cached items.
         response_retrieval_method = self.response_retrieval_method
 
         # Allways return this info
-        kwargs = {
+        response_kwargs = {
             'request': request,
             'url': request.url,
             'body': cached_response.body
         }
 
+        meta_kwargs = dict()
         if response_retrieval_method == 'standard' or response_retrieval_method == 'full':
+            if cached_response.meta:
+                meta_kwargs |= cached_response.meta
+
             if cached_response.headers:
-                raw_headers = to_bytes(cached_response.headers)  # noqa
-                kwargs['headers'] = Headers(raw_headers)
+                raw_headers = headers_raw_to_dict(to_bytes(cached_response.headers))  # noqa
+                response_kwargs['headers'] = Headers(raw_headers)
 
-            kwargs['status'] = cached_response.status
+            response_kwargs['status'] = cached_response.status
 
         if response_retrieval_method == 'full':
             # This will return (almost) all the data Scrachy has about this
             # cached item.
-            kwargs |= {
+            meta_kwargs |= {
                 'scrape_timestamp': cached_response.scrape_timestamp,
                 'extracted_text': cached_response.extracted_text,
                 'body_length': cached_response.body_length,
                 'extracted_text_length': cached_response.extracted_text_length,
                 'scrape_history': cached_response.scrape_history
             }
 
-        return self._make_scrapy_response(**kwargs)
+        return self._make_scrapy_response(response_kwargs, meta_kwargs)
 
     def store_response(
             self,
             spider: Spider,
             request: Request,
             response: Response
     ):
@@ -404,20 +420,20 @@
         Stores the response in the cache.
 
         :param spider: The Scrapy Spider issuing the request.
         :param request: The request describing what data is desired.
         :param response: The response to be stored in the cache as created by
                Scrapy's standard downloading process.
         """
-        if not isinstance(response, TextResponse):
-            log.warning(f"The cache only supports TextResponses but received a '{type(response)}'")
-            return
+        # if not isinstance(response, TextResponse):
+        #     log.warning(f"The cache only supports TextResponses but received a '{type(response)}'")
+        #     return
 
         # log.debug(f"response.body:\n{response.body}")
-        response = cast(TextResponse, response)
+        # response = cast(TextResponse, response)
 
         fingerprint: bytes = self._fingerprinter.fingerprint(request)
         timestamp = now_tzaware()
         cached_response = self._make_cached_response(fingerprint, timestamp, request, response)
 
         # with self.session_scope() as session:
         with session_scope() as session:
@@ -553,22 +569,30 @@
         # with self.session_scope() as session:
         with session_scope() as session:
             repo = ResponseRepository(session)
             scrape_timestamp = repo.find_timestamp_by_fingerprint(fingerprint)
 
             # A missing timestamp indicates the data is not in the cache.
             if not scrape_timestamp:
+                log.debug(
+                    f"Did not find the timestamp for '{request.url}' "
+                    f"with fingerprint '{fingerprint.hex()}' in the cache."
+                )
                 return None
 
             # Don't use the cached data if it is stale.
             # Note the CachePolicy does something different. It only uses
             # info available from the page itself (e.g., the headers) and
             # doesn't know anything about how long (if at all) the data
             # has been in our cache.
             if self._expiration_manager.is_stale(request.url, scrape_timestamp):
+                log.debug(
+                    f"The response with url '{request.url}' "
+                    f"and timestamp '{scrape_timestamp}' is stale"
+                )
                 return None
 
             cached_response = repo.find_by_fingerprint(fingerprint, self.response_retrieval_method)
 
             session.expunge_all()
 
         return cached_response
@@ -582,37 +606,53 @@
             request: Request,
             response: Response
     ):
         cached_response = CachedResponse(
             fingerprint=fingerprint,
             scrape_timestamp=timestamp,
             url=request.url,
-            request_method=request.method,
-            body=response.text,
+            body=response.body,
             status=response.status,
             body_length=len(response.body)
         )
 
+        # For some reason this doesn't work as a constructor parameter anymore
+        cached_response.request_method = request.method
+
         if request.body is not None:
-            cached_response.request_body = to_unicode(request.body)
+            cached_response.request_body = request.body
+
+        if response.request is not None:
+            cached_response.meta = request.meta
 
         if response.headers is not None:
             cached_response.headers = to_unicode(headers_dict_to_raw(response.headers))
 
-        if self._content_extractor is not None:
+        if self._content_extractor is not None and isinstance(response, TextResponse):
             cached_response.extracted_text = self._content_extractor.get_content(response.text)
             cached_response.extracted_text_length = len(to_bytes(cached_response.extracted_text))
 
         return cached_response
 
-    def _make_scrapy_response(self, **kwargs):
-        scrapy_cls = responsetypes.from_args(
-            headers=kwargs.get('headers'),
-            url=kwargs.get('url'),
-            body=kwargs.get('body')
+    def _make_scrapy_response(
+            self,
+            response_kwargs: dict[str, Any],
+            meta_kwargs: dict[str, Any]
+    ) -> Response:
+        response_cls = responsetypes.from_args(
+            headers=response_kwargs.get('headers'),
+            url=response_kwargs.get('url'),
+            body=response_kwargs.get('body')
         )
-        scrachy_cls = CLASS_ADAPTER[scrapy_cls]
 
-        # Always use utf-8
-        return scrachy_cls(encoding=self.default_encoding, **kwargs)
+        if issubclass(response_cls, TextResponse):
+            response = response_cls(encoding=self.default_encoding, **response_kwargs)
+        else:
+            response = response_cls(**response_kwargs)
+
+        if response.request is not None:
+            response.meta.update(meta_kwargs)
+
+        return response
+
     # endregion Common Utilities
     # endregion Utility Methods
```

### Comparing `scrachy-0.5.9/scrachy/middleware/selenium.py` & `scrachy-0.7.0/src/scrachy/middleware/selenium.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,343 +1,466 @@
-#  Copyright 2023 Reid Swanson.
-#
-#  This file is part of scrachy.
-#
-#  scrachy is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  scrachy is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#   You should have received a copy of the GNU Lesser General Public License
-#   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
-
-"""
-Middleware for processing requests with Selenium.
-"""
-
-from __future__ import annotations
-
-# Python Modules
-import logging
-import math
-import os
-import queue
-
-from struct import pack, unpack
-from sys import executable
-from typing import Any, Optional
-
-# 3rd Party Modules
-import pickle
-
-from scrapy import Spider
-from scrapy import signals
-from scrapy.crawler import Crawler
-from scrapy.http import HtmlResponse, Request
-from scrapy.settings import Settings
-from selenium.webdriver.remote.webdriver import WebDriver
-from twisted.internet import reactor
-from twisted.internet.defer import Deferred
-from twisted.internet.protocol import ProcessProtocol
-from twisted.python import failure
-
-# Project Modules
-from scrachy import PROJECT_ROOT
-from scrachy.http_ import SeleniumRequest
-from scrachy.cli.webdriver_server import DEFAULT_BUFFER_SIZE, Message
-from scrachy.settings.defaults.selenium import WebDriverName
-from scrachy.utils.selenium import ShutdownRequest, initialize_driver
-from scrachy.utils.selenium import process_request as process_request_helper
-
-log = logging.getLogger(__name__)
-
-
-class SeleniumMiddleware:
-    """
-    A downloader middleware that uses a Selenium WebDriver to download
-    the content and return an ``HtmlResponse`` if the incoming ``Response``
-    is an instance of :class:`~scrachy.http_.SeleniumRequest`. Otherwise,
-    it returns ``None`` to let another downloader process it.
-    """
-    webdriver_import_base = 'selenium.webdriver'
-
-    def __init__(self, settings: Settings, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.settings = settings
-        self._driver = initialize_driver(self.driver_name, self.driver_options, self.driver_extensions)
-
-    # region Properties
-    def get(self, name: str) -> Any:
-        return self.settings.get(f'SCRACHY_SELENIUM_{name}')
-
-    @property
-    def driver_name(self) -> WebDriverName:
-        return self.get('WEB_DRIVER')
-
-    @property
-    def driver_options(self) -> list[str]:
-        return self.get('WEB_DRIVER_OPTIONS')
-
-    @property
-    def driver_extensions(self) -> list[str]:
-        return self.get('WEB_DRIVER_EXTENSIONS')
-
-    @property
-    def driver(self) -> WebDriver:
-        return self._driver
-
-    # endregion Properties
-
-    # region API
-    @classmethod
-    def from_crawler(cls, crawler: Crawler) -> SeleniumMiddleware:
-        middleware = cls(crawler.settings)
-
-        # See: https://docs.scrapy.org/en/latest/topics/signals.html
-        crawler.signals.connect(middleware.spider_closed, signals.spider_closed)
-
-        return middleware
-
-    def process_request(self, request: Request, spider: Optional[Spider] = None) -> Optional[HtmlResponse]:
-        return process_request_helper(self.driver, request)
-
-    def spider_closed(self, spider: Optional[Spider] = None):
-        self.driver.quit()
-    # endregion API
-
-
-class AsyncSeleniumMiddleware:
-    """
-        A downloader middleware that creates a pool of Selenium WebDrivers
-        and sends any incoming
-        :class:`SeleniumRequests <~scrachy.http_.SeleniumRequest>` to an
-        available driver to be processed.
-        """
-    def __init__(self, settings: Settings, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.settings = settings
-
-        concurrent_requests: int = settings.getint('CONCURRENT_REQUESTS')
-        log_file: str = settings.get('SCRACHY_SELENIUM_LOG_FILE')
-
-        # Create a pool of drivers to increase the throughput. Since there
-        # isn't actually any parallelism involved I don't think I have to
-        # be all that careful with synchronization (e.g., locks).
-        self.drivers = queue.Queue(maxsize=concurrent_requests)
-        for driver in [WebDriverProtocol(i) for i in range(concurrent_requests)]:
-            self.drivers.put(driver)
-
-            args = ['python', '-m', 'scrachy.cli.webdriver_server']
-            args += ['-d', self.driver_name]
-            args += [f'-o "{o}"' for o in self.driver_options]
-            args += [f'-e "{e}"' for e in self.driver_extensions]
-
-            if log_file:
-                args += [f'-f "{log_file}"']
-
-            # noinspection PyUnresolvedReferences
-            reactor.spawnProcess(
-                driver,
-                executable,
-                args,
-                path=PROJECT_ROOT,
-                env=os.environ,
-            )
-
-    # region Properties
-    def get(self, name: str) -> Any:
-        return self.settings.get(f'SCRACHY_SELENIUM_{name}')
-
-    @property
-    def driver_name(self) -> WebDriverName:
-        return self.get('WEB_DRIVER')
-
-    @property
-    def driver_options(self) -> list[str]:
-        return self.get('WEB_DRIVER_OPTIONS')
-
-    @property
-    def driver_extensions(self) -> list[str]:
-        return self.get('WEB_DRIVER_EXTENSIONS')
-    # endregion Properties
-
-    # region API
-    @classmethod
-    def from_crawler(cls, crawler: Crawler) -> AsyncSeleniumMiddleware:
-        middleware = cls(crawler.settings)
-
-        # See: https://docs.scrapy.org/en/latest/topics/signals.html
-        crawler.signals.connect(middleware.spider_closed, signals.spider_closed)
-
-        return middleware
-
-    def process_request(self, request: Request, spider: Optional[Spider] = None) -> Optional[Deferred[HtmlResponse]]:
-        if not isinstance(request, SeleniumRequest):
-            # Let some other downloader handle this request
-            return None
-
-        driver = self.drivers.get()
-
-        d = driver.process_request(request)
-
-        def enqueue_driver(r: HtmlResponse):
-            self.drivers.put(driver)
-            return r
-
-        d.addCallback(enqueue_driver)
-
-        return d
-
-    def spider_closed(self, spider: Optional[Spider] = None):
-        # Closing stdin should shut down the server
-        while not self.drivers.empty():
-            driver = self.drivers.get(block=False)
-            driver.shutdown()
-
-        # Uncommenting the following lines will allow any final messages
-        # sent to stderr from the server just before exiting.
-        # import time
-        # from twisted.internet.threads import deferToThread
-        # yield deferToThread(lambda: time.sleep(0.5))
-    # endregion API
-
-
-class WebDriverProtocol(ProcessProtocol):
-    # The number of bytes in the response message.
-    response_header_size = 4
-
-    def __init__(self, id_: int, process_buffer_size: int = DEFAULT_BUFFER_SIZE):
-        # An identifier for this process
-        self.id = id_
-
-        # The size of the read buffer on the spawned process. We need to send
-        # at lest this many bytes in order for the server's read buffer
-        # to flush. Otherwise, the server will hang until it gets more data.
-        self.process_buffer_size = process_buffer_size
-
-        # Buffer to accumulate incoming messages
-        self.buffer = b''
-
-        # The deferred object we will eventually return
-        self.deferred_response: Optional[Deferred[HtmlResponse]] = None
-
-        # This gets set once the shutdown message is sent and will be used
-        # to prevent any further communication with the protocol.
-        self.is_shutdown = False
-
-    # region Interface Methods
-    def connectionMade(self):
-        log.debug(f"Connection made to: {self.id} with pid: {self.transport.pid}")
-
-    def outReceived(self, data: bytes):
-        self.buffer += data
-        self._extract_message()
-
-    def errReceived(self, data: bytes):
-        log.error(f"Driver process error: {data.decode()}")
-
-    def inConnectionLost(self):
-        log.debug(f"Lost stdin")
-
-    def outConnectionLost(self):
-        log.debug(f"Lost stdout")
-
-    def errConnectionLost(self):
-        log.debug(f"Lost stderr")
-
-    def processExited(self, reason: failure.Failure):
-        log.info(f"Child process exited with exit code: {reason.value.exitCode}")
-
-    def processEnded(self, reason: failure.Failure):
-        log.info(f"Child process ended: {reason.value.exitCode}")
-    # endregion Interface Methods
-
-    def process_request(self, request: SeleniumRequest) -> Deferred[HtmlResponse]:
-        if self.is_shutdown:
-            raise ValueError("You cannot process requests after the server has been shut down.")
-
-        # The original request has references to all sorts of unnecessary
-        # and impossible to pickle objects. Just send over what we need.
-        self._send_message(
-            SeleniumRequest(
-                url=request.url,
-                wait_timeout=request.wait_timeout,
-                wait_until=request.wait_until,
-                screenshot=request.screenshot,
-                script_executor=request.script_executor
-            )
-        )
-
-        # We'll store the response here when it is ready.
-        self.deferred_response = Deferred()
-
-        return self.deferred_response
-
-    def shutdown(self):
-        self._send_message(ShutdownRequest())
-
-        self.transport.closeStdin()
-        self.is_shutdown = True
-
-    def _send_message(self, message: Message):
-        message_data = pickle.dumps(message)
-
-        # The number of bytes to encode the pickled data
-        data_length = len(message_data)
-
-        # The total number of bytes sent in the message (including the header
-        # and padding)
-        msg_length = self._get_message_length(data_length + 8)
-
-        # The number of bytes to pad the message by. The sum of the header,
-        # message, and padding should be an exact multiple of the process
-        # buffer size. This is the difference between the total message length
-        # and the data length and excluding the header.
-        pad_length = (msg_length - data_length) - 8
-
-        data_field = pack('!I', data_length)
-        msg_field = pack('!I', msg_length)
-
-        self.transport.writeSequence([data_field, msg_field, message_data, b' ' * pad_length])  # noqa
-
-    def _get_message_length(self, request_length: int) -> int:
-        return self.process_buffer_size * math.ceil(request_length / self.process_buffer_size)
-
-    def _extract_message(self):
-        while len(self.buffer) >= self.response_header_size:
-            msg_length = unpack('!I', self.buffer[:4])[0]
-            if len(self.buffer) >= msg_length + 4:
-                # Get the data from the buffer
-                data = self.buffer[4:4+msg_length]
-
-                # Remove the processed data from the buffer
-                self.buffer = self.buffer[4+msg_length:]
-
-                # Try to decode the message
-                try:
-                    obj = pickle.loads(data)
-                except pickle.PickleError as e:
-                    if self.deferred_response is not None:
-                        self.deferred_response.errback(e)
-                    else:
-                        log.error(f"There was a pickle error but the deferred response was not ready.")
-                    continue
-
-                if self.deferred_response is None:
-                    log.error(f"Deferred response is not ready!")
-                    continue
-
-                if not isinstance(obj, HtmlResponse):
-                    log.error(f"The message was not an HtmlResponse.")
-                    self.deferred_response.errback(obj)
-                    continue
-
-                self.deferred_response.callback(obj)
-            else:
-                break  # The message is not complete
+#  Copyright 2023 Reid Swanson.
+#
+#  This file is part of scrachy.
+#
+#  scrachy is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  scrachy is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#   You should have received a copy of the GNU Lesser General Public License
+#   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
+
+"""
+Middleware for processing requests with Selenium.
+"""
+
+from __future__ import annotations
+
+# Python Modules
+import logging
+import math
+import os
+import queue
+import signal
+
+from struct import pack, unpack
+from sys import executable
+from typing import Any, Optional, cast
+
+# 3rd Party Modules
+import pickle
+import psutil
+
+from scrapy import Spider
+from scrapy import signals
+from scrapy.crawler import Crawler
+from scrapy.exceptions import IgnoreRequest
+from scrapy.http import HtmlResponse, Request
+from scrapy.settings import Settings
+from selenium.common import WebDriverException
+from selenium.webdriver.remote.webdriver import WebDriver
+from twisted.internet import reactor
+from twisted.internet.defer import Deferred
+from twisted.internet.protocol import ProcessProtocol
+from twisted.python import failure
+
+# Project Modules
+from scrachy import PROJECT_ROOT
+from scrachy.http_ import SeleniumRequest
+from scrachy.cli.webdriver_server import DEFAULT_BUFFER_SIZE, Message
+from scrachy.settings.defaults.selenium import WebDriverName
+from scrachy.utils.selenium import ShutdownRequest, initialize_driver
+from scrachy.utils.selenium import process_request as process_request_helper
+
+log = logging.getLogger(__name__)
+
+
+class SeleniumMiddleware:
+    """
+    A downloader middleware that uses a Selenium WebDriver to download
+    the content and return an ``HtmlResponse`` if the incoming ``Response``
+    is an instance of :class:`~scrachy.http_.SeleniumRequest`. Otherwise,
+    it returns ``None`` to let another downloader process it.
+    """
+    webdriver_import_base = 'selenium.webdriver'
+
+    def __init__(self, settings: Settings, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.settings = settings
+        self._driver = self._initialize_driver()
+
+    # region Properties
+    def get(self, name: str, default_value: Any = None) -> Any:
+        return self.settings.get(f'SCRACHY_SELENIUM_{name}', default_value)
+
+    @property
+    def driver_name(self) -> WebDriverName:
+        return self.get('WEB_DRIVER')
+
+    @property
+    def driver_options(self) -> list[str]:
+        return self.get('WEB_DRIVER_OPTIONS')
+
+    @property
+    def driver_extensions(self) -> list[str]:
+        return self.get('WEB_DRIVER_EXTENSIONS')
+
+    @property
+    def driver_preferences(self) -> dict[str, Any]:
+        return self.get('WEB_DRIVER_PREFERENCES')
+
+    @property
+    def driver_page_load_timeout(self) -> float:
+        return self.get('PAGE_LOAD_TIMEOUT')
+
+    @property
+    def driver_implicit_wait(self) -> Optional[float]:
+        return self.get('IMPLICIT_WAIT')
+
+    @property
+    def driver_verify_proxy(self) -> bool:
+        return self.get('VERIFY_PROXY', False)
+
+    @property
+    def driver(self) -> WebDriver:
+        return self._driver
+
+    # endregion Properties
+
+    # region API
+    @classmethod
+    def from_crawler(cls, crawler: Crawler) -> SeleniumMiddleware:
+        middleware = cls(crawler.settings)
+
+        # See: https://docs.scrapy.org/en/latest/topics/signals.html
+        crawler.signals.connect(middleware.spider_closed, signals.spider_closed)
+
+        return middleware
+
+    def process_request(
+            self,
+            request: Request,
+            spider: Optional[Spider] = None
+    ) -> Optional[HtmlResponse | Request]:
+        request = cast(SeleniumRequest, request)
+
+        try:
+            return process_request_helper(self.driver, request)
+        except IgnoreRequest as e:
+            raise e
+        except WebDriverException as e:
+            import time
+            request.retries += 1
+            if request.retries > request.max_retries:
+                log.error(
+                    f"The request for {request.url} reached the maximum number of retries and "
+                    f"could not be processed."
+                )
+                raise IgnoreRequest()
+
+            log.warning(
+                f"A WebDriverException occurred '{e}'. "
+                f"Retrying ({request.retries} out of {request.max_retries})."
+            )
+
+            request.dont_filter = True
+
+            # Try to reinitialize the driver
+            log.info("Restarting the WebDriver.")
+            self.spider_closed()
+            self._driver = self._initialize_driver()
+
+            # Sleep longer and longer each time we time out
+            sleep_time = request.wait_timeout * request.retries
+
+            log.debug(f"Sleeping for {sleep_time} seconds.")
+            time.sleep(sleep_time)
+
+            return request
+
+    def spider_closed(self, spider: Optional[Spider] = None):
+        """
+        Close the webdriver when the spider is closed.
+
+        :param spider:
+        :return:
+        """
+        if self.driver is not None:
+            try:
+                self.driver.quit()
+            except Exception as e:
+                log.warning(
+                    f"Failed to quit the selenium driver. Will try to kill it.",
+                    exc_info=e
+                )
+            finally:
+                import os
+                import platform
+
+                self._driver = None
+                # Sometimes there are still processes left behind even when
+                # `driver.quit()` is called. I have a hunch it is related to
+                # scrapy's use of twisted, but am not sure. For Chrome and
+                # Firefox we can use some clues and hacks to determine the
+                # parent WebDriver process and kill it manually, which should
+                # kill all the other left over processes.
+                if platform.system() == "Windows":
+                    return
+
+                # Although I wound up doing something different the idea was
+                # inspired by the following post: https://stackoverflow.com/a/38509696
+                for process in psutil.process_iter():
+                    if process.status() == psutil.STATUS_ZOMBIE:
+                        log.warning(
+                            f"Found and terminating a zombie process with pid: {process.pid}"
+                        )
+                        process.terminate()
+                        continue
+
+                    cmdline = " ".join(process.cmdline()).lower()
+                    if "chrom" in cmdline and  "--class=selenium" in cmdline:
+                        # You can add a custom WM_CLASS to chrome using the --class flag.
+                        # If the user uses the class name 'selenium' we can detect the root
+                        # process and kill it here.
+                        log.warning(f"Force terminating Chrome webdriver with pid: {process.pid}")
+                        os.kill(process.pid, signal.SIGKILL)
+                    elif "firefox" in cmdline and  "--marionette" in cmdline :
+                        # The root Firefox WebDriver appears to have the --marionette flag
+                        # associated with it. If it is still running kill it.
+                        log.warning(f"Force terminating Firefox webdriver with pid: {process.pid}")
+                        os.kill(process.pid, signal.SIGKILL)
+                    # os.kill(parent_id, signal.SIGKILL)
+
+    # endregion API
+    def _initialize_driver(self) -> WebDriver:
+        return initialize_driver(
+            self.driver_name,
+            self.driver_options,
+            self.driver_extensions,
+            self.driver_preferences,
+            self.driver_page_load_timeout,
+            self.driver_implicit_wait,
+            self.driver_verify_proxy
+        )
+
+
+class AsyncSeleniumMiddleware:
+    """
+        A downloader middleware that creates a pool of Selenium WebDrivers
+        and sends any incoming
+        :class:`SeleniumRequests <~scrachy.http_.SeleniumRequest>` to an
+        available driver to be processed.
+        """
+    def __init__(self, settings: Settings, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.settings = settings
+
+        concurrent_requests: int = settings.getint('CONCURRENT_REQUESTS')
+        log_file: str = settings.get('SCRACHY_SELENIUM_LOG_FILE')
+
+        # Create a pool of drivers to increase the throughput. Since there
+        # isn't actually any parallelism involved I don't think I have to
+        # be all that careful with synchronization (e.g., locks).
+        self.drivers = queue.Queue(maxsize=concurrent_requests)
+        for driver in [WebDriverProtocol(i) for i in range(concurrent_requests)]:
+            self.drivers.put(driver)
+
+            args = [executable, '-m', 'scrachy.cli.webdriver_server']
+            args += ['-d', self.driver_name]
+            args += [f'-o "{o}"' for o in self.driver_options]
+            args += [f'-e "{e}"' for e in self.driver_extensions]
+
+            if log_file:
+                args += [f'-f "{log_file}"']
+
+            # noinspection PyUnresolvedReferences
+            reactor.spawnProcess(
+                driver,
+                executable,
+                args,
+                path=PROJECT_ROOT,
+                env=os.environ,
+            )
+
+    # region Properties
+    def get(self, name: str) -> Any:
+        return self.settings.get(f'SCRACHY_SELENIUM_{name}')
+
+    @property
+    def driver_name(self) -> WebDriverName:
+        return self.get('WEB_DRIVER')
+
+    @property
+    def driver_options(self) -> list[str]:
+        return self.get('WEB_DRIVER_OPTIONS')
+
+    @property
+    def driver_extensions(self) -> list[str]:
+        return self.get('WEB_DRIVER_EXTENSIONS')
+    # endregion Properties
+
+    # region API
+    @classmethod
+    def from_crawler(cls, crawler: Crawler) -> AsyncSeleniumMiddleware:
+        middleware = cls(crawler.settings)
+
+        # See: https://docs.scrapy.org/en/latest/topics/signals.html
+        crawler.signals.connect(middleware.spider_closed, signals.spider_closed)
+
+        return middleware
+
+    def process_request(
+            self,
+            request: Request,
+            spider: Optional[Spider] = None
+    ) -> Optional[Deferred[HtmlResponse | Request]]:
+        if not isinstance(request, SeleniumRequest):
+            # Let some other downloader handle this request
+            return None
+
+        driver = self.drivers.get()
+
+        d = driver.process_request(request)
+
+        def enqueue_driver(r: HtmlResponse | Request) -> HtmlResponse | Request:
+            self.drivers.put(driver)
+            return r
+
+        d.addCallback(enqueue_driver)
+
+        return d
+
+    def spider_closed(self, spider: Optional[Spider] = None):
+        # Closing stdin should shut down the server
+        while not self.drivers.empty():
+            driver = self.drivers.get(block=False)
+            driver.shutdown()
+
+        # Uncommenting the following lines will allow any final messages
+        # sent to stderr from the server just before exiting.
+        # import time
+        # from twisted.internet.threads import deferToThread
+        # yield deferToThread(lambda: time.sleep(0.5))
+    # endregion API
+
+
+class WebDriverProtocol(ProcessProtocol):
+    # The number of bytes in the response message.
+    response_header_size = 4
+
+    def __init__(self, id_: int, process_buffer_size: int = DEFAULT_BUFFER_SIZE):
+        # An identifier for this process
+        self.id = id_
+
+        # The size of the read buffer on the spawned process. We need to send
+        # at lest this many bytes in order for the server's read buffer
+        # to flush. Otherwise, the server will hang until it gets more data.
+        self.process_buffer_size = process_buffer_size
+
+        # Buffer to accumulate incoming messages
+        self.buffer = b''
+
+        # The deferred object we will eventually return
+        self.deferred_response: Optional[Deferred[HtmlResponse]] = None
+
+        # This gets set once the shutdown message is sent and will be used
+        # to prevent any further communication with the protocol.
+        self.is_shutdown = False
+
+    # region Interface Methods
+    def connectionMade(self):
+        log.debug(f"Connection made to: {self.id} with pid: {self.transport.pid}")
+
+    def outReceived(self, data: bytes):
+        self.buffer += data
+        self._extract_message()
+
+    def errReceived(self, data: bytes):
+        log.error(f"Driver process error: {data.decode()}")
+
+    def inConnectionLost(self):
+        log.debug(f"Lost stdin")
+
+    def outConnectionLost(self):
+        log.debug(f"Lost stdout")
+
+    def errConnectionLost(self):
+        log.debug(f"Lost stderr")
+
+    def processExited(self, reason: failure.Failure):
+        log.info(f"Child process exited with exit code: {reason.value.exitCode}")
+
+    def processEnded(self, reason: failure.Failure):
+        log.info(f"Child process ended: {reason.value.exitCode}")
+    # endregion Interface Methods
+
+    def process_request(self, request: SeleniumRequest) -> Deferred[HtmlResponse]:
+        if self.is_shutdown:
+            raise ValueError("You cannot process requests after the server has been shut down.")
+
+        # The original request has references to all sorts of unnecessary
+        # and impossible to pickle objects. Just send over what we need.
+        self._send_message(
+            SeleniumRequest(
+                url=request.url,
+                wait_timeout=request.wait_timeout,
+                wait_until=request.wait_until,
+                screenshot=request.screenshot,
+                script_executor=request.script_executor
+            )
+        )
+
+        # We'll store the response here when it is ready.
+        self.deferred_response = Deferred()
+
+        return self.deferred_response
+
+    def shutdown(self):
+        self._send_message(ShutdownRequest())
+
+        self.transport.closeStdin()
+        self.is_shutdown = True
+
+    def _send_message(self, message: Message):
+        message_data = pickle.dumps(message)
+
+        # The number of bytes to encode the pickled data
+        data_length = len(message_data)
+
+        # The total number of bytes sent in the message (including the header
+        # and padding)
+        msg_length = self._get_message_length(data_length + 8)
+
+        # The number of bytes to pad the message by. The sum of the header,
+        # message, and padding should be an exact multiple of the process
+        # buffer size. This is the difference between the total message length
+        # and the data length and excluding the header.
+        pad_length = (msg_length - data_length) - 8
+
+        data_field = pack('!I', data_length)
+        msg_field = pack('!I', msg_length)
+
+        self.transport.writeSequence([data_field, msg_field, message_data, b' ' * pad_length])  # noqa
+
+    def _get_message_length(self, request_length: int) -> int:
+        return self.process_buffer_size * math.ceil(request_length / self.process_buffer_size)
+
+    def _extract_message(self):
+        while len(self.buffer) >= self.response_header_size:
+            msg_length = unpack('!I', self.buffer[:4])[0]
+            if len(self.buffer) >= msg_length + 4:
+                # Get the data from the buffer
+                data = self.buffer[4:4+msg_length]
+
+                # Remove the processed data from the buffer
+                self.buffer = self.buffer[4+msg_length:]
+
+                # Try to decode the message
+                try:
+                    obj = pickle.loads(data)
+                except pickle.PickleError as e:
+                    if self.deferred_response is not None:
+                        self.deferred_response.errback(e)
+                    else:
+                        log.error(f"There was a pickle error but the deferred response was not ready.")
+                    continue
+
+                if self.deferred_response is None:
+                    log.error(f"Deferred response is not ready!")
+                    continue
+
+                if not isinstance(obj, HtmlResponse):
+                    log.error(f"The message was not an HtmlResponse. Got '{type(obj)}' instead.")
+                    self.deferred_response.errback(obj)
+                    continue
+
+                self.deferred_response.callback(obj)
+            else:
+                break  # The message is not complete
```

### Comparing `scrachy-0.5.9/scrachy/settings/__init__.py` & `scrachy-0.7.0/src/scrachy/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/settings/defaults/__init__.py` & `scrachy-0.7.0/src/scrachy/settings/defaults/__init__.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/settings/defaults/filter.py` & `scrachy-0.7.0/src/scrachy/settings/defaults/filter.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/settings/defaults/fingerprinter.py` & `scrachy-0.7.0/src/scrachy/settings/defaults/fingerprinter.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/settings/defaults/policy.py` & `scrachy-0.7.0/src/scrachy/settings/defaults/policy.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/settings/defaults/selenium.py` & `scrachy-0.7.0/src/scrachy/settings/defaults/selenium.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,91 @@
-#  Copyright 2023 Reid Swanson.
-#
-#  This file is part of scrachy.
-#
-#  scrachy is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  scrachy is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#   You should have received a copy of the GNU Lesser General Public License
-#   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
-
-"""
-The default settings for configuring the
-:mod:`Selenium <scrachy.middleware.selenium>`. middleware.
-"""
-
-# Python Modules
-from typing import Literal, Optional
-
-# 3rd Party Modules
-
-# Project Modules
-
-
-WebDriverName = Literal['Chrome', 'ChromiumEdge', 'Firefox', 'Safari']
-
-
-SCRACHY_SELENIUM_WEB_DRIVER: WebDriverName = 'Chrome'
-"""
-The name of the webdriver to use.
-"""
-
-SCRACHY_SELENIUM_WEB_DRIVER_OPTIONS: list[str] = []
-"""
-Initialize the webdriver with an ``Options`` object populated with these
-options.
-
-For a list of options see:
-    
-    * Chrome: `https://peter.sh/experiments/chromium-command-line-switches/`
-    * Firefox: `https://www-archive.mozilla.org/docs/command-line-args`
-"""
-
-SCRACHY_SELENIUM_WEB_DRIVER_EXTENSIONS: list[str] = []
-"""
-A list of extensions for the webdriver to load. These should be paths to CRX
-files for Chrome or XPI files for Firefox.
-"""
-
-SCRACHY_SELENIUM_LOG_FILE: Optional[str] = None
-"""
-A file to save logging statements made by a process launched from the
-:class:`~scrachy.middleware.selenium.AsyncSeleniumMiddleware`. 
-"""
+#  Copyright 2023 Reid Swanson.
+#
+#  This file is part of scrachy.
+#
+#  scrachy is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  scrachy is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#   You should have received a copy of the GNU Lesser General Public License
+#   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
+
+"""
+The default settings for configuring the
+:mod:`Selenium <scrachy.middleware.selenium>`. middleware.
+"""
+
+# Python Modules
+from typing import Any, Literal, Optional
+
+# 3rd Party Modules
+
+# Project Modules
+
+
+WebDriverName = Literal['Chrome', 'ChromiumEdge', 'Firefox', 'Safari']
+
+
+SCRACHY_SELENIUM_WEB_DRIVER: WebDriverName = 'Chrome'
+"""
+The name of the webdriver to use.
+"""
+
+SCRACHY_SELENIUM_WEB_DRIVER_OPTIONS: list[str] = []
+"""
+Initialize the webdriver with an ``Options`` object populated with these
+options.
+
+For a list of options see:
+    
+    * Chrome: `https://peter.sh/experiments/chromium-command-line-switches/`
+    * Firefox: `https://www-archive.mozilla.org/docs/command-line-args`
+"""
+
+SCRACHY_SELENIUM_WEB_DRIVER_EXTENSIONS: list[str] = []
+"""
+A list of extensions for the webdriver to load. These should be paths to CRX
+files for Chrome or XPI files for Firefox.
+"""
+
+SCRACHY_SELENIUM_WEB_DRIVER_PREFERENCES: dict[str, Any] = dict()
+"""
+A dictionary of preferences for the webdriver to load. For example,
+See the **Recognized capabilities** section of
+`this page <https://chromedriver.chromium.org/capabilities>`__.
+"""
+
+SCRACHY_SELENIUM_LOG_FILE: Optional[str] = None
+"""
+A file to save logging statements made by a process launched from the
+:class:`~scrachy.middleware.selenium.AsyncSeleniumMiddleware`. 
+"""
+
+SCRACHY_SELENIUM_MAX_RETRIES: int = 5
+"""
+The maximum number of times to retry if the request fails.
+"""
+
+SCRACHY_SELENIUM_PAGE_LOAD_TIMEOUT: float = 10.0
+"""
+The number of seconds to wait during a call to ``driver.get`` before timing
+out if we are unable to get a response from the server.
+"""
+
+SCRACHY_SELENIUM_IMPLICIT_WAIT: Optional[float] = None
+"""
+If not ``None``, set an implicit wait value (``driver.implicitly_wait``) to the
+given value.
+"""
+
+SCRACHY_SELENIUM_VERIFY_PROXY: bool = False
+"""
+If ``True``, an exception will be raised when the webdriver is initialized 
+if requests from the local machine have the same IP address as requests
+made from the webdriver.
+"""
```

### Comparing `scrachy-0.5.9/scrachy/settings/defaults/storage.py` & `scrachy-0.7.0/src/scrachy/settings/defaults/storage.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/__init__.py` & `scrachy-0.7.0/src/scrachy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/datetime.py` & `scrachy-0.7.0/src/scrachy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/db.py` & `scrachy-0.7.0/src/scrachy/utils/db.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/hash.py` & `scrachy-0.7.0/src/scrachy/utils/hash.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/imports.py` & `scrachy-0.7.0/src/scrachy/utils/imports.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/numeric.py` & `scrachy-0.7.0/src/scrachy/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/request.py` & `scrachy-0.7.0/src/scrachy/utils/request.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/settings.py` & `scrachy-0.7.0/src/scrachy/utils/settings.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/scrachy/utils/sqltypes.py` & `scrachy-0.7.0/src/scrachy/utils/sqltypes.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,16 +18,20 @@
 """
 Custom SqlAlchemy types.
 """
 
 # Python Modules
 import datetime
 
+from typing import Any, Optional
+
 # 3rd Party Modules
-from sqlalchemy import TypeDecorator
+from sqlalchemy import Dialect, JSON, TypeDecorator
+from sqlalchemy.dialects.postgresql import JSONB
+from sqlalchemy.sql.type_api import TypeEngine
 from sqlalchemy.types import TIMESTAMP
 
 # Project Modules
 
 
 LOCAL_TIMEZONE = datetime.datetime.utcnow().astimezone().tzinfo
 
@@ -48,24 +52,48 @@
     def __init__(self, timezone: bool = False):
         super().__init__(timezone)
 
     @property
     def python_type(self):
         return datetime.datetime
     
-    def process_literal_param(self, value, dialect):
+    def process_literal_param(self, value: Optional[datetime.datetime], dialect):
+        if value is None:
+            return None
+
         if value.tzinfo is None:
             value = value.astimezone(LOCAL_TIMEZONE)
 
         return value.astimezone(datetime.timezone.utc)
 
-    def process_bind_param(self, value: datetime, dialect):
+    def process_bind_param(self, value: Optional[datetime.datetime], dialect):
+        if value is None:
+            return None
+
         if value.tzinfo is None:
             value = value.astimezone(LOCAL_TIMEZONE)
 
         return value.astimezone(datetime.timezone.utc)
 
-    def process_result_value(self, value, dialect):
+    def process_result_value(self, value: Optional[datetime.datetime], dialect):
+        if value is None:
+            return None
+
         if value.tzinfo is None:
             return value.replace(tzinfo=datetime.timezone.utc)
 
         return value.astimezone(datetime.timezone.utc)
+
+
+class ConditionalJson(TypeDecorator):
+    """Uses JSONB if the dialect is postgresql otherwise uses JSON"""
+    # The common base type
+    impl = JSON
+
+    def load_dialect_impl(self, dialect: Dialect) -> TypeEngine[Any]:
+        if dialect.name == 'postgresql':
+            return dialect.type_descriptor(JSONB())
+
+        if dialect.name in ('sqlite', 'mysql', 'mssql'):
+            return dialect.type_descriptor(JSON())
+
+        raise ValueError(f"The dialect must at least support the JSON data type.")
```

### Comparing `scrachy-0.5.9/scrachy/utils/strings.py` & `scrachy-0.7.0/src/scrachy/utils/strings.py`

 * *Files identical despite different names*

### Comparing `scrachy-0.5.9/test/conftest.py` & `scrachy-0.7.0/src/scrachy/http_.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,8 @@
-#  Copyright 2023 Reid Swanson.
-#
-#  This file is part of scrachy.
-#
-#  scrachy is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  scrachy is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#   You should have received a copy of the GNU Lesser General Public License
-#   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
+#  Copyright 2020 Reid Swanson.
 #
 #  This file is part of scrachy.
 #
 #  scrachy is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
@@ -25,124 +10,92 @@
 #  scrachy is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #   You should have received a copy of the GNU Lesser General Public License
 #   along with scrachy.  If not, see <https://www.gnu.org/licenses/>.
+"""
+Additional ``Request`` and ``Response`` classes for working with Selenium
+and the ``AlchemyCacheStorage`` backend.
+
+Note: Naming this module ``http`` causes a circular import error, so I've appended
+an underscore to avoid conflicts.
+"""
 from __future__ import annotations
 
 # Python Modules
-import dataclasses
-import datetime
 import logging
-import pathlib
 
-from dataclasses import dataclass
-from typing import Any, NamedTuple, Optional
+from typing import Any, Optional, Protocol
 
 # 3rd Party Modules
-import pytest
-import yaml
-
-from scrapy.settings import Settings, iter_default_settings
+from scrapy.http import Request, Response
+from selenium.webdriver.remote.webdriver import WebDriver
 
 # Project Modules
-from scrachy.db.models import Response
-from scrachy.settings.defaults import filter as filter_settings
-from scrachy.settings.defaults import fingerprinter as fingerprinter_settings
-from scrachy.settings.defaults import policy as policy_settings
-from scrachy.settings.defaults import storage as storage_settings
-from test.utils import parse_date
 
 log = logging.getLogger(__name__)
 
 
-class TimestampPair(NamedTuple):
-    scrape_timestamp: datetime.datetime
-    current_timestamp: datetime.datetime
-
-
-@dataclass(kw_only=True)
-class ResponseConfig(yaml.YAMLObject):
-    yaml_tag = '!ResponseConfig'
-    yaml_loader = yaml.SafeLoader
-
-    scrape_timestamp: datetime.datetime
-    fingerprint: str
-    url: str
-    method: str
-    request_body: Optional[str] = None
-    body: str
-    status: Optional[int] = None
-    headers: Optional[str] = None
-    extracted_text: Optional[str] = None
-    body_length: int
-    extracted_text_length: Optional[int] = None
-
-    def to_cached_response(self) -> Response:
-        kwargs = {
-            f.name: getattr(self, f.name)
-            for f in dataclasses.fields(self)
-        }
-        kwargs['fingerprint'] = bytes.fromhex(kwargs['fingerprint'])
-        kwargs['scrape_timestamp'] = kwargs['scrape_timestamp'].replace(tzinfo=datetime.timezone.utc)
-
-        return Response(**kwargs)
-
-
-@dataclass(kw_only=True)
-class SettingsConfig(yaml.YAMLObject):
-    yaml_tag = '!SettingsConfig'
-    yaml_loader = yaml.SafeLoader
-
-    settings: dict[str, Any]
-
-    def to_settings(self):
-        settings = Settings(dict(iter_default_settings()))
-        settings.setmodule(filter_settings)
-        settings.setmodule(fingerprinter_settings)
-        settings.setmodule(policy_settings)
-        settings.setmodule(storage_settings)
-        settings.update(self.settings)
-
-        return settings
-
-
-@pytest.fixture(scope='module')
-def example_urls() -> list[str]:
-    return [
-        'http://www.example.com',
-        'https://www.example.com/page1',
-        'ftp://www.example.com/page2.html',
-        'http://wwwwexample.com',
-        'http://w3.example.com',
-        'https://anything.edu',
-        'http://anything.edu',
-        'https://anything.edu',
-        'ftp://anything.edu/page1',
-        'https://www.anything.edu/page1',
-        'foo://test.com',
-        'http://test.com'
-        'https://test.com/page1'
-    ]
-
-
-@pytest.fixture(scope='module')
-def response_configs() -> list[ResponseConfig]:
-    path = pathlib.Path(__file__).with_name('responses.yaml')
-    with path.open('r') as fh:
-        return yaml.safe_load(fh)
-
-
-@pytest.fixture(scope='module')
-def cached_responses(response_configs) -> list[Response]:
-    return [r.to_cached_response() for r in response_configs]
-
-
-@pytest.fixture(scope='module')
-def settings_choices() -> dict[str, Settings]:
-    path = pathlib.Path(__file__).with_name('settings.yaml')
-    with path.open('r') as fh:
-        settings = yaml.safe_load(fh)
+DEFAULT_POLL_FREQUENCY = 1
+DEFAULT_MAX_RETRIES = 10
+
 
-    return {name: config.to_settings() for name, config in settings.items()} if settings else {}
+class WaitCondition(Protocol):
+    def __call__(self, driver: WebDriver) -> Any:
+        pass
+
+
+class ScriptExecutor(Protocol):
+    def __call__(self, driver: WebDriver, request: Request) -> Optional[Response | list[Response] | dict[str, Response]]:
+        pass
+
+
+class SeleniumRequest(Request):
+    """
+    A subclass of :class:`scrapy.http.Request` that provides extra information for downloading pages using
+    Selenium.
+
+    Based off the code from `Scrapy-Selenium <https://github.com/clemfromspace/scrapy-selenium>`_
+    """
+
+    def __init__(
+            self,
+            wait_timeout: Optional[float] = None,
+            wait_until: Optional[WaitCondition] = None,
+            poll_frequency: float = DEFAULT_POLL_FREQUENCY,
+            screenshot: bool = False,
+            script_executor: Optional[ScriptExecutor] = None,
+            max_retries: int = DEFAULT_MAX_RETRIES,
+            *args,
+            **kwargs
+    ):
+        """
+        A new ``SeleniumRequest``.
+
+        :param wait_timeout: The number of seconds to wait before accessing the data.
+        :param wait_until: One of the "selenium.webdriver.support.expected_conditions". The response
+                           will be returned until the given condition is fulfilled.
+        :param poll_frequency: The sleep interval between calls
+        :param screenshot: If ``True``, a screenshot of the page will be taken and the data of the screenshot
+                           will be returned in the response "meta" attribute.
+        :param script_executor: A function that takes a webdriver and a response as its parameters and optionally
+                                returns a list of new response objects as a side effect of its actions (e.g.,
+                                executing arbitrary javascript code on the page). Any returned responses will
+                                be returned in the ``request.meta`` attribute with the key ``script_result``.
+                                Note that the returned responses will not be further processed by any other
+                                middleware.
+        :param max_retries: The maximum number of times a request will be retried (sent back to
+                            scrapy to be rescheduled) if a TimeoutException is raised because the
+                            wait_until conditions are not satisfied while downloading the source.
+
+        """
+        super().__init__(*args, **kwargs)
+
+        self.wait_timeout = wait_timeout
+        self.wait_until = wait_until
+        self.poll_frequency = poll_frequency
+        self.screenshot = screenshot
+        self.script_executor = script_executor
+        self.retries = 0
+        self.max_retries = max_retries
```

