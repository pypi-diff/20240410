# Comparing `tmp/hwdocer-0.2.1.tar.gz` & `tmp/hwdocer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwdocer-0.2.1.tar", max compression
+gzip compressed data, was "hwdocer-0.2.2.tar", max compression
```

## Comparing `hwdocer-0.2.1.tar` & `hwdocer-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     4495 2024-04-04 22:13:50.943539 hwdocer-0.2.1/doc/release.md
--rw-r--r--   0        0        0     1999 2024-04-04 22:18:33.910169 hwdocer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2845 2024-04-03 19:29:01.034792 hwdocer-0.2.1/readme.md
--rw-r--r--   0        0        0       22 2024-04-04 22:16:42.129870 hwdocer-0.2.1/src/hwdocer/__init__.py
--rw-r--r--   0        0        0      139 2024-03-25 19:30:35.876996 hwdocer-0.2.1/src/hwdocer/__main__.py
--rw-r--r--   0        0        0    18828 2024-04-04 22:11:19.220564 hwdocer-0.2.1/src/hwdocer/hwdocer.py
--rw-r--r--   0        0        0     4679 1970-01-01 00:00:00.000000 hwdocer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4925 2024-04-09 22:12:22.095166 hwdocer-0.2.2/doc/release.md
+-rw-r--r--   0        0        0     1994 2024-04-09 22:14:38.042548 hwdocer-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2845 2024-04-03 19:29:01.034792 hwdocer-0.2.2/readme.md
+-rw-r--r--   0        0        0       53 2024-04-09 22:04:28.591248 hwdocer-0.2.2/src/hwdocer/__init__.py
+-rw-r--r--   0        0        0      139 2024-03-25 19:30:35.876996 hwdocer-0.2.2/src/hwdocer/__main__.py
+-rw-r--r--   0        0        0    20568 2024-04-09 22:06:19.327487 hwdocer-0.2.2/src/hwdocer/hwdocer.py
+-rw-r--r--   0        0        0       18 2024-04-09 22:14:38.042548 hwdocer-0.2.2/src/hwdocer/version.py
+-rw-r--r--   0        0        0     4679 1970-01-01 00:00:00.000000 hwdocer-0.2.2/PKG-INFO
```

### Comparing `hwdocer-0.2.1/doc/release.md` & `hwdocer-0.2.2/doc/release.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,155 @@
 # HWDOCER releases
 
 See what is planned in the [roadmap][roadmap_file]
 
+## 0.2.2
+
+Release date: _2024-04-09_
+
+**Feature:**
+
+- progress bar now displayed in the console
+- added an argument to display software version
+
+**Fix:**
+
+- Segregated file searching and file copying into 2 steps
+
+**Known problem:**
+
+- leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
+- file copy fails to replicate the correct folder structure whit some input (media at same level as subfolder)
+
 ## 0.2.1
 
 Release date: _2024-04-04_
 
-**Features:**
+**Feature:**
 
 - change console output to rich python lib for better logging
 - minimal work stat printed & logged at execution end
 
 **Fix:**
 
 - change wireviz call to run and hopefully get more helpful verbose error (not much info from wireviz itself)
 
-**Known problems:**
+**Known problem:**
 
 - leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
 - file copy fails to replicate the correct folder structure whit some input (media at same level as subfolder)
 
 ## 0.2.0
 
 Release date: _2024-04-03_
 
-**Features:**
+**Feature:**
 
 - automatic removal of undesired file format (wireviz) in output folder (multiple can be kept via `--hrs` args)
 
 **Fix:**
 
 - wrapped wireviz and drawio call in silent subprocess to handle console pollution (unknown exception will still be raised)
 
-**Known problems:**
+**Known problem:**
 
 - leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
 - file copy fails to replicate the correct folder structure whit some input (media at same level as subfolder)
 
 ## 0.1.4
 
 Release date: _2024-04-02_
 
-**Features:**
+**Feature:**
 
 - source files are now copied in output folder
 - refactor the execution to be file based instead of process based
 - all building is now executed in isolated multiprocessor-compatible processes
 - added argument to control the number of processes created
 - added argument to limit the execution time
 - added argument to control the output files format (present but not used yet)
 
 **Fix:**
 
 - image from harnesses are now correctly copied into a similar folder structure inside output folder
 
-**Known problems:**
+**Known problem:**
 
 - **[corrected in 0.2.0]** drawio calls throws some error in console and logs
 - **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - **[corrected in 0.2.0]** leave a lot of undesired generated files in input and output folders
 - leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
 
 ## 0.1.3
 
 Release date: _2024-03-27_
 
