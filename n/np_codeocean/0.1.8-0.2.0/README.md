# Comparing `tmp/np_codeocean-0.1.8.tar.gz` & `tmp/np_codeocean-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_codeocean-0.1.8.tar", last modified: Wed Apr 10 01:56:31 2024, max compression
+gzip compressed data, was "np_codeocean-0.2.0.tar", last modified: Sat Mar 30 00:10:12 2024, max compression
```

## Comparing `np_codeocean-0.1.8.tar` & `np_codeocean-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1425 2024-02-28 19:38:59.404591 np_codeocean-0.1.8/README.md
--rw-r--r--   0        0        0     1858 2024-04-10 01:56:31.353759 np_codeocean-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       66 2023-05-29 21:03:14.073762 np_codeocean-0.1.8/src/np_codeocean/__init__.py
--rw-r--r--   0        0        0     1490 2024-02-28 17:53:06.971522 np_codeocean-0.1.8/src/np_codeocean/scripts/upload_sessions.py
--rw-r--r--   0        0        0    17487 2024-04-10 01:55:26.471754 np_codeocean-0.1.8/src/np_codeocean/upload.py
--rw-r--r--   0        0        0     7367 2023-12-13 23:57:38.208900 np_codeocean-0.1.8/src/np_codeocean/upload_one.py
--rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.8/src/np_codeocean/utils.py
--rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 np_codeocean-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1425 2024-02-28 19:38:59.404591 np_codeocean-0.2.0/README.md
+-rw-r--r--   0        0        0     1858 2024-03-30 00:10:12.491322 np_codeocean-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-05-29 21:03:14.073762 np_codeocean-0.2.0/src/np_codeocean/__init__.py
+-rw-r--r--   0        0        0     1490 2024-02-28 17:53:06.971522 np_codeocean-0.2.0/src/np_codeocean/scripts/upload_sessions.py
+-rw-r--r--   0        0        0    15972 2024-03-29 23:27:35.146819 np_codeocean-0.2.0/src/np_codeocean/upload.py
+-rw-r--r--   0        0        0     7367 2023-12-13 23:57:38.208900 np_codeocean-0.2.0/src/np_codeocean/upload_one.py
+-rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.2.0/src/np_codeocean/utils.py
+-rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 np_codeocean-0.2.0/PKG-INFO
```

### Comparing `np_codeocean-0.1.8/README.md` & `np_codeocean-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.8/pyproject.toml` & `np_codeocean-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 composite = [
     "bump",
     "pdm publish",
 ]
 
 [project]
 name = "np_codeocean"
-version = "0.1.8"
+version = "0.2.0"
 description = "Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean"
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np_session>=0.6.4",
     "np-tools>=0.1.21",
```

### Comparing `np_codeocean-0.1.8/src/np_codeocean/scripts/upload_sessions.py` & `np_codeocean-0.2.0/src/np_codeocean/scripts/upload_sessions.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.8/src/np_codeocean/upload.py` & `np_codeocean-0.2.0/src/np_codeocean/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,58 +79,30 @@
     logger.info(f'Creating symlinks to raw ephys data files in {root_path}...')
     for abs_path, rel_path in np_tools.get_filtered_ephys_paths_relative_to_record_node_parents(
         root_path, specific_recording_dir_names=recording_dirs
         ):
         if not abs_path.is_dir():
             np_tools.symlink(as_posix(abs_path), dest / rel_path)
     logger.debug(f'Finished creating symlinks to raw ephys data files in {root_path}')
-    correct_structure(dest)
-
-def correct_structure(dest: Path) -> None:
-    """
-    In case some probes are missing, remove device entries from structure.oebin
-    files for devices with folders that have not been preserved.
-    """
-    logger.debug('Checking structure.oebin for missing folders...')
-    recording_dirs = dest.rglob('recording[0-9]')
-    for recording_dir in recording_dirs:
-        if not recording_dir.is_dir():
-            continue
-        oebin_path = recording_dir / 'structure.oebin'
-        if not (oebin_path.is_symlink() or oebin_path.exists()):
-            logger.warning(f'No structure.oebin found in {recording_dir}')
-            continue
-        logger.debug(f'Examining oebin: {oebin_path} for correction')
-        oebin_obj = np_tools.read_oebin(np_config.normalize_path(oebin_path.readlink()))
-        any_removed = False
-        for subdir_name in ('events', 'continuous'):    
-            subdir = oebin_path.parent / subdir_name
-            # iterate over copy of list so as to not disrupt iteration when elements are removed
-            for device in [device for device in oebin_obj[subdir_name]]:
-                if not (subdir / device['folder_name']).exists():
-                    logger.info(f'{device["folder_name"]} not found in {subdir}, removing from structure.oebin')
-                    oebin_obj[subdir_name].remove(device)
-                    any_removed = True
-        if any_removed:
-            oebin_path.unlink()
-            oebin_path.write_text(json.dumps(oebin_obj, indent=4))
-            logger.debug('Overwrote symlink to structure.oebin with corrected strcuture.oebin')
 
 def is_behavior_video_file(path: Path) -> bool:
     if path.is_dir() or path.suffix not in ('.mp4', '.avi', '.json'):
         return False
     with contextlib.suppress(ValueError):
         _ = npc_session.extract_mvr_camera_name(path.as_posix())
         return True
     return False
 
