# Comparing `tmp/GeoHD-0.2.2.tar.gz` & `tmp/GeoHD-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.2.2.tar", last modified: Tue Apr  9 17:37:20 2024, max compression
+gzip compressed data, was "GeoHD-0.2.3.tar", last modified: Wed Apr 10 07:27:40 2024, max compression
```

## Comparing `GeoHD-0.2.2.tar` & `GeoHD-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 17:37:20.733774 GeoHD-0.2.2/
-drwxrwxrwx   0        0        0        0 2024-04-09 17:37:20.726890 GeoHD-0.2.2/GeoHD/
--rw-rw-rw-   0        0        0     8641 2024-04-09 17:31:08.000000 GeoHD-0.2.2/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.2.2/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.2.2/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.2.2/GeoHD/process.py
--rw-rw-rw-   0        0        0    32021 2024-04-09 17:31:08.000000 GeoHD-0.2.2/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.2.2/GeoHD/visualize.py
--rw-rw-rw-   0        0        0     9597 2024-04-09 17:31:08.000000 GeoHD-0.2.2/GeoHD/zone.py
-drwxrwxrwx   0        0        0        0 2024-04-09 17:37:20.732773 GeoHD-0.2.2/GeoHD.egg-info/
--rw-rw-rw-   0        0        0     5268 2024-04-09 17:37:20.000000 GeoHD-0.2.2/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-09 17:37:20.000000 GeoHD-0.2.2/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 17:37:20.000000 GeoHD-0.2.2/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-09 17:37:20.000000 GeoHD-0.2.2/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 17:37:20.000000 GeoHD-0.2.2/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     5268 2024-04-09 17:37:20.732773 GeoHD-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4772 2024-04-09 17:36:37.000000 GeoHD-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 17:37:20.733774 GeoHD-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-04-09 17:36:20.000000 GeoHD-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 17:37:20.731774 GeoHD-0.2.2/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.2.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:27:40.823289 GeoHD-0.2.3/
+drwxrwxrwx   0        0        0        0 2024-04-10 07:27:40.814772 GeoHD-0.2.3/GeoHD/
+-rw-rw-rw-   0        0        0     8641 2024-04-09 17:31:08.000000 GeoHD-0.2.3/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.2.3/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.2.3/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.2.3/GeoHD/process.py
+-rw-rw-rw-   0        0        0    32021 2024-04-09 17:31:08.000000 GeoHD-0.2.3/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.2.3/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0     9597 2024-04-09 17:31:08.000000 GeoHD-0.2.3/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:27:40.817340 GeoHD-0.2.3/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0     5268 2024-04-10 07:27:40.000000 GeoHD-0.2.3/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-04-10 07:27:40.000000 GeoHD-0.2.3/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 07:27:40.000000 GeoHD-0.2.3/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-10 07:27:40.000000 GeoHD-0.2.3/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 07:27:40.000000 GeoHD-0.2.3/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     5268 2024-04-10 07:27:40.822282 GeoHD-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4772 2024-04-10 07:24:03.000000 GeoHD-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 07:27:40.823289 GeoHD-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-04-10 07:24:03.000000 GeoHD-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:27:40.817340 GeoHD-0.2.3/test_local/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.2.3/test_local/__init__.py
```

### Comparing `GeoHD-0.2.2/GeoHD/AKDE.py` & `GeoHD-0.2.3/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.2/GeoHD/analyze.py` & `GeoHD-0.2.3/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.2/GeoHD/process.py` & `GeoHD-0.2.3/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.2/GeoHD/utils.py` & `GeoHD-0.2.3/GeoHD/utils.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.2/GeoHD/visualize.py` & `GeoHD-0.2.3/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.2/GeoHD/zone.py` & `GeoHD-0.2.3/GeoHD/zone.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.2/GeoHD.egg-info/PKG-INFO` & `GeoHD-0.2.3/GeoHD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -14,16 +14,16 @@
 Requires-Dist: geopandas
 Requires-Dist: pointpats
 Requires-Dist: h3
 
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.1-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.2.1-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.2.3-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.2.3-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
```

### Comparing `GeoHD-0.2.2/LICENSE` & `GeoHD-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.2/PKG-INFO` & `GeoHD-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -14,16 +14,16 @@
 Requires-Dist: geopandas
 Requires-Dist: pointpats
 Requires-Dist: h3
 
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.1-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.2.1-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.2.3-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.2.3-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
```

### Comparing `GeoHD-0.2.2/README.md` & `GeoHD-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.1-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.2.1-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.2.3-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.2.3-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
```

### Comparing `GeoHD-0.2.2/setup.py` & `GeoHD-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='GeoHD',
-    version='0.2.2',
+    version='0.2.3',
     description='A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data',
     author='Yuchen Yan',
     author_email='ycyan001@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yan-yuchen/GeoHD",    
     packages=find_packages(),
```

