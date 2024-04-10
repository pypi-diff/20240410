# Comparing `tmp/pg_logidater-0.2.1.tar.gz` & `tmp/pg_logidater-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_logidater-0.2.1.tar", max compression
+gzip compressed data, was "pg_logidater-0.3.0.tar", max compression
```

## Comparing `pg_logidater-0.2.1.tar` & `pg_logidater-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.2.1/LICENSE
--rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.2.1/pg_logidater/__init__.py
--rw-r--r--   0        0        0     9583 2024-04-10 07:26:01.552918 pg_logidater-0.2.1/pg_logidater/cli.py
--rw-r--r--   0        0        0     1326 2024-04-10 07:00:49.766735 pg_logidater-0.2.1/pg_logidater/exceptions.py
--rw-r--r--   0        0        0     2220 2024-04-09 08:49:26.288510 pg_logidater-0.2.1/pg_logidater/master.py
--rw-r--r--   0        0        0     1553 2024-04-10 06:46:14.045920 pg_logidater-0.2.1/pg_logidater/replica.py
--rw-r--r--   0        0        0     2813 2024-04-10 07:23:02.468326 pg_logidater-0.2.1/pg_logidater/sqlqueries.py
--rw-r--r--   0        0        0     4858 2024-04-10 07:25:12.766340 pg_logidater-0.2.1/pg_logidater/tartget.py
--rw-r--r--   0        0        0     9008 2024-04-10 07:23:42.306091 pg_logidater-0.2.1/pg_logidater/utils.py
--rw-r--r--   0        0        0      853 2024-04-05 19:35:20.054169 pg_logidater-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pg_logidater-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.3.0/LICENSE
+-rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.3.0/pg_logidater/__init__.py
+-rw-r--r--   0        0        0    10163 2024-04-10 14:25:04.351821 pg_logidater-0.3.0/pg_logidater/cli.py
+-rw-r--r--   0        0        0     1326 2024-04-10 07:00:49.766735 pg_logidater-0.3.0/pg_logidater/exceptions.py
+-rw-r--r--   0        0        0     2220 2024-04-09 08:49:26.288510 pg_logidater-0.3.0/pg_logidater/master.py
+-rw-r--r--   0        0        0     1553 2024-04-10 06:46:14.045920 pg_logidater-0.3.0/pg_logidater/replica.py
+-rw-r--r--   0        0        0     2813 2024-04-10 07:23:02.468326 pg_logidater-0.3.0/pg_logidater/sqlqueries.py
+-rw-r--r--   0        0        0     5565 2024-04-10 14:29:43.585596 pg_logidater-0.3.0/pg_logidater/tartget.py
+-rw-r--r--   0        0        0     9008 2024-04-10 07:23:42.306091 pg_logidater-0.3.0/pg_logidater/utils.py
+-rw-r--r--   0        0        0      873 2024-04-10 14:22:39.175904 pg_logidater-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pg_logidater-0.3.0/PKG-INFO
```

### Comparing `pg_logidater-0.2.1/LICENSE` & `pg_logidater-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.1/README.md` & `pg_logidater-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.1/pg_logidater/cli.py` & `pg_logidater-0.3.0/pg_logidater/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import pwd
 import argparse
 import json
+from threading import Thread, Event
 from psycopg2 import OperationalError
 from logging import getLogger
 from sys import exit
 from pg_logidater.exceptions import (
     PsqlConnectionError,
 )
 from pg_logidater.utils import (
@@ -26,15 +27,16 @@
     create_subscriber,
     create_database,
     target_check,
     sync_roles,
     sync_database,
     get_replica_position,
     sync_seq_pipe,
-    analyse_target
+    analyse_target,
+    db_sync_progress_bar
 )
 
 
 _logger = getLogger(__name__)
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--save-log",
@@ -149,14 +151,20 @@
 
 @cli(
     [
         argument(
             "--ignore-pkey",
             help="Ignore missing pkeys",
             action="store_true"
+        ),
+        argument(
+            "--update-interval",
+            help="Progress update interval, default 2s",
+            default=2,
+            type=float
         )
     ]
 )
 def setup_replica(args) -> None:
     try:
         master_sql = SqlConn(args["master_host"], user=args["psql_user"], db=args["database"])
         replica_sql = SqlConn(args["replica_host"], args["psql_user"])
@@ -198,21 +206,36 @@
         app_name=app_name
     )
     sync_roles(
         host=args["replica_host"],
         tmp_path=args["app_tmp_dir"],
         log_dir=args["app_log_dir"],
     )
+
+    event_finished = Event()
+    progress_thread = Thread(
+        target=db_sync_progress_bar,
+        args=(
+            target_sql,
+            db_size,
+            event_finished,
+            args["database"],
+            args["update_interval"],
+        )
+    )
+    progress_thread.start()
     sync_database(
         host=args["replica_host"],
         user=args["psql_user"],
         database=args["database"],
         tmp_dir=args["app_tmp_dir"],
-        log_dir=args["app_log_dir"]
+        log_dir=args["app_log_dir"],
+        event=event_finished
     )
