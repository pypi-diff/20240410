# Comparing `tmp/barkshark-sql-0.1.3.tar.gz` & `tmp/barkshark-sql-0.1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barkshark-sql-0.1.3.tar", last modified: Mon Apr  8 19:54:16 2024, max compression
+gzip compressed data, was "barkshark-sql-0.1.3.post1.tar", last modified: Wed Apr 10 16:19:22 2024, max compression
```

## Comparing `barkshark-sql-0.1.3.tar` & `barkshark-sql-0.1.3.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/
--rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-19 10:00:01.000000 barkshark-sql-0.1.3/LICENSE.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-03-10 22:34:07.000000 barkshark-sql-0.1.3/README.md
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/barkshark_sql.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      389 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-08 19:54:16.000000 barkshark-sql-0.1.3/barkshark_sql.egg-info/top_level.txt
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/bsql/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-04-08 19:32:15.000000 barkshark-sql-0.1.3/bsql/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     5365 2024-04-08 18:47:11.000000 barkshark-sql-0.1.3/bsql/backends.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    18977 2024-04-02 20:23:43.000000 barkshark-sql-0.1.3/bsql/database.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1178 2024-04-02 20:23:36.000000 barkshark-sql-0.1.3/bsql/enums.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4174 2024-04-08 18:44:46.000000 barkshark-sql-0.1.3/bsql/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-10 22:38:06.000000 barkshark-sql-0.1.3/bsql/py.typed
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7209 2024-04-02 20:23:25.000000 barkshark-sql-0.1.3/bsql/statement.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7732 2024-04-01 17:49:07.000000 barkshark-sql-0.1.3/bsql/table.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2089 2024-04-01 18:22:58.000000 barkshark-sql-0.1.3/pyproject.toml
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/setup.cfg
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-08 19:54:16.446317 barkshark-sql-0.1.3/tests/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1880 2024-04-01 18:22:11.000000 barkshark-sql-0.1.3/tests/test_statements.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)      654 2024-04-01 18:22:18.000000 barkshark-sql-0.1.3/tests/test_tables.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-19 10:00:01.000000 barkshark-sql-0.1.3.post1/LICENSE.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2220 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-03-10 22:34:07.000000 barkshark-sql-0.1.3.post1/README.md
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2220 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      389 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/top_level.txt
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/bsql/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      540 2024-04-10 16:19:14.000000 barkshark-sql-0.1.3.post1/bsql/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     5350 2024-04-10 16:13:17.000000 barkshark-sql-0.1.3.post1/bsql/backends.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    18977 2024-04-02 20:23:43.000000 barkshark-sql-0.1.3.post1/bsql/database.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1178 2024-04-02 20:23:36.000000 barkshark-sql-0.1.3.post1/bsql/enums.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4174 2024-04-08 18:44:46.000000 barkshark-sql-0.1.3.post1/bsql/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-10 22:38:06.000000 barkshark-sql-0.1.3.post1/bsql/py.typed
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7209 2024-04-02 20:23:25.000000 barkshark-sql-0.1.3.post1/bsql/statement.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7732 2024-04-01 17:49:07.000000 barkshark-sql-0.1.3.post1/bsql/table.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2089 2024-04-01 18:22:58.000000 barkshark-sql-0.1.3.post1/pyproject.toml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/tests/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1880 2024-04-01 18:22:11.000000 barkshark-sql-0.1.3.post1/tests/test_statements.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      654 2024-04-01 18:22:18.000000 barkshark-sql-0.1.3.post1/tests/test_tables.py
```

### Comparing `barkshark-sql-0.1.3/LICENSE.md` & `barkshark-sql-0.1.3.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/PKG-INFO` & `barkshark-sql-0.1.3.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-sql
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: Connection pool and query builder for dbapi 2.0 database drivers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/bsql
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/bsql/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/barkshark-sql
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/bsql
```

### Comparing `barkshark-sql-0.1.3/README.md` & `barkshark-sql-0.1.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/barkshark_sql.egg-info/PKG-INFO` & `barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-sql
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: Connection pool and query builder for dbapi 2.0 database drivers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/bsql
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/bsql/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/barkshark-sql
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/bsql
```

### Comparing `barkshark-sql-0.1.3/bsql/__init__.py` & `barkshark-sql-0.1.3.post1/bsql/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __software__ = "Barkshark SQL"
-__version__ = "0.1.3"
+__version__ = "0.1.3-1"
 __author__ = "Zoey Mae"
 __homepage__ = "https://git.barkshark.xyz/barkshark/bsql"
 
 from .backends import Backend, PG8000, Sqlite3
 from .database import Connection, Cursor, Database
 from .enums import BackendType, Comparison, OrderDirection, StrEnum
 from .table import Tables, Table, Column
```

### Comparing `barkshark-sql-0.1.3/bsql/backends.py` & `barkshark-sql-0.1.3.post1/bsql/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,20 @@
 
 	def __init__(self) -> None:
 		self.module.register_adapter(datetime, lambda v: v.timestamp())
 		self.module.register_adapter(dict, json.dumps)
 		self.module.register_adapter(list, json.dumps)
 		self.module.register_adapter(tuple, json.dumps)
 		self.module.register_adapter(set, json.dumps)
-		self.module.register_adapter(bool, lambda v: boolean(v.decode("utf-8")))
+		self.module.register_adapter(bool, lambda v: 1 if v else 0)
 
 		self.module.register_converter("timestamp", Sqlite3.deserialize_timestamp)
 		self.module.register_converter("datetime", Sqlite3.deserialize_timestamp)
 		self.module.register_converter("json", json.loads)
-		self.module.register_converter("boolean", lambda v: True if v == b"1" else False)
+		self.module.register_converter("boolean", lambda v: boolean(v.decode("utf-8")))
 		self.module.register_converter("real", float)
 		self.module.register_converter("integer", int)
 
 	@staticmethod
 	def deserialize_timestamp(raw_value: bytes) -> datetime:
 		"""
 			Method used to serialize ``TIMESTMAP`` and ``DATETIME`` column values.
```

### Comparing `barkshark-sql-0.1.3/bsql/database.py` & `barkshark-sql-0.1.3.post1/bsql/database.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/bsql/enums.py` & `barkshark-sql-0.1.3.post1/bsql/enums.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/bsql/misc.py` & `barkshark-sql-0.1.3.post1/bsql/misc.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/bsql/statement.py` & `barkshark-sql-0.1.3.post1/bsql/statement.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/bsql/table.py` & `barkshark-sql-0.1.3.post1/bsql/table.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/pyproject.toml` & `barkshark-sql-0.1.3.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/tests/test_statements.py` & `barkshark-sql-0.1.3.post1/tests/test_statements.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3/tests/test_tables.py` & `barkshark-sql-0.1.3.post1/tests/test_tables.py`

 * *Files identical despite different names*

