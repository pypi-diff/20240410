# Comparing `tmp/yplib-5.5.7.tar.gz` & `tmp/yplib-5.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-5.5.7.tar", last modified: Tue Mar 26 08:38:23 2024, max compression
+gzip compressed data, was "dist\yplib-5.5.8.tar", last modified: Wed Apr 10 06:44:51 2024, max compression
```

## Comparing `yplib-5.5.7.tar` & `yplib-5.5.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 08:38:23.013491 yplib-5.5.7/
--rw-rw-rw-   0        0        0      400 2024-03-26 08:38:23.012491 yplib-5.5.7/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.5.7/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 08:38:23.013491 yplib-5.5.7/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-03-26 08:38:09.000000 yplib-5.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:38:23.004493 yplib-5.5.7/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.5.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.5.7/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.5.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0    10134 2024-03-26 08:38:02.000000 yplib-5.5.7/yplib/db.py
--rw-rw-rw-   0        0        0     5292 2023-07-17 06:31:43.000000 yplib-5.5.7/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.5.7/yplib/http_util.py
--rw-rw-rw-   0        0        0    40699 2024-03-22 04:18:16.000000 yplib-5.5.7/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.5.7/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.5.7/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.5.7/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.5.7/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:38:23.010494 yplib-5.5.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      400 2024-03-26 08:38:22.000000 yplib-5.5.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-03-26 08:38:22.000000 yplib-5.5.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 08:38:22.000000 yplib-5.5.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-26 08:38:22.000000 yplib-5.5.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:44:51.503811 yplib-5.5.8/
+-rw-rw-rw-   0        0        0      400 2024-04-10 06:44:51.503811 yplib-5.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 06:44:51.504811 yplib-5.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-10 06:44:44.000000 yplib-5.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:44:51.496810 yplib-5.5.8/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.5.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.5.8/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.5.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    10134 2024-03-26 08:38:02.000000 yplib-5.5.8/yplib/db.py
+-rw-rw-rw-   0        0        0     5292 2023-07-17 06:31:43.000000 yplib-5.5.8/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.5.8/yplib/http_util.py
+-rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.5.8/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.5.8/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.5.8/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.5.8/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.5.8/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:44:51.501809 yplib-5.5.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.5.7/setup.py` & `yplib-5.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.5.7",
+    version="5.5.8",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.5.7/yplib/__init__.py` & `yplib-5.5.8/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/chart.py` & `yplib-5.5.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/chart_html.py` & `yplib-5.5.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/db.py` & `yplib-5.5.8/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/file.py` & `yplib-5.5.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/http_util.py` & `yplib-5.5.8/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/index.py` & `yplib-5.5.8/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from datetime import timedelta
 
 import openpyxl
 import xlrd
 
 CONFIG_PATH = '.yp.config'
 
+CONFIG_PATH_BAK = 'yp.config'
+
 
 # 是否是 windows 系统
 def is_win():
     return platform.system().lower() == 'windows'
 
 
 # 是否是 linux 系统, 不是 windows , 就是 linux 系统
@@ -968,15 +970,15 @@
     set_data_in_path(file_name, data, os.path.expanduser("~"))
 
 
 # 在当前的目录中, 获得指定文件的数据
 def get_data_from_path(file_name='config', file_path=None):
     config_path = file_path + '/' + CONFIG_PATH if file_path else CONFIG_PATH
     if not os.path.exists(config_path):
-        return {}
+        config_path = file_path + '/' + CONFIG_PATH_BAK if file_path else CONFIG_PATH_BAK
     file_path = config_path + '/' + file_name + '.json'
     if not os.path.exists(file_path):
         return {}
     return to_json_from_file(file_path)
 
 
 # 在当前的目录中, 设置数据到指定路径下
```

### Comparing `yplib-5.5.7/yplib/mail.py` & `yplib-5.5.8/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/mail_html.py` & `yplib-5.5.8/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.7/yplib/markdown.py` & `yplib-5.5.8/yplib/markdown.py`

 * *Files identical despite different names*

