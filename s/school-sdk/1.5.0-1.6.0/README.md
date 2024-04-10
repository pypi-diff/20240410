# Comparing `tmp/school-sdk-1.5.0.tar.gz` & `tmp/school-sdk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "school-sdk-1.5.0.tar", last modified: Sat Jul 15 15:02:33 2023, max compression
+gzip compressed data, was "school-sdk-1.6.0.tar", last modified: Wed Apr 10 10:17:53 2024, max compression
```

## Comparing `school-sdk-1.5.0.tar` & `school-sdk-1.6.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.651465 school-sdk-1.5.0/
--rw-r--r--   0 farmer     (501) staff       (20)     1074 2023-02-25 03:25:17.000000 school-sdk-1.5.0/LICENSE
--rw-r--r--   0 farmer     (501) staff       (20)     4783 2023-07-15 15:02:33.651337 school-sdk-1.5.0/PKG-INFO
--rw-r--r--   0 farmer     (501) staff       (20)     4119 2023-07-15 15:00:59.000000 school-sdk-1.5.0/README.md
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.646937 school-sdk-1.5.0/school_sdk/
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.648613 school-sdk-1.5.0/school_sdk/PyRsa/
--rw-r--r--   0 farmer     (501) staff       (20)      252 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/PyRsa/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)     2579 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/PyRsa/pyb64.py
--rw-r--r--   0 farmer     (501) staff       (20)    16593 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/PyRsa/pyjsbn.py
--rw-r--r--   0 farmer     (501) staff       (20)     2406 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/PyRsa/pyrng.py
--rw-r--r--   0 farmer     (501) staff       (20)     3023 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/PyRsa/pyrsa.py
--rw-r--r--   0 farmer     (501) staff       (20)      752 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/PyRsa/tools.py
--rw-r--r--   0 farmer     (501) staff       (20)      189 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/__init__.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.649416 school-sdk-1.5.0/school_sdk/check_code/
--rw-r--r--   0 farmer     (501) staff       (20)     1546 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/check_code/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)      739 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/check_code/captcha_setting.py
--rw-r--r--   0 farmer     (501) staff       (20)     1051 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/check_code/dataset.py
--rw-r--r--   0 farmer     (501) staff       (20)     1602 2023-07-15 14:55:59.000000 school-sdk-1.5.0/school_sdk/check_code/model.py
--rw-r--r--   0 farmer     (501) staff       (20)     1895 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/check_code/predict.py
--rw-r--r--   0 farmer     (501) staff       (20)     1087 2023-07-15 15:00:59.000000 school-sdk-1.5.0/school_sdk/check_code/type.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.649864 school-sdk-1.5.0/school_sdk/client/
--rw-r--r--   0 farmer     (501) staff       (20)     6525 2023-07-15 15:00:59.000000 school-sdk-1.5.0/school_sdk/client/__init__.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.650920 school-sdk-1.5.0/school_sdk/client/api/
--rw-r--r--   0 farmer     (501) staff       (20)     2069 2023-03-09 02:28:43.000000 school-sdk-1.5.0/school_sdk/client/api/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)      324 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/client/api/check.py
--rw-r--r--   0 farmer     (501) staff       (20)     1987 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/client/api/class_schedule.py
--rw-r--r--   0 farmer     (501) staff       (20)     9006 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/client/api/login.py
--rw-r--r--   0 farmer     (501) staff       (20)     5038 2023-07-15 15:00:59.000000 school-sdk-1.5.0/school_sdk/client/api/schedule_parse.py
--rw-r--r--   0 farmer     (501) staff       (20)     2926 2023-07-15 15:00:59.000000 school-sdk-1.5.0/school_sdk/client/api/schedules.py
--rw-r--r--   0 farmer     (501) staff       (20)     4369 2023-07-15 15:00:59.000000 school-sdk-1.5.0/school_sdk/client/api/score.py
--rw-r--r--   0 farmer     (501) staff       (20)     1795 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/client/api/user_info.py
--rw-r--r--   0 farmer     (501) staff       (20)     1532 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/client/base.py
--rw-r--r--   0 farmer     (501) staff       (20)      721 2023-03-09 02:31:33.000000 school-sdk-1.5.0/school_sdk/client/exceptions.py
--rw-r--r--   0 farmer     (501) staff       (20)      983 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/client/utils.py
--rw-r--r--   0 farmer     (501) staff       (20)      867 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/config.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.651060 school-sdk-1.5.0/school_sdk/session/
--rw-r--r--   0 farmer     (501) staff       (20)      259 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/session/__init__.py
--rw-r--r--   0 farmer     (501) staff       (20)      813 2023-02-25 03:25:17.000000 school-sdk-1.5.0/school_sdk/utils.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.647690 school-sdk-1.5.0/school_sdk.egg-info/
--rw-r--r--   0 farmer     (501) staff       (20)     4783 2023-07-15 15:02:32.000000 school-sdk-1.5.0/school_sdk.egg-info/PKG-INFO
--rw-r--r--   0 farmer     (501) staff       (20)     1090 2023-07-15 15:02:32.000000 school-sdk-1.5.0/school_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 farmer     (501) staff       (20)        1 2023-07-15 15:02:32.000000 school-sdk-1.5.0/school_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 farmer     (501) staff       (20)        1 2023-02-25 07:34:21.000000 school-sdk-1.5.0/school_sdk.egg-info/not-zip-safe
--rw-r--r--   0 farmer     (501) staff       (20)       59 2023-07-15 15:02:32.000000 school-sdk-1.5.0/school_sdk.egg-info/requires.txt
--rw-r--r--   0 farmer     (501) staff       (20)       11 2023-07-15 15:02:32.000000 school-sdk-1.5.0/school_sdk.egg-info/top_level.txt
--rw-r--r--   0 farmer     (501) staff       (20)       38 2023-07-15 15:02:33.651503 school-sdk-1.5.0/setup.cfg
--rw-r--r--   0 farmer     (501) staff       (20)     1462 2023-07-15 15:01:17.000000 school-sdk-1.5.0/setup.py
-drwxr-xr-x   0 farmer     (501) staff       (20)        0 2023-07-15 15:02:33.651167 school-sdk-1.5.0/test/
--rw-r--r--   0 farmer     (501) staff       (20)     1399 2023-07-15 15:00:59.000000 school-sdk-1.5.0/test/test.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.926791 school-sdk-1.6.0/
+-rw-r--r--   0 farmer     (501) staff       (20)     1074 2023-02-25 03:25:17.000000 school-sdk-1.6.0/LICENSE
+-rw-r--r--   0 farmer     (501) staff       (20)     5065 2024-04-10 10:17:53.926663 school-sdk-1.6.0/PKG-INFO
+-rw-r--r--   0 farmer     (501) staff       (20)     4401 2024-04-10 10:15:04.000000 school-sdk-1.6.0/README.md
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.922567 school-sdk-1.6.0/school_sdk/
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.924070 school-sdk-1.6.0/school_sdk/PyRsa/
+-rw-r--r--   0 farmer     (501) staff       (20)      252 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/PyRsa/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)     2579 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/PyRsa/pyb64.py
+-rw-r--r--   0 farmer     (501) staff       (20)    16593 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/PyRsa/pyjsbn.py
+-rw-r--r--   0 farmer     (501) staff       (20)     2406 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/PyRsa/pyrng.py
+-rw-r--r--   0 farmer     (501) staff       (20)     3023 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/PyRsa/pyrsa.py
+-rw-r--r--   0 farmer     (501) staff       (20)      752 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/PyRsa/tools.py
+-rw-r--r--   0 farmer     (501) staff       (20)      226 2024-04-10 10:14:03.000000 school-sdk-1.6.0/school_sdk/__init__.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.924785 school-sdk-1.6.0/school_sdk/check_code/
+-rw-r--r--   0 farmer     (501) staff       (20)     1546 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/check_code/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)      739 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/check_code/captcha_setting.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1051 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/check_code/dataset.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1602 2023-07-15 14:55:59.000000 school-sdk-1.6.0/school_sdk/check_code/model.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1895 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/check_code/predict.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1087 2023-07-15 15:00:59.000000 school-sdk-1.6.0/school_sdk/check_code/type.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.925273 school-sdk-1.6.0/school_sdk/client/
+-rw-r--r--   0 farmer     (501) staff       (20)     7209 2024-04-10 10:14:03.000000 school-sdk-1.6.0/school_sdk/client/__init__.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.926251 school-sdk-1.6.0/school_sdk/client/api/
+-rw-r--r--   0 farmer     (501) staff       (20)     2069 2023-03-09 02:28:43.000000 school-sdk-1.6.0/school_sdk/client/api/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)      324 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/client/api/check.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1987 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/client/api/class_schedule.py
+-rw-r--r--   0 farmer     (501) staff       (20)     9006 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/client/api/login.py
+-rw-r--r--   0 farmer     (501) staff       (20)     5038 2023-07-15 15:00:59.000000 school-sdk-1.6.0/school_sdk/client/api/schedule_parse.py
+-rw-r--r--   0 farmer     (501) staff       (20)     2926 2023-10-30 07:22:15.000000 school-sdk-1.6.0/school_sdk/client/api/schedules.py
+-rw-r--r--   0 farmer     (501) staff       (20)     4369 2023-07-15 15:00:59.000000 school-sdk-1.6.0/school_sdk/client/api/score.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1795 2023-07-16 03:19:33.000000 school-sdk-1.6.0/school_sdk/client/api/user_info.py
+-rw-r--r--   0 farmer     (501) staff       (20)     1532 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/client/base.py
+-rw-r--r--   0 farmer     (501) staff       (20)      721 2023-03-09 02:31:33.000000 school-sdk-1.6.0/school_sdk/client/exceptions.py
+-rw-r--r--   0 farmer     (501) staff       (20)      983 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/client/utils.py
+-rw-r--r--   0 farmer     (501) staff       (20)      867 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/config.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.926360 school-sdk-1.6.0/school_sdk/session/
+-rw-r--r--   0 farmer     (501) staff       (20)      259 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/session/__init__.py
+-rw-r--r--   0 farmer     (501) staff       (20)      183 2024-04-10 10:14:03.000000 school-sdk-1.6.0/school_sdk/type.py
+-rw-r--r--   0 farmer     (501) staff       (20)      813 2023-02-25 03:25:17.000000 school-sdk-1.6.0/school_sdk/utils.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.923273 school-sdk-1.6.0/school_sdk.egg-info/
+-rw-r--r--   0 farmer     (501) staff       (20)     5065 2024-04-10 10:17:52.000000 school-sdk-1.6.0/school_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 farmer     (501) staff       (20)     1109 2024-04-10 10:17:52.000000 school-sdk-1.6.0/school_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 farmer     (501) staff       (20)        1 2024-04-10 10:17:52.000000 school-sdk-1.6.0/school_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 farmer     (501) staff       (20)        1 2023-02-25 07:34:21.000000 school-sdk-1.6.0/school_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 farmer     (501) staff       (20)       59 2024-04-10 10:17:52.000000 school-sdk-1.6.0/school_sdk.egg-info/requires.txt
+-rw-r--r--   0 farmer     (501) staff       (20)       11 2024-04-10 10:17:52.000000 school-sdk-1.6.0/school_sdk.egg-info/top_level.txt
+-rw-r--r--   0 farmer     (501) staff       (20)       38 2024-04-10 10:17:53.926834 school-sdk-1.6.0/setup.cfg
+-rw-r--r--   0 farmer     (501) staff       (20)     1462 2024-04-10 10:14:03.000000 school-sdk-1.6.0/setup.py
+drwxr-xr-x   0 farmer     (501) staff       (20)        0 2024-04-10 10:17:53.926470 school-sdk-1.6.0/test/
+-rw-r--r--   0 farmer     (501) staff       (20)     1399 2024-01-08 01:46:29.000000 school-sdk-1.6.0/test/test.py
```

### Comparing `school-sdk-1.5.0/LICENSE` & `school-sdk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/PKG-INFO` & `school-sdk-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: school-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: zf School SDK for Python
 Home-page: https://github.com/Farmer-chong/new-school-sdk
 Author: farmer.chillax
 Author-email: farmer-chong@qq.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -40,25 +40,35 @@
     <a href = "https://github.com/FarmerChillax/new-school-sdk/network/members/">
         <img alt = "forks" src = "https://badgen.net/github/forks/FarmerChillax/new-school-sdk/" />
     </a>
 <!-- </p> -->
 
 [在线文档](https://farmerChillax.github.io/new-school-sdk/)
 
+## 支持的登录/验证码方式
+- 帐号密码登录
+- 滑块验证码登录
+- 图形验证码登录
+- cookie 登录（用于扫码登录等场景）
+
+
 ## 测试环境
 - Python == 3.8 
 - 默认验证码识别方式: CPU
 
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

### Comparing `school-sdk-1.5.0/README.md` & `school-sdk-1.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,25 +21,35 @@
     <a href = "https://github.com/FarmerChillax/new-school-sdk/network/members/">
         <img alt = "forks" src = "https://badgen.net/github/forks/FarmerChillax/new-school-sdk/" />
     </a>
 <!-- </p> -->
 
 [在线文档](https://farmerChillax.github.io/new-school-sdk/)
 
+## 支持的登录/验证码方式
+- 帐号密码登录
+- 滑块验证码登录
+- 图形验证码登录
+- cookie 登录（用于扫码登录等场景）
+
+
 ## 测试环境
 - Python == 3.8 
 - 默认验证码识别方式: CPU
 
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

### Comparing `school-sdk-1.5.0/school_sdk/PyRsa/pyb64.py` & `school-sdk-1.6.0/school_sdk/PyRsa/pyb64.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/PyRsa/pyjsbn.py` & `school-sdk-1.6.0/school_sdk/PyRsa/pyjsbn.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/PyRsa/pyrng.py` & `school-sdk-1.6.0/school_sdk/PyRsa/pyrng.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/PyRsa/pyrsa.py` & `school-sdk-1.6.0/school_sdk/PyRsa/pyrsa.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/PyRsa/tools.py` & `school-sdk-1.6.0/school_sdk/PyRsa/tools.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/check_code/__init__.py` & `school-sdk-1.6.0/school_sdk/check_code/__init__.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/check_code/captcha_setting.py` & `school-sdk-1.6.0/school_sdk/check_code/captcha_setting.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/check_code/dataset.py` & `school-sdk-1.6.0/school_sdk/check_code/dataset.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/check_code/model.py` & `school-sdk-1.6.0/school_sdk/check_code/model.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/check_code/predict.py` & `school-sdk-1.6.0/school_sdk/check_code/predict.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/check_code/type.py` & `school-sdk-1.6.0/school_sdk/check_code/type.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/__init__.py` & `school-sdk-1.6.0/school_sdk/client/__init__.py`

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

### Comparing `school-sdk-1.5.0/school_sdk/client/api/__init__.py` & `school-sdk-1.6.0/school_sdk/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/api/class_schedule.py` & `school-sdk-1.6.0/school_sdk/client/api/class_schedule.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/api/login.py` & `school-sdk-1.6.0/school_sdk/client/api/login.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/api/schedule_parse.py` & `school-sdk-1.6.0/school_sdk/client/api/schedule_parse.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/api/schedules.py` & `school-sdk-1.6.0/school_sdk/client/api/schedules.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/api/score.py` & `school-sdk-1.6.0/school_sdk/client/api/score.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/api/user_info.py` & `school-sdk-1.6.0/school_sdk/client/api/user_info.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/base.py` & `school-sdk-1.6.0/school_sdk/client/base.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/exceptions.py` & `school-sdk-1.6.0/school_sdk/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/client/utils.py` & `school-sdk-1.6.0/school_sdk/client/utils.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/config.py` & `school-sdk-1.6.0/school_sdk/config.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk/utils.py` & `school-sdk-1.6.0/school_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `school-sdk-1.5.0/school_sdk.egg-info/PKG-INFO` & `school-sdk-1.6.0/school_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: school-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: zf School SDK for Python
 Home-page: https://github.com/Farmer-chong/new-school-sdk
 Author: farmer.chillax
 Author-email: farmer-chong@qq.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -40,25 +40,35 @@
     <a href = "https://github.com/FarmerChillax/new-school-sdk/network/members/">
         <img alt = "forks" src = "https://badgen.net/github/forks/FarmerChillax/new-school-sdk/" />
     </a>
 <!-- </p> -->
 
 [在线文档](https://farmerChillax.github.io/new-school-sdk/)
 
+## 支持的登录/验证码方式
+- 帐号密码登录
+- 滑块验证码登录
+- 图形验证码登录
+- cookie 登录（用于扫码登录等场景）
+
+
 ## 测试环境
 - Python == 3.8 
 - 默认验证码识别方式: CPU
 
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

### Comparing `school-sdk-1.5.0/school_sdk.egg-info/SOURCES.txt` & `school-sdk-1.6.0/school_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 school_sdk/__init__.py
 school_sdk/config.py
+school_sdk/type.py
 school_sdk/utils.py
 school_sdk.egg-info/PKG-INFO
 school_sdk.egg-info/SOURCES.txt
 school_sdk.egg-info/dependency_links.txt
 school_sdk.egg-info/not-zip-safe
 school_sdk.egg-info/requires.txt
 school_sdk.egg-info/top_level.txt
```

### Comparing `school-sdk-1.5.0/setup.py` & `school-sdk-1.6.0/setup.py`

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

### Comparing `school-sdk-1.5.0/test/test.py` & `school-sdk-1.6.0/test/test.py`

 * *Files identical despite different names*

