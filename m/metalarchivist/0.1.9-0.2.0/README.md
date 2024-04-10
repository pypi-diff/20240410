# Comparing `tmp/metalarchivist-0.1.9.tar.gz` & `tmp/metalarchivist-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.1.9.tar", last modified: Sat Nov 25 16:46:12 2023, max compression
+gzip compressed data, was "metalarchivist-0.2.0.tar", last modified: Wed Apr 10 11:59:58 2024, max compression
```

## Comparing `metalarchivist-0.1.9.tar` & `metalarchivist-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.957296 metalarchivist-0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      674 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-25 16:46:12.957296 metalarchivist-0.1.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.952296 metalarchivist-0.1.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.953296 metalarchivist-0.1.9/src/metalarchivist/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.955296 metalarchivist-0.1.9/src/metalarchivist/export/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/export/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6601 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/export/album.py
--rw-rw-rw-   0 root         (0) root         (0)     3716 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/src/metalarchivist/interface/
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7054 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/interface/album.py
--rw-rw-rw-   0 root         (0) root         (0)    12838 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      674 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      570 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/src/test/
--rw-rw-rw-   0 root         (0) root         (0)     9712 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/test/test_albums.py
--rw-rw-rw-   0 root         (0) root         (0)     5963 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/test/test_band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      674 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      661 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.206329 metalarchivist-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.207329 metalarchivist-0.2.0/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.210329 metalarchivist-0.2.0/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/user-agents.json
+-rwxrwxrwx   0 root         (0) root         (0)     5445 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.211329 metalarchivist-0.2.0/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)      862 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     8202 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/page.py
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.213328 metalarchivist-0.2.0/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      674 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 11:59:58.000000 metalarchivist-0.2.0/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:59:58.212329 metalarchivist-0.2.0/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     4918 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 11:59:45.000000 metalarchivist-0.2.0/src/test/test_themes.py
```

### Comparing `metalarchivist-0.1.9/LICENSE` & `metalarchivist-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.9/PKG-INFO` & `metalarchivist-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.1.9/pyproject.toml` & `metalarchivist-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 [project]
 name = "metalarchivist"
-version = "0.1.9"
+version = "0.2.0"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3" ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
   "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/black-metal-book-club/metallum"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["*.json"]
+
 [tool.ruff]
 line-length = 100
```

### Comparing `metalarchivist-0.1.9/src/metalarchivist/interface/album.py` & `metalarchivist-0.2.0/src/metalarchivist/interface/album.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,143 @@
-
+ 
 import re
 from datetime import datetime
-from dataclasses import dataclass, field, InitVar
-
-from .band import BandLink, Genres
+from dataclasses import dataclass, field, InitVar, asdict
 
+import lxml.etree
 import lxml.html
 
+from .band import BandLink
 
-@dataclass
-class AlbumLink:
-    name: str = field(init=False)
-    link: str = field(init=False)
 
-    def __init__(self, html: str):
-        html_anchor = lxml.html.fragment_fromstring(html)
-        self.name = html_anchor.text
-        self.link = html_anchor.attrib['href']
 
+class ParseError(Exception):
+    ...
 
 
-@dataclass
-class AlbumRelease:    
-    band: BandLink
-    album: AlbumLink
-
-    release_type: str
-    genres: Genres
-    release_date_display: InitVar[str]
-    added_date_display: InitVar[str | None] = field(default=None)
-
-    release_date: str = field(init=False)
-    added_date: str | None = field(init=False)
-
-    def __post_init__(self, release_date_display, added_date_display):
-        release_date = re.sub(r',', '', release_date_display)
-        release_date = re.sub(r'(\d)st', r'\g<1>', release_date)
-        release_date = re.sub(r'(\d)nd', r'\g<1>', release_date)
-        release_date = re.sub(r'(\d)rd', r'\g<1>', release_date)
-        release_date = re.sub(r'(\d)th', r'\g<1>', release_date)
-        release_date = re.sub(r'\s(\d)\s', r' 0\g<1> ', release_date)
-
-        release_date_parsed = self._try_parse_release_date(release_date, '%B %d %Y')
-        if not release_date_parsed:
-            release_date_parsed = self._try_parse_release_date(release_date, '%B %Y')
-        if not release_date_parsed:
-            release_date_parsed = self._try_parse_release_date(release_date, '%Y-%m-%d %H:%M:%S')
-
-        self.release_date = release_date_parsed
-
-        if added_date_display == 'N/A' or added_date_display is None:
-            self.added_date = None
-        else:
-            added_date = re.sub(r'\/(\d)\/', '/0\1/', added_date_display)
-            self.added_date = datetime.strptime(added_date, '%Y-%m-%d %H:%M:%S') \
-                                      .strftime('%Y-%m-%dT%H:%M:%SZ')
+def _parse_release_date(release_date) -> str:
+    """ Normalizes textual release dates to a datetime object """
 
