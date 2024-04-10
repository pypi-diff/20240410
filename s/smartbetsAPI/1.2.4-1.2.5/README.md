# Comparing `tmp/smartbetsAPI-1.2.4.tar.gz` & `tmp/smartbetsAPI-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.2.4.tar", last modified: Wed Apr 10 15:00:54 2024, max compression
+gzip compressed data, was "smartbetsAPI-1.2.5.tar", last modified: Wed Apr 10 15:31:24 2024, max compression
```

## Comparing `smartbetsAPI-1.2.4.tar` & `smartbetsAPI-1.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/LICENSE
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9382 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/README.md
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/setup.cfg
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2407 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/setup.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       95 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/smartbets_API/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/smartbets_API/__init__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/__main__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/bet_analyzer.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2747 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/smartbets_API/bet_at_rest_api_level.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/bet_common.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/configuration_handler.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/figure_harvester.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/googler.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/html_fetcher.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5346 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/smartbets_API/interface.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/predictor.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/proxyh.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/tertiary_bet.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:31:24.807828 smartbetsAPI-1.2.5/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.5/LICENSE
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 15:31:24.807828 smartbetsAPI-1.2.5/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9382 2024-04-10 15:30:04.000000 smartbetsAPI-1.2.5/README.md
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-10 15:31:24.807828 smartbetsAPI-1.2.5/setup.cfg
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2407 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.5/setup.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:31:24.807828 smartbetsAPI-1.2.5/smartbetsAPI.egg-info/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 15:31:24.000000 smartbetsAPI-1.2.5/smartbetsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-10 15:31:24.000000 smartbetsAPI-1.2.5/smartbetsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-10 15:31:24.000000 smartbetsAPI-1.2.5/smartbetsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-10 15:31:24.000000 smartbetsAPI-1.2.5/smartbetsAPI.egg-info/entry_points.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       95 2024-04-10 15:31:24.000000 smartbetsAPI-1.2.5/smartbetsAPI.egg-info/requires.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-10 15:31:24.000000 smartbetsAPI-1.2.5/smartbetsAPI.egg-info/top_level.txt
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:31:24.807828 smartbetsAPI-1.2.5/smartbets_API/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-10 15:30:04.000000 smartbetsAPI-1.2.5/smartbets_API/__init__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.5/smartbets_API/__main__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.5/smartbets_API/bet_analyzer.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2747 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.5/smartbets_API/bet_at_rest_api_level.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.5/smartbets_API/bet_common.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.5/smartbets_API/configuration_handler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.5/smartbets_API/figure_harvester.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.5/smartbets_API/googler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.5/smartbets_API/html_fetcher.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6062 2024-04-10 15:30:04.000000 smartbetsAPI-1.2.5/smartbets_API/interface.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.5/smartbets_API/predictor.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.5/smartbets_API/proxyh.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.5/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.2.4/LICENSE` & `smartbetsAPI-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/PKG-INFO` & `smartbetsAPI-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.4
+Version: 1.2.5
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -41,15 +41,15 @@
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.4&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.5&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.4 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.5 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
```

### Comparing `smartbetsAPI-1.2.4/README.md` & `smartbetsAPI-1.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 align="center">smartbetsAPI</h1>
 <p align="center">
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.4&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.5&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
  
  > "Punter's choice" 
 
  Worldwide soccer-matches predictor with Fast-API and a package for integrating the scripts in your own [Python](https://python.org) code.
 
  ## Features
```

### Comparing `smartbetsAPI-1.2.4/setup.py` & `smartbetsAPI-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbetsAPI.egg-info/PKG-INFO` & `smartbetsAPI-1.2.5/smartbetsAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.4
+Version: 1.2.5
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -41,15 +41,15 @@
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.4&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.5&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.4 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.5 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
```

### Comparing `smartbetsAPI-1.2.4/smartbetsAPI.egg-info/SOURCES.txt` & `smartbetsAPI-1.2.5/smartbetsAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/bet_analyzer.py` & `smartbetsAPI-1.2.5/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/bet_at_rest_api_level.py` & `smartbetsAPI-1.2.5/smartbets_API/bet_at_rest_api_level.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/bet_common.py` & `smartbetsAPI-1.2.5/smartbets_API/bet_common.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/configuration_handler.py` & `smartbetsAPI-1.2.5/smartbets_API/configuration_handler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/figure_harvester.py` & `smartbetsAPI-1.2.5/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/googler.py` & `smartbetsAPI-1.2.5/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/html_fetcher.py` & `smartbetsAPI-1.2.5/smartbets_API/html_fetcher.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/interface.py` & `smartbetsAPI-1.2.5/smartbets_API/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,35 +99,53 @@
 
 v1_auth_scheme = OAuth2PasswordBearer(
     tokenUrl="/v1/token", description="Token set at server launch."
 )
 
 
 class Match(BaseModel):
-    """Football match teams and net flag"""
+    """Football match teams and net flag
+    - `home` : Home team (1)
+    - `away` : Away team (2)
+    - `net` : Use latest data from internet
+    """
 
     home: str
     away: str
     net: bool = False
 
 
 class Prediction(BaseModel):
-    """Match prediction"""
+    """Match prediction
+    - `g` :	Goal-average of the two teams
+    - `gg` : Probability of both teams to score
+    - `ov15` : Probability of having more than 2 goals
+    - `ov25` : Probability of having more than 3 goals
+    - `ov35` : Probability of having more than 4 goals
+    - `choice` : Probability of the specified 'result' to occur
+    - `result` : The most suitable outcome from [1,1x,x,2x,2]
+    - `pick` : The most suitable outcome from [1,1x,x,2x,2,gg,ov15,ov25,ov35]
+    """
 
     g: float
     gg: float
     ov15: float
     ov25: float
     ov35: float
     choice: float
     result: str
     pick: str
 
 
 class ServerStatus(BaseModel):
+    """Checks server's running status
+    - `is_alive` : Is server running?
+    - `as_at` : Datetime when status was generated.
+    """
+
     is_alive: bool = True
     as_at: datetime = datetime.utcnow()
 
 
 def verify_token(token: Annotated[str, Depends(v1_auth_scheme)]):
     """Ensures token passed match the one set"""
     if token and token == args.token:
@@ -144,15 +162,15 @@
 def home():
     """Redirect to api playground"""
     return RedirectResponse("/v1/docs")
 
 
 @app.get("/status")
 def server_status() -> ServerStatus:
-    """Check server status"""
+    """Check server running status"""
     return ServerStatus(as_at=datetime.utcnow())
 
 
 @v1_router.post("/token")
 def fetch_token(form_data: Annotated[OAuth2PasswordRequestForm, Depends()]):
     """Fetch api token"""
     if form_data.username == args.username and form_data.password == args.token:
```

### Comparing `smartbetsAPI-1.2.4/smartbets_API/predictor.py` & `smartbetsAPI-1.2.5/smartbets_API/predictor.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/proxyh.py` & `smartbetsAPI-1.2.5/smartbets_API/proxyh.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.4/smartbets_API/tertiary_bet.py` & `smartbetsAPI-1.2.5/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

