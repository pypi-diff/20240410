# Comparing `tmp/incremental_backup-1.1.0.tar.gz` & `tmp/incremental_backup-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incremental_backup-1.1.0.tar", last modified: Thu Apr  4 09:57:56 2024, max compression
+gzip compressed data, was "incremental_backup-1.2.0.tar", last modified: Wed Apr 10 11:19:28 2024, max compression
```

## Comparing `incremental_backup-1.1.0.tar` & `incremental_backup-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/_utility/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/_utility/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/_utility/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/sum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/incremental_backup/cli/command/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/incremental_backup/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/complete_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/start_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/path_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/prune.py
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/restore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/incremental_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/test/test_path_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/test/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)    26292 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/test/test_restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.978950 incremental_backup-1.2.0/incremental_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/_utility/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/_utility/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/sum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/cli/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/complete_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/start_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/path_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/incremental_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/test/test_path_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/test/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26292 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/test/test_restore.py
```

### Comparing `incremental_backup-1.1.0/LICENCE.txt` & `incremental_backup-1.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/PKG-INFO` & `incremental_backup-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incremental_backup
-Version: 1.1.0
+Version: 1.2.0
 Summary: Incremental file backup tool
 Author-email: Reece Jones <reece.jones131@gmail.com>
 Project-URL: Homepage, https://github.com/MC-DeltaT/IncrementalBackup2
 Project-URL: Issues, https://github.com/MC-DeltaT/IncrementalBackup2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `incremental_backup-1.1.0/README.md` & `incremental_backup-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/backup/backup.py` & `incremental_backup-1.2.0/incremental_backup/backup/backup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Callable, Iterable, Optional, Sequence
+from typing import Callable, Iterable, Optional, overload, Sequence
 
 from incremental_backup.backup.filesystem import scan_filesystem, ScanFilesystemCallbacks
-from incremental_backup.backup.plan import BackupPlan, execute_backup_plan, ExecuteBackupPlanCallbacks
+from incremental_backup.backup.plan import BackupPlan, execute_backup_plan, ExecuteBackupPlanCallbacks, \
+    ExecuteBackupPlanResults
 from incremental_backup.backup.sum import BackupSum
 from incremental_backup.meta import BackupCompleteInfo, BackupDirectoryCreationError, BackupManifest, \
     BackupMetadata, BackupStartInfo, COMPLETE_INFO_FILENAME, create_new_backup_directory, \
     DATA_DIRECTORY_NAME, MANIFEST_FILENAME, read_backups, ReadBackupsCallbacks, START_INFO_FILENAME, \
     write_backup_complete_info_file, write_backup_manifest_file, write_backup_start_info_file
 from incremental_backup.path_exclude import PathExcludePattern
 from incremental_backup._utility import StrPath
@@ -71,90 +72,102 @@
     """Called just before saving the manifest and completion information to file."""
 
     on_write_complete_info_error: Callable[[Path, OSError], None] = lambda path, error: None
     """Called when writing the backup completion information file fails.
         First argument is the path to the file, second argument is the raised exception."""
 
 
+@overload
 def perform_backup(source_directory: StrPath, target_directory: StrPath, exclude_patterns: Iterable[PathExcludePattern],
                    callbacks: BackupCallbacks = BackupCallbacks()) -> BackupResults:
+    ...
+
+@overload
+def perform_backup(source_directory: StrPath, target_directory: StrPath, exclude_patterns: Iterable[PathExcludePattern],
+                   callbacks: BackupCallbacks = BackupCallbacks(), skip_empty: bool = False) -> Optional[BackupResults]:
+    ...
+
+# TODO: clean up this interface. Have an "options" object argument rather than overloads
+def perform_backup(source_directory: StrPath, target_directory: StrPath, exclude_patterns: Iterable[PathExcludePattern],
+                   callbacks: BackupCallbacks = BackupCallbacks(), skip_empty: bool = False) -> Optional[BackupResults]:
     """Performs the entire operation of creating a new backup, including creating the backup directory, copying files,
         and saving metadata.
 
         :param source_directory: Directory to back up.
         :param target_directory: Directory to create the new backup in, and where any previous backups are read from.
             Need not exist.
         :param exclude_patterns: Patterns to match paths which will be excluded from the backup.
         :param callbacks: Callbacks for certain events during execution. See `BackupCallbacks`.
-        :return: Metadata and summary information for the backup operation.
+        :param skip_empty: Only perform the backup if there are file changes to record.
+        :return: Metadata and summary information for the backup operation. None if the backup was skipped.
         :except BackupError: If an error occurs that prevents the backup operation from creating a valid backup. See
             `BackupError`.
     """
 
