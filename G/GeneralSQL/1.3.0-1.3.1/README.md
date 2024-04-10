# Comparing `tmp/GeneralSQL-1.3.0.tar.gz` & `tmp/GeneralSQL-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeneralSQL-1.3.0.tar", last modified: Wed Apr 10 10:06:08 2024, max compression
+gzip compressed data, was "GeneralSQL-1.3.1.tar", last modified: Wed Apr 10 10:19:55 2024, max compression
```

## Comparing `GeneralSQL-1.3.0.tar` & `GeneralSQL-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.117930 GeneralSQL-1.3.0/GeneralSQL/
--rw-r--r--   0 joker     (1000) joker     (1000)     2321 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/Error.py
--rw-r--r--   0 joker     (1000) joker     (1000)    35149 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/LICENSE
--rw-r--r--   0 joker     (1000) joker     (1000)     1368 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/README.md
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/GeneralSQL/Template/
--rw-r--r--   0 joker     (1000) joker     (1000)     1431 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/Template/__init__.py
--rw-r--r--   0 joker     (1000) joker     (1000)     2994 2024-04-10 09:59:53.000000 GeneralSQL-1.3.0/GeneralSQL/Template/base.py
--rw-r--r--   0 joker     (1000) joker     (1000)     2119 2024-04-10 09:50:57.000000 GeneralSQL-1.3.0/GeneralSQL/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/GeneralSQL/db/
--rw-r--r--   0 joker     (1000) joker     (1000)    16294 2024-04-10 10:04:52.000000 GeneralSQL-1.3.0/GeneralSQL/db/Jmysql.py
--rw-r--r--   0 joker     (1000) joker     (1000)       57 2023-11-19 09:55:51.000000 GeneralSQL-1.3.0/GeneralSQL/db/__init__.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/GeneralSQL.egg-info/
--rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)      347 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/SOURCES.txt
--rw-r--r--   0 joker     (1000) joker     (1000)        1 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/dependency_links.txt
--rw-r--r--   0 joker     (1000) joker     (1000)       11 2024-04-10 10:06:08.000000 GeneralSQL-1.3.0/GeneralSQL.egg-info/top_level.txt
--rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/PKG-INFO
--rwxrwxrwx   0 joker     (1000) joker     (1000)      717 2023-12-25 09:51:11.000000 GeneralSQL-1.3.0/pyproject.toml
--rw-r--r--   0 joker     (1000) joker     (1000)       38 2024-04-10 10:06:08.121930 GeneralSQL-1.3.0/setup.cfg
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:19:55.626594 GeneralSQL-1.3.1/
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:19:55.622594 GeneralSQL-1.3.1/GeneralSQL/
+-rw-r--r--   0 joker     (1000) joker     (1000)     2321 2023-11-19 09:55:51.000000 GeneralSQL-1.3.1/GeneralSQL/Error.py
+-rw-r--r--   0 joker     (1000) joker     (1000)    35149 2023-11-19 09:55:51.000000 GeneralSQL-1.3.1/GeneralSQL/LICENSE
+-rw-r--r--   0 joker     (1000) joker     (1000)     1368 2023-11-19 09:55:51.000000 GeneralSQL-1.3.1/GeneralSQL/README.md
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:19:55.622594 GeneralSQL-1.3.1/GeneralSQL/Template/
+-rw-r--r--   0 joker     (1000) joker     (1000)     1431 2023-11-19 09:55:51.000000 GeneralSQL-1.3.1/GeneralSQL/Template/__init__.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     2994 2024-04-10 09:59:53.000000 GeneralSQL-1.3.1/GeneralSQL/Template/base.py
+-rw-r--r--   0 joker     (1000) joker     (1000)     2119 2024-04-10 10:19:42.000000 GeneralSQL-1.3.1/GeneralSQL/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:19:55.622594 GeneralSQL-1.3.1/GeneralSQL/db/
+-rw-r--r--   0 joker     (1000) joker     (1000)    16289 2024-04-10 10:17:20.000000 GeneralSQL-1.3.1/GeneralSQL/db/Jmysql.py
+-rw-r--r--   0 joker     (1000) joker     (1000)       57 2023-11-19 09:55:51.000000 GeneralSQL-1.3.1/GeneralSQL/db/__init__.py
+drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2024-04-10 10:19:55.622594 GeneralSQL-1.3.1/GeneralSQL.egg-info/
+-rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-04-10 10:19:55.000000 GeneralSQL-1.3.1/GeneralSQL.egg-info/PKG-INFO
+-rw-r--r--   0 joker     (1000) joker     (1000)      347 2024-04-10 10:19:55.000000 GeneralSQL-1.3.1/GeneralSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)        1 2024-04-10 10:19:55.000000 GeneralSQL-1.3.1/GeneralSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)       11 2024-04-10 10:19:55.000000 GeneralSQL-1.3.1/GeneralSQL.egg-info/top_level.txt
+-rw-r--r--   0 joker     (1000) joker     (1000)    42412 2024-04-10 10:19:55.626594 GeneralSQL-1.3.1/PKG-INFO
+-rwxrwxrwx   0 joker     (1000) joker     (1000)      717 2023-12-25 09:51:11.000000 GeneralSQL-1.3.1/pyproject.toml
+-rw-r--r--   0 joker     (1000) joker     (1000)       38 2024-04-10 10:19:55.626594 GeneralSQL-1.3.1/setup.cfg
```

### Comparing `GeneralSQL-1.3.0/GeneralSQL/Error.py` & `GeneralSQL-1.3.1/GeneralSQL/Error.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.3.0/GeneralSQL/LICENSE` & `GeneralSQL-1.3.1/GeneralSQL/LICENSE`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.3.0/GeneralSQL/README.md` & `GeneralSQL-1.3.1/GeneralSQL/README.md`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.3.0/GeneralSQL/Template/__init__.py` & `GeneralSQL-1.3.1/GeneralSQL/Template/__init__.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.3.0/GeneralSQL/Template/base.py` & `GeneralSQL-1.3.1/GeneralSQL/Template/base.py`

 * *Files identical despite different names*

### Comparing `GeneralSQL-1.3.0/GeneralSQL/__init__.py` & `GeneralSQL-1.3.1/GeneralSQL/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import functools
 from . import db
 
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 __cls__ = db.__all__
 
 
 def SeniorDB(t):
     if t in __cls__:
         __db = getattr(db, t).DB
