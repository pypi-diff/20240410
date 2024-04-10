# Comparing `tmp/metalarchivist-0.2.3.tar.gz` & `tmp/metalarchivist-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.2.3.tar", last modified: Wed Apr 10 15:17:09 2024, max compression
+gzip compressed data, was "metalarchivist-0.2.4.tar", last modified: Wed Apr 10 15:20:29 2024, max compression
```

## Comparing `metalarchivist-0.2.3.tar` & `metalarchivist-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.146665 metalarchivist-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.147665 metalarchivist-0.2.3/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.150665 metalarchivist-0.2.3/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/label.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/user-agents.json
--rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.152665 metalarchivist-0.2.3/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)      862 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/album.py
--rwxrwxrwx   0 root         (0) root         (0)     8286 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/label.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/page.py
--rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.154665 metalarchivist-0.2.3/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 15:17:09.000000 metalarchivist-0.2.3/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:17:09.153665 metalarchivist-0.2.3/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     4918 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 15:16:57.000000 metalarchivist-0.2.3/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:20:29.314760 metalarchivist-0.2.4/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:20:29.314760 metalarchivist-0.2.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 15:20:29.314760 metalarchivist-0.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:20:29.305760 metalarchivist-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:20:29.306760 metalarchivist-0.2.4/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:20:29.310760 metalarchivist-0.2.4/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/export/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/export/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/export/user-agents.json
+-rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:20:29.312760 metalarchivist-0.2.4/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     8285 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/page.py
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:20:29.314760 metalarchivist-0.2.4/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:20:29.000000 metalarchivist-0.2.4/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 15:20:29.000000 metalarchivist-0.2.4/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:20:29.000000 metalarchivist-0.2.4/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 15:20:29.000000 metalarchivist-0.2.4/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 15:20:29.000000 metalarchivist-0.2.4/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:20:29.313760 metalarchivist-0.2.4/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 15:20:16.000000 metalarchivist-0.2.4/src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.3/LICENSE` & `metalarchivist-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/PKG-INFO` & `metalarchivist-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.3/pyproject.toml` & `metalarchivist-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.2.3"
+version = "0.2.4"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.2.3/src/metalarchivist/export/album.py` & `metalarchivist-0.2.4/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/export/band.py` & `metalarchivist-0.2.4/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/export/genre.py` & `metalarchivist-0.2.4/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/export/label.py` & `metalarchivist-0.2.4/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/export/user-agents.json` & `metalarchivist-0.2.4/src/metalarchivist/export/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/export/util.py` & `metalarchivist-0.2.4/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
-from .band import BandProfile, BandLink, BandExternalLinks
+from .band import BandProfile, BandLink, BandExternalLinks, create_band_key
 from .album import AlbumProfile, AlbumLink
 from .genre import Subgenres, Genre
 from .theme import Themes
 from .label import LabelProfile
 from .search import SearchResults
 from .page import (ReleasePages, ReleasePage, 
                    GenrePages, GenrePage,
                    LabelPage, LabelPages,
                    AlbumReleases, AlbumRelease,
                    BandGenres, BandGenre)
 
 
 __all__ = ['BandProfile', 'BandLink', 'BandExternalLinks',
+           'create_band_key',
            'AlbumProfile', 'AlbumLink',
            'LabelProfile',
            'Subgenres', 'Genre',
            'Themes',
            'SearchResults',
            'ReleasePages', 'ReleasePage',
            'GenrePages', 'GenrePage',
```

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/album.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/band.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/band.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 
 class InvalidPageError(Exception):
     ...
 
 
 def create_band_key(metallum_id: int, band_name: str) -> str:
-    hash_obj = BLAKE2s.new(data=band_name.encode('utf-8'), digest_bytes=12)
-    return str(metallum_id) + '-' + hash_obj.hexdigest()
+    hash_obj = BLAKE2s.new(data=band_name.encode('utf-8'), digest_bytes=12, key=bytes(metallum_id))
+    return hash_obj.hexdigest()
 
 
 @dataclass
 class BandLink:
     """ An HTML anchor tag pointing to a unique band profile """
     name: str = field(init=False)
     link: str = field(init=False)
```

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/base.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/genre.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/label.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/page.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/interface/theme.py` & `metalarchivist-0.2.4/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist/report.py` & `metalarchivist-0.2.4/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.2.4/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.3/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.2.4/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/test/test_albums.py` & `metalarchivist-0.2.4/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/test/test_bands.py` & `metalarchivist-0.2.4/src/test/test_bands.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 
     return metalarchivist, interface, export, config
 
 
 class TestBands(unittest.TestCase):
     metalarchivist, interface, export, config = load_module()
 
+    def test_band_hash(self):
+        band_hash = self.interface.create_band_key(1, 'Amorphis')
+        self.assertEqual(band_hash, 'db6300a85812db4c19ee707b')
+
     def test_band_report(self):
 
         bands = self.metalarchivist.get_bands(['https://www.metal-archives.com/bands/Furia/23765',
                                                'https://www.metal-archives.com/bands/Cult_of_Fire/3540334368',
                                                'https://www.metal-archives.com/bands/Urfaust/19596',
                                                'https://www.metal-archives.com/bands/A_Forest_of_Stars/115504',
                                                'https://www.metal-archives.com/bands/Burzum/88',
```

### Comparing `metalarchivist-0.2.3/src/test/test_genres.py` & `metalarchivist-0.2.4/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.3/src/test/test_themes.py` & `metalarchivist-0.2.4/src/test/test_themes.py`

 * *Files identical despite different names*