-def create_behavior_symlinks(session: np_session.Session, dest: Path) -> None:
+def create_behavior_symlinks(session: np_session.Session, dest: Path | None) -> None:
     """Create symlinks in `dest` pointing to files in top-level of session
     folder on np-exp, plus all files in `exp` subfolder, if present.
     """
+    if dest is None: 
+        logger.debug(f"No behavior folder supplied for {session}")
+        return
     subfolder_names = ('exp', 'qc')
     logger.info(f'Creating symlinks in {dest} to files in {session.npexp_path}...')
     for src in session.npexp_path.glob('*'):
         if not src.is_dir() and not is_behavior_video_file(src):
             np_tools.symlink(as_posix(src), dest / src.relative_to(session.npexp_path))
     logger.debug(f'Finished creating symlinks to top-level files in {session.npexp_path}')
 
@@ -139,18 +111,21 @@
         if not subfolder.exists():
             continue
         for src in subfolder.rglob('*'):
             if not src.is_dir():
                 np_tools.symlink(as_posix(src), dest / src.relative_to(session.npexp_path))
         logger.debug(f'Finished creating symlinks to {name!r} files')
 
-def create_behavior_videos_symlinks(session: np_session.Session, dest: Path) -> None:
+def create_behavior_videos_symlinks(session: np_session.Session, dest: Path | None) -> None:
     """Create symlinks in `dest` pointing to MVR video files and info jsons in top-level of session
     folder on np-exp.
     """
+    if dest is None: 
+        logger.debug(f"No behavior_videos folder supplied for {session}")
+        return
     logger.info(f'Creating symlinks in {dest} to files in {session.npexp_path}...')
     for src in session.npexp_path.glob('*'):
         if is_behavior_video_file(src):
             np_tools.symlink(as_posix(src), dest / src.relative_to(session.npexp_path))
     logger.debug(f'Finished creating symlinks to behavior video files in {session.npexp_path}')
     
 def is_surface_channel_recording(path_name: str) -> bool:
@@ -338,20 +313,18 @@
         session = session, 
         behavior = behavior,
         behavior_videos = behavior_videos,
         ephys = np_config.normalize_path(root / 'ephys') if is_ephys_session(session) else None,
         job = np_config.normalize_path(root / 'upload.csv'),
         force_cloud_sync=force_cloud_sync,
         )
-    if upload.ephys:
-        create_ephys_symlinks(upload.session, upload.ephys, recording_dirs=recording_dirs)
-    if upload.behavior:
-        create_behavior_symlinks(upload.session, upload.behavior)
-    if upload.behavior_videos:
-        create_behavior_videos_symlinks(upload.session, upload.behavior_videos)
+
+    create_ephys_symlinks(upload.session, upload.ephys, recording_dirs=recording_dirs)
+    create_behavior_symlinks(upload.session, upload.behavior)
+    create_behavior_videos_symlinks(upload.session, upload.behavior_videos)
     create_upload_job(upload)    
     return upload
 
 def upload_session(session: str | int | pathlib.Path | np_session.Session, 
                    recording_dirs: Iterable[str] | None = None,
                    force: bool = False,
                    ) -> None:
```

### Comparing `np_codeocean-0.1.8/src/np_codeocean/upload_one.py` & `np_codeocean-0.2.0/src/np_codeocean/upload_one.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.8/src/np_codeocean/utils.py` & `np_codeocean-0.2.0/src/np_codeocean/utils.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.8/PKG-INFO` & `np_codeocean-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np_codeocean
-Version: 0.1.8
+Version: 0.2.0
 Summary: Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