-    @staticmethod
     def _try_parse_release_date(release_date: str, date_format: str):
         try:
             return datetime.strptime(release_date, date_format) \
                            .date().strftime('%Y-%m-%d')
         except ValueError:
             return None
 
+    release_date = re.sub(r',', '', release_date)
+    release_date = re.sub(r'(\d)st', r'\g<1>', release_date)
+    release_date = re.sub(r'(\d)nd', r'\g<1>', release_date)
+    release_date = re.sub(r'(\d)rd', r'\g<1>', release_date)
+    release_date = re.sub(r'(\d)th', r'\g<1>', release_date)
+    release_date = re.sub(r'\s(\d)\s', r' 0\g<1> ', release_date)
+
+    release_date_parsed = _try_parse_release_date(release_date, '%B %d %Y')
+    if not release_date_parsed:
+        release_date_parsed = _try_parse_release_date(release_date, '%B %Y')
+    if not release_date_parsed:
+        release_date_parsed = _try_parse_release_date(release_date, '%Y-%m-%d %H:%M:%S')
+
+    if release_date_parsed is None:
+        raise ParseError('unable to parse release date')
+
+    return release_date_parsed
+
+
+@dataclass
+class AlbumLink:
+    """ The data within an HTML anchor tag pointing to an album page """
+    name: str = field(init=False)
+    link: str = field(init=False)
+
+    def __init__(self, html: str):
+        html_anchor = lxml.html.fragment_fromstring(html)
+        self.name = html_anchor.text
+        self.link = html_anchor.attrib['href']
+
 
 @dataclass
 class AlbumTrackLength:
+    """ Numerically defines the length of an album track """
     length_text: InitVar[str]
-    hours: int = field(init=False)
-    minutes: int = field(init=False)
+    hours: int = field(init=False, default=0)
+    minutes: int = field(init=False, default=0)
     seconds: int = field(init=False)
 
     def __post_init__(self, length_text: str):
-        ...
+        split_length_text = length_text.split(':')[::-1]
+
+        self.seconds = int(split_length_text[0])
+
+        try:
+            self.minutes = int(split_length_text[1])
+            self.hours = int(split_length_text[2])
+        except IndexError:
+            pass
 
 
 @dataclass
 class AlbumTrack:
-    tablerow: InitVar[lxml.html.Element]
+    """ A unique track on an album """
+    tablerow: InitVar[lxml.etree.ElementBase]
 
     metallum_id: int = field(init=False)
     number: str = field(init=False)
     title: str = field(init=False)
     length: AlbumTrackLength = field(init=False)
     lyrics: str = field(init=False)
 
-    def __post_init__(self, tablerow: lxml.html.Element):
+    def __post_init__(self, tablerow: lxml.etree.ElementBase):
         number, title, length, lyrics = tablerow.xpath('./td')
         metallum_id = number.xpath('./a').pop().attrib['name']
 
         self.metallum_id = int(metallum_id)
         self.title = title.text
+        self.number = number.text
+        self.length = AlbumTrackLength(length.text)
+        self.lyrics = lyrics.text
 
 
 @dataclass
 class AlbumDescription:
-    release_type: str
-    release_date: str
-    catalog_id: str
-    label: str
-    media_format: str
+    """ Additional information concerning an album """
+    release_type: str | None
+    release_date: str | None
+    catalog_id: str | None
+    label: str | None
+    media_format: str | None
     version_desc: str | None = field(default=None)
     limitation: str | None = field(default=None)
     reviews: str | None = field(default=None)
 
 
 @dataclass
 class AlbumProfile:
+    """ An album profile page """
     url: str
     html: InitVar[bytes]
 
     name: str = field(init=False)
     metallum_id: int = field(init=False)
