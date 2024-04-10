# Comparing `tmp/zf-school-sdk-1.5.0.tar.gz` & `tmp/zf-school-sdk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zf-school-sdk-1.5.0.tar", last modified: Sat Jul 15 15:02:44 2023, max compression
+gzip compressed data, was "zf-school-sdk-1.6.0.tar", last modified: Wed Apr 10 09:59:17 2024, max compression
```

## Comparing `zf-school-sdk-1.5.0.tar` & `zf-school-sdk-1.6.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.890283 zf-school-sdk-1.5.0/
--rw-r--r--   0 farmer     (501) staff       (20)     1074 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/LICENSE
--rw-r--r--   0 farmer     (501) staff       (20)     4786 2023-07-15 15:02:44.890152 zf-school-sdk-1.5.0/PKG-INFO
--rw-r--r--   0 farmer     (501) staff       (20)     4119 2023-07-15 15:00:59.000000 zf-school-sdk-1.5.0/README.md
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.885297 zf-school-sdk-1.5.0/school_sdk/
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.886097 zf-school-sdk-1.5.0/school_sdk/PyRsa/
--rw-r--r--   0 farmer     (501) staff       (20)      252 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/PyRsa/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)     2579 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/PyRsa/pyb64.py
--rw-r--r--   0 farmer     (501) staff       (20)    16593 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/PyRsa/pyjsbn.py
--rw-r--r--   0 farmer     (501) staff       (20)     2406 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/PyRsa/pyrng.py
--rw-r--r--   0 farmer     (501) staff       (20)     3023 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/PyRsa/pyrsa.py
--rw-r--r--   0 farmer     (501) staff       (20)      752 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/PyRsa/tools.py
--rw-r--r--   0 farmer     (501) staff       (20)      189 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/__init__.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.886958 zf-school-sdk-1.5.0/school_sdk/check_code/
--rw-r--r--   0 farmer     (501) staff       (20)     1546 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/check_code/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)      739 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/check_code/captcha_setting.py
--rw-r--r--   0 farmer     (501) staff       (20)     1051 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/check_code/dataset.py
--rw-r--r--   0 farmer     (501) staff       (20)     1602 2023-07-15 14:55:59.000000 zf-school-sdk-1.5.0/school_sdk/check_code/model.py
--rw-r--r--   0 farmer     (501) staff       (20)     1895 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/check_code/predict.py
--rw-r--r--   0 farmer     (501) staff       (20)     1087 2023-07-15 15:00:59.000000 zf-school-sdk-1.5.0/school_sdk/check_code/type.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.887534 zf-school-sdk-1.5.0/school_sdk/client/
--rw-r--r--   0 farmer     (501) staff       (20)     6525 2023-07-15 15:00:59.000000 zf-school-sdk-1.5.0/school_sdk/client/__init__.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.888795 zf-school-sdk-1.5.0/school_sdk/client/api/
--rw-r--r--   0 farmer     (501) staff       (20)     2069 2023-03-09 02:28:43.000000 zf-school-sdk-1.5.0/school_sdk/client/api/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)      324 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/client/api/check.py
--rw-r--r--   0 farmer     (501) staff       (20)     1987 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/client/api/class_schedule.py
--rw-r--r--   0 farmer     (501) staff       (20)     9006 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/client/api/login.py
--rw-r--r--   0 farmer     (501) staff       (20)     5038 2023-07-15 15:00:59.000000 zf-school-sdk-1.5.0/school_sdk/client/api/schedule_parse.py
--rw-r--r--   0 farmer     (501) staff       (20)     2926 2023-07-15 15:00:59.000000 zf-school-sdk-1.5.0/school_sdk/client/api/schedules.py
--rw-r--r--   0 farmer     (501) staff       (20)     4369 2023-07-15 15:00:59.000000 zf-school-sdk-1.5.0/school_sdk/client/api/score.py
--rw-r--r--   0 farmer     (501) staff       (20)     1795 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/client/api/user_info.py
--rw-r--r--   0 farmer     (501) staff       (20)     1532 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/client/base.py
--rw-r--r--   0 farmer     (501) staff       (20)      721 2023-03-09 02:31:33.000000 zf-school-sdk-1.5.0/school_sdk/client/exceptions.py
--rw-r--r--   0 farmer     (501) staff       (20)      983 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/client/utils.py
--rw-r--r--   0 farmer     (501) staff       (20)      867 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/config.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.888994 zf-school-sdk-1.5.0/school_sdk/session/
--rw-r--r--   0 farmer     (501) staff       (20)      259 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/session/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)      813 2023-02-25 03:25:17.000000 zf-school-sdk-1.5.0/school_sdk/utils.py
--rw-r--r--   0 farmer     (501) staff       (20)       38 2023-07-15 15:02:44.890334 zf-school-sdk-1.5.0/setup.cfg
--rw-r--r--   0 farmer     (501) staff       (20)     1462 2023-07-15 15:01:17.000000 zf-school-sdk-1.5.0/setup.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.889135 zf-school-sdk-1.5.0/test/
--rw-r--r--   0 farmer     (501) staff       (20)     1399 2023-07-15 15:00:59.000000 zf-school-sdk-1.5.0/test/test.py
--rw-r--r--   0 farmer     (501) staff       (20)     1489 2023-07-15 15:01:17.000000 zf-school-sdk-1.5.0/zf-setup.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:44.889934 zf-school-sdk-1.5.0/zf_school_sdk.egg-info/
--rw-r--r--   0 farmer     (501) staff       (20)     4786 2023-07-15 15:02:43.000000 zf-school-sdk-1.5.0/zf_school_sdk.egg-info/PKG-INFO
--rw-r--r--   0 farmer     (501) staff       (20)     1120 2023-07-15 15:02:43.000000 zf-school-sdk-1.5.0/zf_school_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 farmer     (501) staff       (20)        1 2023-07-15 15:02:43.000000 zf-school-sdk-1.5.0/zf_school_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 farmer     (501) staff       (20)        1 2023-02-25 07:33:56.000000 zf-school-sdk-1.5.0/zf_school_sdk.egg-info/not-zip-safe
--rw-r--r--   0 farmer     (501) staff       (20)       59 2023-07-15 15:02:43.000000 zf-school-sdk-1.5.0/zf_school_sdk.egg-info/requires.txt
--rw-r--r--   0 farmer     (501) staff       (20)       11 2023-07-15 15:02:43.000000 zf-school-sdk-1.5.0/zf_school_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.575236 zf-school-sdk-1.6.0/
+-rw-r--r--   0 farmer     (501) staff       (20)     1074 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/LICENSE
+-rw-r--r--   0 farmer     (501) staff       (20)     4913 2024-04-10 09:59:17.575115 zf-school-sdk-1.6.0/PKG-INFO
+-rw-r--r--   0 farmer     (501) staff       (20)     4246 2024-04-10 09:47:56.000000 zf-school-sdk-1.6.0/README.md
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.571038 zf-school-sdk-1.6.0/school_sdk/
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.571719 zf-school-sdk-1.6.0/school_sdk/PyRsa/
+-rw-r--r--   0 farmer     (501) staff       (20)      252 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/PyRsa/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)     2579 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/PyRsa/pyb64.py
+-rw-r--r--   0 farmer     (501) staff       (20)    16593 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/PyRsa/pyjsbn.py
+-rw-r--r--   0 farmer     (501) staff       (20)     2406 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/PyRsa/pyrng.py
+-rw-r--r--   0 farmer     (501) staff       (20)     3023 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/PyRsa/pyrsa.py
+-rw-r--r--   0 farmer     (501) staff       (20)      752 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/PyRsa/tools.py
+-rw-r--r--   0 farmer     (501) staff       (20)      226 2024-04-10 09:47:54.000000 zf-school-sdk-1.6.0/school_sdk/__init__.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.572504 zf-school-sdk-1.6.0/school_sdk/check_code/
+-rw-r--r--   0 farmer     (501) staff       (20)     1546 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/check_code/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)      739 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/check_code/captcha_setting.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1051 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/check_code/dataset.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1602 2023-07-15 14:55:59.000000 zf-school-sdk-1.6.0/school_sdk/check_code/model.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1895 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/check_code/predict.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1087 2023-07-15 15:00:59.000000 zf-school-sdk-1.6.0/school_sdk/check_code/type.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.573007 zf-school-sdk-1.6.0/school_sdk/client/
+-rw-r--r--   0 farmer     (501) staff       (20)     7209 2024-04-10 09:51:40.000000 zf-school-sdk-1.6.0/school_sdk/client/__init__.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.573998 zf-school-sdk-1.6.0/school_sdk/client/api/
+-rw-r--r--   0 farmer     (501) staff       (20)     2069 2023-03-09 02:28:43.000000 zf-school-sdk-1.6.0/school_sdk/client/api/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)      324 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/client/api/check.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1987 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/client/api/class_schedule.py
+-rw-r--r--   0 farmer     (501) staff       (20)     9006 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/client/api/login.py
+-rw-r--r--   0 farmer     (501) staff       (20)     5038 2023-07-15 15:00:59.000000 zf-school-sdk-1.6.0/school_sdk/client/api/schedule_parse.py
+-rw-r--r--   0 farmer     (501) staff       (20)     2926 2023-10-30 07:22:15.000000 zf-school-sdk-1.6.0/school_sdk/client/api/schedules.py
+-rw-r--r--   0 farmer     (501) staff       (20)     4369 2023-07-15 15:00:59.000000 zf-school-sdk-1.6.0/school_sdk/client/api/score.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1795 2023-07-16 03:19:33.000000 zf-school-sdk-1.6.0/school_sdk/client/api/user_info.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1532 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/client/base.py
+-rw-r--r--   0 farmer     (501) staff       (20)      721 2023-03-09 02:31:33.000000 zf-school-sdk-1.6.0/school_sdk/client/exceptions.py
+-rw-r--r--   0 farmer     (501) staff       (20)      983 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/client/utils.py
+-rw-r--r--   0 farmer     (501) staff       (20)      867 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/config.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.574106 zf-school-sdk-1.6.0/school_sdk/session/
+-rw-r--r--   0 farmer     (501) staff       (20)      259 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/session/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)      183 2024-04-10 09:47:54.000000 zf-school-sdk-1.6.0/school_sdk/type.py
+-rw-r--r--   0 farmer     (501) staff       (20)      813 2023-02-25 03:25:17.000000 zf-school-sdk-1.6.0/school_sdk/utils.py
+-rw-r--r--   0 farmer     (501) staff       (20)       38 2024-04-10 09:59:17.575276 zf-school-sdk-1.6.0/setup.cfg
+-rw-r--r--   0 farmer     (501) staff       (20)     1462 2024-04-10 09:59:02.000000 zf-school-sdk-1.6.0/setup.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.574218 zf-school-sdk-1.6.0/test/
+-rw-r--r--   0 farmer     (501) staff       (20)     1399 2024-01-08 01:46:29.000000 zf-school-sdk-1.6.0/test/test.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1489 2024-04-10 09:59:11.000000 zf-school-sdk-1.6.0/zf-setup.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 09:59:17.574910 zf-school-sdk-1.6.0/zf_school_sdk.egg-info/
+-rw-r--r--   0 farmer     (501) staff       (20)     4913 2024-04-10 09:59:16.000000 zf-school-sdk-1.6.0/zf_school_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 farmer     (501) staff       (20)     1139 2024-04-10 09:59:16.000000 zf-school-sdk-1.6.0/zf_school_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 farmer     (501) staff       (20)        1 2024-04-10 09:59:16.000000 zf-school-sdk-1.6.0/zf_school_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 farmer     (501) staff       (20)        1 2023-02-25 07:33:56.000000 zf-school-sdk-1.6.0/zf_school_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 farmer     (501) staff       (20)       59 2024-04-10 09:59:16.000000 zf-school-sdk-1.6.0/zf_school_sdk.egg-info/requires.txt
+-rw-r--r--   0 farmer     (501) staff       (20)       11 2024-04-10 09:59:16.000000 zf-school-sdk-1.6.0/zf_school_sdk.egg-info/top_level.txt
```

### Comparing `zf-school-sdk-1.5.0/LICENSE` & `zf-school-sdk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/PKG-INFO` & `zf-school-sdk-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zf-school-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: zf School SDK for Python
 Home-page: https://github.com/Farmer-chong/new-school-sdk
 Author: farmer.chillax
 Author-email: farmer-chong@qq.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -51,14 +51,17 @@
 ## Usage
 ```Shell
 $ pip install school-sdk
 # or
 $ pip install zf-school-sdk
 ```
 
