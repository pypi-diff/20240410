# Comparing `tmp/work-1.1.0a0.tar.gz` & `tmp/work-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.1.0a0.tar", max compression
+gzip compressed data, was "work-1.1.0a1.tar", max compression
```

## Comparing `work-1.1.0a0.tar` & `work-1.1.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a0/README.md
--rw-r--r--   0        0        0      594 2024-04-09 13:51:26.037597 work-1.1.0a0/pyproject.toml
--rw-r--r--   0        0        0    89902 2024-04-09 13:51:26.045597 work-1.1.0a0/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a0/src/work_components/__init__.py
--rw-r--r--   0        0        0    24359 2024-04-08 19:32:29.849389 work-1.1.0a0/src/work_components/arguments.py
--rw-r--r--   0        0        0     2214 2024-04-09 13:51:26.037597 work-1.1.0a0/src/work_components/consts.py
--rw-r--r--   0        0        0    21865 2024-04-09 13:47:01.527495 work-1.1.0a0/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a0/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    16847 2024-04-09 13:51:26.029596 work-1.1.0a0/src/work_components/dao/core.py
--rw-r--r--   0        0        0      270 2024-04-08 19:32:29.853389 work-1.1.0a0/src/work_components/dao/env.py
--rw-r--r--   0        0        0     1643 2024-04-08 19:32:29.853389 work-1.1.0a0/src/work_components/dao/flags.py
--rw-r--r--   0        0        0    11503 2024-04-08 19:32:29.853389 work-1.1.0a0/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    11011 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     6212 2024-04-08 20:41:54.408996 work-1.1.0a0/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/migrate.py
--rw-r--r--   0        0        0      344 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/protocols.py
--rw-r--r--   0        0        0     1664 2024-04-09 13:47:01.531495 work-1.1.0a0/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8067 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/util.py
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 work-1.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a1/README.md
+-rw-r--r--   0        0        0      594 2024-04-10 09:59:43.930579 work-1.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0    89735 2024-04-10 09:59:27.238446 work-1.1.0a1/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a1/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24359 2024-04-08 19:32:29.849389 work-1.1.0a1/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2214 2024-04-10 09:59:38.582536 work-1.1.0a1/src/work_components/consts.py
+-rw-r--r--   0        0        0    21865 2024-04-09 13:47:01.527495 work-1.1.0a1/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a1/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    16847 2024-04-09 13:51:26.029596 work-1.1.0a1/src/work_components/dao/core.py
+-rw-r--r--   0        0        0      270 2024-04-08 19:32:29.853389 work-1.1.0a1/src/work_components/dao/env.py
+-rw-r--r--   0        0        0     1643 2024-04-08 19:32:29.853389 work-1.1.0a1/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0    11503 2024-04-08 19:32:29.853389 work-1.1.0a1/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    11011 2024-04-08 18:05:30.527145 work-1.1.0a1/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     6212 2024-04-08 20:41:54.408996 work-1.1.0a1/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a1/src/work_components/migrate.py
+-rw-r--r--   0        0        0      344 2024-04-08 18:05:30.527145 work-1.1.0a1/src/work_components/protocols.py
+-rw-r--r--   0        0        0     1664 2024-04-09 13:47:01.531495 work-1.1.0a1/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8067 2024-04-08 18:05:30.527145 work-1.1.0a1/src/work_components/util.py
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 work-1.1.0a1/PKG-INFO
```

### Comparing `work-1.1.0a0/README.md` & `work-1.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/pyproject.toml` & `work-1.1.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.1.0a0"
+version = "1.1.0a1"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.1.0a0/src/work.py` & `work-1.1.0a1/src/work.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,16 +322,14 @@
     ### Modes ###
 
     # start #
 
     def start(self, args) -> None:
         """Start the protocol based on the given arguments."""
 
-        raise NotImplementedError("END TIME 0")
-
         start_time: dt.datetime = self.get_single_time(args)
         self._start(start_time=start_time, force=args.force, dry_run=args.dry_run)
         print(f"Started work at {self._readable_dt(start_time)}")
 
     def ensure_valid_start_time(
         self,
         start_time: dt.datetime,
@@ -431,17 +429,14 @@
         return util.minutes_difference(start=start_time, end=end_time)
 
     # add #
 
     def add(self, args) -> None:
         """Add a protocol entry consisting of start time, end time and optional date flag."""
 
-        # raise NotImplementedError("END TIME 0")
-        print(" TODO TO DOJFS KFDJLK JSDL JFSD END TIME 0:00!!!!")
-
         start_time: dt.datetime
         end_time: dt.datetime
         baseline_date: dt.date = self.get_selected_date(args)
         start_time, end_time = self.get_time_from_and_to(args, baseline_date)
 
         self._can_i_add_this(
             start_time=start_time,
```

### Comparing `work-1.1.0a0/src/work_components/arguments.py` & `work-1.1.0a1/src/work_components/arguments.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/consts.py` & `work-1.1.0a1/src/work_components/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """ Shared constants """
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.1.0a0"
+VERSION: str = "1.1.0a1"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
```

### Comparing `work-1.1.0a0/src/work_components/container.py` & `work-1.1.0a1/src/work_components/container.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/dao/core.py` & `work-1.1.0a1/src/work_components/dao/core.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/dao/flags.py` & `work-1.1.0a1/src/work_components/dao/flags.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/dao/rc.py` & `work-1.1.0a1/src/work_components/dao/rc.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/dao/recess.py` & `work-1.1.0a1/src/work_components/dao/recess.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/dt_parse.py` & `work-1.1.0a1/src/work_components/dt_parse.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/migrate.py` & `work-1.1.0a1/src/work_components/migrate.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/timestamps.py` & `work-1.1.0a1/src/work_components/timestamps.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/src/work_components/util.py` & `work-1.1.0a1/src/work_components/util.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a0/PKG-INFO` & `work-1.1.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.1.0a0
+Version: 1.1.0a1
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