+    
+    band: BandLink = field(init=False)
     tracklist: list[AlbumTrack] = field(init=False)
     description: AlbumDescription = field(init=False)
 
     def __post_init__(self, profile_html):
         self.metallum_id = int(self.url.split('/')[-1])
 
         profile_document = lxml.html.document_fromstring(profile_html)
+
+        self.name = profile_document.xpath('.//h1[@class="album_name"]/a/text()').pop()
+
+        band_link = profile_document.xpath('.//h2[@class="band_name"]/a').pop()
+        band_link_str = lxml.etree.tostring(band_link).decode('utf-8').split('\n')[0]
+        self.band = BandLink(band_link_str)
+
         album_desc_titles_xpath = '//div[@id="album_info"]/dl/dt/text()'
         album_desc_titles = profile_document.xpath(album_desc_titles_xpath)
 
         album_desc_detail_xpath = '//div[@id="album_info"]/dl/dd/text()'
         album_desc_detail = profile_document.xpath(album_desc_detail_xpath)
 
         self.description = self._parse_description(album_desc_titles, album_desc_detail)
@@ -157,55 +171,15 @@
         if key == 'type':
             return 'release_type'
 
         if key == 'format':
             return 'media_format'
 
         return key
-
-
-@dataclass
-class ReleasePage:
-    total_records: int = field(init=False)
-    total_display_records: int = field(init=False)
-    echo: int = field(init=False)
-    data: list[AlbumRelease] = field(init=False)
-
-    def __init__(self, i_total_records: int, i_total_display_records: int,
-                 s_echo: int, aa_data: list):
-
-        self.total_records = i_total_records
-        self.total_display_records = i_total_display_records
-        self.echo = s_echo
-        self.data = sum(list(map(self._process_album_release, aa_data)), [])
-
-    def __add__(self, other):
-        if not isinstance(other, self.__class__):
-            raise TypeError('ReleasePage objects can only be summed '
-                            'with other ReleasePage objects')
-
-        self.data += other.data
-        return self
     
-    @staticmethod
-    def _process_album_release(record: list[str]) -> list[AlbumRelease]:
-        """ returns a list to handle the potential for splits """
-
-        band_link, album_link, release_type, genres, themes, *dates = record
-
-        if re.search(r'>\s?\/\s?<', band_link):
-            band_links = band_link.split(' / ')
-            genre_list = genres.split(' | ')
-
-            return [AlbumRelease(BandLink(link), AlbumLink(album_link), 
-                                 release_type, Genres(genre), *dates)
-                    for link, genre in zip(band_links, genre_list)]
-
-        return [AlbumRelease(BandLink(band_link), AlbumLink(album_link), 
-                             release_type, Genres(genres), *dates)]
-
-
-class ReleasePages(list):
-    def combine(self) -> ReleasePage:
-        first_page, *remaining = self
-        return sum(remaining, start=first_page)
-
+    @property
+    def release_date(self):
+        return _parse_release_date(self.description.release_date)
+    
+    
+    def to_json(self):
+        return asdict(self)
```

### Comparing `metalarchivist-0.1.9/src/metalarchivist/report.py` & `metalarchivist-0.2.0/src/metalarchivist/report.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,92 @@
+from datetime import datetime
 from dataclasses import asdict
 
-from .export import Band, Album
+from .export import Band, Album, Genre
 
+Series = list[str | int | float]
+Record = dict[str, str | float | int | list]
+Dataset = list[Record]
 
-def select(from_list, column) -> list[dict]:
+
+def series(from_list, column) -> Series:
+    return [[v for k, v in d.items() if k == column].pop() for d in from_list]
+
+
+def select(from_list, column) -> Dataset:
     return list(map(lambda n: {column: n[column]}, from_list))
 
 
-def expand(from_list, column) -> list[dict]:
+def expand(from_list, column) -> Dataset:
     return list(map(lambda n: dict(**n[column]), from_list))
 
 
-def drop(from_list, *columns) -> list[dict]:
+def drop(from_list, *columns) -> Dataset:
     return [{k: v for k, v in d.items() if k not in columns} for d in from_list]
 
 
-def series(from_list, column) -> list[str | int | float]:
-    return [[v for k, v in d.items() if k == column].pop() for d in from_list]
+def rename(from_list, column_map: dict) -> Dataset:
+    return [{column_map.get(k, k): v for k, v in d.items()} for d in from_list]
 
 
-def join(first_list, second_list, on_column) -> list[dict]:
+def join(first_list: Dataset, second_list: Dataset, on_column: str) -> Dataset:
     return [dict(**left, **{k: v for k, v in right.items() if k not in left}) 
             for left in first_list for right in second_list 
             if left[on_column] == right[on_column]]
 
 
