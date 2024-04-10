# Comparing `tmp/pg_logidater-0.1.0b0.tar.gz` & `tmp/pg_logidater-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_logidater-0.1.0b0.tar", max compression
+gzip compressed data, was "pg_logidater-0.2.0.tar", max compression
```

## Comparing `pg_logidater-0.1.0b0.tar` & `pg_logidater-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.1.0b0/LICENSE
--rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.1.0b0/README.md
--rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.1.0b0/pg_logidater/__init__.py
--rw-r--r--   0        0        0     9131 2024-04-05 18:40:28.872527 pg_logidater-0.1.0b0/pg_logidater/cli.py
--rw-r--r--   0        0        0     1059 2024-03-31 04:40:04.882765 pg_logidater-0.1.0b0/pg_logidater/exceptions.py
--rw-r--r--   0        0        0     1519 2024-04-04 09:09:12.988223 pg_logidater-0.1.0b0/pg_logidater/master.py
--rw-r--r--   0        0        0     1454 2024-04-04 09:16:11.717639 pg_logidater-0.1.0b0/pg_logidater/replica.py
--rw-r--r--   0        0        0     2242 2024-04-04 11:34:45.892987 pg_logidater-0.1.0b0/pg_logidater/sqlqueries.py
--rw-r--r--   0        0        0     5011 2024-04-05 18:43:10.841757 pg_logidater-0.1.0b0/pg_logidater/tartget.py
--rw-r--r--   0        0        0     8770 2024-04-05 18:39:36.832184 pg_logidater-0.1.0b0/pg_logidater/utils.py
--rw-r--r--   0        0        0      853 2024-04-05 19:35:20.054169 pg_logidater-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 pg_logidater-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.2.0/LICENSE
+-rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.2.0/pg_logidater/__init__.py
+-rw-r--r--   0        0        0     9458 2024-04-09 10:08:30.794716 pg_logidater-0.2.0/pg_logidater/cli.py
+-rw-r--r--   0        0        0     1286 2024-04-09 07:10:21.531164 pg_logidater-0.2.0/pg_logidater/exceptions.py
+-rw-r--r--   0        0        0     2220 2024-04-09 08:49:26.288510 pg_logidater-0.2.0/pg_logidater/master.py
+-rw-r--r--   0        0        0     1659 2024-04-09 06:46:37.067914 pg_logidater-0.2.0/pg_logidater/replica.py
+-rw-r--r--   0        0        0     2781 2024-04-09 07:22:18.368803 pg_logidater-0.2.0/pg_logidater/sqlqueries.py
+-rw-r--r--   0        0        0     4745 2024-04-09 09:49:10.786143 pg_logidater-0.2.0/pg_logidater/tartget.py
+-rw-r--r--   0        0        0     9115 2024-04-09 07:26:50.788417 pg_logidater-0.2.0/pg_logidater/utils.py
+-rw-r--r--   0        0        0      853 2024-04-05 19:35:20.054169 pg_logidater-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pg_logidater-0.2.0/PKG-INFO
```

### Comparing `pg_logidater-0.1.0b0/LICENSE` & `pg_logidater-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0b0/README.md` & `pg_logidater-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0b0/pg_logidater/cli.py` & `pg_logidater-0.2.0/pg_logidater/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pg_logidater.tartget import (
     create_subscriber,
     create_database,
     target_check,
     sync_roles,
     sync_database,
     get_replica_position,
-    dump_restore_seq
+    sync_seq_pipe
 )
 
 
 _logger = getLogger(__name__)
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--save-log",
@@ -124,61 +124,75 @@
             for arg in args:
                 parser.add_argument(*arg[0], **arg[1])
             parser.set_defaults(func=func)
         return decorator
 
 
 def drop_privileges(user) -> None:
-    _logger.info(f"Chnaging user to: {user}")
     try:
+        current_uid = os.getuid()
         change_user = pwd.getpwnam(user)
+        if current_uid == change_user.pw_uid:
+            return
+        _logger.info(f"Chnaging user to: {user}")
         os.setgid(change_user.pw_gid)
         os.setuid(change_user.pw_uid)
         os.environ["HOME"] = change_user.pw_dir
     except PermissionError:
         _logger.error("Program must be executed as root!!")
         exit(1)
     except KeyError:
         _logger.error(f"{user} user doesn't exist")
         exit(1)
 
 
