# Comparing `tmp/pysquril-0.6.0.tar.gz` & `tmp/pysquril-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysquril-0.6.0.tar", max compression
+gzip compressed data, was "pysquril-0.6.2.tar", max compression
```

## Comparing `pysquril-0.6.0.tar` & `pysquril-0.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      179 2024-03-22 12:45:15.860114 pysquril-0.6.0/README.md
--rw-r--r--   0        0        0      539 2024-03-22 12:45:15.860114 pysquril-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 12:45:15.860114 pysquril-0.6.0/pysquril/__init__.py
--rw-r--r--   0        0        0    33941 2024-03-22 12:45:15.860114 pysquril-0.6.0/pysquril/backends.py
--rw-r--r--   0        0        0      412 2024-03-22 12:45:15.860114 pysquril-0.6.0/pysquril/exc.py
--rw-r--r--   0        0        0    24631 2024-03-22 12:45:15.860114 pysquril-0.6.0/pysquril/generator.py
--rw-r--r--   0        0        0    14457 2024-03-22 12:45:15.860114 pysquril-0.6.0/pysquril/parser.py
--rw-r--r--   0        0        0     2482 2024-03-22 12:45:15.860114 pysquril-0.6.0/pysquril/test_data.py
--rw-r--r--   0        0        0    33598 2024-03-22 12:45:15.860114 pysquril-0.6.0/pysquril/tests.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 pysquril-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      179 2024-04-10 11:04:36.758264 pysquril-0.6.2/README.md
+-rw-r--r--   0        0        0      539 2024-04-10 11:04:36.758264 pysquril-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/__init__.py
+-rw-r--r--   0        0        0    34186 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/backends.py
+-rw-r--r--   0        0        0      412 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/exc.py
+-rw-r--r--   0        0        0    24631 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/generator.py
+-rw-r--r--   0        0        0    14457 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/parser.py
+-rw-r--r--   0        0        0     2482 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/test_data.py
+-rw-r--r--   0        0        0    33976 2024-04-10 11:04:36.758264 pysquril-0.6.2/pysquril/tests.py
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 pysquril-0.6.2/PKG-INFO
```

### Comparing `pysquril-0.6.0/pyproject.toml` & `pysquril-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysquril"
-version = "0.6.0"
+version = "0.6.2"
 description = "Python implementation of structured URI query language"
 readme = "README.md"
 repository = "https://github.com/unioslo/pysquril"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
     "Eirik Haatveit <haatveit@uio.no>",
 ]
```

### Comparing `pysquril-0.6.0/pysquril/backends.py` & `pysquril-0.6.2/pysquril/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         # fetch the desired state
         if "order" in query_parts:
             uri_query = uri_query.split("&order")[0]
         uri_query = f"{uri_query}&order=timestamp.asc" # sorted from old to new
         target_data = list(self.table_select(f"{table_name}_audit", uri_query))
         if not target_data:
             return work_done # nothing to do
-        tsc = AuditTransaction(self.requestor, message)
+        tsc = AuditTransaction(self.requestor, message, self.requestor_name)
         session_func = self._session_func()
         try:
             # ensure the table exists, may have been deleted
             with session_func(self.engine) as session:
                 self.table_create(table_name, session)
         except psycopg2.errors.DuplicateObject as e:
             pass # already exists