-def rename(from_list, column_map: dict):
-    return [{column_map.get(k, k): v for k, v in d.items()} for d in from_list]
-
-
-def get_bands(profile_urls: list[str], verbose=False) -> list[dict]:
-    band_profile = Band.get_profiles(profile_urls, verbose=verbose)
+def get_bands(profile_urls: list[str], wait=3.) -> Dataset:
+    band_profile = Band.get_profiles(profile_urls, wait=wait)
     band_profile = list(map(lambda n: n.to_dict(), band_profile))
     
     band_desc = expand(select(band_profile, 'description'), 'description')
     band_desc = drop(band_desc, 'genre', 'themes', 'lyrical_themes')
 
+    band_ids = series(band_profile, 'metallum_id')
+    band_ids = [int(band_id) for band_id in band_ids]
+    band_links = Band.get_profiles_links(band_ids, wait=wait)
+    band_links = list(map(asdict, band_links))
+
     genres = expand(select(band_profile, 'genres'), 'genres')
     themes = expand(select(band_profile, 'themes'), 'themes')
 
     band_profile = drop(band_profile, 'genres', 'themes',  'description')
+    band_profile = join(band_profile, band_links, 'metallum_id')
+
     band_zip = zip(band_profile, band_desc, genres, themes)
 
     return [dict(**bp, **bd, **g, **t) for bp, bd, g, t in band_zip]
 
 
-def get_albums(range_start=None, range_stop=None, verbose=False) -> list[dict]:
+def get_albums(range_start: datetime | None = None, range_stop: datetime | None = None, 
+               wait=3., retries=3, timeout=3.) -> Dataset:
     if range_start:
-        release_page = Album.get_range(range_start, range_stop, verbose=verbose)
+        release_page = Album.get_range(range_start, range_stop, wait=wait, retries=retries, 
+                                       timeout_cxn=timeout, timeout_read=timeout * 3)
     else:
-        release_page = Album.get_upcoming(verbose=verbose)
+        release_page = Album.get_upcoming(wait=wait, retries=retries, timeout_cxn=timeout, 
+                                          timeout_read=timeout * 3)
 
     release = list(map(asdict, release_page.data))
 
     # hoist out the link attributes from each band
     profile_urls = select(expand(select(release, 'band'), 'band'), 'link')
     profile_urls = series(profile_urls, 'link')
+    profile_urls = [str(p) for p in profile_urls]
 
-    band = get_bands(profile_urls, verbose=verbose)
+    band = get_bands(profile_urls, wait=wait)
 
     album = expand(select(release, 'album'), 'album')
     album = rename(album, dict(name='album', link='album_url'))
 
     band = rename(band, dict(url='band_url', name='band'))
     release = drop(release, 'genres', 'band', 'album')
-    album_zip = zip(album, band, release)
+    profile_urls = [dict(band_url=u) for u in profile_urls]
+    album_zip = zip(album, profile_urls, release)
 
-    album = [dict(**a, **b, **r) for a, b, r in album_zip]
+    album = [dict(**a, **u, **r) for a, u, r in album_zip]
 
     return join(album, band, 'band_url')
+
+
+def get_genres():
+    ...
```

### Comparing `metalarchivist-0.1.9/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.2.0/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.1.9/src/test/test_albums.py` & `metalarchivist-0.2.0/src/test/test_albums.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import unittest
 import importlib.util
 from types import ModuleType
 from enum import Enum
 
 from configparser import ConfigParser
-from datetime import datetime, date
+from datetime import datetime, date, timedelta
 
 
 class Submodule(Enum):
     MODULE = 'metalarchivist', './src/metalarchivist/__init__.py'
     EXPORT = 'metalarchivist.export', './src/metalarchivist/export/__init__.py'
     IFACE = 'metalarchivist.interface', './src/metalarchivist/interface/__init__.py'
 
@@ -20,255 +20,248 @@
 def run_test_cases():
     unittest.main(argv=[''], verbosity=2)
 
 
 def prepare_submodule(submodule: Submodule) -> ModuleType:
     submodule_name, submodule_path = submodule.value
     spec = importlib.util.spec_from_file_location(submodule_name, submodule_path)