+> 如果机器内存不足，可以使用 pip `--no-cache-dir` 选项来安装
+> e.g: `pip --no-cache-dir install school-sdk`
+
 ```Python
 from school_sdk import SchoolClient
 
 # 先实例化一个学校，再实例化用户
 school = SchoolClient("172.16.254.1")
 user:UserClient = school.user_login("2018xxxxx", "xxxxxxxx")
 course = user.get_schedule(year=2020, term=2)
```

### Comparing `zf-school-sdk-1.5.0/README.md` & `zf-school-sdk-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 ## Usage
 ```Shell
 $ pip install school-sdk
 # or
 $ pip install zf-school-sdk
 ```
 
+> 如果机器内存不足，可以使用 pip `--no-cache-dir` 选项来安装
+> e.g: `pip --no-cache-dir install school-sdk`
+
 ```Python
 from school_sdk import SchoolClient
 
 # 先实例化一个学校，再实例化用户
 school = SchoolClient("172.16.254.1")
 user:UserClient = school.user_login("2018xxxxx", "xxxxxxxx")
 course = user.get_schedule(year=2020, term=2)
```

### Comparing `zf-school-sdk-1.5.0/school_sdk/PyRsa/pyb64.py` & `zf-school-sdk-1.6.0/school_sdk/PyRsa/pyb64.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/PyRsa/pyjsbn.py` & `zf-school-sdk-1.6.0/school_sdk/PyRsa/pyjsbn.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/PyRsa/pyrng.py` & `zf-school-sdk-1.6.0/school_sdk/PyRsa/pyrng.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/PyRsa/pyrsa.py` & `zf-school-sdk-1.6.0/school_sdk/PyRsa/pyrsa.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/PyRsa/tools.py` & `zf-school-sdk-1.6.0/school_sdk/PyRsa/tools.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/check_code/__init__.py` & `zf-school-sdk-1.6.0/school_sdk/check_code/__init__.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/check_code/captcha_setting.py` & `zf-school-sdk-1.6.0/school_sdk/check_code/captcha_setting.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/check_code/dataset.py` & `zf-school-sdk-1.6.0/school_sdk/check_code/dataset.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/check_code/model.py` & `zf-school-sdk-1.6.0/school_sdk/check_code/model.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/check_code/predict.py` & `zf-school-sdk-1.6.0/school_sdk/check_code/predict.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/check_code/type.py` & `zf-school-sdk-1.6.0/school_sdk/check_code/type.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/__init__.py` & `zf-school-sdk-1.6.0/school_sdk/client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from school_sdk.client.api.schedules import Schedule
 from school_sdk.client.exceptions import LoginException
 import time
 from school_sdk.client.api.login import ZFLogin
 from school_sdk.client.base import BaseUserClient
 
 
