# Comparing `tmp/django_sync_env-0.2.9.tar.gz` & `tmp/django_sync_env-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.2.9.tar", max compression
+gzip compressed data, was "django_sync_env-0.3.0.tar", max compression
```

## Comparing `django_sync_env-0.2.9.tar` & `django_sync_env-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.2.9/README.md
--rw-r--r--   0        0        0      497 2024-02-07 21:28:28.094401 django_sync_env-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      303 2024-02-07 21:28:28.095420 django_sync_env-0.2.9/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.2.9/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-02-07 19:58:44.767684 django_sync_env-0.2.9/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      194 2024-02-07 19:58:44.767857 django_sync_env-0.2.9/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.2.9/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.2.9/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.2.9/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.2.9/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.2.9/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     3988 2024-02-07 19:58:44.769120 django_sync_env-0.2.9/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.2.9/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.2.9/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.2.9/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.2.9/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5237 2024-02-07 19:58:44.770356 django_sync_env-0.2.9/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     2467 2024-02-07 21:28:28.097749 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.2.9/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1634 2024-02-07 19:58:44.772377 django_sync_env-0.2.9/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.2.9/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.2.9/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14531 2024-02-07 19:58:44.773054 django_sync_env-0.2.9/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 django_sync_env-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-04-10 02:17:37.067178 django_sync_env-0.3.0/README.md
+-rw-r--r--   0        0        0      497 2024-04-10 02:21:08.041198 django_sync_env-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-10 02:17:37.069573 django_sync_env-0.3.0/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-04-10 02:17:37.069705 django_sync_env-0.3.0/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      941 2024-04-10 02:17:37.069823 django_sync_env-0.3.0/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      194 2024-04-10 02:17:37.069930 django_sync_env-0.3.0/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:17:37.070048 django_sync_env-0.3.0/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-04-10 02:17:37.070328 django_sync_env-0.3.0/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-04-10 02:17:37.070503 django_sync_env-0.3.0/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-04-10 02:17:37.070659 django_sync_env-0.3.0/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-04-10 02:17:37.070809 django_sync_env-0.3.0/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     5116 2024-04-10 03:54:56.625179 django_sync_env-0.3.0/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-04-10 02:17:37.071078 django_sync_env-0.3.0/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-04-10 02:17:37.071194 django_sync_env-0.3.0/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:17:37.071310 django_sync_env-0.3.0/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:17:37.071665 django_sync_env-0.3.0/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5237 2024-04-10 02:17:37.072154 django_sync_env-0.3.0/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-04-10 02:17:37.072564 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-04-10 02:17:37.072820 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     5758 2024-04-10 03:29:10.073282 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_download_db.py
+-rw-r--r--   0        0        0     2467 2024-04-10 02:17:37.072996 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2386 2024-04-10 02:17:37.073125 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-04-10 02:17:37.073512 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-04-10 02:17:37.073807 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-04-10 02:17:37.074063 django_sync_env-0.3.0/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1634 2024-04-10 02:59:23.723343 django_sync_env-0.3.0/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-04-10 02:17:37.074329 django_sync_env-0.3.0/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-04-10 02:17:37.074407 django_sync_env-0.3.0/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14531 2024-04-10 02:17:37.074621 django_sync_env-0.3.0/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 django_sync_env-0.3.0/PKG-INFO
```

### Comparing `django_sync_env-0.2.9/README.md` & `django_sync_env-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/checks.py` & `django_sync_env-0.3.0/src/django_sync_env/checks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/db/base.py` & `django_sync_env-0.3.0/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.3.0/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/db/mysql.py` & `django_sync_env-0.3.0/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.3.0/src/django_sync_env/db/postgresql.py`

 * *Files 18% similar despite different names*

```diff
@@ -110,18 +110,49 @@
             cmd += f" --exclude-table-data={table}"
         cmd = f"{self.dump_prefix} {cmd} {self.dump_suffix}"
         # logger.info(cmd)
         stdout, stderr = self.run_command(cmd, env=self.dump_env)
         return stdout
 
     def _restore_dump(self, dump):
-        dbname = create_postgres_uri(self)
-        cmd = f"{self.restore_cmd} {dbname} --clean --if-exists --no-owner"
+        connection_string = create_postgres_uri(self)
+        cmd = f"{self.restore_cmd} {connection_string} --clean --if-exists --no-owner"
 
         if self.single_transaction:
             cmd += " --single-transaction"
         if self.drop:
             cmd += ""
         cmd = f"{self.restore_prefix} {cmd} {self.restore_suffix}"
-        # logger.info(cmd)
+
+        # Drop the PUBLIC schema first
+        try:
+            self._drop_schema()
+        except:
+            logger.info("failed to drop public schema")
+
+        try:
+            self._create_schema()
+        except:
+            logger.info("recreate public schema")
+
         stdout, stderr = self.run_command(cmd, stdin=dump, env=self.restore_env)
         return stdout, stderr
+
+
+    def _drop_schema(self, schema_name='PUBLIC', cascade=True):
+        connection_string = create_postgres_uri(self)
+        if cascade:
+            cmd = f'psql {connection_string} -c "DROP SCHEMA {schema_name} CASCADE;"'
+        else:
+            cmd = f'psql {connection_string} -c "DROP SCHEMA {schema_name};"'
+
+        cmd = f"{self.restore_prefix} {cmd} {self.restore_suffix}"
+        # logger.info(cmd)
+        stdout, stderr = self.run_command(cmd, env=self.restore_env)
+        return stdout, stderr
+
+    def _create_schema(self, schema_name='PUBLIC'):
+        connection_string = create_postgres_uri(self)
+        cmd = f'psql {connection_string} -c "CREATE SCHEMA {schema_name};"'
+        cmd = f"{self.restore_prefix} {cmd} {self.restore_suffix}"
+        stdout, stderr = self.run_command(cmd, env=self.restore_env)
+        return stdout, stderr
```

### Comparing `django_sync_env-0.2.9/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.3.0/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.3.0/src/django_sync_env/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/notifications.py` & `django_sync_env-0.3.0/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/settings.py` & `django_sync_env-0.3.0/src/django_sync_env/settings.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/storage.py` & `django_sync_env-0.3.0/src/django_sync_env/storage.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/tasks.py` & `django_sync_env-0.3.0/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/src/django_sync_env/utils.py` & `django_sync_env-0.3.0/src/django_sync_env/utils.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.2.9/PKG-INFO` & `django_sync_env-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.2.9
+Version: 0.3.0
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

