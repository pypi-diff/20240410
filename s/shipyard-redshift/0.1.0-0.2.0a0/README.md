# Comparing `tmp/shipyard_redshift-0.1.0.tar.gz` & `tmp/shipyard_redshift-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_redshift-0.1.0.tar", max compression
+gzip compressed data, was "shipyard_redshift-0.2.0a0.tar", max compression
```

## Comparing `shipyard_redshift-0.1.0.tar` & `shipyard_redshift-0.2.0a0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-14 16:50:02.444245 shipyard_redshift-0.1.0/README.md
--rw-r--r--   0        0        0      681 2024-03-21 14:52:56.584403 shipyard_redshift-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-08-14 16:50:02.444534 shipyard_redshift-0.1.0/shipyard_redshift/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:38.971096 shipyard_redshift-0.1.0/shipyard_redshift/cli/__init__.py
--rw-r--r--   0        0        0     1021 2024-03-08 19:26:38.971308 shipyard_redshift-0.1.0/shipyard_redshift/cli/authtest.py
--rw-r--r--   0        0        0     5322 2024-03-08 19:26:38.971622 shipyard_redshift-0.1.0/shipyard_redshift/cli/download.py
--rw-r--r--   0        0        0     3154 2024-03-08 19:26:38.971860 shipyard_redshift-0.1.0/shipyard_redshift/cli/execute_query.py
--rw-r--r--   0        0        0     7144 2024-01-04 01:57:22.702638 shipyard_redshift-0.1.0/shipyard_redshift/cli/upload.py
--rw-r--r--   0        0        0     1186 2023-08-14 16:51:48.021075 shipyard_redshift-0.1.0/shipyard_redshift/redshift.py
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 shipyard_redshift-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-14 16:50:02.444245 shipyard_redshift-0.2.0a0/README.md
+-rw-r--r--   0        0        0      697 2024-04-05 17:12:57.670079 shipyard_redshift-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-08-14 16:50:02.444534 shipyard_redshift-0.2.0a0/shipyard_redshift/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-05 17:12:57.671197 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/authtest.py
+-rw-r--r--   0        0        0     2913 2024-04-05 17:12:57.671975 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/download.py
+-rw-r--r--   0        0        0     1987 2024-04-05 17:12:57.672417 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/execute_query.py
+-rw-r--r--   0        0        0     4472 2024-04-05 17:12:57.673126 shipyard_redshift-0.2.0a0/shipyard_redshift/cli/upload.py
+-rw-r--r--   0        0        0     7982 2024-04-05 17:12:57.673664 shipyard_redshift-0.2.0a0/shipyard_redshift/redshift.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 shipyard_redshift-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_redshift-0.1.0/shipyard_redshift/cli/download.py` & `shipyard_redshift-0.2.0a0/shipyard_redshift/cli/upload.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,122 @@
 import argparse
-import os
-import code
-import csv
+import re
+import sys
+import shipyard_bp_utils as shipyard
 import pandas as pd
-from sqlalchemy import create_engine, text
-from sqlalchemy.engine.url import URL
+from shipyard_templates import ShipyardLogger, Database, ExitCodeException
+from shipyard_redshift import RedshiftClient
+
+logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--username", dest="username", required=False)
     parser.add_argument("--password", dest="password", required=False)
     parser.add_argument("--host", dest="host", required=False)
     parser.add_argument("--database", dest="database", required=False)
     parser.add_argument("--port", dest="port", default="5439", required=False)
-    parser.add_argument("--query", dest="query", required=True)
+    parser.add_argument("--url-parameters", dest="url_parameters", required=False)
+    parser.add_argument(
+        "--source-file-name-match-type",
+        dest="source_file_name_match_type",
+        default="exact_match",
+        choices={"exact_match", "regex_match"},
+        required=False,
+    )
     parser.add_argument(
-        "--destination-file-name",
-        dest="destination_file_name",
+        "--source-file-name",
+        dest="source_file_name",
         default="output.csv",
         required=True,
     )
     parser.add_argument(
-        "--destination-folder-name",
-        dest="destination_folder_name",
-        default="",
-        required=False,
+        "--source-folder-name", dest="source_folder_name", default="", required=False
     )
+    parser.add_argument("--table-name", dest="table_name", default=None, required=True)
     parser.add_argument(
-        "--file-header", dest="file_header", default="True", required=False
+        "--insert-method",
+        dest="insert_method",
+        choices={"replace", "append"},
+        default="append",
+        required=False,
     )
-    parser.add_argument("--url-parameters", dest="url_parameters", required=False)
-    parser.add_argument("--db-connection-url", dest="db_connection_url", required=False)
+    parser.add_argument("--schema", dest="schema", required=False, default="")
     args = parser.parse_args()
 
-    if (
-        not args.db_connection_url
-        and not (args.host or args.database or args.username)
-        and not os.environ.get("DB_CONNECTION_URL")
-    ):
-        parser.error(
-            """This Blueprint requires at least one of the following to be provided:\n
-            1) --db-connection-url\n
-            2) --host, --database, and --username\n
-            3) DB_CONNECTION_URL set as environment variable"""
-        )
     if args.host and not (args.database or args.username):
         parser.error("--host requires --database and --username")
     if args.database and not (args.host or args.username):
         parser.error("--database requires --host and --username")
     if args.username and not (args.host or args.username):
         parser.error("--username requires --host and --username")
     return args
 
 
