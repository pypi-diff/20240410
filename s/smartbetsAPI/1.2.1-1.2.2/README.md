# Comparing `tmp/smartbetsAPI-1.2.1.tar.gz` & `tmp/smartbetsAPI-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.2.1.tar", last modified: Wed Apr 10 13:59:05 2024, max compression
+gzip compressed data, was "smartbetsAPI-1.2.2.tar", last modified: Wed Apr 10 14:03:38 2024, max compression
```

## Comparing `smartbetsAPI-1.2.1.tar` & `smartbetsAPI-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 13:59:05.095154 smartbetsAPI-1.2.1/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.1/LICENSE
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11529 2024-04-10 13:59:05.095154 smartbetsAPI-1.2.1/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9382 2024-04-10 13:58:46.000000 smartbetsAPI-1.2.1/README.md
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-10 13:59:05.095154 smartbetsAPI-1.2.1/setup.cfg
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2412 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/setup.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 13:59:05.091821 smartbetsAPI-1.2.1/smartbetsAPI.egg-info/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11529 2024-04-10 13:59:04.000000 smartbetsAPI-1.2.1/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-10 13:59:05.000000 smartbetsAPI-1.2.1/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-10 13:59:04.000000 smartbetsAPI-1.2.1/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-10 13:59:04.000000 smartbetsAPI-1.2.1/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       99 2024-04-10 13:59:04.000000 smartbetsAPI-1.2.1/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-10 13:59:04.000000 smartbetsAPI-1.2.1/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 13:59:05.091821 smartbetsAPI-1.2.1/smartbets_API/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-10 13:58:38.000000 smartbetsAPI-1.2.1/smartbets_API/__init__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/smartbets_API/__main__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.1/smartbets_API/bet_analyzer.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2746 2024-04-10 13:57:50.000000 smartbetsAPI-1.2.1/smartbets_API/bet_at_rest_api_level.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/smartbets_API/bet_common.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/smartbets_API/configuration_handler.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.1/smartbets_API/figure_harvester.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.1/smartbets_API/googler.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/smartbets_API/html_fetcher.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5079 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/smartbets_API/interface.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/smartbets_API/predictor.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.1/smartbets_API/proxyh.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.1/smartbets_API/tertiary_bet.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 14:03:38.713166 smartbetsAPI-1.2.2/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.2/LICENSE
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11551 2024-04-10 14:03:38.713166 smartbetsAPI-1.2.2/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9382 2024-04-10 13:58:46.000000 smartbetsAPI-1.2.2/README.md
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-10 14:03:38.713166 smartbetsAPI-1.2.2/setup.cfg
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2430 2024-04-10 14:02:48.000000 smartbetsAPI-1.2.2/setup.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 14:03:38.713166 smartbetsAPI-1.2.2/smartbetsAPI.egg-info/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11551 2024-04-10 14:03:38.000000 smartbetsAPI-1.2.2/smartbetsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-10 14:03:38.000000 smartbetsAPI-1.2.2/smartbetsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-10 14:03:38.000000 smartbetsAPI-1.2.2/smartbetsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-10 14:03:38.000000 smartbetsAPI-1.2.2/smartbetsAPI.egg-info/entry_points.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      106 2024-04-10 14:03:38.000000 smartbetsAPI-1.2.2/smartbetsAPI.egg-info/requires.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-10 14:03:38.000000 smartbetsAPI-1.2.2/smartbetsAPI.egg-info/top_level.txt
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-10 14:03:38.713166 smartbetsAPI-1.2.2/smartbets_API/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-10 14:03:22.000000 smartbetsAPI-1.2.2/smartbets_API/__init__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.2/smartbets_API/__main__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.2/smartbets_API/bet_analyzer.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2746 2024-04-10 13:57:50.000000 smartbetsAPI-1.2.2/smartbets_API/bet_at_rest_api_level.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.2/smartbets_API/bet_common.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.2/smartbets_API/configuration_handler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.2/smartbets_API/figure_harvester.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.2/smartbets_API/googler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.2/smartbets_API/html_fetcher.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5079 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.2/smartbets_API/interface.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.2/smartbets_API/predictor.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.2/smartbets_API/proxyh.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.2/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.2.1/LICENSE` & `smartbetsAPI-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/PKG-INFO` & `smartbetsAPI-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -30,15 +30,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fastapi[uvicorn]==0.110.1
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn==0.29.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
 
 <h1 align="center">smartbetsAPI</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.1 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.2 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