```

### Comparing `GeneralSQL-1.3.0/GeneralSQL/db/Jmysql.py` & `GeneralSQL-1.3.1/GeneralSQL/db/Jmysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,15 @@
     # factor = filter_data.get('factor', None)
     # if factor and factor.upper() not in factor_list: raise Error.ParamsError(400004)
     # if factor:
     #     factor = factor.upper()
     #     result += factor
     # 表 as 名称替换 field
     if filter_data.get('table_as'):
-        field = f"{filter_data.get('table_as')}.{repr(field)}"
-
+        field = f"{filter_data.get('table_as')}.`{field}`"
 
     # 自定义 value 处理
     if filter_data.get('val_format'):
         val = filter_data.get('val_format')(val)
     else:
         # 默认 value 处理
         if isinstance(val, (dict)) and val.get('start') and val.get('end'):
```

### Comparing `GeneralSQL-1.3.0/GeneralSQL.egg-info/PKG-INFO` & `GeneralSQL-1.3.1/GeneralSQL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeneralSQL
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sql generator tool.
 Author-email: joker-zzp <joker_zzp@qq.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `GeneralSQL-1.3.0/PKG-INFO` & `GeneralSQL-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeneralSQL
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sql generator tool.
 Author-email: joker-zzp <joker_zzp@qq.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `GeneralSQL-1.3.0/pyproject.toml` & `GeneralSQL-1.3.1/pyproject.toml`

 * *Files identical despite different names*