-**Features:**
+**Feature:**
 
 - copy all images defined in harness with tag `image`.`src` to output path (for html correct render)
 
-**Known problems:**
+**Known problem:**
 
 - **[corrected in 0.2.0]** drawio calls throws some error in console and logs
 - **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - **[corrected in 0.1.4]** image copy doesn't recreate sub-folder structure into output destination
 - **[corrected in 0.2.0]** leave a lot of undesired generated files in input and output folders
 - leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
 
 ## 0.1.2
 
 Release date: _2024-03-27_
 
-**Features:**
+**Feature:**
 
 - Improve debug verbosity
 - Input file search is more iterative now
 
 **Change:**
 
 - Changed input file search to use glob instead of os.walk
 
-**Known problems:**
+**Known problem:**
 
 - **[corrected in 0.2.0]** drawio calls throws some error in console and logs
 - **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - **[corrected in 0.2.0]** leave a lot of undesired generated files in input and output folders
 - leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
 
 ## 0.1.1
 
 Release date: _2024-03-26_
 
 **Fix:**
 
 - Project publishing metadata added/corrected
 
-**Known problems:**
+**Known problem:**
 
 - **[corrected in 0.2.0]** drawio calls throws some error in console and logs
 - **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - **[corrected in 0.2.0]** leave a lot of undesired generated files in input and output folders
 - leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
 
 ## 0.1.0
 
 Release date: _2024-03-26_
 
-**Features:**
+**Feature:**
 
 - Initial functional release
 - development venv setup
 - logging in multiprocessing thread
 - drawio automatic drawing via system call
 - wireviz automatic drawing
 - basic functional test for diagram and harness
 - selectable verbosity in console and log (one argument for both)
 - buildable & deployable with poetry
 
-**Known problems:**
+**Known problem:**
 
 - **[corrected in 0.2.0]** drawio calls throws some error in console and logs
 - **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - **[corrected in 0.2.0]** leave a lot of undesired generated files in input and output folders
 - leave failed graphviz file without extension in _output folder_ when wireviz syntax is invalid
 
 ---
```

### Comparing `hwdocer-0.2.1/pyproject.toml` & `hwdocer-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hwdocer"
-version = "0.2.1"
+version = "0.2.2"
 description = "Wireviz, drawio and other documentation build tool"
 authors = ["Laurence DV <laurencedv@realee.tech>"]
 homepage = "https://gitlab.com/real-ee/public/hwdocer"
 repository = "https://gitlab.com/real-ee/public/hwdocer"
 documentation = "https://gitlab.com/real-ee/public/hwdocer/-/tree/master/doc"
 readme = "readme.md"
 license = "GPL-3.0-or-later"
@@ -40,22 +40,22 @@
 rich = "^13.7.1"
 
 [tool.poetry.group.dev.dependencies]
 bumpver = "^2023.1129"
 pytest = "^7.4.0"
 
 [tool.bumpver]