@@ -16,18 +16,18 @@
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment Requires-Python: >=3.9 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: fastapi
-[uvicorn]==0.110.1 Requires-Dist: appdirs==1.4.4 Requires-Dist:
-requests==2.31.0 Requires-Dist: colorama==0.4.6 Requires-Dist: bs4==0.0.1
-Requires-Dist: Faker==15.3.4
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+fastapi==0.110.1 Requires-Dist: uvicorn==0.29.0 Requires-Dist: appdirs==1.4.4
+Requires-Dist: requests==2.31.0 Requires-Dist: colorama==0.4.6 Requires-Dist:
+bs4==0.0.1 Requires-Dist: Faker==15.3.4
                           ************ ssmmaarrttbbeettssAAPPII ************
      _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_A_c_c_u_r_a_c_y_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]
                                   _[_D_o_w_n_l_o_a_d_s_]
 
 > "Punter's choice" Worldwide soccer-matches predictor with Fast-API and a
 package for integrating the scripts in your own [Python](https://python.org)
 code. ## Features - REST-API - Script integration (package) - Non-ML ##
```

### Comparing `smartbetsAPI-1.2.1/README.md` & `smartbetsAPI-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/setup.py` & `smartbetsAPI-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     author_email="smartwacaleb@gmail.com",
     maintainer="Smartwa Caleb",
     maintainer_email="smartwacaleb@gmail.com",
     description="Simple football prediction API",
     long_description="\n".join(get_file("README.md")),
     long_description_content_type="text/markdown",
     install_requires=[
-        "fastapi[uvicorn]==0.110.1",
+        "fastapi==0.110.1",
+        "uvicorn==0.29.0",
         "appdirs==1.4.4",
         "requests==2.31.0",
         "colorama==0.4.6",
         "bs4==0.0.1",
         "Faker==15.3.4",
     ],
     python_requires =">=3.9",
```

### Comparing `smartbetsAPI-1.2.1/smartbetsAPI.egg-info/PKG-INFO` & `smartbetsAPI-1.2.2/smartbetsAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -30,15 +30,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fastapi[uvicorn]==0.110.1
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn==0.29.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
 
 <h1 align="center">smartbetsAPI</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.1 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.2 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
@@ -16,18 +16,18 @@
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment Requires-Python: >=3.9 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: fastapi
-[uvicorn]==0.110.1 Requires-Dist: appdirs==1.4.4 Requires-Dist:
-requests==2.31.0 Requires-Dist: colorama==0.4.6 Requires-Dist: bs4==0.0.1
-Requires-Dist: Faker==15.3.4
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+fastapi==0.110.1 Requires-Dist: uvicorn==0.29.0 Requires-Dist: appdirs==1.4.4
+Requires-Dist: requests==2.31.0 Requires-Dist: colorama==0.4.6 Requires-Dist:
+bs4==0.0.1 Requires-Dist: Faker==15.3.4
                           ************ ssmmaarrttbbeettssAAPPII ************
      _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_A_c_c_u_r_a_c_y_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]
                                   _[_D_o_w_n_l_o_a_d_s_]
 
 > "Punter's choice" Worldwide soccer-matches predictor with Fast-API and a
 package for integrating the scripts in your own [Python](https://python.org)
 code. ## Features - REST-API - Script integration (package) - Non-ML ##
```

### Comparing `smartbetsAPI-1.2.1/smartbetsAPI.egg-info/SOURCES.txt` & `smartbetsAPI-1.2.2/smartbetsAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/bet_analyzer.py` & `smartbetsAPI-1.2.2/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/bet_at_rest_api_level.py` & `smartbetsAPI-1.2.2/smartbets_API/bet_at_rest_api_level.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/bet_common.py` & `smartbetsAPI-1.2.2/smartbets_API/bet_common.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/configuration_handler.py` & `smartbetsAPI-1.2.2/smartbets_API/configuration_handler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/figure_harvester.py` & `smartbetsAPI-1.2.2/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/googler.py` & `smartbetsAPI-1.2.2/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/html_fetcher.py` & `smartbetsAPI-1.2.2/smartbets_API/html_fetcher.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/interface.py` & `smartbetsAPI-1.2.2/smartbets_API/interface.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/predictor.py` & `smartbetsAPI-1.2.2/smartbets_API/predictor.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/proxyh.py` & `smartbetsAPI-1.2.2/smartbets_API/proxyh.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.1/smartbets_API/tertiary_bet.py` & `smartbetsAPI-1.2.2/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