+CAPTCHA: str = 'captcha'
+KCAPTCHA: str = 'kap'
+
 class SchoolClient():
 
     def __init__(self, host, port: int = 80, ssl: bool = False, name=None, exist_verify: bool = False,
                  captcha_type: str = "captcha", retry: int = 10, lan_host=None, lan_port=80, timeout=10,
                  login_url_path=None, url_endpoints=None) -> None:
         """初始化学校配置
 
@@ -64,14 +67,27 @@
         Args:
             account (str): 用户账号
             password (str): 用户密码
         """
         user = UserClient(self, account=account, password=password, **kwargs)
         return user.login()
 
+    def user_login_with_cookies(self, cookies: str, account: str = "cookie login account", **kwargs):
+        """使用cookies登录
+            该方法因缺失帐号密码，因此无法刷新session，需要手动刷新
+            传参中的 account 主要用于标识当前登录用户、记录日志信息等用途，不会用于登录
+
+        Args:
+            cookies (str): Cookies字符串
+            account (str, optional): 账号. Defaults to "cookie login account".
+        """
+
+        user = UserClient(self, account=account, password="cookies login password", **kwargs)
+        return user.get_dev_user(cookies)
+
     def init_dev_user(self, cookies: str = None):
         dev_user = UserClient(self, account="dev account",
                               password="dev password")
         return dev_user.get_dev_user(cookies)
 
 
 class UserClient(BaseUserClient):
