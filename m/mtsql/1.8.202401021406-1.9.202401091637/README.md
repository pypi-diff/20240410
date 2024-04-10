# Comparing `tmp/mtsql-1.8.202401021406-py3-none-any.whl.zip` & `tmp/mtsql-1.9.202401091637-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21995 bytes, number of entries: 12
--rw-r--r--  2.0 unx       44 b- defN 23-Jan-22 22:24 mt/sql/__init__.py
--rw-r--r--  2.0 unx     9780 b- defN 24-Jan-02 18:10 mt/sql/base.py
--rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 11:50 mt/sql/mysql.py
--rw-r--r--  2.0 unx    66036 b- defN 24-Jan-02 18:10 mt/sql/psql.py
--rw-r--r--  2.0 unx    14789 b- defN 24-Jan-02 18:10 mt/sql/redshift.py
--rw-r--r--  2.0 unx     8678 b- defN 23-Feb-23 10:22 mt/sql/sqlite.py
--rw-r--r--  2.0 unx      396 b- defN 24-Jan-02 18:10 mt/sql/version.py
--rw-r--r--  2.0 unx     1070 b- defN 24-Jan-02 18:12 mtsql-1.8.202401021406.dist-info/LICENSE
--rw-r--r--  2.0 unx      589 b- defN 24-Jan-02 18:12 mtsql-1.8.202401021406.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-02 18:12 mtsql-1.8.202401021406.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 24-Jan-02 18:12 mtsql-1.8.202401021406.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      939 b- defN 24-Jan-02 18:12 mtsql-1.8.202401021406.dist-info/RECORD
-12 files, 107310 bytes uncompressed, 20429 bytes compressed:  81.0%
+Zip file size: 22270 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       44 b- defN 23-Mar-28 14:19 mt/sql/__init__.py
+-rw-rw-r--  2.0 unx    10608 b- defN 24-Jan-09 16:36 mt/sql/base.py
+-rw-rw-r--  2.0 unx     4894 b- defN 23-Mar-28 14:19 mt/sql/mysql.py
+-rw-rw-r--  2.0 unx    65964 b- defN 24-Jan-09 16:27 mt/sql/psql.py
+-rw-rw-r--  2.0 unx    14808 b- defN 24-Jan-09 16:19 mt/sql/redshift.py
+-rw-rw-r--  2.0 unx     8678 b- defN 23-Mar-28 14:19 mt/sql/sqlite.py
+-rw-rw-r--  2.0 unx      396 b- defN 24-Jan-09 16:37 mt/sql/version.py
+-rw-rw-r--  2.0 unx     1070 b- defN 24-Jan-09 16:37 mtsql-1.9.202401091637.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      589 b- defN 24-Jan-09 16:37 mtsql-1.9.202401091637.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Jan-09 16:37 mtsql-1.9.202401091637.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 24-Jan-09 16:37 mtsql-1.9.202401091637.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      940 b- defN 24-Jan-09 16:37 mtsql-1.9.202401091637.dist-info/RECORD
+12 files, 108086 bytes uncompressed, 20704 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.8.202401021406.dist-info/LICENSE
+Filename: mtsql-1.9.202401091637.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.8.202401021406.dist-info/METADATA
+Filename: mtsql-1.9.202401091637.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.8.202401021406.dist-info/WHEEL
+Filename: mtsql-1.9.202401091637.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.8.202401021406.dist-info/top_level.txt
+Filename: mtsql-1.9.202401091637.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.8.202401021406.dist-info/RECORD
+Filename: mtsql-1.9.202401091637.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/base.py

