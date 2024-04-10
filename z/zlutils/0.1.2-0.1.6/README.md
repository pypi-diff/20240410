# Comparing `tmp/zlutils-0.1.2.tar.gz` & `tmp/zlutils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlutils-0.1.2.tar", last modified: Fri Mar 29 15:16:16 2024, max compression
+gzip compressed data, was "zlutils-0.1.6.tar", last modified: Wed Apr 10 18:19:19 2024, max compression
```

## Comparing `zlutils-0.1.2.tar` & `zlutils-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-03-29 15:16:16.796159 zlutils-0.1.2/
--rw-r--r--   0 zlols     (1000) zlols     (1000)      367 2024-03-29 15:16:16.796159 zlutils-0.1.2/PKG-INFO
--rw-r--r--   0 zlols     (1000) zlols     (1000)        2 2024-03-20 17:14:30.000000 zlutils-0.1.2/README.md
--rw-r--r--   0 zlols     (1000) zlols     (1000)       38 2024-03-29 15:16:16.796159 zlutils-0.1.2/setup.cfg
--rw-r--r--   0 zlols     (1000) zlols     (1000)      599 2024-03-29 14:58:45.000000 zlutils-0.1.2/setup.py
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-03-29 15:16:16.795159 zlutils-0.1.2/zlutils/
--rw-r--r--   0 zlols     (1000) zlols     (1000)       23 2024-03-29 14:58:26.000000 zlutils-0.1.2/zlutils/__init__.py
--rw-r--r--   0 zlols     (1000) zlols     (1000)     5141 2024-03-22 11:36:15.000000 zlutils-0.1.2/zlutils/shared.py
-drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-03-29 15:16:16.795159 zlutils-0.1.2/zlutils.egg-info/
--rw-r--r--   0 zlols     (1000) zlols     (1000)      367 2024-03-29 15:16:16.000000 zlutils-0.1.2/zlutils.egg-info/PKG-INFO
--rw-r--r--   0 zlols     (1000) zlols     (1000)      180 2024-03-29 15:16:16.000000 zlutils-0.1.2/zlutils.egg-info/SOURCES.txt
--rw-r--r--   0 zlols     (1000) zlols     (1000)        1 2024-03-29 15:16:16.000000 zlutils-0.1.2/zlutils.egg-info/dependency_links.txt
--rw-r--r--   0 zlols     (1000) zlols     (1000)        8 2024-03-29 15:16:16.000000 zlutils-0.1.2/zlutils.egg-info/top_level.txt
+drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:19:19.739838 zlutils-0.1.6/
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      367 2024-04-10 18:19:19.739838 zlutils-0.1.6/PKG-INFO
+-rw-r--r--   0 zlols     (1000) zlols     (1000)        2 2024-03-20 17:14:30.000000 zlutils-0.1.6/README.md
+-rw-r--r--   0 zlols     (1000) zlols     (1000)       38 2024-04-10 18:19:19.739838 zlutils-0.1.6/setup.cfg
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      599 2024-04-10 14:52:27.000000 zlutils-0.1.6/setup.py
+drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:19:19.739838 zlutils-0.1.6/zlutils/
+-rw-r--r--   0 zlols     (1000) zlols     (1000)       46 2024-04-10 10:31:55.000000 zlutils-0.1.6/zlutils/__init__.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     1897 2024-04-10 15:07:09.000000 zlutils-0.1.6/zlutils/const.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     1119 2024-04-10 15:09:05.000000 zlutils-0.1.6/zlutils/event.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)     5258 2024-03-30 03:58:57.000000 zlutils-0.1.6/zlutils/shared.py
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      371 2024-03-31 05:47:19.000000 zlutils-0.1.6/zlutils/wrapper.py
+drwxr-xr-x   0 zlols     (1000) zlols     (1000)        0 2024-04-10 18:19:19.739838 zlutils-0.1.6/zlutils.egg-info/
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      367 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/PKG-INFO
+-rw-r--r--   0 zlols     (1000) zlols     (1000)      233 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/SOURCES.txt
+-rw-r--r--   0 zlols     (1000) zlols     (1000)        1 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/dependency_links.txt
+-rw-r--r--   0 zlols     (1000) zlols     (1000)        8 2024-04-10 18:19:19.000000 zlutils-0.1.6/zlutils.egg-info/top_level.txt
```

### Comparing `zlutils-0.1.2/setup.py` & `zlutils-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 discription = "a package of utils"
 
 setuptools.setup(
   name="zlutils",
-  version='0.1.2',
+  version='0.1.6',
   python_requires=">=3.6",
   author="zlols",
   author_email="zlols@foxmail.com",
   description=discription,
   long_description=discription,
   long_description_content_type="text/markdown",
   url="https://github.com/zlolss/zlutils.py.git",
```

### Comparing `zlutils-0.1.2/zlutils/shared.py` & `zlutils-0.1.6/zlutils/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 '''
 v0.1 2024-03-22
+# 共享列表在linux,py310环境下有bug,当创建者断开时丢失
 '''
 
 import logging, time
 日志 = logging.getLogger()
 
 _默认字符串编码 = 'utf-8'
 _允许的数据类型 = [int, float, str]
@@ -39,15 +40,16 @@
         类变量_元类 = vars(元类)
         变量名列表_元类 = [变量名 for 变量名 in 类变量_元类 if (type(类变量_元类[变量名]) in _允许的数据类型)and(变量名[:1]!='_')]
         变量名列表_合成 = 变量名列表 + 变量名列表_元类
         from multiprocessing import shared_memory
         try:
             共享列表 = shared_memory.ShareableList( name=共享列表名 )
             日志.info("载入共享列表, 覆盖默认值")
-        except:
+        except Exception as e:
+            日志.warning(e)
             值列表 = [ 类变量[变量名] for 变量名 in 变量名列表 ]
             值列表_元类 = [类变量_元类[变量名] for 变量名 in 变量名列表_元类]
             值列表_合成 = 值列表+值列表_元类
             共享列表 = shared_memory.ShareableList( sequence = 值列表_合成, name=共享列表名 )
             日志.info("以默认值创建共享列表")
         类变量[f'_{类名}___共享列表'] = 共享列表
         for 索引值, 变量名 in enumerate(变量名列表_合成):
```

