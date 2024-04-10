# Comparing `tmp/metalarchivist-0.2.6.tar.gz` & `tmp/metalarchivist-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.2.6.tar", last modified: Wed Apr 10 15:54:12 2024, max compression
+gzip compressed data, was "metalarchivist-0.2.7.tar", last modified: Wed Apr 10 16:48:23 2024, max compression
```

## Comparing `metalarchivist-0.2.6.tar` & `metalarchivist-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.622405 metalarchivist-0.2.6/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:54:12.622405 metalarchivist-0.2.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 15:54:12.622405 metalarchivist-0.2.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.615405 metalarchivist-0.2.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.616405 metalarchivist-0.2.6/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.619405 metalarchivist-0.2.6/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/label.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/user-agents.json
--rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.620405 metalarchivist-0.2.6/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/album.py
--rwxrwxrwx   0 root         (0) root         (0)     8342 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/label.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/page.py
--rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.621405 metalarchivist-0.2.6/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.621405 metalarchivist-0.2.6/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:48:23.252465 metalarchivist-0.2.7/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 16:48:23.252465 metalarchivist-0.2.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:48:23.252465 metalarchivist-0.2.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:48:23.244465 metalarchivist-0.2.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:48:23.246465 metalarchivist-0.2.7/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:48:23.248465 metalarchivist-0.2.7/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/export/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/export/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/export/user-agents.json
+-rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:48:23.250465 metalarchivist-0.2.7/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     8342 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/page.py
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:48:23.252465 metalarchivist-0.2.7/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 16:48:23.000000 metalarchivist-0.2.7/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 16:48:23.000000 metalarchivist-0.2.7/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 16:48:23.000000 metalarchivist-0.2.7/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 16:48:23.000000 metalarchivist-0.2.7/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 16:48:23.000000 metalarchivist-0.2.7/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:48:23.251465 metalarchivist-0.2.7/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 16:48:10.000000 metalarchivist-0.2.7/src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.6/LICENSE` & `metalarchivist-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/PKG-INFO` & `metalarchivist-0.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.6/pyproject.toml` & `metalarchivist-0.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.2.6"
+version = "0.2.7"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.2.6/src/metalarchivist/export/album.py` & `metalarchivist-0.2.7/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/export/band.py` & `metalarchivist-0.2.7/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/export/genre.py` & `metalarchivist-0.2.7/src/metalarchivist/export/genre.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import urllib3
 
 from .util import MetalArchives, normalize_keyword_casing, perform_request
 from ..interface import Genre, GenrePage, GenrePages
 
 
 class GenreError(Exception):
-    def __init__(self, status_code, url):
+    def __init__(self, status_code):
         self.status_code = status_code
-        self.url = url
 
     def __repr__(self):
-        return repr(self) + f'<{self.status_code}: {self.url}>'
+        return repr(self) + f'<{self.status_code}>'
 
 
 class GenreBands:
 
     @classmethod
     def get_genre_size(cls, genre: Genre, timeout_cxn=3., timeout_read=9.) -> int:
         timeout = urllib3.Timeout(connect=timeout_cxn, read=timeout_read)
```

### Comparing `metalarchivist-0.2.6/src/metalarchivist/export/label.py` & `metalarchivist-0.2.7/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/export/user-agents.json` & `metalarchivist-0.2.7/src/metalarchivist/export/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/export/util.py` & `metalarchivist-0.2.7/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/album.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/band.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/base.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/genre.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/label.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/page.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/interface/theme.py` & `metalarchivist-0.2.7/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist/report.py` & `metalarchivist-0.2.7/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.2.7/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.6/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.2.7/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/test/test_albums.py` & `metalarchivist-0.2.7/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/test/test_bands.py` & `metalarchivist-0.2.7/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/test/test_genres.py` & `metalarchivist-0.2.7/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.6/src/test/test_themes.py` & `metalarchivist-0.2.7/src/test/test_themes.py`

 * *Files identical despite different names*