```diff
@@ -1,9 +1,10 @@
 """Base functions dealing with an SQL database."""
 
+import uuid
 import sqlalchemy as sa
 import sqlalchemy.exc as se
 import psycopg2 as ps
 from halo import Halo
 
 from mt import tp, logg, pd, ctx
 from mt.base import deprecated_func
@@ -18,14 +19,15 @@
     "read_sql",
     "read_sql_table",
     "exec_sql",
     "list_schemas",
     "list_tables",
     "list_views",
     "table_exists",
+    "create_temp_id_table",
 ]
 
 
 def frame_sql(frame_name, schema: tp.Optional[str] = None):
     return frame_name if schema is None else "{}.{}".format(schema, frame_name)
 
 
@@ -39,15 +41,15 @@
 
 
 def run_func(
     func,
     *args,
     nb_trials: int = 3,
     logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
-    **kwargs
+    **kwargs,
 ):
     """Attempt to run a function a number of times to overcome OperationalError exceptions.
 
     Parameters
     ----------
     func: function
         function to be invoked
@@ -102,15 +104,15 @@
     sql,
     engine,
     index_col: tp.Union[str, tp.List[str], None] = None,
     chunksize: tp.Optional[int] = None,
     nb_trials: int = 3,
     exception_handling: str = "raise",
     logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
-    **kwargs
+    **kwargs,
 ) -> pd.DataFrame:
     """Read an SQL query with a number of trials to overcome OperationalError.
 
     The function wraps :func:`pandas.read_sql_query`. However, when `chunksize` is not None, it
     iterates over chunks and concatenates them. In addition, if `logger` is not None, a progress
     bar is shown in that case.
 
@@ -170,15 +172,15 @@
             pd.read_sql,
             sql,
             conn,
             index_col=index_col,
             chunksize=chunksize,
             nb_trials=nb_trials,
             logger=logger,
-            **kwargs
+            **kwargs,
         )
 
     if chunksize is None:
         return res
 
     try:
         dfs = []
@@ -210,15 +212,15 @@
 
 
 def read_sql_table(
     table_name,
     engine,
     nb_trials: int = 3,
     logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
-    **kwargs
+    **kwargs,
 ):
     """Read an SQL table with a number of trials to overcome OperationalError.
 
     Parameters
     ----------
     table_name : str
         name of the table to be read
@@ -236,25 +238,25 @@
     """
     return run_func(
         pd.read_sql_table,
         table_name,
         engine,
         nb_trials=nb_trials,
         logger=logger,
-        **kwargs
+        **kwargs,
     )
 
 
 def exec_sql(
     sql,
     engine,
     *args,
     nb_trials: int = 3,
     logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
-    **kwargs
+    **kwargs,
 ):
     """Execute an SQL query with a number of trials to overcome OperationalError.
 
     Parameters
     ----------
     sql : str
         SQL query to be executed
@@ -352,7 +354,35 @@
     Returns
     -------
     retval: bool
         whether a table or a view exists with the given name
     """
 
     return sa.inspect(engine).has_table(table_name, schema=schema)
+
+
+def create_temp_id_table(l_ids: list, conn: sa.engine.Connection) -> str:
+    """Creates a temporary table to containing a list of ids.
+
+    Parameters
+    ----------
+    l_ids : list
+        list of ids to be inserted into the table
+    conn : sqlalchemy.engine.Connection
+        a connection that has been opened
+
+    Returns
+    -------
+    table_name : str
+        name of the temporary table. The table will be deleted at the end of the connection
+    """
+
+    table_name = f"tab_{uuid.uuid4().hex}"
+
+    query_str = f"CREATE TEMP TABLE {table_name}(id int);"
+    conn.execute(sa.text(query_str))
+
+    values = ",".join((f"({id})" for id in l_ids))
+    query_str = f"INSERT INTO {table_name}(id) VALUES {values};"
+    conn.execute(sa.text(query_str))
+
+    return table_name
```

## mt/sql/psql.py

```diff
@@ -2000,19 +2000,17 @@
 
             new_df = pd.concat(new_dfs)
             if not hash_name in new_df.columns:
                 new_df = new_df.join(new_md5_df)
 
             if len(new_md5_df) != len(new_df):
                 if logger:
-                    logger.debug("New dataframe:\n{}".format(str(new_df)))
-                    logger.debug("Hash dataframe:\n{}".format(str(new_md5_df)))
-                msg = "Something must have gone wrong. Number of hashes {} != number of records {}.".format(
-                    len(new_md5_df), len(new_df)
-                )
+                    logger.debug(f"New dataframe:\n{str(new_df)}")
+                    logger.debug(f"Hash dataframe:\n{str(new_md5_df)}")
+                msg = f"Something must have gone wrong. Number of hashes {len(new_md5_df)} != number of records {len(new_df)}."
                 if raise_exception_upon_mismatch:
                     raise RuntimeError(msg)
                 elif logger:
                     logger.warn(msg)
         else:
             new_df = None  # nothing new
 
@@ -2029,14 +2027,14 @@
             )
         if new_df is not None:
             df.index = df.index.astype(new_md5_df.index.dtype)
         df = df.groupby(df.index).first().sort_index()
 
         # write back
         if logger:
-            logger.debug("Saving all {} records to file...".format(len(df)))
+            logger.debug(f"Saving all {len(df)} records to file...")
         if bg_write_csv is True:
             bg = BgInvoke(pd.dfsave, df, df_filepath, index=True)
             return df, bg
         else:
             pd.dfsave(df, df_filepath, index=True)
             return df
```

