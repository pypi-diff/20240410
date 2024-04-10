# Comparing `tmp/ZJFootballAutoSign-0.1.2.tar.gz` & `tmp/ZJFootballAutoSign-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ZJFootballAutoSign-0.1.2.tar", last modified: Wed Mar 27 09:36:05 2024, max compression
+gzip compressed data, was "dist\ZJFootballAutoSign-0.1.3.tar", last modified: Wed Apr 10 11:08:15 2024, max compression
```

## Comparing `ZJFootballAutoSign-0.1.2.tar` & `ZJFootballAutoSign-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/
--rw-rw-rw-   0        0        0     1100 2024-03-27 06:32:16.000000 ZJFootballAutoSign-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      442 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-03-27 08:52:52.000000 ZJFootballAutoSign-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign/
--rw-rw-rw-   0        0        0       52 2024-03-27 09:30:32.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign/__init__.py
--rw-rw-rw-   0        0        0     2852 2024-03-27 09:35:47.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign/signIn.py
-drwxrwxrwx   0        0        0        0 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign.egg-info/
--rw-rw-rw-   0        0        0      442 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/ZJFootballAutoSign.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 09:36:05.000000 ZJFootballAutoSign-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-03-27 09:31:13.000000 ZJFootballAutoSign-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/
+-rw-rw-rw-   0        0        0     1100 2024-03-27 06:32:16.000000 ZJFootballAutoSign-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      442 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-03-27 09:42:36.000000 ZJFootballAutoSign-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign/
+-rw-rw-rw-   0        0        0       52 2024-03-27 09:30:32.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign/__init__.py
+-rw-rw-rw-   0        0        0     2858 2024-03-27 09:37:47.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign/signIn.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign.egg-info/
+-rw-rw-rw-   0        0        0      442 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/ZJFootballAutoSign.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 11:08:15.000000 ZJFootballAutoSign-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-10 11:07:41.000000 ZJFootballAutoSign-0.1.3/setup.py
```

### Comparing `ZJFootballAutoSign-0.1.2/LICENSE` & `ZJFootballAutoSign-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ZJFootballAutoSign-0.1.2/ZJFootballAutoSign/signIn.py` & `ZJFootballAutoSign-0.1.3/ZJFootballAutoSign/signIn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 def trySignIn(account,password,edgeDriverPath = ''):
     from selenium import webdriver
     from selenium.webdriver.common.by import By
     from selenium.webdriver.edge.service import Service
     from selenium.webdriver.edge.options import Options
     import time
     from os import getcwd
+    
     edge_options = Options()
     edge_options.add_argument('--headless')
     edge_options.add_argument('--disable-gpu')
     edge_options.add_argument('--no-sandbox')
     edge_options.add_argument('--disable-dev-shm-usage')
     edge_options.add_experimental_option('excludeSwitches', ['enable-logging'])
```

### Comparing `ZJFootballAutoSign-0.1.2/setup.py` & `ZJFootballAutoSign-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(name='ZJFootballAutoSign',
-        version='0.1.2',
+        version='0.1.3',
         packages=find_packages(),
         include_package_data=False,
         package_data={'data': []},
         install_requires = ['selenium'],
         description='A script used for automatically signing in on Zhejiang Professional Football Club\'s website.',
         author='konata321',
         author_email='megumi321@163.com',
```

