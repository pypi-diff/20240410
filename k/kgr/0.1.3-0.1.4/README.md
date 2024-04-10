# Comparing `tmp/kgr-0.1.3.tar.gz` & `tmp/kgr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.1.3.tar", last modified: Wed Apr 10 15:51:12 2024, max compression
+gzip compressed data, was "kgr-0.1.4.tar", last modified: Wed Apr 10 16:06:59 2024, max compression
```

## Comparing `kgr-0.1.3.tar` & `kgr-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-04-10 14:38:49.000000 kgr-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2024-04-10 14:34:29.000000 kgr-0.1.3/README.md
--rw-r--r--   0        0        0      737 2024-04-10 15:51:12.381149 kgr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 14:21:46.000000 kgr-0.1.3/src/kgr/__init__.py
--rw-r--r--   0        0        0     8963 2024-04-10 14:22:03.000000 kgr-0.1.3/src/kgr/__main__.py
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 kgr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-10 14:38:49.000000 kgr-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-10 14:34:29.000000 kgr-0.1.4/README.md
+-rw-r--r--   0        0        0      692 2024-04-10 16:06:59.370105 kgr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 14:21:46.000000 kgr-0.1.4/src/kgr/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-10 16:04:38.945223 kgr-0.1.4/src/kgr/__main__.py
+-rw-r--r--   0        0        0     8926 2024-04-10 16:04:20.034492 kgr-0.1.4/src/kgr/lib.py
+-rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 kgr-0.1.4/PKG-INFO
```

### Comparing `kgr-0.1.3/LICENSE` & `kgr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.1.3/pyproject.toml` & `kgr-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
@@ -27,11 +27,8 @@
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.license]
 file = "LICENSE"
 
-[project.scripts]
-kgr = "kgr.__main__:main"
-
 [tool]
```

### Comparing `kgr-0.1.3/src/kgr/__main__.py` & `kgr-0.1.4/src/kgr/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from argparse import ArgumentParser
-from random import uniform
 from csv import DictReader, DictWriter
-from requests import get
-from xml.dom.minidom import Document
+from random import uniform
 from sys import stderr
+from xml.dom.minidom import Document
 
-from geopy.geocoders import Nominatim
 from bs4 import BeautifulSoup
+from geopy.geocoders import Nominatim
+from requests import get
 
 
 def get_description_and_img(src: str):
 	soup = BeautifulSoup(get(src).content, 'html.parser')
 	description_tag = soup.select_one('div.human-dossier__art > p > p')
 	if not description_tag or description_tag.text.strip().startswith("Включение конкретного человека в список"):
 		description_tag = soup.select_one('div.human-dossier__art > p')
@@ -225,11 +225,7 @@
 			prepare(args)
 		case "geocode":
 			geocode(args)
 		case "convert":
 			convert(args)
 		case _:
 			parser.print_help()
-
-
-if __name__ == "__main__":
-	main()
```

### Comparing `kgr-0.1.3/PKG-INFO` & `kgr-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Miltitool for convert data from https://memopzk.org to Google Maps
 Author-Email: Dmitry Luschan <dluschan@gmail.com>
 Maintainer-Email: Dmitry Luschan <dluschan@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

