# Comparing `tmp/pg_logidater-0.2.0.tar.gz` & `tmp/pg_logidater-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_logidater-0.2.0.tar", max compression
+gzip compressed data, was "pg_logidater-0.2.1.tar", max compression
```

## Comparing `pg_logidater-0.2.0.tar` & `pg_logidater-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.2.0/LICENSE
--rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.2.0/pg_logidater/__init__.py
--rw-r--r--   0        0        0     9458 2024-04-09 10:08:30.794716 pg_logidater-0.2.0/pg_logidater/cli.py
--rw-r--r--   0        0        0     1286 2024-04-09 07:10:21.531164 pg_logidater-0.2.0/pg_logidater/exceptions.py
--rw-r--r--   0        0        0     2220 2024-04-09 08:49:26.288510 pg_logidater-0.2.0/pg_logidater/master.py
--rw-r--r--   0        0        0     1659 2024-04-09 06:46:37.067914 pg_logidater-0.2.0/pg_logidater/replica.py
--rw-r--r--   0        0        0     2781 2024-04-09 07:22:18.368803 pg_logidater-0.2.0/pg_logidater/sqlqueries.py
--rw-r--r--   0        0        0     4745 2024-04-09 09:49:10.786143 pg_logidater-0.2.0/pg_logidater/tartget.py
--rw-r--r--   0        0        0     9115 2024-04-09 07:26:50.788417 pg_logidater-0.2.0/pg_logidater/utils.py
--rw-r--r--   0        0        0      853 2024-04-05 19:35:20.054169 pg_logidater-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pg_logidater-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.2.1/LICENSE
+-rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.2.1/pg_logidater/__init__.py
+-rw-r--r--   0        0        0     9583 2024-04-10 07:26:01.552918 pg_logidater-0.2.1/pg_logidater/cli.py
+-rw-r--r--   0        0        0     1326 2024-04-10 07:00:49.766735 pg_logidater-0.2.1/pg_logidater/exceptions.py
+-rw-r--r--   0        0        0     2220 2024-04-09 08:49:26.288510 pg_logidater-0.2.1/pg_logidater/master.py
+-rw-r--r--   0        0        0     1553 2024-04-10 06:46:14.045920 pg_logidater-0.2.1/pg_logidater/replica.py
+-rw-r--r--   0        0        0     2813 2024-04-10 07:23:02.468326 pg_logidater-0.2.1/pg_logidater/sqlqueries.py
+-rw-r--r--   0        0        0     4858 2024-04-10 07:25:12.766340 pg_logidater-0.2.1/pg_logidater/tartget.py
+-rw-r--r--   0        0        0     9008 2024-04-10 07:23:42.306091 pg_logidater-0.2.1/pg_logidater/utils.py
+-rw-r--r--   0        0        0      853 2024-04-05 19:35:20.054169 pg_logidater-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pg_logidater-0.2.1/PKG-INFO
```

### Comparing `pg_logidater-0.2.0/LICENSE` & `pg_logidater-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.0/README.md` & `pg_logidater-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.0/pg_logidater/cli.py` & `pg_logidater-0.2.1/pg_logidater/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from logging import getLogger
 from sys import exit
 from pg_logidater.exceptions import (
     PsqlConnectionError,
 )
 from pg_logidater.utils import (
     SqlConn,
+    ServerConn,
     setup_logging,
     prepare_directories
 )
 from pg_logidater.master import (
     master_prepare,
     master_checks
 )
@@ -24,15 +25,16 @@
 from pg_logidater.tartget import (
     create_subscriber,
     create_database,
     target_check,
     sync_roles,
     sync_database,
     get_replica_position,
-    sync_seq_pipe
+    sync_seq_pipe,
+    analyse_target
 )
 
 
 _logger = getLogger(__name__)
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--save-log",
@@ -169,31 +171,32 @@
     )
     target_check(
         psql=target_sql,
         database=args["database"],
         name=args["repl_name"],
         db_size=db_size
     )
