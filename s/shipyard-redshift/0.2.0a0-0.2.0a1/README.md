# Comparing `tmp/shipyard_redshift-0.2.0a0.tar.gz` & `tmp/shipyard_redshift-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_redshift-0.2.0a0.tar", max compression
+gzip compressed data, was "shipyard_redshift-0.2.0a1.tar", max compression
```

## Comparing `shipyard_redshift-0.2.0a0.tar` & `shipyard_redshift-0.2.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-14 16:50:02.444245 shipyard_redshift-0.2.0a0/README.md
--rw-r--r--   0        0        0      697 2024-04-05 17:12:57.670079 shipyard_redshift-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-08-14 16:50:02.444534 shipyard_redshift-0.2.0a0/shipyard_redshift/__init__.py
--rw-r--r--   0        0        0      807 2024-04-05 17:12:57.671197 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/authtest.py
--rw-r--r--   0        0        0     2913 2024-04-05 17:12:57.671975 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/download.py
--rw-r--r--   0        0        0     1987 2024-04-05 17:12:57.672417 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/execute_query.py
--rw-r--r--   0        0        0     4472 2024-04-05 17:12:57.673126 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/upload.py
--rw-r--r--   0        0        0     7982 2024-04-05 17:12:57.673664 shipyard_redshift-0.2.0a0/shipyard_redshift/redshift.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 shipyard_redshift-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-14 16:50:02.444245 shipyard_redshift-0.2.0a1/README.md
+-rw-r--r--   0        0        0      697 2024-04-10 17:02:55.398316 shipyard_redshift-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-08-14 16:50:02.444534 shipyard_redshift-0.2.0a1/shipyard_redshift/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-05 17:12:57.671197 shipyard_redshift-0.2.0a1/shipyard_redshift/cli/authtest.py
+-rw-r--r--   0        0        0     2963 2024-04-10 16:50:38.893221 shipyard_redshift-0.2.0a1/shipyard_redshift/cli/download.py
+-rw-r--r--   0        0        0     2036 2024-04-10 16:50:09.148005 shipyard_redshift-0.2.0a1/shipyard_redshift/cli/execute_query.py
+-rw-r--r--   0        0        0     4521 2024-04-10 16:51:02.209654 shipyard_redshift-0.2.0a1/shipyard_redshift/cli/upload.py
+-rw-r--r--   0        0        0     8134 2024-04-10 17:03:36.882652 shipyard_redshift-0.2.0a1/shipyard_redshift/redshift.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 shipyard_redshift-0.2.0a1/PKG-INFO
```

### Comparing `shipyard_redshift-0.2.0a0/pyproject.toml` & `shipyard_redshift-0.2.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-redshift"
-version = "0.2.0a0"
+version = "0.2.0a1"
 description = "A local client for connecting and working with Redshift Databases"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_redshift"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_redshift-0.2.0a0/shipyard_redshift/cli/authtest.py` & `shipyard_redshift-0.2.0a1/shipyard_redshift/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_redshift-0.2.0a0/shipyard_redshift/cli/download.py` & `shipyard_redshift-0.2.0a1/shipyard_redshift/cli/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,16 +55,18 @@
         "host": args.host,
         "user": args.username,
         "pwd": args.password,
         "database": args.database,
         "port": args.port,
         "url_params": args.url_parameters if args.url_parameters != "" else None,
     }
-    redshift = RedshiftClient(**redshift_args)
+
+    redshift = None
     try:
+        redshift = RedshiftClient(**redshift_args)
         if target_dir:
             shipyard.files.create_folder_if_dne(target_dir)
         redshift.read_chunks(query, target_path, file_header)
         logger.info(f"Successfully downloaded query results to {target_path}")
 
     except ExitCodeException as ec:
         logger.error(ec.message)
@@ -72,12 +74,13 @@
 
     except Exception as e:
         logger.error(
             f"An unexpected error occurred when attempting to fetch results from Redshift. Message from the server reads: {e}"
         )
         sys.exit(Database.EXIT_CODE_UNKNOWN)
     finally:
