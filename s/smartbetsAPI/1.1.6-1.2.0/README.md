# Comparing `tmp/smartbetsAPI-1.1.6.tar.gz` & `tmp/smartbetsAPI-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.1.6.tar", last modified: Thu Dec 21 10:55:35 2023, max compression
+gzip compressed data, was "smartbetsAPI-1.2.0.tar", last modified: Wed Apr 10 13:17:49 2024, max compression
```

## Comparing `smartbetsAPI-1.1.6.tar` & `smartbetsAPI-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:55:35.530326 smartbetsAPI-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2023-12-21 10:55:35.530326 smartbetsAPI-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 10:55:35.530326 smartbetsAPI-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:55:35.530326 smartbetsAPI-1.1.6/smartbetsAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2023-12-21 10:55:35.000000 smartbetsAPI-1.1.6/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-21 10:55:35.000000 smartbetsAPI-1.1.6/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 10:55:35.000000 smartbetsAPI-1.1.6/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-21 10:55:35.000000 smartbetsAPI-1.1.6/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-21 10:55:35.000000 smartbetsAPI-1.1.6/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-21 10:55:35.000000 smartbetsAPI-1.1.6/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 10:55:35.530326 smartbetsAPI-1.1.6/smartbets_API/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/bet_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/bet_at_api_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11304 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/bet_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/configuration_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/figure_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/googler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/html_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/proxyh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-21 10:55:27.000000 smartbetsAPI-1.1.6/smartbets_API/tertiary_bet.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 13:17:49.414625 smartbetsAPI-1.2.0/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.0/LICENSE
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11529 2024-04-10 13:17:49.414625 smartbetsAPI-1.2.0/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9382 2024-04-10 13:06:02.000000 smartbetsAPI-1.2.0/README.md
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-10 13:17:49.414625 smartbetsAPI-1.2.0/setup.cfg
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2412 2024-04-10 12:58:36.000000 smartbetsAPI-1.2.0/setup.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 13:17:49.414625 smartbetsAPI-1.2.0/smartbetsAPI.egg-info/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11529 2024-04-10 13:17:49.000000 smartbetsAPI-1.2.0/smartbetsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-10 13:17:49.000000 smartbetsAPI-1.2.0/smartbetsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-10 13:17:49.000000 smartbetsAPI-1.2.0/smartbetsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-10 13:17:49.000000 smartbetsAPI-1.2.0/smartbetsAPI.egg-info/entry_points.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       99 2024-04-10 13:17:49.000000 smartbetsAPI-1.2.0/smartbetsAPI.egg-info/requires.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-10 13:17:49.000000 smartbetsAPI-1.2.0/smartbetsAPI.egg-info/top_level.txt
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 13:17:49.411292 smartbetsAPI-1.2.0/smartbets_API/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-10 13:09:52.000000 smartbetsAPI-1.2.0/smartbets_API/__init__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 11:51:14.000000 smartbetsAPI-1.2.0/smartbets_API/__main__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.0/smartbets_API/bet_analyzer.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2738 2024-04-10 12:48:45.000000 smartbetsAPI-1.2.0/smartbets_API/bet_at_rest_api_level.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 11:51:14.000000 smartbetsAPI-1.2.0/smartbets_API/bet_common.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 11:51:14.000000 smartbetsAPI-1.2.0/smartbets_API/configuration_handler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.0/smartbets_API/figure_harvester.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.0/smartbets_API/googler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 11:51:14.000000 smartbetsAPI-1.2.0/smartbets_API/html_fetcher.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5079 2024-04-10 12:48:45.000000 smartbetsAPI-1.2.0/smartbets_API/interface.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 11:51:14.000000 smartbetsAPI-1.2.0/smartbets_API/predictor.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 11:51:14.000000 smartbetsAPI-1.2.0/smartbets_API/proxyh.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.0/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.1.6/LICENSE` & `smartbetsAPI-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.6/PKG-INFO` & `smartbetsAPI-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,87 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.1.6
+Version: 1.2.0
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
+Project-URL: Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new
+Project-URL: Homepage, https://github.com/Simatwa/smartbetsAPI
+Project-URL: Source Code, https://github.com/Simatwa/smartbetsAPI
+Project-URL: Issue Tracker, https://github.com/Simatwa/smartbetsAPI/issues
+Project-URL: Download, https://github.com/Simatwa/smartbetsAPI/releases
+Project-URL: Documentation, https://github.com/Simatwa/smartbetsAPI/blob/main/README.md
 Keywords: Football,Predictions,Betting API,Soccer predictions,Football Predictions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Flask==2.2.2
+Requires-Dist: fastapi[uvicorn]==0.110.1
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
-Requires-Dist: Werkzeug==2.2.2
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.6&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.0&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice" 
 
 
 
- Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
+ Worldwide soccer-matches predictor with Fast-API and a package for integrating the scripts in your own [Python](https://python.org) code.
 
 
 
  ## Features
 
+
+
  - REST-API
 
- - Script intergration (package)
+ - Script integration (package)
 
- - Non-AI 
+ - Non-ML
 
 
 
  ## Installation and usage
 
 
 
  ### Installation
 
 
 
-1. Linux 
-
-
-
-*Python 3.7+* is required for this script to be fruitful to you. 
+*Python 3.9+* is required for this script to be fruitful to you. 
 
 - Installing through pip is always the most preferred way:
 
 
 
  ```sh
 
@@ -140,15 +143,15 @@
 
 
 
 1. Terminal
 
 
 
- Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](/pallets/Flask) server with the following default configurations.
+ Running `$ smartbetsAPI <token/password>`  will fire up the FastAPI server with the following default configurations.
 
 
 
 <table align="center"> 
 
 <thead>
 
@@ -184,39 +187,43 @@
 
 
 
 - For instance :
 
 
 
- ```sh
+```sh
 
  $ smartbetsAPI mypass9876
 
 
 
-``` 
+```
 
 
 
-Here is an example of a [simple program](examples/bet_at_api_level.py) that makes prediction using the `api`.
+> [!TIP]
 
+> `Docs` will be available at : http://localhost:8000/v1/docs
+
+> `Redoc` will be available at : http://localhost:8000/v1/redoc
 
 
-![api running](assets/api_running.gif)
 
+Here is an example of a [simple program](examples/bet_at_rest_api_level.py) that makes prediction using the REST API.
 
 
 
+![api running](assets/api_running.gif)
+
 
-> **Note** 
 
-  - Content-Type of the response (predictions) is `application/json`
+> [!Note]
 
-  - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
+> Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
 
 
 
 > Example predicting using REST API
```

#### html2text {}

```diff
@@ -1,63 +1,69 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.6 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.0 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
-Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Keywords:
+Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
+Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
+Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
+https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
+github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
+github.com/Simatwa/smartbetsAPI/releases Project-URL: Documentation, https://
+github.com/Simatwa/smartbetsAPI/blob/main/README.md Keywords:
 Football,Predictions,Betting API,Soccer predictions,Football Predictions
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Customer Service Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Natural Language :: English Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic :: Games/
-Entertainment Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: Flask==2.2.2 Requires-Dist: appdirs==1.4.4 Requires-Dist:
-requests==2.28.1 Requires-Dist: colorama==0.4.6 Requires-Dist: bs4==0.0.1
-Requires-Dist: Faker==15.3.4 Requires-Dist: Werkzeug==2.2.2
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Games/Entertainment Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: fastapi
+[uvicorn]==0.110.1 Requires-Dist: appdirs==1.4.4 Requires-Dist:
+requests==2.31.0 Requires-Dist: colorama==0.4.6 Requires-Dist: bs4==0.0.1
+Requires-Dist: Faker==15.3.4
                           ************ ssmmaarrttbbeettssAAPPII ************
      _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_A_c_c_u_r_a_c_y_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]
                                   _[_D_o_w_n_l_o_a_d_s_]
 
-> "Punter's choice" Worldwide soccer-matches predictor with a dedicated
-standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and
-a package for intergrating the scripts in your own [Python](https://python.org)
-code. ## Features - REST-API - Script intergration (package) - Non-AI ##
-Installation and usage ### Installation 1. Linux *Python 3.7+* is required for
-this script to be fruitful to you. - Installing through pip is always the most
+> "Punter's choice" Worldwide soccer-matches predictor with Fast-API and a
+package for integrating the scripts in your own [Python](https://python.org)
+code. ## Features - REST-API - Script integration (package) - Non-ML ##
+Installation and usage ### Installation *Python 3.9+* is required for this
+script to be fruitful to you. - Installing through pip is always the most
 preferred way: ```sh pip install smartbetsAPI ``` - For those who like enjoying
 the **latest** releases from [Github](https://github.com) like [me](https://
 github.com/Simatwa), rather than waiting for the next release: ```sh pip
 install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
 guys with _trust issues_ are very much sorted this way: ```sh git clone https:/
 /github.com/Simatwa/smartbetsAPI.git cd smartbetsAPI bash install.sh #or sudo
-bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI ` will fire
-up the [Flask](/pallets/Flask) server with the following default
+bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI
+assword>` will fire up the FastAPI server with the following default
 configurations.
                             CCoommmmaanndd         DDeeffaauulltt
                             Port            8000
                             Username        API
                             Filename        None
                             level (Logging) 20
                             host            False
                             debug           False
                             no-net          False
                             log             False
                             colorize        False
                             gui (Termux)    False
-- For instance : ```sh $ smartbetsAPI mypass9876 ``` Here is an example of a
-[simple program](examples/bet_at_api_level.py) that makes prediction using the
-`api`. ![api running](assets/api_running.gif) > **Note** - Content-Type of the
-response (predictions) is `application/json` - Reinstall with `sudo` privileges
-if `smartbetsAPI` command can't be found. > Example predicting using REST API
-```py from smartbets_API import predictor predict = predictor('http://
+- For instance : ```sh $ smartbetsAPI mypass9876 ``` > [!TIP] > `Docs` will be
+available at : http://localhost:8000/v1/docs > `Redoc` will be available at :
+http://localhost:8000/v1/redoc Here is an example of a [simple program]
+(examples/bet_at_rest_api_level.py) that makes prediction using the REST API. !
+[api running](assets/api_running.gif) > [!Note] > Reinstall with `sudo`
+privileges if `smartbetsAPI` command can't be found. > Example predicting using
+REST API ```py from smartbets_API import predictor predict = predictor('http://
 localhost:8080','password') bets=predict.get_predictions
 ('Arsenal','Manchester') print(bets) #Output #(True, {'choice': 55.56, 'g':
 14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15',
 'result': '1'}) ``` * For more information you can run `smartbetsAPI -h` 2.
 Importing Package Module `predictor` provides two ways of interacting with it
 at the programming level, based on the `data-type` in which the teams have been
 packed and parsed to it: * Using `predictorL` object which accepts *teams*
```

### Comparing `smartbetsAPI-1.1.6/README.md` & `smartbetsAPI-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 <h1 align="center">smartbetsAPI</h1>
 <p align="center">
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.6&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.0&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
  
  > "Punter's choice" 
 
- Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
+ Worldwide soccer-matches predictor with Fast-API and a package for integrating the scripts in your own [Python](https://python.org) code.
 
  ## Features
+
  - REST-API
- - Script intergration (package)
- - Non-AI 
+ - Script integration (package)
+ - Non-ML
 
  ## Installation and usage
 
  ### Installation
 
-1. Linux 
-
-*Python 3.7+* is required for this script to be fruitful to you. 
+*Python 3.9+* is required for this script to be fruitful to you. 
 - Installing through pip is always the most preferred way:
 
  ```sh
  pip  install smartbetsAPI
  
  ```
 
@@ -48,15 +47,15 @@
 
 ```
 
 ### Usage
 
 1. Terminal
 
- Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](/pallets/Flask) server with the following default configurations.
+ Running `$ smartbetsAPI <token/password>`  will fire up the FastAPI server with the following default configurations.
 
 <table align="center"> 
 <thead>
 <tr><th>Command        </th><th>Default  </th></tr>
 </thead>
 <tbody>
 <tr><td>Port           </td><td>8000     </td></tr>
@@ -70,27 +69,29 @@
 <tr><td>colorize       </td><td>False    </td></tr>
 <tr><td>gui (Termux)   </td><td>False    </td></tr>
 </tbody>
 </table>
 
 - For instance :
 
- ```sh
+```sh
  $ smartbetsAPI mypass9876
 
-``` 
+```
 
-Here is an example of a [simple program](examples/bet_at_api_level.py) that makes prediction using the `api`.
+> [!TIP]
+> `Docs` will be available at : http://localhost:8000/v1/docs
+> `Redoc` will be available at : http://localhost:8000/v1/redoc
 
-![api running](assets/api_running.gif)
+Here is an example of a [simple program](examples/bet_at_rest_api_level.py) that makes prediction using the REST API.
 
+![api running](assets/api_running.gif)
 
-> **Note** 
-  - Content-Type of the response (predictions) is `application/json`
-  - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
+> [!Note]
+> Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
 
 > Example predicting using REST API
 
 ```py
 from smartbets_API import predictor
 predict = predictor('http://localhost:8080','password')
 bets=predict.get_predictions('Arsenal','Manchester')
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
                           ************ ssmmaarrttbbeettssAAPPII ************
      _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_A_c_c_u_r_a_c_y_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]
                                   _[_D_o_w_n_l_o_a_d_s_]
 
-> "Punter's choice" Worldwide soccer-matches predictor with a dedicated
-standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and
-a package for intergrating the scripts in your own [Python](https://python.org)
-code. ## Features - REST-API - Script intergration (package) - Non-AI ##
-Installation and usage ### Installation 1. Linux *Python 3.7+* is required for
-this script to be fruitful to you. - Installing through pip is always the most
+> "Punter's choice" Worldwide soccer-matches predictor with Fast-API and a
+package for integrating the scripts in your own [Python](https://python.org)
+code. ## Features - REST-API - Script integration (package) - Non-ML ##
+Installation and usage ### Installation *Python 3.9+* is required for this
+script to be fruitful to you. - Installing through pip is always the most
 preferred way: ```sh pip install smartbetsAPI ``` - For those who like enjoying
 the **latest** releases from [Github](https://github.com) like [me](https://
 github.com/Simatwa), rather than waiting for the next release: ```sh pip
 install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
 guys with _trust issues_ are very much sorted this way: ```sh git clone https:/
 /github.com/Simatwa/smartbetsAPI.git cd smartbetsAPI bash install.sh #or sudo
-bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI ` will fire
-up the [Flask](/pallets/Flask) server with the following default
+bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI
+assword>` will fire up the FastAPI server with the following default
 configurations.
                             CCoommmmaanndd         DDeeffaauulltt
                             Port            8000
                             Username        API
                             Filename        None
                             level (Logging) 20
                             host            False
                             debug           False
                             no-net          False
                             log             False
                             colorize        False
                             gui (Termux)    False
-- For instance : ```sh $ smartbetsAPI mypass9876 ``` Here is an example of a
-[simple program](examples/bet_at_api_level.py) that makes prediction using the
-`api`. ![api running](assets/api_running.gif) > **Note** - Content-Type of the
-response (predictions) is `application/json` - Reinstall with `sudo` privileges
-if `smartbetsAPI` command can't be found. > Example predicting using REST API
-```py from smartbets_API import predictor predict = predictor('http://
+- For instance : ```sh $ smartbetsAPI mypass9876 ``` > [!TIP] > `Docs` will be
+available at : http://localhost:8000/v1/docs > `Redoc` will be available at :
+http://localhost:8000/v1/redoc Here is an example of a [simple program]
+(examples/bet_at_rest_api_level.py) that makes prediction using the REST API. !
+[api running](assets/api_running.gif) > [!Note] > Reinstall with `sudo`
+privileges if `smartbetsAPI` command can't be found. > Example predicting using
+REST API ```py from smartbets_API import predictor predict = predictor('http://
 localhost:8080','password') bets=predict.get_predictions
 ('Arsenal','Manchester') print(bets) #Output #(True, {'choice': 55.56, 'g':
 14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15',
 'result': '1'}) ``` * For more information you can run `smartbetsAPI -h` 2.
 Importing Package Module `predictor` provides two ways of interacting with it
 at the programming level, based on the `data-type` in which the teams have been
 packed and parsed to it: * Using `predictorL` object which accepts *teams*
```

### Comparing `smartbetsAPI-1.1.6/setup.py` & `smartbetsAPI-1.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,37 +17,44 @@
     author_email="smartwacaleb@gmail.com",
     maintainer="Smartwa Caleb",
     maintainer_email="smartwacaleb@gmail.com",
     description="Simple football prediction API",
     long_description="\n".join(get_file("README.md")),
     long_description_content_type="text/markdown",
     install_requires=[
-        "Flask==2.2.2",
+        "fastapi[uvicorn]==0.110.1",
         "appdirs==1.4.4",
-        "requests==2.28.1",
+        "requests==2.31.0",
         "colorama==0.4.6",
         "bs4==0.0.1",
         "Faker==15.3.4",
-        "Werkzeug==2.2.2",
     ],
+    python_requires =">=3.9",
+    project_urls={
+        "Bug Report": "https://github.com/Simatwa/smartbetsAPI/issues/new",
+        "Homepage": "https://github.com/Simatwa/smartbetsAPI",
+        "Source Code": "https://github.com/Simatwa/smartbetsAPI",
+        "Issue Tracker": "https://github.com/Simatwa/smartbetsAPI/issues",
+        "Download": "https://github.com/Simatwa/smartbetsAPI/releases",
+        "Documentation": "https://github.com/Simatwa/smartbetsAPI/blob/main/README.md",
+    },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Intended Audience :: Other Audience",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Games/Entertainment",
     ],
     keywords=[
         "Football",
         "Predictions",
```

### Comparing `smartbetsAPI-1.1.6/smartbetsAPI.egg-info/PKG-INFO` & `smartbetsAPI-1.2.0/smartbetsAPI.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,87 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.1.6
+Version: 1.2.0
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
+Project-URL: Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new
+Project-URL: Homepage, https://github.com/Simatwa/smartbetsAPI
+Project-URL: Source Code, https://github.com/Simatwa/smartbetsAPI
+Project-URL: Issue Tracker, https://github.com/Simatwa/smartbetsAPI/issues
+Project-URL: Download, https://github.com/Simatwa/smartbetsAPI/releases
+Project-URL: Documentation, https://github.com/Simatwa/smartbetsAPI/blob/main/README.md
 Keywords: Football,Predictions,Betting API,Soccer predictions,Football Predictions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Flask==2.2.2
+Requires-Dist: fastapi[uvicorn]==0.110.1
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
-Requires-Dist: Werkzeug==2.2.2
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.6&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.0&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice" 
 
 
 
- Worldwide soccer-matches predictor with a  dedicated standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and a package for intergrating the scripts in your own [Python](https://python.org) code.
+ Worldwide soccer-matches predictor with Fast-API and a package for integrating the scripts in your own [Python](https://python.org) code.
 
 
 
  ## Features
 
+
+
  - REST-API
 
- - Script intergration (package)
+ - Script integration (package)
 
- - Non-AI 
+ - Non-ML
 
 
 
  ## Installation and usage
 
 
 
  ### Installation
 
 
 
-1. Linux 
-
-
-
-*Python 3.7+* is required for this script to be fruitful to you. 
+*Python 3.9+* is required for this script to be fruitful to you. 
 
 - Installing through pip is always the most preferred way:
 
 
 
  ```sh
 
@@ -140,15 +143,15 @@
 
 
 
 1. Terminal
 
 
 
- Running `$ smartbetsAPI <api-password>`  will fire up the [Flask](/pallets/Flask) server with the following default configurations.
+ Running `$ smartbetsAPI <token/password>`  will fire up the FastAPI server with the following default configurations.
 
 
 
 <table align="center"> 
 
 <thead>
 
@@ -184,39 +187,43 @@
 
 
 
 - For instance :
 
 
 
- ```sh
+```sh
 
  $ smartbetsAPI mypass9876
 
 
 
-``` 
+```
 
 
 
-Here is an example of a [simple program](examples/bet_at_api_level.py) that makes prediction using the `api`.
+> [!TIP]
 
+> `Docs` will be available at : http://localhost:8000/v1/docs
+
+> `Redoc` will be available at : http://localhost:8000/v1/redoc
 
 
-![api running](assets/api_running.gif)
 
+Here is an example of a [simple program](examples/bet_at_rest_api_level.py) that makes prediction using the REST API.
 
 
 
+![api running](assets/api_running.gif)
+
 
-> **Note** 
 
-  - Content-Type of the response (predictions) is `application/json`
+> [!Note]
 
-  - Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
+> Reinstall with `sudo` privileges if `smartbetsAPI` command can't be found.
 
 
 
 > Example predicting using REST API
```

#### html2text {}

```diff
@@ -1,63 +1,69 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.6 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.0 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
-Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Keywords:
+Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
+Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
+Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
+https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
+github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
+github.com/Simatwa/smartbetsAPI/releases Project-URL: Documentation, https://
+github.com/Simatwa/smartbetsAPI/blob/main/README.md Keywords:
 Football,Predictions,Betting API,Soccer predictions,Football Predictions
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Customer Service Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Natural Language :: English Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic :: Games/
-Entertainment Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: Flask==2.2.2 Requires-Dist: appdirs==1.4.4 Requires-Dist:
-requests==2.28.1 Requires-Dist: colorama==0.4.6 Requires-Dist: bs4==0.0.1
-Requires-Dist: Faker==15.3.4 Requires-Dist: Werkzeug==2.2.2
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Games/Entertainment Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: fastapi
+[uvicorn]==0.110.1 Requires-Dist: appdirs==1.4.4 Requires-Dist:
+requests==2.31.0 Requires-Dist: colorama==0.4.6 Requires-Dist: bs4==0.0.1
+Requires-Dist: Faker==15.3.4
                           ************ ssmmaarrttbbeettssAAPPII ************
      _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_A_c_c_u_r_a_c_y_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]
                                   _[_D_o_w_n_l_o_a_d_s_]
 
-> "Punter's choice" Worldwide soccer-matches predictor with a dedicated
-standalone [Flask](https://github.com/pallets/Flask) server as an endpoint and
-a package for intergrating the scripts in your own [Python](https://python.org)
-code. ## Features - REST-API - Script intergration (package) - Non-AI ##
-Installation and usage ### Installation 1. Linux *Python 3.7+* is required for
-this script to be fruitful to you. - Installing through pip is always the most
+> "Punter's choice" Worldwide soccer-matches predictor with Fast-API and a
+package for integrating the scripts in your own [Python](https://python.org)
+code. ## Features - REST-API - Script integration (package) - Non-ML ##
+Installation and usage ### Installation *Python 3.9+* is required for this
+script to be fruitful to you. - Installing through pip is always the most
 preferred way: ```sh pip install smartbetsAPI ``` - For those who like enjoying
 the **latest** releases from [Github](https://github.com) like [me](https://
 github.com/Simatwa), rather than waiting for the next release: ```sh pip
 install git+https://github.com/Simatwa/smartbetsAPI.git ``` - The hard-core
 guys with _trust issues_ are very much sorted this way: ```sh git clone https:/
 /github.com/Simatwa/smartbetsAPI.git cd smartbetsAPI bash install.sh #or sudo
-bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI ` will fire
-up the [Flask](/pallets/Flask) server with the following default
+bash install.sh ``` ### Usage 1. Terminal Running `$ smartbetsAPI
+assword>` will fire up the FastAPI server with the following default
 configurations.
                             CCoommmmaanndd         DDeeffaauulltt
                             Port            8000
                             Username        API
                             Filename        None
                             level (Logging) 20
                             host            False
                             debug           False
                             no-net          False
                             log             False
                             colorize        False
                             gui (Termux)    False
-- For instance : ```sh $ smartbetsAPI mypass9876 ``` Here is an example of a
-[simple program](examples/bet_at_api_level.py) that makes prediction using the
-`api`. ![api running](assets/api_running.gif) > **Note** - Content-Type of the
-response (predictions) is `application/json` - Reinstall with `sudo` privileges
-if `smartbetsAPI` command can't be found. > Example predicting using REST API
-```py from smartbets_API import predictor predict = predictor('http://
+- For instance : ```sh $ smartbetsAPI mypass9876 ``` > [!TIP] > `Docs` will be
+available at : http://localhost:8000/v1/docs > `Redoc` will be available at :
+http://localhost:8000/v1/redoc Here is an example of a [simple program]
+(examples/bet_at_rest_api_level.py) that makes prediction using the REST API. !
+[api running](assets/api_running.gif) > [!Note] > Reinstall with `sudo`
+privileges if `smartbetsAPI` command can't be found. > Example predicting using
+REST API ```py from smartbets_API import predictor predict = predictor('http://
 localhost:8080','password') bets=predict.get_predictions
 ('Arsenal','Manchester') print(bets) #Output #(True, {'choice': 55.56, 'g':
 14.0, 'gg': 80.0, 'ov15': 80.0, 'ov25': 65.0, 'ov35': 55.0, 'pick': 'ov15',
 'result': '1'}) ``` * For more information you can run `smartbetsAPI -h` 2.
 Importing Package Module `predictor` provides two ways of interacting with it
 at the programming level, based on the `data-type` in which the teams have been
 packed and parsed to it: * Using `predictorL` object which accepts *teams*
```

### Comparing `smartbetsAPI-1.1.6/smartbetsAPI.egg-info/SOURCES.txt` & `smartbetsAPI-1.2.0/smartbetsAPI.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 smartbetsAPI.egg-info/dependency_links.txt
 smartbetsAPI.egg-info/entry_points.txt
 smartbetsAPI.egg-info/requires.txt
 smartbetsAPI.egg-info/top_level.txt
 smartbets_API/__init__.py
 smartbets_API/__main__.py
 smartbets_API/bet_analyzer.py
-smartbets_API/bet_at_api_level.py
+smartbets_API/bet_at_rest_api_level.py
 smartbets_API/bet_common.py
 smartbets_API/configuration_handler.py
 smartbets_API/figure_harvester.py
 smartbets_API/googler.py
 smartbets_API/html_fetcher.py
 smartbets_API/interface.py
 smartbets_API/predictor.py
```

### Comparing `smartbetsAPI-1.1.6/smartbets_API/bet_analyzer.py` & `smartbetsAPI-1.2.0/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.6/smartbets_API/bet_common.py` & `smartbetsAPI-1.2.0/smartbets_API/bet_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 tbe = "Bet_" + tablee
 predictionTb = "Prediction_" + tablee
 developer = "Smartwa"
 root_image = os.getcwd() + "static/image/"
 logo = root_image + "logo.jpg"
 predbets_img = root_image + "predbets.png"
 dirs = AppDirs("Smartwa", "smartbets_API").user_data_dir
-config_filepath=os.path.join(dirs,'configurations.json')
+config_filepath = os.path.join(dirs, "configurations.json")
 
 
 # Runs system cmds at API level
 def get_output(command):
     success = False
     try:
         output = subprocess.check_output(command, stderr=subprocess.STDOUT).decode()
@@ -225,15 +225,15 @@
     if str(name).lower() == "none":
         name = "?"
     return name
 
 
 # Generating google search link
 def google(search):
-    key = re.sub("\s", "+", search)
+    key = re.sub(f"\s", "+", search)
     stat = f"""https://www.google.com/search?q={key}"""
     return stat
 
 
 # Saves text-like files
 def saver(data, link, fmt, mode="w", dir=ht):
     fnm = filter(link, fmt)
@@ -251,15 +251,15 @@
     except:
         data = 0
     finally:
         return data
 
 
 def getInt(score):
-    score = re.sub("\s", "", score)
+    score = re.sub(f"\s", "", score)
     after = []
     score = score.split("-")
     for dat in score:
         for letter in dat:
             if not letter.isdigit():
                 dat = dat.replace(letter, "")
         after.append(int(dat))
@@ -295,22 +295,25 @@
 # Updates configurations parsed
 class booter:
     def __init__(self):
         self.target = ["log", "color", "filename", "gui", "level", "proxy"]
 
     def get_info(self):
         from json import load
+
         try:
             with open(config_filepath) as fh:
                 config.update(load(fh))
         except Exception as e:
-            exit('Failed to load configurations - '+config_filepath+' '+str(e))
+            exit("Failed to load configurations - " + config_filepath + " " + str(e))
+
 
 booter().get_info()
 
+
 # Logging configurations
 def log_level():
     tg = int(config["level"])
     return tg if tg > 0 else 60
 
 
 if config.get("log"):
```

### Comparing `smartbetsAPI-1.1.6/smartbets_API/configuration_handler.py` & `smartbetsAPI-1.2.0/smartbets_API/configuration_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sqlite3
 import subprocess
 from sys import exit, prefix
 import colorama as col
 from appdirs import AppDirs
 from json import dumps
+
 dirs = AppDirs("Smartwa", "smartbets_API").user_data_dir
 
 
 def get_output(command):
     success = False
     try:
         output = subprocess.check_output(command, stderr=subprocess.STDOUT).decode()
@@ -124,23 +125,41 @@
         except Exception as e:
             pass
 
 
 class set_config:
     def __init__(self, args):
         self.target = ["log", "color", "filename", "gui", "level", "proxy"]
-        self.values = [args.log, args.color, args.filename, args.gui, args.level, args.proxy]
-        self.config_filepath=os.path.join(dirs,'configurations.json')
+        log_level = {
+            "debug": 10,
+            "info": 20,
+            "warning": 30,
+            "error": 40,
+            "critical": 50,
+        }
+        self.values = [
+            args.log,
+            args.color,
+            args.filename,
+            args.gui,
+            log_level[args.level],
+            args.proxy,
+        ]
+        self.config_filepath = os.path.join(dirs, "configurations.json")
 
     # Creates db initially
     def createTable(self):
         self.db.queryDb("DROP TABLE Booter")
         run = f"""CREATE TABLE IF NOT EXISTS Booter(ID INTEGER PRIMARY 
 		KEY AUTOINCREMENT, log TEXT, Color TEXT, Filename TEXT, Gui TEXT, Level INTEGER, Proxy TEXT)"""
         self.db.queryDb(run)
 
     def main(self):
         try:
-            with open(self.config_filepath,'w') as fh:
-                fh.write(dumps(dict(zip(self.target,self.values))))
+            with open(self.config_filepath, "w") as fh:
+                fh.write(dumps(dict(zip(self.target, self.values))))
         except Exception as e:
-            exit(print(f'[*] Failed to save configurations - {self.config_filepath} - {e}'))
+            exit(
+                print(
+                    f"[*] Failed to save configurations - {self.config_filepath} - {e}"
+                )
+            )
```

### Comparing `smartbetsAPI-1.1.6/smartbets_API/figure_harvester.py` & `smartbetsAPI-1.2.0/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.6/smartbets_API/googler.py` & `smartbetsAPI-1.2.0/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.6/smartbets_API/html_fetcher.py` & `smartbetsAPI-1.2.0/smartbets_API/html_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from .proxyh import hunter45
 
 
 class web:
     def __init__(self):
         self.used, self.exc, self.user_agent, self.ref = [], [], [], []
         self.hunter = hunter45(req)
-        pr = self.hunter.get_proxy() 
+        pr = self.hunter.get_proxy()
         if pr[0]:
             self.proxies = pr[1]
         else:
             logging.error(pr[1])
-            self.proxies = [] 
+            self.proxies = []
 
     def sampl(self):
         etc = [
             "int",
             "ke",
             "us",
             "ca",
@@ -102,51 +102,51 @@
             "Connection": "Keep-Alive",
             "User-Agent": userA,
             "Sec-Fetch-Site": setchF,
             "Sec-Fetch-Mode": "navigate",
             "Sec-Fetch-Dest": "document",
         }
         return content
-    
-    def get_proxy(self,code:int=429) -> dict:
+
+    def get_proxy(self, code: int = 429) -> dict:
         """Hunts down proxies"""
         proxy = None
-        if not config.get('proxy'):
+        if not config.get("proxy"):
             return proxy
         if code == 429 or code == 403:
             pr = self.hunter.sample(self.proxies)
             if pr[0]:
                 proxy = pr[1]
-                logging.info('Loading new proxy - '+proxy['https'])
-                logging.debug(f'Proxy assigned - {proxy}')
+                logging.info("Loading new proxy - " + proxy["https"])
+                logging.debug(f"Proxy assigned - {proxy}")
             else:
                 logging.error(pr[1])
         return proxy
 
     # Getting html from web
-    def sender(self, link, info="Requesting", g=0, head=0,proxy=None):
+    def sender(self, link, info="Requesting", g=0, head=0, proxy=None):
         ht = "http"
         if ht in link:
             url = link
         else:
             url = "https://" + link
         try:
             logging.info(f"{info} - {url}")
-            params= {'url':url, 'headers':self.header(),'timeout':15}
+            params = {"url": url, "headers": self.header(), "timeout": 15}
             if proxy:
-                params['proxies']=proxy
+                params["proxies"] = proxy
             resp = req.get(**params)
         except TimeoutError:
-            return (self.sender,info,g,head,self.get_proxy())
+            return (self.sender, info, g, head, self.get_proxy())
         except Exception as e:
             if len(self.exc) > 1:
                 return "0"
             logging.error(str(e))
             self.exc.append("1")
-            return self.sender(url, "Retrying",proxy=self.get_proxy())
+            return self.sender(url, "Retrying", proxy=self.get_proxy())
         else:
             self.ref.insert(0, url)
             self.status(resp.status_code, resp.reason)
             try:
                 content = resp.text
             except:
                 pass
@@ -155,21 +155,21 @@
                 g += 1
                 if not code == 200:
                     proxy = self.get_proxy(code)
                     self.user_agent.clear()
                     gui.toast(f"Http-code {code}", b="red", c="lime")
                     logging.debug(f"{g}s of SLEEP")
                     time.sleep(g)
-                    return self.sender(self.repair(url), "Retrying", g, 1,proxy)
+                    return self.sender(self.repair(url), "Retrying", g, 1, proxy)
                 if "access denied" in soupHtml(content).lower():
                     logging.warning("ACCESS DENIED".center(37))
                     self.user_agent.clear()
                     logging.warning(f"{g}s of SLEEP")
                     time.sleep(g)
-                    return self.sender(self.repair(url), "Retrying", g, 1,proxy)
+                    return self.sender(self.repair(url), "Retrying", g, 1, proxy)
                 nm = filter(link, "html")
                 queryDb(f"DELETE FROM html where F_name='{nm}' ")
                 insertDb("Html", "F_name", "File", nm, content)
                 return self.launcher(link)
 
     # Query link's contents from db
     def launcher(self, link):
```

### Comparing `smartbetsAPI-1.1.6/smartbets_API/predictor.py` & `smartbetsAPI-1.2.0/smartbets_API/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
     def __init__(self, **kwargs):
         v = lambda t: kwargs[t]
         self.log = v("log")
         self.color = v("color")
         self.filename = v("filename")
         self.gui = v("gui")
         self.level = v("level")
-        self.proxy=v("proxy")
+        self.proxy = v("proxy")
 
 
 class predictor:
     def __init__(
         self,
         include_position=False,
         log=False,
         level=0,
         filename=None,
         color=False,
         gui=False,
         api=False,
-        proxy =None,
+        proxy=None,
     ):
         """Initializes the class.
 
         :param include_position: (optional) Include team's league ranking in making predictions.
         :type include_position: bool
         :param log: (optional) Log at api default log's path.
         :type log: bool
@@ -43,15 +43,15 @@
 
             args = {
                 "log": log,
                 "color": color,
                 "filename": filename,
                 "gui": gui,
                 "level": level,
-                "proxy":proxy
+                "proxy": proxy,
             }
             set_config(args_handler(**args)).main()
         from .bet_common import logging
         from .bet_analyzer import analyze
         from .figure_harvester import harvest
 
         self.logging, self.harvest, self.analyze = logging, harvest, analyze
```

### Comparing `smartbetsAPI-1.1.6/smartbets_API/proxyh.py` & `smartbetsAPI-1.2.0/smartbets_API/proxyh.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,62 @@
-#Hunts down open proxies from github
-from random import choice 
+# Hunts down open proxies from github
+from random import choice
+
+
 class hunter45:
-    def __init__(self,requests:object):
-        self.links ={'socks5':'https://github.com/TheSpeedX/PROXY-List/raw/master/socks5.txt',
-        'socks4':'https://github.com/TheSpeedX/PROXY-List/raw/master/socks4.txt',
-        'https':'https://github.com/TheSpeedX/PROXY-List/raw/master/http.txt'
+    def __init__(self, requests: object):
+        self.links = {
+            "socks5": "https://github.com/TheSpeedX/PROXY-List/raw/master/socks5.txt",
+            "socks4": "https://github.com/TheSpeedX/PROXY-List/raw/master/socks4.txt",
+            "https": "https://github.com/TheSpeedX/PROXY-List/raw/master/http.txt",
         }
         self.requests = requests
-        self.type = 'socks5'
+        self.type = "socks5"
         self.picked = []
-    def get_proxy(self,type:str='socks5') -> list:
+
+    def get_proxy(self, type: str = "socks5") -> list:
         """fetches proxy"""
         try:
             self.type = type
             rp = self.requests.get(self.links[type])
-            if rp.status_code==200:
-                return (True,rp.text.split('\n'))
+            if rp.status_code == 200:
+                return (True, rp.text.split("\n"))
         except Exception as e:
-            return (False,e.args[1] if len(e.args)>1 else e)
-    def sample(self,current_proxies:list=[]) -> dict:
-        if len(current_proxies)>1:
+            return (False, e.args[1] if len(e.args) > 1 else e)
+
+    def sample(self, current_proxies: list = []) -> dict:
+        if len(current_proxies) > 1:
+
             def pick():
                 pk = choice(current_proxies)
                 if pk in self.picked:
                     return pick()
                 try:
                     current_proxies.remove(pk)
                 except:
                     pass
-                return self.type+'://'+pk
+                return self.type + "://" + pk
+
             pk = pick()
-            return (True,{
-                'http': pk,
-                'https': pk,
-            })
+            return (
+                True,
+                {
+                    "http": pk,
+                    "https": pk,
+                },
+            )
         else:
             self.type = choice(list(self.links.keys()))
             sp = self.get_proxy()
             if sp[0]:
-                return True,self.sample(sp[1])
+                return True, self.sample(sp[1])
             else:
                 return sp
 
-if __name__=='__main__':
+
+if __name__ == "__main__":
     import requests as req
-    run=hunter45(req)
-    all_proxies =run.get_proxy()[1]
+
+    run = hunter45(req)
+    all_proxies = run.get_proxy()[1]
     for x in all_proxies:
-        print(run.sample(all_proxies))
+        print(run.sample(all_proxies))
```

### Comparing `smartbetsAPI-1.1.6/smartbets_API/tertiary_bet.py` & `smartbetsAPI-1.2.0/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