-@cli()
+@cli(
+    [
+        argument(
+            "--ignore-pkey",
+            help="Ignore missing pkeys",
+            action="store_true"
+        )
+    ]
+)
 def setup_replica(args) -> None:
     try:
         master_sql = SqlConn(args["master_host"], user=args["psql_user"], db=args["database"])
         replica_sql = SqlConn(args["replica_host"], args["psql_user"])
         target_sql = SqlConn("/tmp", user="postgres", db="postgres")
     except PsqlConnectionError as e:
         _logger.critical(e)
-    master_checks(
+    db_size = master_checks(
         psql=master_sql,
         slot_name=args["repl_name"],
-        pub_name=args["repl_name"]
+        pub_name=args["repl_name"],
+        skip_pkey_check=args["ignore_pkey"]
     )
     target_check(
         psql=target_sql,
         database=args["database"],
-        name=args["repl_name"])
-
+        name=args["repl_name"],
+        db_size=db_size
+    )
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
     app_name, slot_name = replica_info(
-        host=args["replica_host"]
+        host=args["replica_host"],
+        psql=replica_sql
     )
     replica_stop_position = get_replica_position(
         psql=master_sql,
         app_name=app_name
     )
     sync_roles(
         host=args["replica_host"],
@@ -220,17 +234,16 @@
     replica_sql = SqlConn(args["replica_host"], args["psql_user"])
     replica_sql.resume_replica()
 
 
 @cli()
 def sync_sequences(args) -> None:
     master_sql = SqlConn(args["master_host"], user=args["psql_user"], db=args["database"])
-    dump_restore_seq(
+    sync_seq_pipe(
         psql=master_sql,
-        tmp_dir=args["app_tmp_dir"],
         log_dir=args["app_log_dir"]
     )
 
 
 @cli()
 def remove_repl_config(args) -> None:
     _logger.info("Removing logical replication configuration")
@@ -292,14 +305,17 @@
     reduce_dict(args)
     merged_dicts = args | conf
     return merged_dicts
 
 
 def main():
     args = parser.parse_args()
+    if args.cli is None:
+        parser.print_help()
+        exit(0)
     if args.debug:
         setup_logging(
             log_level="debug",
             debug_ssh=True,
             save_log=args.save_log,
             log_path=args.app_log_dir
         )
@@ -313,17 +329,15 @@
         setup_logging(
             log_level=args.log_level,
             save_log=args.save_log,
             log_path=args.app_log_dir
         )
     _logger.debug(f"Cli args: {args}")
     args_dict = vars(args)
-    if args.cli is None:
-        parser.print_help()
-    elif args.cli == "save-cli-options":
+    if args.cli == "save-cli-options":
         args.func(args_dict)
     else:
         if args.saved_conf is not None:
             args_dict = resolve_config(args_dict)
         drop_privileges(args_dict.pop("user"))
         prepare_directories(args_dict["app_log_dir"], args_dict["app_tmp_dir"])
         args.func(args_dict)
```

### Comparing `pg_logidater-0.1.0b0/pg_logidater/exceptions.py` & `pg_logidater-0.2.0/pg_logidater/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,7 +34,18 @@
 
 
 class PublicationExists(Exception):
     def __init__(self, message=None):
         if not message:
             message = "Publication exists"
         super().__init__(message)
+
+
+class VersionNotSupported(Exception):
+    def __init__(self, message=None):
+        if not message:
+            message = "Version not supported"
+        super().__init__(message)
+
+
+class DiskSpaceTooLow(Exception):
+    pass
```

### Comparing `pg_logidater-0.1.0b0/pg_logidater/master.py` & `pg_logidater-0.2.0/pg_logidater/master.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,42 @@
 PG_DUMP = "/usr/bin/pg_dump --no-publications --no-subscriptions"
 PG_DUMPALL = "/usr/bin/pg_dumpall"
 PSQL = "/usr/bin/psql"
 
 _logger = getLogger(__name__)
 
 
-def master_checks(psql: SqlConn, slot_name: str, pub_name: str) -> None:
-    _logger.info("Starting master checks")
+def master_checks(psql: SqlConn, slot_name: str, pub_name: str, skip_pkey_check: bool) -> int:
+    _logger.info("Executing master checks")
     _logger.debug("Checking wal_level")
     wal_level = psql.get_wal_level()
     if wal_level != "logical":
         raise ReplicaLevelNotCorrect(f"Current wal_level: {wal_level}, minimum required: logical")
     _logger.debug(f"Checking if replication slot {slot_name} doesn't exists")
     replica_slot = psql.get_replica_slot(slot_name)
     if replica_slot:
         raise ReplicaSlotExists(f"Replication slot {slot_name} already exists!")
     _logger.debug(f"Checking in publication {pub_name} doesn't exists")
     publication = psql.is_pub_exists(pub_name)
     if publication:
         raise PublicationExists(f"Publication {pub_name} already exists for db: {psql.sql_conn.get_dsn_parameters()['dbname']}")
+    if not skip_pkey_check:
+        _logger.debug("Checking tables without primary keys")
+        no_keys_list = psql.get_no_primary_key()
+        if no_keys_list:
+            _logger.warning("Database have tables without primary key, that can cause issues with logical replication")
+            _logger.warning("Following tables doesn't have primary key")
+            for item in no_keys_list:
+                print(f"{item[0]}.{item[1]}")
+            _logger.warning("If that's fine, add --ignore-pkey switch")
+            exit(1)
+    _logger.debug("Getting db size")
+    db = psql.sql_conn.get_dsn_parameters()["dbname"]
+    db_size = psql.get_db_size(db)
+    return db_size
 
 
 def master_prepare(psql: SqlConn, name: str, database: str) -> str:
     _logger.info("Creating logical replication slot")
     psql.create_logical_slot(name)
     _logger.info("Creating publication")
     psql.create_publication(name)
```

### Comparing `pg_logidater-0.1.0b0/pg_logidater/sqlqueries.py` & `pg_logidater-0.2.0/pg_logidater/sqlqueries.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 SQL_SET_SLOT_NAME = "ALTER SUBSCRIPTION {name} SET (slot_name={slot_name})"
 SQL_DISABLE_SUBSCRIPTION = "ALTER SUBSCRIPTION {name} DISABLE"
 SQL_GET_DB_SUBSCRIPTION = "SELECT subname FROM pg_subscription"
 SQL_CREATE_REPL_LOGICAL_SLOT = "SELECT pg_create_logical_replication_slot('{0}', 'pgoutput')"
 SQL_DROP_REPL_SLOT = "SELECT pg_drop_replication_slot('{0}')"
 SQL_CREAATE_PUB = "CREATE publication {0} for all tables"
 SQL_DROP_PUB = "DROP publication {0}"
+SQL_DATA_DIRECTORY = "SHOW data_directory"
+SQL_DB_SIZE = "SELECT pg_database_size('{db}')"
 
 SQL_SELECT_ALL_SEQUENCES = """
 SELECT
   sequence_schema,
   sequence_name
 FROM
   information_schema.sequences
@@ -88,7 +90,25 @@
   roname
 FROM
   pg_subscription sub,
   pg_replication_origin ro
 WHERE
   'pg_' || sub.oid = ro.roname AND
   sub.subname = '{name}'"""
+
+SQL_NO_PRIMARY_KEYS = """
+SELECT
+  t.table_schema,
+  t.table_name
+FROM
+  information_schema.tables AS t
+  LEFT JOIN information_schema.table_constraints AS tc ON (
+    t.table_schema = t.table_schema
+    AND t.table_name = tc.table_name
+    AND tc.constraint_type = 'PRIMARY KEY'
+  )
+WHERE
+  t.table_type = 'BASE TABLE'
+  AND t.table_schema NOT IN ('pg_catalog', 'information_schema')
+  AND tc.constraint_name IS NULL
+ORDER BY
+  t.table_schema"""
```

### Comparing `pg_logidater-0.1.0b0/pg_logidater/tartget.py` & `pg_logidater-0.2.0/pg_logidater/tartget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 from logging import getLogger
 from pg_logidater.utils import SqlConn
-from subprocess import Popen
+from subprocess import Popen, PIPE
 from os import path
+from shutil import disk_usage
 from pg_logidater.exceptions import (
-    DatabaseExists
+    DatabaseExists,
+    DiskSpaceTooLow
 )
 
-PG_DUMP_DB = "/usr/bin/pg_dump --no-publications --no-subscriptions -h {host} -d {db} -U {user}"
+PG_DUMP_DB = "/usr/bin/pg_dump --no-publications --no-subscriptions -h {host} -U {user} {db}"
 PG_DUMP_SEQ = "/usr/bin/pg_dump --no-publications --no-subscriptions -h {host} -d {db} -U {user} -t {seq_name}"
 PG_DUMP_ROLES = "/usr/bin/pg_dumpall --roles-only -h {host} -U repmgr"
 PSQL_SQL_RESTORE = "/usr/bin/psql -f {file} -d {db}"
+PSQL_SQL_PIPE_RESTORE = "/usr/bin/psql -d {db}"
+
 
 _logger = getLogger(__name__)
 
 
-def target_check(psql: SqlConn, database: str, name: str) -> None:
+def target_check(psql: SqlConn, database: str, name: str, db_size: int) -> None:
+    _logger.info("Executing target checks")
+    _logger.debug("Checking available disk space")
+    data_path = psql.get_datadirectory()
+    available_disk = int(disk_usage(path=data_path).free * 0.9)
+    if available_disk < db_size:
+        raise DiskSpaceTooLow(f"Low disk space for {data_path}")
+    _logger.debug("Checking if database not exists")
     if psql.check_database(database):
         raise DatabaseExists
 
 
-def run_local_cli(cli, std_log, err_log) -> None:
+def run_local_cli(cli, std_log, err_log, cli2: str = None, pipe: bool = False) -> None:
     with open(std_log, "w") as log:
         with open(err_log, "w") as err:
-            _logger.debug(f"Executing: {cli}")
-            Popen(cli.split(), stdout=log, stderr=err).communicate()
+            if pipe:
+                if not cli2:
+                    _logger.critical("cli2 parameter mandaroty for pipe true")
+                    exit(1)
+                _logger.debug(f"Running: {cli} | {cli2}")
+                pipe_output = Popen(cli.split(), stdout=PIPE)
+                pipe_sync = Popen(cli2.split(), stdin=pipe_output.stdout, stdout=log, stderr=err)
+                pipe_sync.communicate()
+            else:
+                _logger.debug(f"Executing: {cli}")
+                Popen(cli.split(), stdout=log, stderr=err).communicate()
 
 
 def get_replica_position(psql: SqlConn, app_name: str) -> str:
     _logger.info("Getting replication position")
     return psql.get_replay_lsn(app_name)
 
 
@@ -49,29 +69,22 @@
         roles_restore_log,
         roles_restore_err_log
     )
 
 
 def sync_database(host: str, user: str, database: str, tmp_dir: str, log_dir: str) -> None:
     _logger.info(f"Syncing database {database}")
-    db_dump_path = path.join(tmp_dir, f"{database}.sql")
-    db_dump_err_log = path.join(log_dir, f"{database}.err")
-    _logger.debug(f"Dumping {database} to {db_dump_path} from {host}")
-    run_local_cli(
-        PG_DUMP_DB.format(db=database, host=host, user=user),
-        db_dump_path,
-        db_dump_err_log
-    )
-    db_restore_log = path.join(log_dir, f"{database}_restore.log")
-    db_restore_err_log = path.join(tmp_dir, f"{database}_restore.err")
-    _logger.debug(f"Restoring {database} from {db_dump_path} on target")
+    sync_log = path.join(log_dir, f"sync_{database}.log")
+    sync_err_log = path.join(log_dir, f"sync_{database}.err")
     run_local_cli(
-        PSQL_SQL_RESTORE.format(file=db_dump_path, db=database),
-        db_restore_log,
-        db_restore_err_log
+        cli=PG_DUMP_DB.format(db=database, host=host, user=user),
+        cli2=PSQL_SQL_PIPE_RESTORE.format(db=database),
+        std_log=sync_log,
+        err_log=sync_err_log,
+        pipe=True
     )
 
 
 def create_subscriber(sub_target: str, database: str, slot_name: str, repl_position: str) -> None:
     psql = SqlConn("/tmp", user="postgres", db=database)
     _logger.info(f"Creating subsriber to {sub_target}")
     sub_id = psql.create_subscriber(
@@ -91,53 +104,26 @@
     _logger.info(f"Creating database {database}")
     psql.create_database(
         database=database,
         owner=owner
     )
 
 
-def dump_restore_seq(psql: SqlConn, tmp_dir: str, log_dir: str) -> None:
+def sync_seq_pipe(psql: SqlConn, log_dir: str) -> None:
     dsn = psql.sql_conn.get_dsn_parameters()
     database = dsn["dbname"]
     host = dsn["host"]
     user = dsn["user"]
     _logger.info(f"Syncing sequences for {database}")
     sequences = psql.get_sequences()
     for seq in sequences:
-        sql_seq_name = f"{seq[0]}.\"{seq[1]}\""
         file_seq_name = f"{seq[0]}.{seq[1]}"
-        dump_path = path.join(tmp_dir, f"seq_dump_{sql_seq_name}.sql")
-        dump_err_log = path.join(log_dir, f"seq_dump_{file_seq_name}.err")
-        restore_log = path.join(log_dir, f"seq_restore_{file_seq_name}.log")
-        restore_err_log = path.join(log_dir, f"seq_restore_{file_seq_name}.err")
-        dump_seq(
-            host=host,
-            database=database,
-            user=user,
-            seq_name=sql_seq_name,
-            file_path=dump_path,
-            err_log=dump_err_log
-        )
-        restore_seq(
-            file_path=dump_path,
-            database=database,
-            restore_log=restore_log,
-            restore_err_log=restore_err_log
+        sql_seq_name = f"{seq[0]}.\"{seq[1]}\""
+        sync_seq_log = path.join(log_dir, f"sync_seq_{file_seq_name}.log")
+        sync_seq_err_log = path.join(log_dir, f"sync_seq_{file_seq_name}.err")
+        run_local_cli(
+            cli=PG_DUMP_SEQ.format(host=host, db=database, user=user, seq_name=sql_seq_name),
+            cli2=PSQL_SQL_PIPE_RESTORE.format(db=database),
+            std_log=sync_seq_log,
+            err_log=sync_seq_err_log,
+            pipe=True
         )
-
-
-def dump_seq(host: str, database: str, user: str, seq_name: str, file_path: str, err_log: str) -> None:
-    _logger.debug(f"Dumping sequence: {seq_name}")
-    run_local_cli(
-        cli=PG_DUMP_SEQ.format(host=host, db=database, user=user, seq_name=seq_name),
-        std_log=file_path,
-        err_log=err_log
-    )
-
-
-def restore_seq(file_path: str, database: str, restore_log: str, restore_err_log: str) -> None:
-    _logger.debug(f"Restoring {file_path}")
-    run_local_cli(
-        cli=PSQL_SQL_RESTORE.format(file=file_path, db=database),
-        std_log=restore_log,
-        err_log=restore_err_log
-    )
```

### Comparing `pg_logidater-0.1.0b0/pg_logidater/utils.py` & `pg_logidater-0.2.0/pg_logidater/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,14 +196,23 @@
         if self.query(sql.SQL_CHECK_PUBLICATION.format(name), fetchone=True):
             return True
         return False
 
     def get_sequences(self) -> list[tuple]:
         return self.query(sql.SQL_SELECT_ALL_SEQUENCES, fetchall=True)
 
+    def get_datadirectory(self) -> float:
+        return (self.query(sql.SQL_DATA_DIRECTORY, fetchone=True))[0]
+
+    def get_db_size(self, db) -> int:
+        return (self.query(sql.SQL_DB_SIZE.format(db=db), fetchone=True))[0]
+
+    def get_no_primary_key(self) -> list[tuple]:
+        return self.query(sql.SQL_NO_PRIMARY_KEYS, fetchall=True)
+
 
 def setup_logging(log_level: str, save_log: str, debug_ssh: bool = False,  log_path: str = None) -> None:
     log_level_int = logging.getLevelName(str(log_level).upper())
     handlers = []
     if debug_ssh:
         logging.getLogger("paramiko").setLevel(logging.DEBUG)
     else:
```

### Comparing `pg_logidater-0.1.0b0/pyproject.toml` & `pg_logidater-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0b0/PKG-INFO` & `pg_logidater-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-logidater
-Version: 0.1.0b0
+Version: 0.2.0
 Summary: Postgresql logical replication setup utility
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Keywords: postgres
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
```

