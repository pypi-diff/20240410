# Comparing `tmp/weedata-0.2.1.tar.gz` & `tmp/weedata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weedata-0.2.1.tar", last modified: Sat Mar  9 17:57:02 2024, max compression
+gzip compressed data, was "weedata-0.2.2.tar", last modified: Wed Apr 10 00:19:45 2024, max compression
```

## Comparing `weedata-0.2.1.tar` & `weedata-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 17:57:02.184431 weedata-0.2.1/
--rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    18735 2024-03-09 17:57:02.181431 weedata-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    15769 2024-03-09 14:54:16.000000 weedata-0.2.1/README.md
--rw-rw-rw-   0        0        0     1417 2024-03-09 17:51:32.000000 weedata-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-09 17:57:02.185431 weedata-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-09 17:57:02.074432 weedata-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-09 17:57:02.121431 weedata-0.2.1/src/weedata/
--rw-rw-rw-   0        0        0      497 2024-03-09 02:13:09.000000 weedata-0.2.1/src/weedata/__init__.py
--rw-rw-rw-   0        0        0    31670 2024-03-09 17:55:21.000000 weedata-0.2.1/src/weedata/client.py
--rw-rw-rw-   0        0        0    15138 2024-03-09 14:24:49.000000 weedata-0.2.1/src/weedata/fields.py
--rw-rw-rw-   0        0        0     9591 2024-03-09 14:46:27.000000 weedata-0.2.1/src/weedata/model.py
--rw-rw-rw-   0        0        0     8012 2024-02-27 13:14:36.000000 weedata-0.2.1/src/weedata/queries.py
-drwxrwxrwx   0        0        0        0 2024-03-09 17:57:02.178431 weedata-0.2.1/src/weedata.egg-info/
--rw-rw-rw-   0        0        0    18735 2024-03-09 17:57:02.000000 weedata-0.2.1/src/weedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-03-09 17:57:02.000000 weedata-0.2.1/src/weedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 17:57:02.000000 weedata-0.2.1/src/weedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-09 17:57:02.000000 weedata-0.2.1/src/weedata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-09 17:57:02.172431 weedata-0.2.1/tests/
--rw-rw-rw-   0        0        0     4294 2024-02-24 10:32:47.000000 weedata-0.2.1/tests/test_base.py
--rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.1/tests/test_connection.py
--rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.1/tests/test_delete.py
--rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.1/tests/test_fields.py
--rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.1/tests/test_queries.py
--rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.1/tests/test_save.py
--rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.1/tests/test_update.py
+drwxrwxrwx   0        0        0        0 2024-04-10 00:19:45.114628 weedata-0.2.2/
+-rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    18951 2024-04-10 00:19:45.111628 weedata-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15977 2024-04-10 00:18:06.000000 weedata-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1417 2024-04-10 00:15:00.000000 weedata-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 00:19:45.115628 weedata-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 00:19:44.901607 weedata-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 00:19:44.962619 weedata-0.2.2/src/weedata/
+-rw-rw-rw-   0        0        0      497 2024-03-09 02:13:09.000000 weedata-0.2.2/src/weedata/__init__.py
+-rw-rw-rw-   0        0        0    31685 2024-03-25 21:24:11.000000 weedata-0.2.2/src/weedata/client.py
+-rw-rw-rw-   0        0        0    15497 2024-03-23 21:38:50.000000 weedata-0.2.2/src/weedata/fields.py
+-rw-rw-rw-   0        0        0     9591 2024-03-09 14:46:27.000000 weedata-0.2.2/src/weedata/model.py
+-rw-rw-rw-   0        0        0     8012 2024-02-27 13:14:36.000000 weedata-0.2.2/src/weedata/queries.py
+drwxrwxrwx   0        0        0        0 2024-04-10 00:19:45.106628 weedata-0.2.2/src/weedata.egg-info/
+-rw-rw-rw-   0        0        0    18951 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 00:19:44.000000 weedata-0.2.2/src/weedata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 00:19:45.085628 weedata-0.2.2/tests/
+-rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.2/tests/test_base.py
+-rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.2/tests/test_connection.py
+-rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.2/tests/test_delete.py
+-rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.2/tests/test_fields.py
+-rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.2/tests/test_queries.py
+-rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.2/tests/test_save.py
+-rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.2/tests/test_update.py
```

### Comparing `weedata-0.2.1/LICENSE` & `weedata-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/PKG-INFO` & `weedata-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.1
+Version: 0.2.2
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -132,14 +132,17 @@
 
 > **Important Notice:**
 > Redis functions as an in-memory database. Although it includes disk persistence capabilities, this feature does not ensure 100% data integrity and presents a potential risk of data loss. Prior to implementing Redis as a storage database, it is crucial to grasp pertinent knowledge and configure it appropriately, including enabling RDB (Redis Database) or AOF (Append Only File) functionality.
 For example, you can add two lines in redis.conf:
 ```
 appendonly yes
 appendfsync always
+or
+appendonly yes
+appendfsync everysec
 ```
 
 
 ### PickleDbClient
 weedata also provides a simple database implementation PickleDbClient using Python's pickle library, which can be used for testing purposes and in applications with limited resources and low data integrity requirements.   
 The parameter "dbName" is the filename of pickle file, if set to ":memory:", an in-memory database is created.  
 ```python
@@ -476,14 +479,19 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.2
+1. Delays connecting to the pymongo database until the first operation.   
+2. The default Index property of TextField/BlobField/JSONField is set to False.   
+
+
 * v0.2.1
 1. Set index=False will exclude the field from indexes in datastore
 2. Bugfix: datastore update query removes the fields unmodified
 
 
 * v0.2.0
 1. Supports Redis
```

