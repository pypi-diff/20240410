# Comparing `tmp/metalarchivist-0.2.5.tar.gz` & `tmp/metalarchivist-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.2.5.tar", last modified: Wed Apr 10 15:48:26 2024, max compression
+gzip compressed data, was "metalarchivist-0.2.6.tar", last modified: Wed Apr 10 15:54:12 2024, max compression
```

## Comparing `metalarchivist-0.2.5.tar` & `metalarchivist-0.2.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:48:26.995513 metalarchivist-0.2.5/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:48:26.995513 metalarchivist-0.2.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 15:48:26.995513 metalarchivist-0.2.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:48:26.988513 metalarchivist-0.2.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:48:26.989513 metalarchivist-0.2.5/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:48:26.991513 metalarchivist-0.2.5/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/export/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/export/label.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/export/user-agents.json
--rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:48:26.993513 metalarchivist-0.2.5/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/album.py
--rwxrwxrwx   0 root         (0) root         (0)     8342 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/label.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/page.py
--rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:48:26.994513 metalarchivist-0.2.5/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:48:26.000000 metalarchivist-0.2.5/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 15:48:26.000000 metalarchivist-0.2.5/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:48:26.000000 metalarchivist-0.2.5/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 15:48:26.000000 metalarchivist-0.2.5/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 15:48:26.000000 metalarchivist-0.2.5/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:48:26.994513 metalarchivist-0.2.5/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 15:48:14.000000 metalarchivist-0.2.5/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.622405 metalarchivist-0.2.6/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:54:12.622405 metalarchivist-0.2.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 15:54:12.622405 metalarchivist-0.2.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.615405 metalarchivist-0.2.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.616405 metalarchivist-0.2.6/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.619405 metalarchivist-0.2.6/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/user-agents.json
+-rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.620405 metalarchivist-0.2.6/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     8342 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/page.py
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.621405 metalarchivist-0.2.6/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 15:54:12.000000 metalarchivist-0.2.6/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:54:12.621405 metalarchivist-0.2.6/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 15:53:58.000000 metalarchivist-0.2.6/src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.5/LICENSE` & `metalarchivist-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/PKG-INFO` & `metalarchivist-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.5/pyproject.toml` & `metalarchivist-0.2.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.2.5"
+version = "0.2.6"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.2.5/src/metalarchivist/export/album.py` & `metalarchivist-0.2.6/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/export/band.py` & `metalarchivist-0.2.6/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/export/genre.py` & `metalarchivist-0.2.6/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/export/label.py` & `metalarchivist-0.2.6/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/export/user-agents.json` & `metalarchivist-0.2.6/src/metalarchivist/export/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/export/util.py` & `metalarchivist-0.2.6/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/album.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/band.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/base.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/genre.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/label.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/page.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/interface/theme.py` & `metalarchivist-0.2.6/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist/report.py` & `metalarchivist-0.2.6/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.2.6/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.5/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.2.6/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/test/test_albums.py` & `metalarchivist-0.2.6/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/test/test_bands.py` & `metalarchivist-0.2.6/src/test/test_bands.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 class TestBands(unittest.TestCase):
     metalarchivist, interface, export, config = load_module()
 
     def test_band_hash(self):
         band_hash = self.interface.create_band_key(1, 'Amorphis')
-        self.assertEqual(band_hash, 'db6300a85812db4c19ee707b')
+        self.assertEqual(band_hash, '6bdefdd6445b150526b32308')
 
     def test_band_report(self):
 
         bands = self.metalarchivist.get_bands(['https://www.metal-archives.com/bands/Furia/23765',
                                                'https://www.metal-archives.com/bands/Cult_of_Fire/3540334368',
                                                'https://www.metal-archives.com/bands/Urfaust/19596',
                                                'https://www.metal-archives.com/bands/A_Forest_of_Stars/115504',
```

### Comparing `metalarchivist-0.2.5/src/test/test_genres.py` & `metalarchivist-0.2.6/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.5/src/test/test_themes.py` & `metalarchivist-0.2.6/src/test/test_themes.py`

 * *Files identical despite different names*

