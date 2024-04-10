# Comparing `tmp/metalarchivist-0.2.2.tar.gz` & `tmp/metalarchivist-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.2.2.tar", last modified: Wed Apr 10 15:13:34 2024, max compression
+gzip compressed data, was "metalarchivist-0.2.3.tar", last modified: Wed Apr 10 15:17:09 2024, max compression
```

## Comparing `metalarchivist-0.2.2.tar` & `metalarchivist-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:13:34.250740 metalarchivist-0.2.2/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:13:34.250740 metalarchivist-0.2.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 15:13:34.250740 metalarchivist-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:13:34.242740 metalarchivist-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:13:34.244740 metalarchivist-0.2.2/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:13:34.247740 metalarchivist-0.2.2/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/export/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/export/label.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/export/user-agents.json
--rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:13:34.248740 metalarchivist-0.2.2/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)      862 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/album.py
--rwxrwxrwx   0 root         (0) root         (0)     8245 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/label.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/page.py
--rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:13:34.249740 metalarchivist-0.2.2/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:13:34.000000 metalarchivist-0.2.2/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 15:13:34.000000 metalarchivist-0.2.2/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:13:34.000000 metalarchivist-0.2.2/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 15:13:34.000000 metalarchivist-0.2.2/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 15:13:34.000000 metalarchivist-0.2.2/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:13:34.249740 metalarchivist-0.2.2/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     4918 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 15:13:21.000000 metalarchivist-0.2.2/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.146665 metalarchivist-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.147665 metalarchivist-0.2.3/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.150665 metalarchivist-0.2.3/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/user-agents.json
+-rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.152665 metalarchivist-0.2.3/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)      862 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     8286 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/page.py
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.153665 metalarchivist-0.2.3/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     4918 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.2/LICENSE` & `metalarchivist-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/PKG-INFO` & `metalarchivist-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.2/pyproject.toml` & `metalarchivist-0.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.2.2"
+version = "0.2.3"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.2.2/src/metalarchivist/export/album.py` & `metalarchivist-0.2.3/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/export/band.py` & `metalarchivist-0.2.3/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/export/genre.py` & `metalarchivist-0.2.3/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/export/label.py` & `metalarchivist-0.2.3/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/export/user-agents.json` & `metalarchivist-0.2.3/src/metalarchivist/export/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/export/util.py` & `metalarchivist-0.2.3/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/album.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/band.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/band.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 
 class InvalidPageError(Exception):
     ...
 
 
 def create_band_key(metallum_id: int, band_name: str) -> str:
-    return str(metallum_id) + '-' + BLAKE2s.new(data=band_name.encode('utf-8')).hexdigest()
+    hash_obj = BLAKE2s.new(data=band_name.encode('utf-8'), digest_bytes=12)
+    return str(metallum_id) + '-' + hash_obj.hexdigest()
 
 
 @dataclass
 class BandLink:
     """ An HTML anchor tag pointing to a unique band profile """
     name: str = field(init=False)
     link: str = field(init=False)
```

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/base.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/genre.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/label.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/page.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/interface/theme.py` & `metalarchivist-0.2.3/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist/report.py` & `metalarchivist-0.2.3/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.2.3/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.2/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.2.3/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/test/test_albums.py` & `metalarchivist-0.2.3/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/test/test_bands.py` & `metalarchivist-0.2.3/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/test/test_genres.py` & `metalarchivist-0.2.3/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.2/src/test/test_themes.py` & `metalarchivist-0.2.3/src/test/test_themes.py`

 * *Files identical despite different names*