-    return _BackupOperation(source_directory, target_directory, exclude_patterns, callbacks).perform_backup()
+    return _BackupOperation(source_directory, target_directory, exclude_patterns, skip_empty, callbacks).perform_backup()
 
 
 class _BackupOperation:
     """Implementation of the backup creation operation."""
 
     def __init__(self, source_directory: StrPath, target_directory: StrPath,
-                 exclude_patterns: Iterable[PathExcludePattern], callbacks: BackupCallbacks = BackupCallbacks()) -> None:
+                 exclude_patterns: Iterable[PathExcludePattern], skip_empty: bool,
+                 callbacks: BackupCallbacks = BackupCallbacks()) -> None:
         self.source_directory = Path(source_directory)
         self.target_directory = Path(target_directory)
         self.exclude_patterns = tuple(exclude_patterns)
+        self.skip_empty = skip_empty
         self.callbacks = callbacks
 
         self._init_working_state()
 
-    def perform_backup(self) -> BackupResults:
+    def perform_backup(self) -> Optional[BackupResults]:
         """Creates a new backup.
 
             :except BackupError: If an error occurs that prevents the backup operation from creating a valid backup. See
                 `BackupError`.
         """
 
         self._init_working_state()
 
         self._validate_source_directory()
         self._validate_target_directory()
 
         previous_backups = self._read_previous_backups()
         backup_sum = BackupSum.from_backups(previous_backups)
 
-        (self.callbacks.on_before_initialise_backup)()
-        self._create_backup_directory()
-        assert self.backup_path is not None
-        data_path = self._create_data_directory(self.backup_path)
-        self._create_start_info()
+        start_time = datetime.now(timezone.utc)
+        if not self.skip_empty:
+            # If skip_empty is not specified, keep the old behaviour.
+            # If skip_empty is true, have to defer creating the backup till we know it's not empty.
+            backup_path, data_path, start_info = self._initialise_backup(start_time)
 
         backup_plan = self._compute_backup_plan(backup_sum)
-        self._back_up_files(data_path, backup_plan)
 
-        (self.callbacks.on_before_save_metadata)()
-        self._save_manifest()
-        self._save_complete_info()
-
-        assert self.start_info is not None
-        assert self.manifest is not None
-        assert self.complete_info is not None
-        assert self.files_copied is not None
-        assert self.files_removed is not None
+        if self.skip_empty:
+            if self._is_backup_plan_empty(backup_plan):
+                return None
+
+            backup_path, data_path, start_info = self._initialise_backup(start_time)
+
+        execute_results = self._back_up_files(data_path, backup_plan)
+        complete_info = self._create_complete_info()
+
+        self.callbacks.on_before_save_metadata()
+        self._save_manifest(backup_path, execute_results.manifest)
+        self._save_complete_info(backup_path, complete_info)
+
         return BackupResults(
-            self.backup_path, self.start_info, self.manifest, self.complete_info, self.files_copied, self.files_removed)
+            backup_path, start_info, execute_results.manifest, complete_info, execute_results.files_copied,
+            execute_results.files_removed)
 
     def _init_working_state(self) -> None:
         """Initialises various shared data used by and operated on by the methods in this class."""
 
-        self.backup_path: Optional[Path] = None
-        self.start_info: Optional[BackupStartInfo] = None
-        self.manifest: Optional[BackupManifest] = None
-        self.complete_info: Optional[BackupCompleteInfo] = None
-        self.paths_skipped: Optional[bool] = None
-        self.files_copied: Optional[int] = None
-        self.files_removed: Optional[int] = None
+        self.paths_skipped = False
 
     def _validate_source_directory(self) -> None:
         """Validates the backup source directory.
             Should mostly prevent other parts of the backup operation from failing strangely for invalid inputs.
 
             :except BackupError: If the source directory is not an accessible directory.
         """