```

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/api/__init__.py` & `zf-school-sdk-1.6.0/school_sdk/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/api/class_schedule.py` & `zf-school-sdk-1.6.0/school_sdk/client/api/class_schedule.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/api/login.py` & `zf-school-sdk-1.6.0/school_sdk/client/api/login.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/api/schedule_parse.py` & `zf-school-sdk-1.6.0/school_sdk/client/api/schedule_parse.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/api/schedules.py` & `zf-school-sdk-1.6.0/school_sdk/client/api/schedules.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/api/score.py` & `zf-school-sdk-1.6.0/school_sdk/client/api/score.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/api/user_info.py` & `zf-school-sdk-1.6.0/school_sdk/client/api/user_info.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/base.py` & `zf-school-sdk-1.6.0/school_sdk/client/base.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/exceptions.py` & `zf-school-sdk-1.6.0/school_sdk/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/client/utils.py` & `zf-school-sdk-1.6.0/school_sdk/client/utils.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/config.py` & `zf-school-sdk-1.6.0/school_sdk/config.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/school_sdk/utils.py` & `zf-school-sdk-1.6.0/school_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/setup.py` & `zf-school-sdk-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 with open(path.join(basedir, "README.md"), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name="school-sdk",
     author="farmer.chillax",
-    version="1.5.0",
+    version="1.6.0",
     license='MIT',
     author_email="farmer-chong@qq.com",
     description="zf School SDK for Python",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Farmer-chong/new-school-sdk',
     packages=find_packages(),
```