-    module = importlib.util.module_from_spec(spec)
-    sys.modules[submodule_name] = module
-    spec.loader.exec_module(module)
+    if spec is not None and spec.loader is not None:
+        module = importlib.util.module_from_spec(spec)
+        sys.modules[submodule_name] = module
+        spec.loader.exec_module(module)
+    else:
+        raise ImportError(f'could not load {submodule_name}')
 
     return module
 
 
-def load_submodules() -> tuple[ModuleType, ModuleType, ModuleType]:
+def load_module():
+    config = ConfigParser()
+    config.read_dict({'unittests': {'OUTPUTDIR': './'}})
+    config.read('metallum.cfg')
+
+    metalarchivist = prepare_submodule(Submodule.MODULE)
     interface = prepare_submodule(Submodule.IFACE)
     export = prepare_submodule(Submodule.EXPORT)
-    metalarchivist = prepare_submodule(Submodule.REPORT)
 
-    return interface, export, metalarchivist
+    return metalarchivist, interface, export, config
 
 
 class TestMetalArchivesDirectory(unittest.TestCase):
-
-    def test_releases_endpoint(self):
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
-
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
-        
-        self.assertIn('MetalArchivesDirectory', dir(export))
+    metalarchivist, interface, export, config = load_module()
+    
+    def test_releases_endpoint(self):        
+        self.assertIn('MetalArchives', dir(self.export))
 
         range_start = datetime(1990, 1, 1).strftime('%Y-%m-%d')
         range_stop = datetime(1990, 12, 31).strftime('%Y-%m-%d')
 
         self.assertEqual(range_start, '1990-01-01')
         self.assertEqual(range_stop, '1990-12-31')
 
         expected_endpoint = ('https://www.metal-archives.com/release/ajax-upcoming/json/1'
                              '?sEcho=0&iDisplayStart=0&iDisplayLength=100'
                              '&fromDate=1990-01-01&toDate=1990-12-31')
 
         endpoint_query = dict(from_date=range_start, to_date=range_stop)
-        actual_endpoint = export.MetalArchivesDirectory.upcoming_releases(**endpoint_query)
+        actual_endpoint = self.export.MetalArchives.upcoming_releases(**endpoint_query)
 
         self.assertEqual(expected_endpoint, actual_endpoint)
 
 
 class TestAlbums(unittest.TestCase):
+    metalarchivist, interface, export, config = load_module()
+    
+    def test_date_formatting(self):
+        album_profile = self.export.Album.get_profile('https://www.metal-archives.com/albums/Panopticon/The_Rime_of_Memory/1163524')
+        self.assertEqual(album_profile.release_date, '2023-11-29')
+
+    def test_release_date_formatting(self):
+        release_page = self.export.Album.get_range(datetime(2023, 11, 29), datetime(2023, 11, 29), timeout_read=90.)
+        for release in release_page.data:
+            self.assertEqual(release.release_date, '2023-11-29')
 
     def test_releases(self):
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
+        self.assertIn('Album', dir(self.export))
 
-        export = prepare_submodule(Submodule.EXPORT)
-        
-        self.assertIn('Album', dir(export))
-
-        upcoming_component_attributes = dir(export.Album)
+        upcoming_component_attributes = dir(self.export.Album)
         self.assertIn('get_all', upcoming_component_attributes)
         self.assertIn('get_upcoming', upcoming_component_attributes)
         self.assertIn('get_range', upcoming_component_attributes)
 
     def test_release_fields(self):
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
-
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
-        
-        releases = export.Album.get_upcoming(verbose=True)
+        releases = self.export.Album.get_range(date.today(), date.today() + timedelta(days=1))
 
         releases_attributes = dir(releases)
         self.assertIn('total_records', releases_attributes)
         self.assertIn('total_display_records', releases_attributes)
         self.assertIn('echo', releases_attributes)
         self.assertIn('data', releases_attributes)
 
         self.assertIsInstance(releases.total_records, int)
         self.assertIsInstance(releases.total_display_records, int)
         self.assertIsInstance(releases.echo, int)
         self.assertIsInstance(releases.data, list)
 
         self.assertEqual(releases.total_records, releases.total_display_records)
