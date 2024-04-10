# Comparing `tmp/pih-file-0.1.tar.gz` & `tmp/pih-file-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-file-0.1.tar", last modified: Mon Feb 26 08:59:48 2024, max compression
+gzip compressed data, was "pih-file-0.11.tar", last modified: Wed Apr 10 01:41:32 2024, max compression
```

## Comparing `pih-file-0.1.tar` & `pih-file-0.11.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 08:59:49.022139 pih-file-0.1/
-drwxrwxrwx   0        0        0        0 2024-02-26 08:59:48.444038 pih-file-0.1/FileWatchdogService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-file-0.1/FileWatchdogService/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-15 01:20:33.000000 pih-file-0.1/FileWatchdogService/__main__.py
--rw-rw-rw-   0        0        0      509 2024-02-26 08:55:15.000000 pih-file-0.1/FileWatchdogService/const.py
--rw-rw-rw-   0        0        0     3912 2024-02-25 05:29:07.000000 pih-file-0.1/FileWatchdogService/service.py
--rw-rw-rw-   0        0        0      251 2024-02-26 08:59:49.022139 pih-file-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-15 01:18:41.000000 pih-file-0.1/file_build.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:59:48.959638 pih-file-0.1/pih_file.egg-info/
--rw-rw-rw-   0        0        0      251 2024-02-26 08:59:47.000000 pih-file-0.1/pih_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-02-26 08:59:47.000000 pih-file-0.1/pih_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 08:59:47.000000 pih-file-0.1/pih_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-02-26 08:59:47.000000 pih-file-0.1/pih_file.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-02-26 08:59:47.000000 pih-file-0.1/pih_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-26 08:59:47.000000 pih-file-0.1/pih_file.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 08:59:49.022139 pih-file-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:41:32.907974 pih-file-0.11/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:41:32.437116 pih-file-0.11/FileWatchdogService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-file-0.11/FileWatchdogService/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-02-15 01:20:33.000000 pih-file-0.11/FileWatchdogService/__main__.py
+-rw-rw-rw-   0        0        0      510 2024-04-10 00:01:38.000000 pih-file-0.11/FileWatchdogService/const.py
+-rw-rw-rw-   0        0        0     3847 2024-03-14 22:53:57.000000 pih-file-0.11/FileWatchdogService/service.py
+-rw-rw-rw-   0        0        0      298 2024-04-10 01:41:32.875697 pih-file-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:41:32.844456 pih-file-0.11/pih_file.egg-info/
+-rw-rw-rw-   0        0        0      298 2024-04-10 01:41:31.000000 pih-file-0.11/pih_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 01:41:32.000000 pih-file-0.11/pih_file.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:41:32.923620 pih-file-0.11/setup.cfg
```

### Comparing `pih-file-0.1/FileWatchdogService/service.py` & `pih-file-0.11/FileWatchdogService/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         from watchdog.events import FileSystemEventHandler, FileSystemEvent
 
         path_list: list[str] = []
         host_info_map: dict[str, HostInfo] = {}
         observer_map: dict[str, Observer] = {}  # type: ignore
 
         def on_new_file(value: str) -> None:
-            #A.PTH.save_timestamp_for_directory_info(file_path)
             A.E.new_file_detected(value)
 
         class Handler(FileSystemEventHandler):
             def on_created(self, event: FileSystemEvent):
                 if not event.is_directory:
                     on_new_file(A.PTH.path(event.src_path))
```