+    progress_thread.join()
     create_subscriber(
        sub_target=args["master_host"],
        database=args["database"],
        slot_name=args["repl_name"],
        repl_position=replica_stop_position
     )
     _logger.info("Rresuming replication")
```

### Comparing `pg_logidater-0.2.1/pg_logidater/exceptions.py` & `pg_logidater-0.3.0/pg_logidater/exceptions.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.1/pg_logidater/master.py` & `pg_logidater-0.3.0/pg_logidater/master.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.1/pg_logidater/replica.py` & `pg_logidater-0.3.0/pg_logidater/replica.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.1/pg_logidater/sqlqueries.py` & `pg_logidater-0.3.0/pg_logidater/sqlqueries.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.1/pg_logidater/tartget.py` & `pg_logidater-0.3.0/pg_logidater/tartget.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from subprocess import Popen, PIPE
 from os import path
 from shutil import disk_usage
 from pg_logidater.exceptions import (
     DatabaseExists,
     DiskSpaceTooLow
 )
+from pycotore.progress import ProgressBar
+from threading import Event
 
 PG_DUMP_DB = "/usr/bin/pg_dump --no-publications --no-subscriptions -h {host} -U {user} {db}"
 PG_DUMP_SEQ = "/usr/bin/pg_dump --no-publications --no-subscriptions -h {host} -d {db} -U {user} -t {seq_name}"
 PG_DUMP_ROLES = "/usr/bin/pg_dumpall --roles-only -h {host} -U repmgr"
 PSQL_SQL_RESTORE = "/usr/bin/psql -f {file} -d {db}"
 PSQL_SQL_PIPE_RESTORE = "/usr/bin/psql -d {db}"
 
@@ -67,25 +69,46 @@
     run_local_cli(
         PSQL_SQL_RESTORE.format(file=roles_dump_path, db='postgres'),
         roles_restore_log,
         roles_restore_err_log
     )
 
 
-def sync_database(host: str, user: str, database: str, tmp_dir: str, log_dir: str) -> None:
+def sync_database(host: str, user: str, database: str, tmp_dir: str, log_dir: str, event: Event) -> None:
     _logger.info(f"Syncing database {database}")
     sync_log = path.join(log_dir, f"sync_{database}.log")
     sync_err_log = path.join(log_dir, f"sync_{database}.err")
+    event.set()
     run_local_cli(
         cli=PG_DUMP_DB.format(db=database, host=host, user=user),
         cli2=PSQL_SQL_PIPE_RESTORE.format(db=database),
         std_log=sync_log,
         err_log=sync_err_log,
         pipe=True
     )
+    event.set()
+
+
+def db_sync_progress_bar(psql: SqlConn, total: float, event: Event, db: str, update_interval: float) -> None:
+    _logger.debug("Startign progress bar function")
+    bar = ProgressBar()
+    suffix = f"{db} sync in progress"
+    bar.set_suffix(suffix)
+    bar.set_total(total)
+    event.wait(timeout=10)
+    _logger.debug("Continue progrss function")
+    event.clear()
+    while True:
+        if event.is_set():
+            break
+        synced_size = psql.get_db_size(db)
+        bar.update_progress(synced_size)
+        bar.draw()
+        event.wait(update_interval)
+    bar.flush_line()
 
 
 def create_subscriber(sub_target: str, database: str, slot_name: str, repl_position: str) -> None:
     psql = SqlConn("/tmp", user="postgres", db=database)
     _logger.info(f"Creating subsriber to {sub_target}")
     sub_id = psql.create_subscriber(
         name=slot_name,
```

### Comparing `pg_logidater-0.2.1/pg_logidater/utils.py` & `pg_logidater-0.3.0/pg_logidater/utils.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.1/pyproject.toml` & `pg_logidater-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 [tool.poetry.scripts]
 pg-logidater = 'pg_logidater.cli:main'
 
 [tool.poetry.dependencies]
 python = "~3.9"
 psycopg2-binary = "^2.9.9"
 paramiko = "^3.4.0"
+pycotore = "^0.0.3"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 tox = "^4.14.2"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 wheel = "^0.43.0"
```

### Comparing `pg_logidater-0.2.1/PKG-INFO` & `pg_logidater-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pg-logidater
-Version: 0.2.1
+Version: 0.3.0
 Summary: Postgresql logical replication setup utility
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Keywords: postgres
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
+Requires-Dist: pycotore (>=0.0.3,<0.0.4)
 Project-URL: Repository, https://github.com/niekosau/pg-logidater
 Description-Content-Type: text/markdown
 
 pg-logidater
 ============
 > [!CAUTION]
 > Use with yout own risk, not batletested
```

