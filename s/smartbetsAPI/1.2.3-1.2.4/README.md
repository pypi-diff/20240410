# Comparing `tmp/smartbetsAPI-1.2.3.tar.gz` & `tmp/smartbetsAPI-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.2.3.tar", last modified: Wed Apr 10 14:15:17 2024, max compression
+gzip compressed data, was "smartbetsAPI-1.2.4.tar", last modified: Wed Apr 10 15:00:54 2024, max compression
```

## Comparing `smartbetsAPI-1.2.3.tar` & `smartbetsAPI-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 14:15:17.234590 smartbetsAPI-1.2.3/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.3/LICENSE
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 14:15:17.234590 smartbetsAPI-1.2.3/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9382 2024-04-10 14:03:57.000000 smartbetsAPI-1.2.3/README.md
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-10 14:15:17.234590 smartbetsAPI-1.2.3/setup.cfg
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2408 2024-04-10 14:14:59.000000 smartbetsAPI-1.2.3/setup.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 14:15:17.234590 smartbetsAPI-1.2.3/smartbetsAPI.egg-info/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 14:15:17.000000 smartbetsAPI-1.2.3/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-10 14:15:17.000000 smartbetsAPI-1.2.3/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-10 14:15:17.000000 smartbetsAPI-1.2.3/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-10 14:15:17.000000 smartbetsAPI-1.2.3/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       95 2024-04-10 14:15:17.000000 smartbetsAPI-1.2.3/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-10 14:15:17.000000 smartbetsAPI-1.2.3/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 14:15:17.234590 smartbetsAPI-1.2.3/smartbets_API/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-10 14:14:59.000000 smartbetsAPI-1.2.3/smartbets_API/__init__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.3/smartbets_API/__main__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.3/smartbets_API/bet_analyzer.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2746 2024-04-10 13:57:50.000000 smartbetsAPI-1.2.3/smartbets_API/bet_at_rest_api_level.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.3/smartbets_API/bet_common.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.3/smartbets_API/configuration_handler.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.3/smartbets_API/figure_harvester.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.3/smartbets_API/googler.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.3/smartbets_API/html_fetcher.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5079 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.3/smartbets_API/interface.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.3/smartbets_API/predictor.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.3/smartbets_API/proxyh.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.3/smartbets_API/tertiary_bet.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/LICENSE
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9382 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/README.md
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/setup.cfg
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2407 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/setup.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11525 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/entry_points.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       95 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/requires.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-10 15:00:54.000000 smartbetsAPI-1.2.4/smartbetsAPI.egg-info/top_level.txt
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 15:00:54.750931 smartbetsAPI-1.2.4/smartbets_API/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/smartbets_API/__init__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/__main__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/bet_analyzer.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2747 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/smartbets_API/bet_at_rest_api_level.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/bet_common.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/configuration_handler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/figure_harvester.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/googler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/html_fetcher.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5346 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.4/smartbets_API/interface.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/predictor.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.4/smartbets_API/proxyh.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.4/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.2.3/LICENSE` & `smartbetsAPI-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/PKG-INFO` & `smartbetsAPI-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.3
+Version: 1.2.4
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
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.1&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.4&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.3 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.4 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
```

### Comparing `smartbetsAPI-1.2.3/README.md` & `smartbetsAPI-1.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 align="center">smartbetsAPI</h1>
 <p align="center">
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.1&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.4&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
  
  > "Punter's choice" 
 
  Worldwide soccer-matches predictor with Fast-API and a package for integrating the scripts in your own [Python](https://python.org) code.
 
  ## Features
```

### Comparing `smartbetsAPI-1.2.3/setup.py` & `smartbetsAPI-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "fastapi[all]==0.110.1",
         "appdirs==1.4.4",
         "requests==2.31.0",
         "colorama==0.4.6",
         "bs4==0.0.1",
         "Faker==15.3.4",
     ],