-        redshift.close()
+        if redshift:
+            redshift.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_redshift-0.2.0a0/shipyard_redshift/cli/execute_query.py` & `shipyard_redshift-0.2.0a1/shipyard_redshift/cli/execute_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,24 +34,26 @@
         "user": args.username,
         "pwd": args.password,
         "database": args.database,
         "port": args.port,
         "url_params": args.url_parameters if args.url_parameters != "" else None,
     }
 
-    redshift = RedshiftClient(**redshift_args)
+    redshift = None
     try:
+        redshift = RedshiftClient(**redshift_args)
         redshift.execute_query(query)
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(
             f"An unepxected error occurred when attempting to execute query in Redshift. Message from the server reads {e}"
         )
         sys.exit(Database.EXIT_CODE_UNKNOWN)
     finally:
-        redshift.close()
+        if redshift:
+            redshift.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_redshift-0.2.0a0/shipyard_redshift/cli/upload.py` & `shipyard_redshift-0.2.0a1/shipyard_redshift/cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,17 @@
         "pwd": args.password,
         "database": args.database,
         "port": args.port,
         "schema": args.schema if args.schema != "" else None,
         "url_params": args.url_parameters if args.url_parameters != "" else None,
     }
 
-    redshift = RedshiftClient(**redshift_args)
+    redshift = None
     try:
+        redshift = RedshiftClient(**redshift_args)
         if match_type == "regex_match":
             file_names = shipyard.files.find_all_local_file_names(src_dir)
             matching_file_names = shipyard.files.find_all_file_matches(
                 file_names, re.compile(src_file)
             )
             if n_matches := len(matching_file_names) == 0:
                 logger.error(f"No matches found for pattern {src_file}")
@@ -111,12 +112,13 @@
 
     except Exception as e:
         logger.error(
             f"An unpexpected error occurred when attempting to upload into Redshift. Message from the server reads: {e}"
         )
 
     finally:
-        redshift.close()
+        if redshift:
+            redshift.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_redshift-0.2.0a0/shipyard_redshift/redshift.py` & `shipyard_redshift-0.2.0a1/shipyard_redshift/redshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         Raises:
             ExitCodeException: If an exit code exception occurs during the execution of the method.
             UploadError: If an error occurs during the upload process.
 
         """
         try:
             if self.schema:
+                logger.info("Creating schema if it does not already exist")
                 self.execute_query(f"CREATE SCHEMA IF NOT EXISTS {self.schema}")
             if os.path.getsize(file) < self.MAX_FILE_SIZE:
                 df = pd.read_csv(file)
                 self.upload_df(df, table_name=table_name, insert_method=insert_method)
             else:
                 self.upload_file(
                     file, table_name=table_name, insert_method=insert_method
@@ -194,14 +195,15 @@
         """
         try:
             df.to_sql(
                 table_name,
                 con=self.conn,
                 index=False,
                 if_exists=insert_method,
+                schema=self.schema,
                 method="multi",
             )
         except Exception as e:
             raise UploadError(table=table_name, error_msg=e)
 
     def upload_file(
         self, file_path: str, table_name: str, insert_method: str = "replace"
@@ -222,14 +224,15 @@
         try:
             for chunk in pd.read_csv(file_path, chunksize=self.CHUNKSIZE):
                 chunk.to_sql(
                     table_name,
                     con=self.conn,
                     index=False,
                     if_exists=insert_method,
+                    schema=self.schema,
                     method="multi",
                 )
                 if insert_method == "replace":
                     insert_method = "append"
         except Exception as e:
             raise UploadError(table=table_name, error_msg=e)
```

### Comparing `shipyard_redshift-0.2.0a0/PKG-INFO` & `shipyard_redshift-0.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-redshift
-Version: 0.2.0a0
+Version: 0.2.0a1
 Summary: A local client for connecting and working with Redshift Databases
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