-current_version = "0.2.1"
+current_version = "0.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Version increase {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/hwdocer/__init__.py" = ['__version__ = "{version}"']
+"src/hwdocer/version.py" = ['version = "{version}"']
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hwdocer-0.2.1/readme.md` & `hwdocer-0.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `hwdocer-0.2.1/src/hwdocer/hwdocer.py` & `hwdocer-0.2.2/src/hwdocer/hwdocer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+from . import version
 import os
 import errno
 import sys
 import glob
 import shutil
 import argparse
 import pathlib
 import time
 import yaml
 from subprocess import DEVNULL, check_call, run
 from rich import print
+from rich.progress import Progress
 
 # logging
 from multiprocessing import Process, Queue, current_process
 from logging.handlers import TimedRotatingFileHandler, QueueHandler
 from rich.logging import RichHandler
 import logging
 
@@ -41,20 +43,21 @@
 
     def __init__(self, arg):
         super(HwDocer, self).__init__()
         self.time_start = time.time()
         self.arg = arg  # save passed arguments
 
         # Arguments
-        argParse = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+        argParse = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter, prog=__name__)
         argParse.add_argument("-v", "--verbose", help="Increase the verbosity level (can be used upto 4 times)", action='count', default=0)
         argParse.add_argument("-i", "--input", help="input directory to search for docs to build", default=self.__def_input__, type=pathlib.Path)
         argParse.add_argument("-o", "--output", help="output build directory", default=self.__def_output__, type=pathlib.Path)
         argParse.add_argument("-w", "--worker", help="maximum number of worker process to spawn", default=self.__def_worker_nb__, type=int)
         argParse.add_argument("-t", "--timeout", help="maximum execution time allowed (in sec)", default=self.__def_timeout__, type=int)
+        argParse.add_argument("--version", action="version", version=f'%(prog)s {version.version}')
         argParse.add_argument("--dia", help="diagram output file format", choices=self.__dia_format_choices__, default=self.__def_dia_format__, type=str)
         argParse.add_argument("--hrs", help="harness output files to keep (many can be choosen)", choices=self.__hrs_format_choices__, default=self.__def_hrs_format__, nargs='*', type=str)
         self.args = argParse.parse_args()  # Parse & save all arguments
 
         # region Logger
         self.verbosity = self.__verb_levels__[min(self.args.verbose, len(self.__verb_levels__) - 1)]
         self.log_q = Queue()
@@ -101,45 +104,40 @@
         self.logger.debug(f'args - dia format: \'{self.dia_format}\'')
 
         # arg - harness format
         self.hrs_format = self.args.hrs
         self.logger.debug(f'args - hrs format: \'{self.hrs_format}\'')
 
         # start with empty work queues
+        self.copy_q = Queue()
         self.work_q = Queue()
         self.done_q = Queue()
-        self.logger.debug(f'work queue: {id(self.work_q)}, done queue: {id(self.done_q)}')
+        self.logger.debug(f'copy queue: {id(self.copy_q)}, work queue: {id(self.work_q)}, done queue: {id(self.done_q)}')
 
         self.time_creation = time.time()
         self.logger.debug(f'{__name__} created successfully in {self.time_creation - self.time_start:.6f} sec')
 
-    def _search_and_copy_files(self):
+    def _search_input_files(self):
         self.logger.debug(f'searching in {self.src_path} for {self.__search_folder__}')     # first search all subfolder to known the complete structure
 
         # searching in subfolders
         for folder in glob.iglob(self.src_path + self.__search_folder__, recursive=True):
             self.logger.debug(f'folder found: {folder}')
 
             # searching for harnesses
             self.logger.debug(f'searching in {folder} for {self.__search_hrs__}')
             for file in glob.iglob(folder + self.__search_hrs__):
                 self.logger.debug(f'harness found: {os.path.basename(file)}')
-                copied_file = self._copy_src_files(file)
-                if os.path.basename(copied_file) == os.path.basename(file):     # ensure the copied file atleast as the same name as original
-                    self.logger.debug(f'work added: {os.path.basename(copied_file)}')
-                    self.work_q.put(copied_file)
+                self.copy_q.put(file)
 
             # searching for diagrams
             self.logger.debug(f'searching in {folder} for {self.__search_dia__}')
             for file in glob.iglob(folder + self.__search_dia__):
                 self.logger.debug(f'diagram found: {os.path.basename(file)}')
-                copied_file = self._copy_src_files(file)
-                if os.path.basename(copied_file) == os.path.basename(file):     # ensure the copied file atleast as the same name as original
-                    self.logger.debug(f'work added: {os.path.basename(copied_file)}')
-                    self.work_q.put(copied_file)
+                self.copy_q.put(file)
 
         self.time_search = time.time()
         self.logger.info(f'found {self.work_q.qsize()} buildable files in {self.time_search - self.time_creation:.6f} sec')
 
     def _prep_output(self):
         self.logger.debug(f'outut folder preparation')
 
@@ -280,57 +278,95 @@
         return image_list
 
     def run(self):
         status = 0
 
         self.logger.info(f'S execution, pid: {current_process().pid}')
 
-        # 1. Prepare output folder
-        self._prep_output()
-
-        # 2. Search all supported files
-        self._search_and_copy_files()
-
-        # 3. Start workers
-        nb_of_file = self.work_q.qsize()
-        self.worker_nb = min(self.worker_nb, nb_of_file)   # worker number is the lowest of: number of file or argument passed
-        self.logger.info(f'starting {self.worker_nb} workers')
-        processes = []
-        for i in range(self.worker_nb):
-            processes.append(Process(target=self.worker_process, args=(self.log_q, self.work_q, self.done_q), daemon=True))
-            processes[i].start()
-
-        # 4. Wait for results
-        while True:
-            if self.done_q.qsize() >= nb_of_file:
-                self.time_done = time.time()
-                self.logger.info(f'all file built in {self.time_done - self.time_search:.3f} sec')
-                break
-            waited = time.time() - self.time_search
-            if waited >= self.exec_timeout:
-                self.time_done = time.time()
-                self.logger.warning(f'timeout reached after {waited:.3f} sec')
-                for i in range(len(processes)):
-                    # TODO: send explicit stop signal to workers
-                    pass
-                break
-            time.sleep(0.1)
+        with Progress() as progress:
+            out_prep = progress.add_task("Preparing output...", total=1)
+            search_task = progress.add_task("Searching files...", total=None)
+            copy_task = progress.add_task("Copying input files...", total=None)
+            build_task = progress.add_task("Building files...", total=None)
+
+            # 1. Prepare output folder
+            self._prep_output()
+            progress.update(out_prep, advance=1)
+
+            # 2. Search all supported files
+            progress.update(search_task, total=1)
+            self._search_input_files()
+            progress.update(search_task, advance=1)
+
+            # 3. Copy all files
+            nb_copy_file = self.copy_q.qsize()
+            progress.update(copy_task, total=nb_copy_file)               # we now know how much input file to copy but not how much image in harness to copy
+            while self.copy_q.qsize():
+                file = self.copy_q.get()
+                copied_file = self._copy_src_files(file)
+                progress.update(copy_task, advance=1)
+                if os.path.basename(copied_file) == os.path.basename(file):     # ensure the copied file atleast as the same name as original
+                    self.logger.debug(f'work added: {os.path.basename(copied_file)}')
+                    self.work_q.put(copied_file)
+                else:
+                    self.logger.error(f'problem copying {file} to {copied_file}')
+            self.time_copy = time.time()
+            self.logger.debug(f'copied {nb_copy_file} in {self.time_copy - self.time_search:.3f} sec')
+
+            # 4. Start workers
+            nb_work_file = self.work_q.qsize()
+            progress.update(build_task, total=nb_work_file)
+            self.worker_nb = min(self.worker_nb, nb_work_file)   # worker number is the lowest of: number of file or argument passed
+            self.logger.info(f'starting {self.worker_nb} workers')
+            processes = []
+            for i in range(self.worker_nb):
+                processes.append(Process(target=self.worker_process, args=(self.log_q, self.work_q, self.done_q), daemon=True))
+                processes[i].start()
+
+            # 4. Wait for results
+            last_check = 0
+            while True:
+
+                # Check if some file have been done
+                check = self.done_q.qsize()
+                if check > last_check:
+                    delta = check - last_check
+                    last_check = check
+                    progress.update(build_task, advance=delta)
+                    self.logger.debug(f'build {delta} more file(s)')
+
+                # All file have been done
+                if self.done_q.qsize() >= nb_work_file:
+                    self.time_done = time.time()
+                    self.logger.info(f'all file built in {self.time_done - self.time_copy:.3f} sec')
+                    break
+
+                # Timeout reach
+                waited = time.time() - self.time_copy
+                if waited >= self.exec_timeout:
+                    self.time_done = time.time()
+                    self.logger.warning(f'timeout reached after {waited:.3f} sec')
+                    for i in range(len(processes)):
+                        # TODO: send explicit stop signal to workers
+                        pass
+                    break
+                time.sleep(0.1)
 
         # work stats
         hrs_count = 0
         dia_count = 0
         for _ in range(self.done_q.qsize()):
             file = self.done_q.get()
             if pathlib.Path(file).suffix == self.__suffix_hrs__:
                 hrs_count += 1
             elif pathlib.Path(file).suffix == self.__suffix_dia__:
                 dia_count += 1
 
         # graceful end of exec
-        print(f'built [dark_orange bold]{hrs_count} harnesses[/] and [purple bold]{dia_count} diagrams[/] in {self.time_done - self.time_start:.6f} sec')
+        print(f'{__name__} {version.version} built [dark_orange bold]{hrs_count} harnesses[/] and [purple bold]{dia_count} diagrams[/] in {self.time_done - self.time_start:.6f} sec')
         self.logger.info(f'P execution, pid: {current_process().pid}, built {hrs_count} harnesses and {dia_count} diagrams in {self.time_done - self.time_start:.6f} sec')
         self.log_q.put(None)
         return status
 
     def worker_process(self, log_q: Queue, q_in: Queue, q_out: Queue) -> int:
         """worker isolated process to generate output files from input file
```

### Comparing `hwdocer-0.2.1/PKG-INFO` & `hwdocer-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdocer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Wireviz, drawio and other documentation build tool
 Home-page: https://gitlab.com/real-ee/public/hwdocer
 License: GPL-3.0-or-later
 Keywords: drawio,wireviz,toolchain,automation,documentation
 Author: Laurence DV
 Author-email: laurencedv@realee.tech
 Requires-Python: >=3.8,<4.0
```