@@ -184,44 +197,64 @@
         """Reads existing backups' metadata from the backup target directory.
 
             If any backup's metadata cannot be read, skips that backup.
 
             :except BackupError: If the target directory cannot be enumerated.
         """
 
-        (self.callbacks.on_before_read_previous_backups)()
+        self.callbacks.on_before_read_previous_backups()
 
         try:
             if not self.target_directory.exists():
                 backups = []
             else:
                 backups = read_backups(self.target_directory, self.callbacks.read_backups)
         except OSError as e:
             raise BackupError(f'Failed to enumerate target directory: {e}') from e
         backups = tuple(backups)
 
-        (self.callbacks.on_after_read_previous_backups)(backups)
+        self.callbacks.on_after_read_previous_backups(backups)
 
         return backups
 
-    def _create_backup_directory(self) -> None:
+    def _initialise_backup(self, start_time: datetime) -> tuple[Path, Path, BackupStartInfo]:
+        """Creates the backup directory and start info file.
+
+            :return: Tuple of (backup_path, data_path, start_info).
+            :except BackupError: If a fatal error occurs.
+        """
+
+        self.callbacks.on_before_initialise_backup()
+        backup_path = self._create_backup_directory()
+        data_path = self._create_data_directory(backup_path)
+        start_info = self._create_and_write_start_info(backup_path, start_time)
+        return backup_path, data_path, start_info
+
+    @staticmethod
+    def _is_backup_plan_empty(backup_plan: BackupPlan) -> bool:
+        root = backup_plan.root
+        return not (root.copied_files or root.removed_files or root.removed_directories or root.subdirectories
+            or root.contains_copied_files or root.contains_removed_items or root.removed_directory_file_count)
+
+    def _create_backup_directory(self) -> Path:
         """Creates a new backup directory within the target directory.
 
             :except BackupError: If the directory could not be created.
         """
 
         try:
             backup_name = create_new_backup_directory(self.target_directory)
         except BackupDirectoryCreationError as e:
             raise BackupError(str(e)) from e
 
         backup_path = self.target_directory / backup_name
-        self.backup_path = backup_path
 