### Comparing `zf-school-sdk-1.5.0/test/test.py` & `zf-school-sdk-1.6.0/test/test.py`

 * *Files identical despite different names*

### Comparing `zf-school-sdk-1.5.0/zf-setup.py` & `zf-school-sdk-1.6.0/zf-setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 with open(path.join(basedir, "README.md"), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name="zf-school-sdk",
     author="farmer.chillax",
-    version="1.5.0",
+    version="1.6.0",
     license='MIT',
     author_email="farmer-chong@qq.com",
     description="zf School SDK for Python",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Farmer-chong/new-school-sdk',
     packages=find_packages(),
```

### Comparing `zf-school-sdk-1.5.0/zf_school_sdk.egg-info/PKG-INFO` & `zf-school-sdk-1.6.0/zf_school_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zf-school-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: zf School SDK for Python
 Home-page: https://github.com/Farmer-chong/new-school-sdk
 Author: farmer.chillax
 Author-email: farmer-chong@qq.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -51,14 +51,17 @@
 ## Usage
 ```Shell
 $ pip install school-sdk
 # or
 $ pip install zf-school-sdk
 ```
 
+> 如果机器内存不足，可以使用 pip `--no-cache-dir` 选项来安装
+> e.g: `pip --no-cache-dir install school-sdk`
+
 ```Python
 from school_sdk import SchoolClient
 
 # 先实例化一个学校，再实例化用户
 school = SchoolClient("172.16.254.1")
 user:UserClient = school.user_login("2018xxxxx", "xxxxxxxx")
 course = user.get_schedule(year=2020, term=2)
```

### Comparing `zf-school-sdk-1.5.0/zf_school_sdk.egg-info/SOURCES.txt` & `zf-school-sdk-1.6.0/zf_school_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 zf-setup.py
 school_sdk/__init__.py
 school_sdk/config.py
+school_sdk/type.py
 school_sdk/utils.py
 school_sdk/PyRsa/__init__.py
 school_sdk/PyRsa/pyb64.py
 school_sdk/PyRsa/pyjsbn.py
 school_sdk/PyRsa/pyrng.py
 school_sdk/PyRsa/pyrsa.py
 school_sdk/PyRsa/tools.py
```