### Comparing `weedata-0.2.1/README.md` & `weedata-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
 > **Important Notice:**
 > Redis functions as an in-memory database. Although it includes disk persistence capabilities, this feature does not ensure 100% data integrity and presents a potential risk of data loss. Prior to implementing Redis as a storage database, it is crucial to grasp pertinent knowledge and configure it appropriately, including enabling RDB (Redis Database) or AOF (Append Only File) functionality.
 For example, you can add two lines in redis.conf:
 ```
 appendonly yes
 appendfsync always
+or
+appendonly yes
+appendfsync everysec
 ```
 
 
 ### PickleDbClient
 weedata also provides a simple database implementation PickleDbClient using Python's pickle library, which can be used for testing purposes and in applications with limited resources and low data integrity requirements.   
 The parameter "dbName" is the filename of pickle file, if set to ":memory:", an in-memory database is created.  
 ```python
@@ -426,14 +429,19 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.2
+1. Delays connecting to the pymongo database until the first operation.   
+2. The default Index property of TextField/BlobField/JSONField is set to False.   
+
+
 * v0.2.1
 1. Set index=False will exclude the field from indexes in datastore
 2. Bugfix: datastore update query removes the fields unmodified
 
 
 * v0.2.0
 1. Supports Redis
```

### Comparing `weedata-0.2.1/pyproject.toml` & `weedata-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "weedata"
-version = "0.2.1"
+version = "0.2.2"
 description = "an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 keywords = ["peewee", "ORM", "ODM", "google cloud datastore", "MongoDB", "redis"]
 dependencies = [
 #  "google-cloud-datastore",
```

### Comparing `weedata-0.2.1/src/weedata/client.py` & `weedata-0.2.2/src/weedata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     def close(self):
         self.client.close()
 
 class MongoDbClient(NosqlClient):
     def __init__(self, project, dbUrl='mongodb://127.0.0.1:27017/'):
         self.project = project
         self.dbUrl = dbUrl
-        self.client = pymongo.MongoClient(self.dbUrl)
+        self.client = pymongo.MongoClient(self.dbUrl, connect=False)
         self._db = self.client[project]
     
     @classmethod
     def db_id_name(cls):
         return "_id"
 
     def insert_one(self, klass, data: dict):
```

### Comparing `weedata-0.2.1/src/weedata/fields.py` & `weedata-0.2.2/src/weedata/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -339,19 +339,27 @@
             return value
     def python_value(self, value):
         if self.bytes_store:
             return value.decode('utf-8') if isinstance(value, bytes) else value
         else:
             return value
 
-TextField = CharField
 FixedCharField = CharField
 UUIDField = CharField
 
+class TextField(CharField):
+    def __init__(self, **kwargs):
+        kwargs.setdefault('index', False)
+        super().__init__(*kwargs)
+
 class BlobField(Field):
+    def __init__(self, **kwargs):
+        kwargs.setdefault('index', False)
+        super().__init__(*kwargs)
+        
     def check_type(self, value):
         return isinstance(value, bytes)
     def db_value(self, value):
         return value
     def python_value(self, value):
         return value
 
@@ -375,14 +383,18 @@
             else:
                 value = value.decode('utf-8') if isinstance(value, bytes)  else value
                 return datetime.datetime.fromisoformat(value)
         else:
             return value
 
 class JSONField(Field):
+    def __init__(self, **kwargs):
+        kwargs.setdefault('index', False)
+        super().__init__(*kwargs)
+
     def check_type(self, value):
         json_types = [type(None), bool, int, float, str, list, dict, tuple]
         return any(isinstance(value, json_type) for json_type in json_types)
     def db_value(self, value):
         if self.bytes_store:
             return json.dumps(value).encode('utf-8')
         else:
```

### Comparing `weedata-0.2.1/src/weedata/model.py` & `weedata-0.2.2/src/weedata/model.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/src/weedata/queries.py` & `weedata-0.2.2/src/weedata/queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/src/weedata.egg-info/PKG-INFO` & `weedata-0.2.2/src/weedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.1
+Version: 0.2.2
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -132,14 +132,17 @@
 
 > **Important Notice:**
 > Redis functions as an in-memory database. Although it includes disk persistence capabilities, this feature does not ensure 100% data integrity and presents a potential risk of data loss. Prior to implementing Redis as a storage database, it is crucial to grasp pertinent knowledge and configure it appropriately, including enabling RDB (Redis Database) or AOF (Append Only File) functionality.
 For example, you can add two lines in redis.conf:
 ```
 appendonly yes
 appendfsync always
+or
+appendonly yes
+appendfsync everysec
 ```
 
 
 ### PickleDbClient
 weedata also provides a simple database implementation PickleDbClient using Python's pickle library, which can be used for testing purposes and in applications with limited resources and low data integrity requirements.   
 The parameter "dbName" is the filename of pickle file, if set to ":memory:", an in-memory database is created.  
 ```python
@@ -476,14 +479,19 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.2
+1. Delays connecting to the pymongo database until the first operation.   
+2. The default Index property of TextField/BlobField/JSONField is set to False.   
+
+
 * v0.2.1
 1. Set index=False will exclude the field from indexes in datastore
 2. Bugfix: datastore update query removes the fields unmodified
 
 
 * v0.2.0
 1. Supports Redis
```

### Comparing `weedata-0.2.1/tests/test_base.py` & `weedata-0.2.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/tests/test_connection.py` & `weedata-0.2.2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/tests/test_delete.py` & `weedata-0.2.2/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/tests/test_fields.py` & `weedata-0.2.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/tests/test_queries.py` & `weedata-0.2.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/tests/test_save.py` & `weedata-0.2.2/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.1/tests/test_update.py` & `weedata-0.2.2/tests/test_update.py`

 * *Files identical despite different names*