@@ -497,15 +497,15 @@
         Delete the intended data from the table if a uri_query
         is present, otherwise drop the table. All deletions
         are recorded in the audit log.
 
         """
         audit_data = []
         sql = self.generator_class(f'{self._fqtn(table_name)}', uri_query)
-        tsc = AuditTransaction(self.requestor, sql.message)
+        tsc = AuditTransaction(self.requestor, sql.message, self.requestor_name)
         for row in self.table_select(table_name, uri_query):
             audit_data.append(tsc.event_delete(diff=None, previous=row, query=uri_query))
         with self._session_func()(self.engine) as session:
             session.execute(sql.delete_query)
             if not table_name.endswith("_audit"):
                 self.table_create(f'{table_name}_audit', session)
                 self.table_insert(f'{table_name}_audit', audit_data, session)
@@ -523,15 +523,15 @@
     ) -> bool:
         """
         Update one or more keys, recording changes in the audit log.
 
         """
         audit_data = []
         sql = self.generator_class(f'{self._fqtn(table_name)}', uri_query, data=data)
-        tsc = AuditTransaction(self.requestor, sql.message) if not tsc else tsc
+        tsc = AuditTransaction(self.requestor, sql.message, self.requestor_name) if not tsc else tsc
         for val in self.table_select(table_name, uri_query, data=data):
             audit_data.append(tsc.event_update(diff=data, previous=val, query=uri_query))
         if session:
             session.execute(sql.update_query)
             self.table_insert(f'{table_name}_audit', audit_data, session)
         else:
             with self._session_func()(self.engine) as session:
@@ -610,21 +610,23 @@
         self,
         engine: sqlite3.Connection,
         verbose: bool = False,
         schema: str = None,
         requestor: str = None,
         backup_days: Optional[int] = None,
         schema_pattern: Optional[str] = None,
+        requestor_name: Optional[str] = None,
     ) -> None:
         self.engine = engine
         self.verbose = verbose
         self.table_definition = '(data json unique not null)'
         self.schema = schema if schema else ""
         self.sep = "_" if self.schema else ""
         self.requestor = requestor
+        self.requestor_name = requestor_name
         self.backup_days = backup_days
         self.schema_pattern = schema_pattern
 
     def _session_func(self) -> Callable:
         return sqlite_session
 
     def _fqtn(self, table_name: str, schema_name: Optional[str] = None, no_schema: bool = False) -> str:
@@ -772,20 +774,22 @@
         self,
         pool: psycopg2.pool.SimpleConnectionPool,
         verbose: bool = False,
         schema: str = None,
         requestor: str = None,
         backup_days: Optional[int] = None,
         schema_pattern: Optional[str] = None,
+        requestor_name: Optional[str] = None,
     ) -> None:
         self.engine = pool
         self.verbose = verbose
         self.table_definition = '(data jsonb not null, uniq text unique not null)'
         self.schema = schema if schema else 'public'
         self.requestor = requestor
+        self.requestor_name = requestor_name
         self.backup_days = backup_days
         self.schema_pattern = schema_pattern
 
     def _session_func(self) -> Callable:
         return postgres_session
 
     def _fqtn(self, table_name: str, schema_name: Optional[str] = None, no_schema: bool = False) -> str:
```

### Comparing `pysquril-0.6.0/pysquril/generator.py` & `pysquril-0.6.2/pysquril/generator.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.6.0/pysquril/parser.py` & `pysquril-0.6.2/pysquril/parser.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.6.0/pysquril/test_data.py` & `pysquril-0.6.2/pysquril/test_data.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.6.0/pysquril/tests.py` & `pysquril-0.6.2/pysquril/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     max_conn = 5
     dsn = f"dbname={dbconfig['dbname']} user={dbconfig['user']} password={dbconfig['pw']} host={dbconfig['host']}"
     pool = psycopg2.pool.SimpleConnectionPool(
         min_conn, max_conn, dsn
     )
     return pool
 
+TEST_REQUESTOR = "p11-treq"
+TEST_REQUESTOR_NAME = "Test Requestor"
+
 class TestParser(object):
 
     def test_select(self) -> None:
         c = SelectClause("x[*|a,b],y.z")
         assert len(c.split_clause()) == 2
 
     def test_where(self) -> None:
@@ -652,14 +655,16 @@
         self.assertEqual(audit_event["diff"], new_data)
         self.assertEqual(audit_event["event"], "update")
         self.assertTrue(audit_event["transaction_id"] is not None)
         self.assertTrue(audit_event["event_id"] is not None)
         self.assertTrue(audit_event["timestamp"] is not None)
         self.assertTrue(audit_event["query"] is not None)
         self.assertEqual(audit_event["message"], message)
+        self.assertEqual(audit_event["identity"], TEST_REQUESTOR)
+        self.assertEqual(audit_event["identity_name"], TEST_REQUESTOR_NAME)
 
         # restore updates
         with self.assertRaises(ParseError): # missing restore directive
             self.backend.table_restore(table_name=test_table, uri_query="")
         with self.assertRaises(ParseError): # missing primary key
             self.backend.table_restore(table_name=test_table, uri_query="restore")
         with self.assertRaises(ParseError): # still missing primary key
@@ -832,15 +837,17 @@
 class TestSqliteBackend(TestSqlBackend):
     __test__ = True
 
     def setUp(self) -> None:
         self.directory = tempfile.gettempdir()
         self.file = f"{__package__}_test.db"
         self.engine = sqlite_init(self.directory, name=self.file)
-        self.backend = SqliteBackend(self.engine)
+        self.backend = SqliteBackend(
+            self.engine, requestor=TEST_REQUESTOR, requestor_name=TEST_REQUESTOR_NAME
+        )
         self.session_func = sqlite_session
         self.backend_class = SqliteBackend
     
     def tearDown(self) -> None:
         self.engine.close()
         if os.path.exists(f"{self.directory}/{self.file}"):
             os.remove(f"{self.directory}/{self.file}")
@@ -853,14 +860,16 @@
             {
                 "dbname": os.environ.get("PYSQURIL_POSTGRES_DB", "pysquril_db"),
                 "user": os.environ.get("PYSQURIL_POSTGRES_USER", "pysquril_user"),
                 "pw": os.environ.get("PYSQURIL_POSTGRES_PASSWORD", ""),
                 "host": os.environ.get("PYSQURIL_POSTGRES_HOST", "localhost"),
             }
         )
-        self.backend = PostgresBackend(self.engine)
+        self.backend = PostgresBackend(
+            self.engine, requestor=TEST_REQUESTOR, requestor_name=TEST_REQUESTOR_NAME
+        )
         self.backend.initialise()
         self.session_func = postgres_session
         self.backend_class = PostgresBackend
 
     def tearDown(self) -> None:
         self.engine.closeall()
```

### Comparing `pysquril-0.6.0/PKG-INFO` & `pysquril-0.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysquril
-Version: 0.6.0
+Version: 0.6.2
 Summary: Python implementation of structured URI query language
 Home-page: https://github.com/unioslo/pysquril
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

