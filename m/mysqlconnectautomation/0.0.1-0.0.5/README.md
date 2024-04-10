# Comparing `tmp/mysqlconnectautomation-0.0.1.tar.gz` & `tmp/mysqlconnectautomation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlconnectautomation-0.0.1.tar", last modified: Fri Mar 29 12:10:05 2024, max compression
+gzip compressed data, was "mysqlconnectautomation-0.0.5.tar", last modified: Wed Apr 10 08:48:41 2024, max compression
```

## Comparing `mysqlconnectautomation-0.0.1.tar` & `mysqlconnectautomation-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:10:05.630920 mysqlconnectautomation-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-29 12:09:36.000000 mysqlconnectautomation-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-29 12:10:05.630920 mysqlconnectautomation-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-29 12:09:36.000000 mysqlconnectautomation-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-29 12:09:36.000000 mysqlconnectautomation-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-29 12:10:05.630920 mysqlconnectautomation-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-29 12:09:36.000000 mysqlconnectautomation-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:10:05.626920 mysqlconnectautomation-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:10:05.626920 mysqlconnectautomation-0.0.1/src/mysql_connect_automation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:09:36.000000 mysqlconnectautomation-0.0.1/src/mysql_connect_automation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-29 12:09:36.000000 mysqlconnectautomation-0.0.1/src/mysql_connect_automation/mysql_crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:10:05.626920 mysqlconnectautomation-0.0.1/src/mysqlconnectautomation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-29 12:10:05.000000 mysqlconnectautomation-0.0.1/src/mysqlconnectautomation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-29 12:10:05.000000 mysqlconnectautomation-0.0.1/src/mysqlconnectautomation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:10:05.000000 mysqlconnectautomation-0.0.1/src/mysqlconnectautomation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-29 12:10:05.000000 mysqlconnectautomation-0.0.1/src/mysqlconnectautomation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-29 12:10:05.000000 mysqlconnectautomation-0.0.1/src/mysqlconnectautomation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:41.173581 mysqlconnectautomation-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 08:48:15.000000 mysqlconnectautomation-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-10 08:48:41.173581 mysqlconnectautomation-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 08:48:15.000000 mysqlconnectautomation-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 08:48:15.000000 mysqlconnectautomation-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-10 08:48:41.177582 mysqlconnectautomation-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-10 08:48:15.000000 mysqlconnectautomation-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:41.173581 mysqlconnectautomation-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:41.173581 mysqlconnectautomation-0.0.5/src/mysql_connect_automation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:15.000000 mysqlconnectautomation-0.0.5/src/mysql_connect_automation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-10 08:48:15.000000 mysqlconnectautomation-0.0.5/src/mysql_connect_automation/mysql_crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:48:41.173581 mysqlconnectautomation-0.0.5/src/mysqlconnectautomation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-10 08:48:41.000000 mysqlconnectautomation-0.0.5/src/mysqlconnectautomation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 08:48:41.000000 mysqlconnectautomation-0.0.5/src/mysqlconnectautomation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:48:41.000000 mysqlconnectautomation-0.0.5/src/mysqlconnectautomation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 08:48:41.000000 mysqlconnectautomation-0.0.5/src/mysqlconnectautomation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 08:48:41.000000 mysqlconnectautomation-0.0.5/src/mysqlconnectautomation.egg-info/top_level.txt
```

### Comparing `mysqlconnectautomation-0.0.1/LICENSE` & `mysqlconnectautomation-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlconnectautomation-0.0.1/PKG-INFO` & `mysqlconnectautomation-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlconnectautomation
-Version: 0.0.1
+Version: 0.0.5
 Summary: A python package for connecting with database.
 Home-page: https://github.com/sujeetkumae132/mysqlconnect
 Author: sujeetkumae132
 Author-email: kumar.sujeet132@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sujeetkumae132/mysqlconnect/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mysqlconnectautomation-0.0.1/setup.py` & `mysqlconnectautomation-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from typing import List
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()     
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.5"
 REPO_NAME = "mysqlconnect"
 PKG_NAME= "mysqlconnectautomation"
 AUTHOR_USER_NAME = "sujeetkumae132"
 AUTHOR_EMAIL = "kumar.sujeet132@gmail.com"
 
 setup(
     name=PKG_NAME,
```

### Comparing `mysqlconnectautomation-0.0.1/src/mysql_connect_automation/mysql_crud.py` & `mysqlconnectautomation-0.0.5/src/mysql_connect_automation/mysql_crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         # Create a Secrets Manager client
         session = boto3.session.Session(aws_access_key_id=self.aws_access_key_id_o,
         aws_secret_access_key=self.aws_secret_access_key_o,region_name=self.region_name_o)
         client = session.client(service_name="secretsmanager", region_name=self.region_name_o)
         return client.get_secret_value(SecretId=self.secret_name_o)["SecretString"]
 
     def create_engine_conn(self):
-        dbname=self.db_name
+        dbname=self.db_name_o
         secret_value = self.get_secret()
         if secret_value:
             secret_data = json.loads(secret_value)
             rds_user = secret_data["username"]
             rds_pass = secret_data["password"]
             rds_host = secret_data["host"]
             rds_port = secret_data["port"]
```

### Comparing `mysqlconnectautomation-0.0.1/src/mysqlconnectautomation.egg-info/PKG-INFO` & `mysqlconnectautomation-0.0.5/src/mysqlconnectautomation.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlconnectautomation
-Version: 0.0.1
+Version: 0.0.5
 Summary: A python package for connecting with database.
 Home-page: https://github.com/sujeetkumae132/mysqlconnect
 Author: sujeetkumae132
 Author-email: kumar.sujeet132@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sujeetkumae132/mysqlconnect/issues
 Classifier: Programming Language :: Python :: 3.8
```