+    with ServerConn(args["replica_host"], args["user"]) as ssh:
+        app_name, slot_name = replica_info(
+            psql=replica_sql,
+            ssh=ssh
+        )
     db_owner = master_prepare(
         psql=master_sql,
         name=args["repl_name"],
         database=args["database"]
     )
     create_database(
         psql=target_sql,
         database=args["database"],
         owner=db_owner
     )
     pause_replica(
         psql=replica_sql
     )
-    app_name, slot_name = replica_info(
-        host=args["replica_host"],
-        psql=replica_sql
-    )
     replica_stop_position = get_replica_position(
         psql=master_sql,
         app_name=app_name
     )
     sync_roles(
         host=args["replica_host"],
         tmp_path=args["app_tmp_dir"],
@@ -210,14 +213,15 @@
        sub_target=args["master_host"],
        database=args["database"],
        slot_name=args["repl_name"],
        repl_position=replica_stop_position
     )
     _logger.info("Rresuming replication")
     replica_sql.resume_replica()
+    analyse_target(target_sql)
 
 
 @cli()
 def drop_setup(args) -> None:
     _logger.info("Cleaning target server")
     try:
         target_sql = SqlConn("/tmp", user="postgres", db=args["database"])
@@ -334,15 +338,15 @@
     _logger.debug(f"Cli args: {args}")
     args_dict = vars(args)
     if args.cli == "save-cli-options":
         args.func(args_dict)
     else:
         if args.saved_conf is not None:
             args_dict = resolve_config(args_dict)
-        drop_privileges(args_dict.pop("user"))
+        drop_privileges(args_dict["user"])
         prepare_directories(args_dict["app_log_dir"], args_dict["app_tmp_dir"])
         args.func(args_dict)
         _logger.info(f"App debug log: {args.save_log}")
         _logger.info(f"Dump/restore logs: {args.app_log_dir}")
 
 
 if __name__ == "__main__":
```

### Comparing `pg_logidater-0.2.0/pg_logidater/exceptions.py` & `pg_logidater-0.2.1/pg_logidater/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,8 +44,10 @@
     def __init__(self, message=None):
         if not message:
             message = "Version not supported"
         super().__init__(message)
 
 
 class DiskSpaceTooLow(Exception):
-    pass
+    """
+    Disk space too low exception
+    """
```

### Comparing `pg_logidater-0.2.0/pg_logidater/master.py` & `pg_logidater-0.2.1/pg_logidater/master.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.0/pg_logidater/replica.py` & `pg_logidater-0.2.1/pg_logidater/replica.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,30 +17,29 @@
 def pause_replica(psql: SqlConn) -> None:
     _logger.info("Pausing replica")
     if psql.is_replica_pause():
         raise ReplicaPaused
     psql.pause_replica()
 
 
-def replica_info(host, psql: SqlConn, user="postgres") -> (str, str):
+def replica_info(psql: SqlConn, ssh: ServerConn) -> (str, str):
     _logger.info("Collecting replica info")
     pgdata = psql.get_datadirectory()
     psql_version = int(psql.server_version())
     if psql_version not in RECOVYRY_CONF_BY_VERSION.keys():
         raise VersionNotSupported
     recovey_conf = RECOVYRY_CONF_BY_VERSION[psql_version]