## mt/sql/redshift.py

```diff
@@ -503,18 +503,17 @@
             index=False,
             index_label=None,
             nb_trials=nb_trials,
             logger=logger,
             **kwargs,
         )
 
-        query_str = (
-            f"ALTER TABLE {frame_sql_str} ADD PRIMARY KEY ({','.join(local_indices)});"
-        )
-        exec_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
+        if if_exists == "replace":
+            query_str = f"ALTER TABLE {frame_sql_str} ADD PRIMARY KEY ({','.join(local_indices)});"
+            exec_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
     else:
         retval = run_func(
             df.to_sql,
             name,
             engine,
             schema=schema,
             if_exists=if_exists,
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2024
 VERSION_MONTH = int('01')
-VERSION_DAY = int('02')
-VERSION_HOUR = int('14')
-VERSION_MINUTE = int('06')
+VERSION_DAY = int('09')
+VERSION_HOUR = int('16')
+VERSION_MINUTE = int('37')
 MAJOR_VERSION = 1
-MINOR_VERSION = 8
-PATCH_VERSION = 202401021406
-version_date = '2024/01/02 14:06'
+MINOR_VERSION = 9
+PATCH_VERSION = 202401091637
+version_date = '2024/01/09 16:37'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.8.202401021406.dist-info/LICENSE` & `mtsql-1.9.202401091637.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.8.202401021406.dist-info/METADATA` & `mtsql-1.9.202401091637.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.8.202401021406
+Version: 1.9.202401091637
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy
```

## Comparing `mtsql-1.8.202401021406.dist-info/RECORD` & `mtsql-1.9.202401091637.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mt/sql/__init__.py,sha256=b7zO50apZxt9Hg2eOkJhRLrXgACR8eS5b-Rphdn5qNQ,44
-mt/sql/base.py,sha256=FoK42rNDxVkqwtGiDJGvW1g02FJtSoqkMtbPlxBElA0,9780
+mt/sql/base.py,sha256=GJLSQfz0GNXgFBzK6dSCVqQ4rjyTvFEBPmsM37d8eXc,10608
 mt/sql/mysql.py,sha256=n2ENDctdUqZuSaDAcrqZYtPtawq3Wx4dOPCRsCB5Q4w,4894
-mt/sql/psql.py,sha256=JBdwPKwk1G6QzOJGRjUbIcxKosjPQ_PADG2VwDxCR4M,66036
-mt/sql/redshift.py,sha256=cDDSPUqy6vIyKcKUNsQnZLESGLhgC8NYGyyIWhFTrNk,14789
+mt/sql/psql.py,sha256=m41LsBQ57OVVtakUZ01o_YY-vBwY5Z3TVPvSUMylNaU,65964
+mt/sql/redshift.py,sha256=EliV4C9E3VuNjqFXWnTrU8Dm_utQrVwht5DF4oHl7qY,14808
 mt/sql/sqlite.py,sha256=T2ak_hhNi_zRfpg_gp8JhNHn7D2kl4i-Ey6-9ANMtz0,8678
-mt/sql/version.py,sha256=gnhJJ-02mxUSXuUdVmoieNHefSOLt5692teFJSVykOA,396
-mtsql-1.8.202401021406.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtsql-1.8.202401021406.dist-info/METADATA,sha256=vlwY4ZndshEQJY6Ux4D1N907fFbl7b_7K1erSDkPkuA,589
-mtsql-1.8.202401021406.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtsql-1.8.202401021406.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtsql-1.8.202401021406.dist-info/RECORD,,
+mt/sql/version.py,sha256=nb0i2eAMsoLqFeLpvANq9ovAtp3TRIZsz2c02XZ4xBs,396
+mtsql-1.9.202401091637.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtsql-1.9.202401091637.dist-info/METADATA,sha256=0OS_X0KCiNKKzDFiiXTnttkBWJSeS6OoEsdmykC4JAc,589
+mtsql-1.9.202401091637.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtsql-1.9.202401091637.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtsql-1.9.202401091637.dist-info/RECORD,,
```