-        (self.callbacks.on_created_backup_directory)(backup_path)
+        self.callbacks.on_created_backup_directory(backup_path)
+
+        return backup_path
 
     @staticmethod
     def _create_data_directory(backup_path: Path, /) -> Path:
         """Creates the backup data directory (directory which contains the copied files).
 
             :return: Path to the created directory.
             :except BackupError: If the directory could not be created.
@@ -230,81 +263,79 @@
         path = backup_path / DATA_DIRECTORY_NAME
         try:
             path.mkdir(parents=True, exist_ok=False)
         except OSError as e:
             raise BackupError(f'Failed to create backup data directory: {e}') from e
         return path
 
-    def _create_start_info(self) -> None:
+    @staticmethod
+    def _create_and_write_start_info(backup_path: Path, start_time: datetime) -> BackupStartInfo:
         """Creates and writes the backup start information to file within the backup directory.
 
             :except BackupError: If the file could not be written to.
         """
 
-        start_info = BackupStartInfo(datetime.now(timezone.utc))
-        self.start_info = start_info
-        assert self.backup_path is not None
-        file_path = self.backup_path / START_INFO_FILENAME
+        start_info = BackupStartInfo(start_time)
+        file_path = backup_path / START_INFO_FILENAME
         try:
             write_backup_start_info_file(file_path, start_info)
         except OSError as e:
             raise BackupError(f'Failed to write backup start information file: {e}') from e
+        return start_info
 
     def _compute_backup_plan(self, backup_sum: BackupSum) -> BackupPlan:
         """Scans the source directory and generates the backup plan."""
 
-        (self.callbacks.on_before_scan_source)()
+        self.callbacks.on_before_scan_source()
 
         scan_results = scan_filesystem(self.source_directory, self.exclude_patterns, self.callbacks.scan_source)
         self.paths_skipped = self.paths_skipped or scan_results.paths_skipped
         backup_plan = BackupPlan.new(scan_results.tree, backup_sum)
         return backup_plan
 
-    def _back_up_files(self, destination_path: StrPath, backup_plan: BackupPlan) -> None:
+    def _back_up_files(self, destination_path: StrPath, backup_plan: BackupPlan) -> ExecuteBackupPlanResults:
         """Backs up files from the source directory to the backup directory according to the backup plan."""
 
-        (self.callbacks.on_before_copy_files)()
+        self.callbacks.on_before_copy_files()
 
         execute_results = execute_backup_plan(
             backup_plan, self.source_directory, destination_path, self.callbacks.execute_plan)
 
         self.paths_skipped = self.paths_skipped or execute_results.paths_skipped
-        self.manifest = execute_results.manifest
-        self.complete_info = BackupCompleteInfo(datetime.now(timezone.utc), self.paths_skipped)
-        self.files_copied = execute_results.files_copied
-        self.files_removed = execute_results.files_removed
 
-    def _save_manifest(self) -> None:
+        return execute_results
+
+    def _create_complete_info(self) -> BackupCompleteInfo:
+        return BackupCompleteInfo(datetime.now(timezone.utc), self.paths_skipped)
+
+    @staticmethod
+    def _save_manifest(backup_path: Path, manifest: BackupManifest) -> None:
         """Writes the backup manifest to file within the backup directory.
 
             :except BackupError: If the file could not be written to.
         """
 
-        assert self.backup_path is not None
-        file_path = self.backup_path / MANIFEST_FILENAME
+        file_path = backup_path / MANIFEST_FILENAME
         try:
-            assert self.manifest is not None
-            write_backup_manifest_file(file_path, self.manifest)
+            write_backup_manifest_file(file_path, manifest)
         except OSError as e:
             raise BackupError(f'Failed to write backup manifest file: {e}') from e
 
-    def _save_complete_info(self) -> None:
+    def _save_complete_info(self, backup_path: Path, complete_info: BackupCompleteInfo) -> None:
         """Writes the backup completion information to file within the backup directory.
 
             It is not a fatal error if this operation fails, since the completion information is not required by the
             application at this time."""
 
-        assert self.backup_path is not None
-        file_path = self.backup_path / COMPLETE_INFO_FILENAME
+        file_path = backup_path / COMPLETE_INFO_FILENAME
         try:
-            assert self.complete_info is not None
-            write_backup_complete_info_file(file_path, self.complete_info)
+            write_backup_complete_info_file(file_path, complete_info)
         except OSError as e:
             # Not fatal since the completion info isn't currently used by the software.
-            (self.callbacks.on_write_complete_info_error)(file_path, e)
+            self.callbacks.on_write_complete_info_error(file_path, e)
 
 
 class BackupError(Exception):
     """Raised when creating a backup fails such that a valid backup cannot be produced.
 
         Some cases where this exception is raised:
          - The source directory cannot be accessed at all.
```

### Comparing `incremental_backup-1.1.0/incremental_backup/backup/filesystem.py` & `incremental_backup-1.2.0/incremental_backup/backup/filesystem.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/backup/plan.py` & `incremental_backup-1.2.0/incremental_backup/backup/plan.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/backup/sum.py` & `incremental_backup-1.2.0/incremental_backup/backup/sum.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/cli/command/backup.py` & `incremental_backup-1.2.0/incremental_backup/cli/command/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 from pathlib import Path
-from typing import Sequence
+from typing import Optional, Sequence
 
 from incremental_backup.backup import BackupCallbacks, BackupError, BackupResults, ExecuteBackupPlanCallbacks, \
     perform_backup, ScanFilesystemCallbacks
 from incremental_backup.cli.command.command import Command
 from incremental_backup.cli.command.exception import CommandRuntimeError
 from incremental_backup.meta import ReadBackupsCallbacks
 from incremental_backup.path_exclude import PathExcludePattern
@@ -27,37 +27,41 @@
 
         parser = subparser.add_parser(
             BackupCommand.COMMAND_STRING, description='Creates a new backup.', help='Creates a new backup.')
         parser.add_argument('source_dir', type=Path, help='Directory to back up.')
         parser.add_argument('target_dir', type=Path, help='Directory to back up into.')
         parser.add_argument(
             '--exclude', nargs='+', type=PathExcludePattern, required=False, help='Path patterns to exclude.')
+        parser.add_argument('--skip-empty', action='store_true', default=False,
+            help='Only back up if there are file changes to record.')
 
     def __init__(self, arguments: argparse.Namespace, /) -> None:
         """
             :param arguments: The parsed command line arguments object acquired from argparse.
         """
 
         super().__init__(arguments)
         self.source_path: Path = arguments.source_dir
         self.target_path: Path = arguments.target_dir
         self.exclude_patterns: Sequence[PathExcludePattern] = arguments.exclude or ()