-        self.assertEqual(releases.echo, 0)
+        self.assertGreaterEqual(releases.echo, 0)
 
     def test_upcoming(self):
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
-
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
-
-        releases = export.Album.get_upcoming(verbose=True)
+        releases = self.export.Album.get_upcoming(timeout_read=90.)
         self.assertIsNotNone(releases)
-        self.assertIsInstance(releases, interface.ReleasePage)
+        self.assertIsInstance(releases, self.interface.ReleasePage)
 
         data = releases.data
         self.assertIsInstance(data, list)
         self.assertGreaterEqual(len(data), releases.total_records)
 
         album_release = data.pop()
-        self.assertIsInstance(album_release, interface.AlbumRelease)
+        self.assertIsInstance(album_release, self.interface.AlbumRelease)
 
     def test_range(self):
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
-
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
 
-        self.assertIn('Album', dir(export))
+        self.assertIn('Album', dir(self.export))
 
-        releases = export.Album.get_range(datetime(1990, 1, 1), datetime(1990, 12, 31), 
-                                          verbose=True)
+        releases = self.export.Album.get_range(datetime(1990, 1, 1), datetime(1990, 1, 31), timeout_read=90.)
         self.assertIsNotNone(releases)
-        self.assertIsInstance(releases, interface.ReleasePage)
+        self.assertIsInstance(releases, self.interface.ReleasePage)
 
         total_records = releases.total_records
         total_display_records = releases.total_display_records
         self.assertEqual(total_records, total_display_records)
 
-        self.assertEqual(releases.echo, 0)
+        self.assertGreaterEqual(releases.echo, 0)
 
         data = releases.data
         self.assertIsInstance(data, list)
         self.assertGreaterEqual(len(data), total_records)
 
         album_release = data.pop()
-        self.assertIsInstance(album_release, interface.AlbumRelease)
+        self.assertIsInstance(album_release, self.interface.AlbumRelease)
+
+    # def test_decode_error_handling(self):
+
+    #     self.assertIn('Album', dir(self.export))
+
+    #     releases = self.export.Album.get_range(datetime(2011, 1, 30), datetime(2011, 1, 30))
+    #     self.assertIsNotNone(releases)
+    #     self.assertIsInstance(releases, self.interface.ReleasePage)
+    #     self.assertIsNotNone(releases.error)
+
+    #     total_records = releases.total_records
+    #     total_display_records = releases.total_display_records
+    #     self.assertEqual(total_records, total_display_records)
+
+    #     self.assertGreaterEqual(releases.echo, 0)
+
+    #     data = releases.data
+    #     self.assertIsInstance(data, list)
+    #     self.assertGreaterEqual(len(data), total_records)
+
+    #     album_release = data.pop()
+    #     self.assertIsInstance(album_release, self.interface.AlbumRelease)
 
     def test_range_with_null_upper_bound(self):
         interface = prepare_submodule(Submodule.IFACE)
         self.assertIsNotNone(interface)
 
         export = prepare_submodule(Submodule.EXPORT)
         self.assertIsNotNone(export)
 
         self.assertIn('Album', dir(export))
 
-        releases = export.Album.get_range(datetime(2023, 11, 1), verbose=True)
+        releases = export.Album.get_range(date.today(), timeout_read=90.)
         self.assertIsNotNone(releases)
         self.assertIsInstance(releases, interface.ReleasePage)
 
         total_records = releases.total_records
         total_display_records = releases.total_display_records
         self.assertEqual(total_records, total_display_records)
 
-        self.assertEqual(releases.echo, 0)
+        self.assertGreaterEqual(releases.echo, 0)
 
         data = releases.data
         self.assertIsInstance(data, list)
         self.assertGreaterEqual(len(data), total_records)
 
         album_release = data.pop()
         self.assertIsInstance(album_release, interface.AlbumRelease)
 
     def test_album_release(self):
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
 
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
-
-        self.assertIn('Album', dir(export))
+        self.assertIn('Album', dir(self.export))
 
-        releases = export.Album.get_range(datetime(2023, 8, 11), verbose=True)
+        releases = self.export.Album.get_range(datetime(2023, 8, 11), datetime(2023, 8, 11), timeout_read=90.)
 
         data = releases.data
         self.assertIsInstance(data, list)
 
         # can be greater than total records due to split albums
         self.assertGreaterEqual(len(data), releases.total_records)
 
         album_release = data.pop()