-    python_requires =">=3.9",
+    python_requires=">=3.9",
     project_urls={
         "Bug Report": "https://github.com/Simatwa/smartbetsAPI/issues/new",
         "Homepage": "https://github.com/Simatwa/smartbetsAPI",
         "Source Code": "https://github.com/Simatwa/smartbetsAPI",
         "Issue Tracker": "https://github.com/Simatwa/smartbetsAPI/issues",
         "Download": "https://github.com/Simatwa/smartbetsAPI/releases",
         "Documentation": "https://github.com/Simatwa/smartbetsAPI/blob/main/README.md",
```

### Comparing `smartbetsAPI-1.2.3/smartbetsAPI.egg-info/PKG-INFO` & `smartbetsAPI-1.2.4/smartbetsAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.3
+Version: 1.2.4
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
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.1&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.4&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.3 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.4 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
```

### Comparing `smartbetsAPI-1.2.3/smartbetsAPI.egg-info/SOURCES.txt` & `smartbetsAPI-1.2.4/smartbetsAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/bet_analyzer.py` & `smartbetsAPI-1.2.4/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/bet_at_rest_api_level.py` & `smartbetsAPI-1.2.4/smartbets_API/bet_at_rest_api_level.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sys import exit
 from os import path
 
 
 class predictor:
     def __init__(self, api_url: str, token: str):
         from requests import Session
+
         self.url = api_url
         self.session = Session()
         self.session.headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
             "Authorization": f"Bearer {token}",
         }
```

### Comparing `smartbetsAPI-1.2.3/smartbets_API/bet_common.py` & `smartbetsAPI-1.2.4/smartbets_API/bet_common.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/configuration_handler.py` & `smartbetsAPI-1.2.4/smartbets_API/configuration_handler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/figure_harvester.py` & `smartbetsAPI-1.2.4/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/googler.py` & `smartbetsAPI-1.2.4/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/html_fetcher.py` & `smartbetsAPI-1.2.4/smartbets_API/html_fetcher.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/interface.py` & `smartbetsAPI-1.2.4/smartbets_API/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 from .predictor import predictor
 from fastapi import FastAPI, status, HTTPException, Depends, APIRouter
 from fastapi.responses import RedirectResponse
 from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
 from pydantic import BaseModel
 from typing import Annotated
+from datetime import datetime
 
 app = FastAPI(
     title="smartbetsAPI",
     summary="Worldwide soccer-matches predictor",
     version=__version__,
     description="""View official docs at [Simatwa/smartbets](https://github.com/Simatwa/smartbetsapi)""",
     license_info={
@@ -118,14 +119,19 @@
     ov25: float
     ov35: float
     choice: float
     result: str
     pick: str
 
 
+class ServerStatus(BaseModel):
+    is_alive: bool = True
+    as_at: datetime = datetime.utcnow()
+
+
 def verify_token(token: Annotated[str, Depends(v1_auth_scheme)]):
     """Ensures token passed match the one set"""
     if token and token == args.token:
         return token
     else:
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
@@ -136,14 +142,20 @@
 
 @app.get("/")
 def home():
     """Redirect to api playground"""
     return RedirectResponse("/v1/docs")
 
 
+@app.get("/status")
+def server_status() -> ServerStatus:
+    """Check server status"""
+    return ServerStatus(as_at=datetime.utcnow())
+
+
 @v1_router.post("/token")
 def fetch_token(form_data: Annotated[OAuth2PasswordRequestForm, Depends()]):
     """Fetch api token"""
     if form_data.username == args.username and form_data.password == args.token:
         return {
             "access_token": args.token,
             "token_type": "bearer",
```

### Comparing `smartbetsAPI-1.2.3/smartbets_API/predictor.py` & `smartbetsAPI-1.2.4/smartbets_API/predictor.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/proxyh.py` & `smartbetsAPI-1.2.4/smartbets_API/proxyh.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.3/smartbets_API/tertiary_bet.py` & `smartbetsAPI-1.2.4/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