+        self.skip_empty: bool = arguments.skip_empty
 
     def run(self) -> None:
         """Executes the backup command.
 
             :except CommandRuntimeError: If an error occurs such that a valid backup cannot be produced.
         """
 
         self._print_config()
 
         callbacks = self._backup_callbacks()
 
         try:
-            results = perform_backup(self.source_path, self.target_path, self.exclude_patterns, callbacks)
+            results = perform_backup(
+                self.source_path, self.target_path, self.exclude_patterns, callbacks, self.skip_empty)
         except BackupError as e:
             raise CommandRuntimeError(str(e)) from e
 
         self._print_results(results)
 
     @staticmethod
     def _backup_callbacks() -> BackupCallbacks:
@@ -98,14 +102,20 @@
         print(f'Target directory: {self.target_path}')
         print('Exclude patterns:')
         if self.exclude_patterns:
             for pattern in self.exclude_patterns:
                 print(f'  {pattern}')
         else:
             print('  <none>')
+        if self.skip_empty:
+            print('Skip empty backup: yes')
         print()
 
     @staticmethod
-    def _print_results(results: BackupResults, /) -> None:
+    def _print_results(results: Optional[BackupResults], /) -> None:
         """Prints backup results to the console."""
 
-        print(f'+{results.files_copied} / -{results.files_removed} files')
+        files_copied = results.files_copied if results else 0
+        files_removed = results.files_removed if results else 0
+        print(f'+{files_copied} / -{files_removed} files')
+        if results is None:
+            print('Skipping empty backup')
```

### Comparing `incremental_backup-1.1.0/incremental_backup/cli/command/command.py` & `incremental_backup-1.2.0/incremental_backup/cli/command/command.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/cli/command/exception.py` & `incremental_backup-1.2.0/incremental_backup/cli/command/exception.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/cli/command/prune.py` & `incremental_backup-1.2.0/incremental_backup/cli/command/prune.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/cli/command/registry.py` & `incremental_backup-1.2.0/incremental_backup/cli/command/registry.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/cli/command/restore.py` & `incremental_backup-1.2.0/incremental_backup/cli/command/restore.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/cli/main.py` & `incremental_backup-1.2.0/incremental_backup/cli/main.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/meta/complete_info.py` & `incremental_backup-1.2.0/incremental_backup/meta/complete_info.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/meta/manifest.py` & `incremental_backup-1.2.0/incremental_backup/meta/manifest.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/meta/meta.py` & `incremental_backup-1.2.0/incremental_backup/meta/meta.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/meta/start_info.py` & `incremental_backup-1.2.0/incremental_backup/meta/start_info.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/path_exclude.py` & `incremental_backup-1.2.0/incremental_backup/path_exclude.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/prune.py` & `incremental_backup-1.2.0/incremental_backup/prune.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup/restore.py` & `incremental_backup-1.2.0/incremental_backup/restore.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/incremental_backup.egg-info/PKG-INFO` & `incremental_backup-1.2.0/incremental_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incremental_backup
-Version: 1.1.0
+Version: 1.2.0
 Summary: Incremental file backup tool
 Author-email: Reece Jones <reece.jones131@gmail.com>
 Project-URL: Homepage, https://github.com/MC-DeltaT/IncrementalBackup2
 Project-URL: Issues, https://github.com/MC-DeltaT/IncrementalBackup2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `incremental_backup-1.1.0/incremental_backup.egg-info/SOURCES.txt` & `incremental_backup-1.2.0/incremental_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/pyproject.toml` & `incremental_backup-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "incremental_backup"
 # TODO: update when making changes.
-version = "1.1.0"
+version = "1.2.0"
 authors = [
     { name="Reece Jones", email="reece.jones131@gmail.com" }
 ]
 description = "Incremental file backup tool"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `incremental_backup-1.1.0/test/test_path_exclude.py` & `incremental_backup-1.2.0/test/test_path_exclude.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/test/test_prune.py` & `incremental_backup-1.2.0/test/test_prune.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.1.0/test/test_restore.py` & `incremental_backup-1.2.0/test/test_restore.py`

 * *Files identical despite different names*

