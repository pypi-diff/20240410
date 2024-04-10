# Comparing `tmp/metalarchivist-0.2.0.tar.gz` & `tmp/metalarchivist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.2.0.tar", last modified: Wed Apr 10 11:59:58 2024, max compression
+gzip compressed data, was "metalarchivist-0.2.1.tar", last modified: Wed Apr 10 14:58:58 2024, max compression
```

## Comparing `metalarchivist-0.2.0.tar` & `metalarchivist-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)      661 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.206329 metalarchivist-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.207329 metalarchivist-0.2.0/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.210329 metalarchivist-0.2.0/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/label.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/user-agents.json
--rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.211329 metalarchivist-0.2.0/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)      862 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/album.py
--rwxrwxrwx   0 root         (0) root         (0)     8202 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/label.py
--rw-rw-rw-   0 root         (0) root         (0)     3885 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/page.py
--rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.212329 metalarchivist-0.2.0/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     4918 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:58.695404 metalarchivist-0.2.1/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 14:58:58.694404 metalarchivist-0.2.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 14:58:58.695404 metalarchivist-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:58.687404 metalarchivist-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:58.688404 metalarchivist-0.2.1/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:58.691404 metalarchivist-0.2.1/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/export/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/export/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/export/user-agents.json
+-rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:58.693404 metalarchivist-0.2.1/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)      862 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     8240 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/page.py
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:58.694404 metalarchivist-0.2.1/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 14:58:58.000000 metalarchivist-0.2.1/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 14:58:58.000000 metalarchivist-0.2.1/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 14:58:58.000000 metalarchivist-0.2.1/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 14:58:58.000000 metalarchivist-0.2.1/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 14:58:58.000000 metalarchivist-0.2.1/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:58:58.694404 metalarchivist-0.2.1/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     4918 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 14:58:45.000000 metalarchivist-0.2.1/src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.0/LICENSE` & `metalarchivist-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/PKG-INFO` & `metalarchivist-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: lxml
 Requires-Dist: urllib3
+Requires-Dist: pycryptodome
 
 # MetalArchivist
 
 A Python package for extracting data from [Encyclopaedia Metallum](https://metal-archives.com)
```

### Comparing `metalarchivist-0.2.0/pyproject.toml` & `metalarchivist-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "metalarchivist"
-version = "0.2.0"
+version = "0.2.1"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
-dependencies = [ "rich", "lxml", "urllib3" ]
+dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
   "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `metalarchivist-0.2.0/src/metalarchivist/export/album.py` & `metalarchivist-0.2.1/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/export/band.py` & `metalarchivist-0.2.1/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/export/genre.py` & `metalarchivist-0.2.1/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/export/label.py` & `metalarchivist-0.2.1/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/export/user-agents.json` & `metalarchivist-0.2.1/src/metalarchivist/export/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/export/util.py` & `metalarchivist-0.2.1/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/album.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/band.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/band.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 
 from dataclasses import dataclass, field, asdict, InitVar
 from urllib.parse import unquote
 
 import lxml.html
 import lxml.etree
 
+from Crypto.Hash import BLAKE2s
+
 from .genre import Subgenres
 from .theme import Themes
 
 
 
 class InvalidAttributeError(Exception):
     ...
 
 
 class InvalidPageError(Exception):
     ...
 
 
 def create_band_key(metallum_id: int, band_name: str) -> str:
-    return str(metallum_id) + '-' + str(hash(band_name) % 2**sys.hash_info.width)
+    return str(metallum_id) + '-' + BLAKE2s.new(band_name.encode('utf-8')).hexdigest()
 
 
 @dataclass
 class BandLink:
     """ An HTML anchor tag pointing to a unique band profile """
     name: str = field(init=False)
     link: str = field(init=False)
```

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/base.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/genre.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/label.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/page.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,38 +4,59 @@
 from datetime import datetime
 from dataclasses import field, InitVar, dataclass
 
 import lxml.html
 
 from .base import Page, Pages, PageDataType
 
-from .band import BandLink
+from .band import BandLink, create_band_key
 from .album import AlbumLink, _parse_release_date
 from .genre import Subgenres
 from .label import LabelLink
 
 
 
 @dataclass
 class Label(PageDataType):
     label: LabelLink
-
-    specialisation: str
     status: str
-    website: str
     has_shop: bool
 
+    specialisation: str | None
+    country: str | None
+    website: str | None
+
 
 @dataclass
 class Labels(list, PageDataType):
     label_page_record: InitVar[list[str]]
 
     def __post_init__(self, label_page_record: list[str]):
-        (edit_link, label_link_text, specialisation, status_text, 
-         country, website_link, has_shop_text) = label_page_record
+        (_, label_link_text, specialisation, status_text, 
+         country, website_link_text, has_shop_text) = label_page_record
+        
+        label_link = LabelLink(label_link_text)
+        status = lxml.html.fragment_fromstring(status_text).text
+
+        has_shop = len(has_shop_text.replace('&nbsp;', '').strip()) > 0
+
+        specialisation = specialisation.replace('&nbsp;', '').strip()
+        if len(specialisation) == 0:
+            specialisation = None
+
+        country = country.replace('&nbsp;', '').strip()
+        if len(country) == 0:
+            country = None
+
+        if len(website_link_text.replace('&nbsp;', '')) > 0:
+            website = lxml.html.fragment_fromstring(website_link_text).attrib['href']
+        else:
+            website = None
+
+        self.append(Label(label_link, status, has_shop, specialisation, country, website))
         
 
 
 @dataclass
 class BandGenre(PageDataType):
     profile_url: InitVar[str]
     band_key: str = field(init=False)
@@ -43,15 +64,15 @@
     band: str
     subgenre: str
     genre: str
 
     def __post_init__(self, profile_url: str):
         metallum_id = profile_url.split('/')[-1]
         self.metallum_id = int(metallum_id)
-        self.band_key = metallum_id + '-' + str(hash(self.band) % 2**sys.hash_info.width)
+        self.band_key = create_band_key(self.metallum_id, self.band)
 
 
 @dataclass
 class BandGenres(list, PageDataType):
     genre_page_record: InitVar[list[str]]
     genre: str = field(kw_only=True)
```

### Comparing `metalarchivist-0.2.0/src/metalarchivist/interface/theme.py` & `metalarchivist-0.2.1/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist/report.py` & `metalarchivist-0.2.1/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.2.1/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: lxml
 Requires-Dist: urllib3
+Requires-Dist: pycryptodome
 
 # MetalArchivist
 
 A Python package for extracting data from [Encyclopaedia Metallum](https://metal-archives.com)
```

### Comparing `metalarchivist-0.2.0/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.2.1/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/test/test_albums.py` & `metalarchivist-0.2.1/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/test/test_bands.py` & `metalarchivist-0.2.1/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/test/test_genres.py` & `metalarchivist-0.2.1/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.0/src/test/test_themes.py` & `metalarchivist-0.2.1/src/test/test_themes.py`

 * *Files identical despite different names*