-def create_connection_string(args):
-    """
-    Set the database connection string as an environment variable using the keyword arguments provided.
-    This will override system defaults.
-    """
-    if args.db_connection_url:
-        os.environ["DB_CONNECTION_URL"] = args.db_connection_url
-    elif args.host and args.username and args.database:
-        os.environ["DB_CONNECTION_URL"] = (
-            f"postgresql://{args.username}:{args.password}@{args.host}:{args.port}/{args.database}?{args.url_parameters}"
-        )
-
-    db_string = os.environ.get("DB_CONNECTION_URL")
-    return db_string
-
-
-def convert_to_boolean(string):
-    """
-    Shipyard can't support passing Booleans to code, so we have to convert
-    string values to their boolean values.
-    """
-    if string in ["True", "true", "TRUE"]:
-        value = True
-    else:
-        value = False
-    return value
-
-
-def combine_folder_and_file_name(folder_name, file_name):
-    """
-    Combine together the provided folder_name and file_name into one path variable.
-    """
-    combined_name = os.path.normpath(
-        f'{folder_name}{"/" if folder_name else ""}{file_name}'
-    )
-
-    return combined_name
-
-
-def create_csv(query, db_connection, destination_full_path, file_header=True):
-    """
-    Read in data from a SQL query. Store the data as a csv.
-    """
-    i = 1
-    for chunk in pd.read_sql_query(query, db_connection, chunksize=10000):
-        if i == 1:
-            chunk.to_csv(
-                destination_full_path, mode="a", header=file_header, index=False
-            )
-        else:
-            chunk.to_csv(destination_full_path, mode="a", header=False, index=False)
-        i += 1
-    print(f"Successfully stored results as {destination_full_path}.")
-    return
-
-
-def create_connection_url(
-    host: str, password: str, user: str, database: str, port=5439
-):
-    url = URL.create(
-        drivername="redshift+redshift_connector",
-        host=host,
-        password=password,
-        username=user,
-        port=port,
-        database=database,
-    )
-    return url
-
-
 def main():
     args = get_args()
-    destination_file_name = args.destination_file_name
-    destination_folder_name = args.destination_folder_name
-    destination_full_path = combine_folder_and_file_name(
-        folder_name=destination_folder_name, file_name=destination_file_name
-    )
-    file_header = convert_to_boolean(args.file_header)
-    query = text(args.query)
-    database = args.database
-    host = args.host
-    password = args.password
-    user = args.username
-    port = args.port
+    match_type = args.source_file_name_match_type
+    src_file = args.source_file_name
+    src_dir = args.source_folder_name
+    src_path = shipyard.files.combine_folder_and_file_name(
+        folder_name=src_dir, file_name=src_file
+    )
+    table_name = args.table_name
+    insert_method = args.insert_method
+    redshift_args = {
+        "host": args.host,
+        "user": args.username,
+        "pwd": args.password,
+        "database": args.database,
+        "port": args.port,
+        "schema": args.schema if args.schema != "" else None,
+        "url_params": args.url_parameters if args.url_parameters != "" else None,
+    }
 
-    db_string = create_connection_url(
-        host=host, password=password, user=user, database=database, port=port
-    )
+    redshift = RedshiftClient(**redshift_args)
     try:
-        db_connection = create_engine(
-            db_string, execution_options=dict(stream_results=True)
-        )
-    except Exception as e:
-        print(f"Failed to connect to database {database}")
-        raise (e)
+        if match_type == "regex_match":
+            file_names = shipyard.files.find_all_local_file_names(src_dir)
+            matching_file_names = shipyard.files.find_all_file_matches(
+                file_names, re.compile(src_file)
+            )
+            if n_matches := len(matching_file_names) == 0:
+                logger.error(f"No matches found for pattern {src_file}")
+                sys.exit(Database.EXIT_CODE_NO_FILE_MATCHES)
+            logger.info(
+                f"{len(matching_file_names)} files found. Preparing to upload..."
+            )
 
-    if not os.path.exists(destination_folder_name) and (destination_folder_name != ""):
-        os.makedirs(destination_folder_name)
+            for file_match in matching_file_names:
+                redshift.upload(
+                    file=file_match, table_name=table_name, insert_method=insert_method
+                )
+                if insert_method == "replace":
+                    insert_method = "append"
+            else:
+                logger.info(f"Successfully loaded all files to {table_name}")
+        else:
+            redshift.upload(
+                file=src_path, table_name=table_name, insert_method=insert_method
+            )
+            logger.info(f"Successfully loaded {src_path} to {table_name}")
+    except FileNotFoundError:
+        logger.error(
+            f"File {src_path} was not found. Please ensure that file name and folder name (if provided) are correcet"
+        )
+        sys.exit(Database.EXIT_CODE_FILE_NOT_FOUND)
+    except ExitCodeException as ec:
+        logger.error(ec.message)
+        sys.exit(ec.exit_code)
 
-    create_csv(
-        query=query,
-        db_connection=db_connection,
-        destination_full_path=destination_full_path,
-    )
+    except Exception as e:
+        logger.error(
+            f"An unpexpected error occurred when attempting to upload into Redshift. Message from the server reads: {e}"
+        )
 
-    db_connection.dispose()
+    finally:
+        redshift.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_redshift-0.1.0/PKG-INFO` & `shipyard_redshift-0.2.0a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: shipyard-redshift
-Version: 0.1.0
+Version: 0.2.0a0
 Summary: A local client for connecting and working with Redshift Databases
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: redshift-connector (==2.0.913)
-Requires-Dist: shipyard-bp-utils (==0.1.1)
-Requires-Dist: shipyard-templates (==0.4.3)
+Requires-Dist: shipyard-bp-utils (==1.2.0)
+Requires-Dist: shipyard-templates (==0.8.0a2)
 Requires-Dist: sqlalchemy-redshift (==0.8.14)
 Description-Content-Type: text/markdown
```