-        self.assertIsInstance(album_release, interface.AlbumRelease)
+        self.assertIsInstance(album_release, self.interface.AlbumRelease)
 
         self.assertIn('release_type', dir(album_release))
         self.assertIn('genres', dir(album_release))
         self.assertIn('release_date', dir(album_release))
         self.assertIn('added_date', dir(album_release))
         self.assertIn('band', dir(album_release))
         self.assertIn('album', dir(album_release))
 
-        self.assertIsInstance(album_release.genres, interface.Genres)
-
+        self.assertIsInstance(album_release.genres, self.interface.Subgenres)
         self.assertIsInstance(album_release.release_date, str)
 
         if album_release.added_date:
             self.assertIsInstance(album_release.added_date, str)
 
-        self.assertIsInstance(album_release.band, interface.BandLink)
-        self.assertIsInstance(album_release.album, interface.AlbumLink)
+        self.assertIsInstance(album_release.band, self.interface.BandLink)
+        self.assertIsInstance(album_release.album, self.interface.AlbumLink)
 
     def test_release_report(self):
-        config = ConfigParser({'unittests': {'OUTPUTDIR': './'}})
-        config.read('metallum.cfg')
-
-        metalarchivist = prepare_submodule(Submodule.MODULE)
-        self.assertIsNotNone(metalarchivist)
-
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
-
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
 
-        releases = metalarchivist.get_albums(datetime(2023, 11, 22), datetime(2023, 11, 23), verbose=True)
+        releases = self.metalarchivist.get_albums(date.today(), date.today(), wait=.5, timeout=90.)
         self.assertIsInstance(releases, list)
 
-        output_path = os.path.join(config['unittests']['OUTPUTDIR'], 'test-bands.json')
+        for release in releases:
+            album_band = release['album_url'].split('/')[-3]
+            band = release['band_url'].split('/')[-2]
+            self.assertIn(band, album_band)
+
+        output_path = os.path.join(self.config['unittests']['OUTPUTDIR'], 'test-releases.json')
         json.dump(releases, open(output_path, 'w'))
 
     def test_album_profile(self):
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
+        self.assertIn('Album', dir(self.export))
 
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
-
-        self.assertIn('Album', dir(export))
-
-        album = export.Album.get_profile('https://www.metal-archives.com/albums/Urfaust/Untergang/1161736')
+        album = self.export.Album.get_profile('https://www.metal-archives.com/albums/Urfaust/Untergang/1161736')
         self.assertIsNotNone(album)
 
-    def test_album_profiles(self):  
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
+        album_json = album.to_json()
+        album_band_link = album_json['band']
 
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
+        self.assertIn('band_key', album_band_link)
 
-        self.assertIn('Album', dir(export))
+    def test_album_profiles(self):
+
+        self.assertIn('Album', dir(self.export))
 
-        album = export.Album.get_profiles(['https://www.metal-archives.com/albums/Urfaust/Untergang/1161736',
-                                           'https://www.metal-archives.com/albums/Furia/Huta_Luna/1166382',
-                                           'https://www.metal-archives.com/albums/Hades_Almighty/...Again_Shall_Be/91367'])
+        album = self.export.Album.get_profiles(['https://www.metal-archives.com/albums/Urfaust/Untergang/1161736',
+                                                'https://www.metal-archives.com/albums/Furia/Huta_Luna/1166382',
+                                                'https://www.metal-archives.com/albums/Hades_Almighty/...Again_Shall_Be/91367'])
         self.assertIsNotNone(album)
 
-    def test_album_themes(self):
-        metalarchivist = prepare_submodule(Submodule.MODULE)
-        self.assertIsNotNone(metalarchivist)
+    # def test_album_themes(self):
+    #     metalarchivist = prepare_submodule(Submodule.MODULE)
+    #     self.assertIsNotNone(metalarchivist)
 
-        interface = prepare_submodule(Submodule.IFACE)
-        self.assertIsNotNone(interface)
+    #     interface = prepare_submodule(Submodule.IFACE)
+    #     self.assertIsNotNone(interface)
 
-        export = prepare_submodule(Submodule.EXPORT)
-        self.assertIsNotNone(export)
+    #     export = prepare_submodule(Submodule.EXPORT)
+    #     self.assertIsNotNone(export)
 
-        albums = metalarchivist.get_albums(verbose=True)
+    #     albums = metalarchivist.get_albums()
 
 
 if __name__ == '__main__':
     run_test_cases()
```