-    with ServerConn(host, user) as ssh:
-        auto_conf_name = path.join(pgdata, recovey_conf)
-        cli = f"cat {auto_conf_name}"
-        _logger.debug(f"Executing: {cli}")
-        psql_auto_conf = ssh.run_cmd(cli)
-        for line in reversed(psql_auto_conf.splitlines()):
-            if "application_name" in line:
-                replica_app_name = line.split(" ")[-1].removeprefix("application_name=").strip("'")
-                _logger.debug(f"Got replica app name: {replica_app_name}")
-                break
-        for line in reversed(psql_auto_conf.splitlines()):
-            if "primary_slot_name" in line:
-                replica_slot_name = line.split(" ")[-1].strip("'")
-                _logger.debug(f"Got replica slot name: {replica_slot_name}")
-                break
-        return replica_app_name, replica_slot_name
+    auto_conf_name = path.join(pgdata, recovey_conf)
+    cli = f"cat {auto_conf_name}"
+    _logger.debug(f"Executing: {cli}")
+    psql_auto_conf = ssh.run_cmd(cli)
+    for line in reversed(psql_auto_conf.splitlines()):
+        if "application_name" in line:
+            replica_app_name = line.split(" ")[-1].removeprefix("application_name=").strip("'")
+            _logger.debug(f"Got replica app name: {replica_app_name}")
+            break
+    for line in reversed(psql_auto_conf.splitlines()):
+        if "primary_slot_name" in line:
+            replica_slot_name = line.split(" ")[-1].strip("'")
+            _logger.debug(f"Got replica slot name: {replica_slot_name}")
+            break
+    return replica_app_name, replica_slot_name
```

### Comparing `pg_logidater-0.2.0/pg_logidater/sqlqueries.py` & `pg_logidater-0.2.1/pg_logidater/sqlqueries.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 SQL_GET_DB_SUBSCRIPTION = "SELECT subname FROM pg_subscription"
 SQL_CREATE_REPL_LOGICAL_SLOT = "SELECT pg_create_logical_replication_slot('{0}', 'pgoutput')"
 SQL_DROP_REPL_SLOT = "SELECT pg_drop_replication_slot('{0}')"
 SQL_CREAATE_PUB = "CREATE publication {0} for all tables"
 SQL_DROP_PUB = "DROP publication {0}"
 SQL_DATA_DIRECTORY = "SHOW data_directory"
 SQL_DB_SIZE = "SELECT pg_database_size('{db}')"
+SQL_ANALYZE = "ANALYZE VERBOSE"
 
 SQL_SELECT_ALL_SEQUENCES = """
 SELECT
   sequence_schema,
   sequence_name
 FROM
   information_schema.sequences
```

### Comparing `pg_logidater-0.2.0/pg_logidater/tartget.py` & `pg_logidater-0.2.1/pg_logidater/tartget.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,7 +123,12 @@
         run_local_cli(
             cli=PG_DUMP_SEQ.format(host=host, db=database, user=user, seq_name=sql_seq_name),
             cli2=PSQL_SQL_PIPE_RESTORE.format(db=database),
             std_log=sync_seq_log,
             err_log=sync_seq_err_log,
             pipe=True
         )
+
+
+def analyse_target(psql: SqlConn) -> None:
+    _logger.info("Updating database statistics")
+    psql.analyze()
```

### Comparing `pg_logidater-0.2.0/pg_logidater/utils.py` & `pg_logidater-0.2.1/pg_logidater/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,15 @@
         super().__init__()
         self.set_missing_host_key_policy(paramiko.AutoAddPolicy)
         self.load_system_host_keys()
         self.host = host
         self.user = user
 
     def __enter__(self):
-        try:
-            self.connect(hostname=self.host, username=self.user)
-        except paramiko.ssh_exception.SSHException:
-            _logger.critical(f"Unable connect to {self.host} with user: {self.user}")
-            exit(1)
+        self.connect(hostname=self.host, username=self.user)
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
 
     def run_cmd(self, command: str) -> str:
         _, out, err = self.exec_command(command=command, timeout=60)
@@ -205,14 +201,17 @@
 
     def get_db_size(self, db) -> int:
         return (self.query(sql.SQL_DB_SIZE.format(db=db), fetchone=True))[0]
 
     def get_no_primary_key(self) -> list[tuple]:
         return self.query(sql.SQL_NO_PRIMARY_KEYS, fetchall=True)
 
+    def analyze(self) -> None:
+        self.query(sql.SQL_ANALYZE)
+
 
 def setup_logging(log_level: str, save_log: str, debug_ssh: bool = False,  log_path: str = None) -> None:
     log_level_int = logging.getLevelName(str(log_level).upper())
     handlers = []
     if debug_ssh:
         logging.getLogger("paramiko").setLevel(logging.DEBUG)
     else:
```

### Comparing `pg_logidater-0.2.0/pyproject.toml` & `pg_logidater-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.2.0/PKG-INFO` & `pg_logidater-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-logidater
-Version: 0.2.0
+Version: 0.2.1
 Summary: Postgresql logical replication setup utility
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Keywords: postgres
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
```

