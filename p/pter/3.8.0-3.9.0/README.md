# Comparing `tmp/pter-3.8.0.tar.gz` & `tmp/pter-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pter-3.8.0.tar", last modified: Fri Jun 23 09:45:04 2023, max compression
+gzip compressed data, was "pter-3.9.0.tar", last modified: Sun Oct 15 13:19:14 2023, max compression
```

## Comparing `pter-3.8.0.tar` & `pter-3.9.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.336876 pter-3.8.0/
--rw-r--r--   0 robert    (1000) robert    (1000)    12126 2023-06-23 09:43:15.000000 pter-3.8.0/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1097 2022-04-15 06:59:55.000000 pter-3.8.0/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      218 2022-02-19 08:34:12.000000 pter-3.8.0/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-06-23 09:45:04.336876 pter-3.8.0/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     2313 2022-07-24 08:17:34.000000 pter-3.8.0/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)   365846 2022-02-19 08:34:12.000000 pter-3.8.0/doc/pter-demo.gif
--rw-r--r--   0 robert    (1000) robert    (1000)    47149 2023-06-23 09:15:08.000000 pter-3.8.0/doc/pter.rst
--rw-r--r--   0 robert    (1000) robert    (1000)    29201 2022-02-19 08:34:12.000000 pter-3.8.0/doc/qpter.png
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/extras/
--rw-r--r--   0 robert    (1000) robert    (1000)     8834 2022-02-19 08:34:12.000000 pter-3.8.0/extras/example.conf
--rw-r--r--   0 robert    (1000) robert    (1000)      196 2022-02-19 08:34:12.000000 pter-3.8.0/extras/pter.desktop
--rw-r--r--   0 robert    (1000) robert    (1000)      296 2022-02-19 08:34:12.000000 pter-3.8.0/extras/qpter.desktop
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    54422 2023-06-23 09:45:04.000000 pter-3.8.0/man/pter.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter/
--rw-r--r--   0 robert    (1000) robert    (1000)        0 2023-05-11 17:11:53.000000 pter-3.8.0/pter/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     5458 2023-06-23 08:05:52.000000 pter-3.8.0/pter/common.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6844 2023-06-23 07:37:57.000000 pter-3.8.0/pter/configuration.py
--rw-r--r--   0 robert    (1000) robert    (1000)    94139 2023-06-23 09:40:58.000000 pter-3.8.0/pter/curses.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    85420 2023-06-23 09:45:04.000000 pter-3.8.0/pter/docs/pter.html
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter/icons/
--rw-r--r--   0 robert    (1000) robert    (1000)     1083 2022-02-19 08:34:12.000000 pter-3.8.0/pter/icons/qpter_16x16.png
--rw-r--r--   0 robert    (1000) robert    (1000)     1598 2022-02-19 08:34:12.000000 pter-3.8.0/pter/icons/qpter_32x32.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5399 2023-05-11 17:11:53.000000 pter-3.8.0/pter/key.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4358 2023-06-23 08:13:15.000000 pter-3.8.0/pter/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)    75198 2023-05-11 17:11:53.000000 pter-3.8.0/pter/qtui.py
--rw-r--r--   0 robert    (1000) robert    (1000)    19345 2023-05-11 17:11:53.000000 pter-3.8.0/pter/searcher.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2261 2023-05-11 17:11:53.000000 pter-3.8.0/pter/source.py
--rw-r--r--   0 robert    (1000) robert    (1000)       31 2023-05-11 17:11:53.000000 pter-3.8.0/pter/tr.py
--rw-r--r--   0 robert    (1000) robert    (1000)    17809 2023-05-11 17:11:53.000000 pter-3.8.0/pter/utils.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-06-23 09:10:28.000000 pter-3.8.0/pter/version.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)      762 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       76 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       49 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        5 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       50 2023-06-23 08:59:37.000000 pter-3.8.0/pyproject.toml
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-23 09:45:04.336876 pter-3.8.0/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     2773 2022-02-19 08:34:12.000000 pter-3.8.0/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.336876 pter-3.8.0/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     1518 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_displaynames.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1684 2022-10-31 18:55:16.000000 pter-3.8.0/tests/test_priochange.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1221 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_pter.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6496 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_rec.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12855 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_searcher.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1618 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_sorting.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1475 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_taskid.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.842152 pter-3.9.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)    12429 2023-10-15 12:12:36.000000 pter-3.9.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1097 2023-10-15 13:14:37.000000 pter-3.9.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      218 2023-09-17 07:19:26.000000 pter-3.9.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-10-15 13:19:14.842152 pter-3.9.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     2313 2023-09-17 07:19:26.000000 pter-3.9.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.838819 pter-3.9.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)   365846 2023-09-17 07:19:26.000000 pter-3.9.0/doc/pter-demo.gif
+-rw-r--r--   0 robert    (1000) robert    (1000)    50078 2023-10-15 12:53:40.000000 pter-3.9.0/doc/pter.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)    29201 2023-09-17 07:19:26.000000 pter-3.9.0/doc/qpter.png
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.838819 pter-3.9.0/extras/
+-rw-r--r--   0 robert    (1000) robert    (1000)     9718 2023-10-15 13:03:30.000000 pter-3.9.0/extras/example.conf
+-rw-r--r--   0 robert    (1000) robert    (1000)      196 2023-09-17 07:19:26.000000 pter-3.9.0/extras/pter.desktop
+-rw-r--r--   0 robert    (1000) robert    (1000)      296 2023-09-17 07:19:26.000000 pter-3.9.0/extras/qpter.desktop
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.838819 pter-3.9.0/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    54422 2023-09-30 11:21:51.000000 pter-3.9.0/man/pter.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.838819 pter-3.9.0/pter/
+-rw-r--r--   0 robert    (1000) robert    (1000)        0 2023-09-17 07:19:26.000000 pter-3.9.0/pter/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     5821 2023-10-15 13:08:21.000000 pter-3.9.0/pter/common.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     7085 2023-10-15 12:49:09.000000 pter-3.9.0/pter/configuration.py
+-rw-r--r--   0 robert    (1000) robert    (1000)   100437 2023-10-15 13:08:12.000000 pter-3.9.0/pter/curses.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.842152 pter-3.9.0/pter/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    85420 2023-09-30 11:21:51.000000 pter-3.9.0/pter/docs/pter.html
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.842152 pter-3.9.0/pter/icons/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1083 2023-09-17 07:19:26.000000 pter-3.9.0/pter/icons/qpter_16x16.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     1598 2023-09-17 07:19:26.000000 pter-3.9.0/pter/icons/qpter_32x32.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5399 2023-09-17 07:19:26.000000 pter-3.9.0/pter/key.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4400 2023-10-15 09:33:01.000000 pter-3.9.0/pter/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    75169 2023-10-15 09:11:53.000000 pter-3.9.0/pter/qtui.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    19345 2023-09-17 07:19:26.000000 pter-3.9.0/pter/searcher.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2261 2023-09-17 07:19:26.000000 pter-3.9.0/pter/source.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       31 2023-09-17 07:19:26.000000 pter-3.9.0/pter/tr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    18235 2023-10-15 09:32:16.000000 pter-3.9.0/pter/utils.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-10-15 12:24:10.000000 pter-3.9.0/pter/version.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.842152 pter-3.9.0/pter.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-10-15 13:19:14.000000 pter-3.9.0/pter.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)      762 2023-10-15 13:19:14.000000 pter-3.9.0/pter.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-10-15 13:19:14.000000 pter-3.9.0/pter.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       76 2023-10-15 13:19:14.000000 pter-3.9.0/pter.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       49 2023-10-15 13:19:14.000000 pter-3.9.0/pter.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        5 2023-10-15 13:19:14.000000 pter-3.9.0/pter.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       50 2023-09-17 07:19:26.000000 pter-3.9.0/pyproject.toml
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-10-15 13:19:14.842152 pter-3.9.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     2773 2023-09-17 07:19:26.000000 pter-3.9.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-10-15 13:19:14.842152 pter-3.9.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1518 2023-09-17 07:19:26.000000 pter-3.9.0/tests/test_displaynames.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1684 2023-09-17 07:19:26.000000 pter-3.9.0/tests/test_priochange.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1221 2023-09-17 07:19:26.000000 pter-3.9.0/tests/test_pter.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6496 2023-09-17 07:19:26.000000 pter-3.9.0/tests/test_rec.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12855 2023-09-17 07:19:26.000000 pter-3.9.0/tests/test_searcher.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1618 2023-09-17 07:19:26.000000 pter-3.9.0/tests/test_sorting.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1475 2023-09-17 07:19:26.000000 pter-3.9.0/tests/test_taskid.py
```

### Comparing `pter-3.8.0/CHANGELOG.md` & `pter-3.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+## 3.9.0
+### Added
+- `files` option in `General` section. These files will be opened if you don't provide files on the commandline.
+- Support for detailed notes per task via the `note:` tag
+
+### Fixed
+- Desktop file `pter.desktop` can now actually work (due to `files` option in `General`, see above)
+
+
 ## 3.8.0
 ### Added
 - Archiving is now a thing. Default key binding for `archive` function is `%`
 - Archive location can be configured, see `archive-is` configuration option
 - New function `edit-file-external`, by default not mapped to a key
 
 ### Fixed
```

### Comparing `pter-3.8.0/LICENSE` & `pter-3.9.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Robert Labudda <https://vonshednob.cc/>
+Copyright (c) 2023 Robert Labudda <https://vonshednob.cc/>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pter-3.8.0/PKG-INFO` & `pter-3.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pter
-Version: 3.8.0
+Version: 3.9.0
 Summary: Console UI to manage your todo.txt file(s).
 Home-page: https://vonshednob.cc/pter
 Author: R
 Author-email: contact+pter@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pter-3.8.0/README.md` & `pter-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/doc/pter-demo.gif` & `pter-3.9.0/doc/pter-demo.gif`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/doc/pter.rst` & `pter-3.9.0/doc/pter.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
  - Sort tasks through search queries (see `Sorting`_)
  - Convenient entering of dates (see `Relative Dates`_)
  - Configurable behaviour, shortcuts, and colors (see `Files`_)
  - Task sequencing (see `Task Sequences`_)
  - Automatic identifiers (see `Unique Task Identifiers`_)
  - `Time Tracking`_
  - `Recurring Tasks`_
+ - `Task Notes`_
 
 qpter is the Qt version of pter (ie. pter with a graphical user interface)
 and supports mostly the same features but sometimes looks for other
 sections in the configuration.
 
 
 Options
@@ -60,14 +61,17 @@
   ``-n task``
     Add ``task`` to the todo.txt file. The advantage of using this over
     just ``echo "task" >> todo.txt`` is that relative dates are properly
     expanded (see `Relative Dates`_).
     If you provide ``-`` instead of a task, the task will be read from
     stdin. Multiple tasks can be added, one per line.
 
+    If you don't provide a todo.txt file on the commandline, the first file
+    from the ``files`` option in your configuration file will be used.
+
   ``-s search``
     Only available for pter: load this named search upon startup. If a
     named search by that name does not exist, use this as a search term
     from the start.
 
   ``-a``
     Only available for qpter: either start qpter, immediately open the New
@@ -81,14 +85,16 @@
   ``--log-file``
     In what file to log the messages. This is also the file where you can
     find information about crashes, if you encounter any.
 
   ``filename``
     Path to your todo.txt file. The first file that you provide is the one
     where new tasks will be created in.
+    You may choose to not provide any files here. In that case the files
+    configured in the ``[General]`` section (in ``files``) will be loaded.
 
 
 Files
 =====
 
 Aside from the data files in the todo.txt format (see `Conforming to`_),
 pter's behaviour can be configured through a configuration file.
@@ -281,14 +287,63 @@
 
     ``force`` is the same as ``yes``, but if the current task does not have
     an ``id:`` attribute, it will be given one. In other words, this option
     may modify your ``todo.txt`` file.
 
     Defaults to ``yes``.
 
+  ``files``
+    Default todo file(s) to load. This option is ignored when pter is given
+    some todo.txt file(s) in the command line parameters.
+
+    For example: ``files = ~/Documents/todo.txt``.
+    
+    To provide multiple files, separate them with newlines, like this::
+
+        [General]
+        files =
+            ~/shared/group_todo.txt
+            ~/Documents/todo.txt
+
+    This option does not apply to qpter, which tracks opened files differently.
+
+  ``notes``
+    The directories where notes should be looked for when references as ``note:``
+    in a task.
+
+    For example: ``notes = ~/Documents/task_notes/``.
+
+    To provide multiple folder, separate them with newlines, like this::
+
+        [General]
+        notes =
+            ~/shared/group_notes/
+            ~/Documents/task_notes/
+
+    Multiple folders will be searched in order when opening a task note. If no
+    note exists, it will be created in the first given folder.
+
+  ``note-suffix``
+    The file extension that's used when finding notes when the file extension is not
+    provided.
+
+    Defaults to ``.txt``.
+
+  ``note-naming``
+    Defines the behaviour of pter when you edit a task's note, but no ``note:`` tag
+    is defined.
+
+    Possible options are:
+
+       - ``cancel``, don't try to edit the task's note
+       - ``auto``, create a file based on the task's ID, create a task ID if necessary
+       - ``user-input``, ask the user for the name of the file
+
+    Defaults to ``user-input``.
+
 
 Symbols
 -------
 
 The following symbols (single unicode characters or even longer strings of
 unicode characters) can be defined:
 
@@ -747,14 +802,15 @@
  - "B": Set the priority of this task to ``(B)``
  - "C": Set the priority of this task to ``(C)``
  - "D": Set the priority of this task to ``(D)``
  - "+": Increase the priority of this task
  - "-": Decrease the priority of this task
  - "=": Remove the priority of this task
  - "%": Move this task into the archive
+ - "N": Edit or create this task's note
 
 In edit fields the following keyboard controls are available:
 
  - "←", "→" (cursor keys): move the cursor one character to the left or right
  - "Home": move the cursor to the first charater
  - "End": move the cursor to the last character
  - "Backspace", "^H": delete the character to the left of the cursor
@@ -1241,14 +1297,43 @@
 the same relative time to the due date as the original task.
 
 So, if you set up a due date 2021-06-05 and a threshold ``t:2021-06-04``
 the new task will also have a threshold in such a way that the task is
 hidden until one day before the due date.
 
 
+Task Notes
+==========
+
+This extension only works in ``pter``, not in ``qpter``.
+
+You may provide a text file with additional notes about a task using the ``note:`` tag.
+
+The location of notes is managed via the configuration file in the ``General``
+section with the ``notes`` option.
+
+Notes are assumed to be ``.txt`` text files, but you can overwrite that with
+the ``note-suffix`` configuration option.
+
+For example, if you define a task with ``note:details``, pter will assume you
+meant a file with the name ``details.txt``.
+
+However, you can just define the full filename with extension in which case pter
+will not use the ``note-suffix`` default. For example ``Some task note:details.md``.
+
+The function ``edit-note`` (usually on shortcut ``N``) will either edit the
+note of this task or create a note.
+
+Have a look at the ``note-naming`` option to change the behaviour how new notes
+are created.
+
+For editing, ``pter`` will use the external text editor configured with
+``editor`` in the configuration file's ``General`` section.
+
+
 Getting Things Done
 ===================
 
 With pter you can apply the Getting Things Done method to a single todo.txt
 file by using context and project tags, avoiding multiple lists.
 
 For example, you could have a ``@in`` context for the list of all tasks
@@ -1270,14 +1355,15 @@
 - ``id:3``, allows you to assign a unique identifier to entries in the todo.txt, like ``3``. pter will accept when there non-unique IDs, but of course uniquely identifying entries will be tricky.
 - ``rec:1w``, indicate that this task should be recurring in 1 week intervals.
 - ``ref:6``, indicate that this task refers to the task with ``id:6``.  Comma-separated IDs are supported, like ``ref:13,9``.
 - ``spent:5h3m``, pter can be used for time tracking and will store the time spent on a task in the ``spent`` attribute.
 - ``t:2070-12-24``, the threshold tag can be used to hide before the given date has come.
 - ``to:person``, when a task has been delegated (by using a delegation marker like ``@delegated``), ``to`` can be used to indicate to whom the task has been delegated. The option is configurable, see ``delegation-to`` above for details.
 - ``tracking:``, a technical tag used for time tracking. It indicates that you started working on the task and wanted to do time tracking. The value is the date and time when you started working. Upon stopping tracking, the spent time will be stored in the ``spent`` tag.
+- ``note:``, a filename with additional notes about this task
 
 
 Conforming to
 =============
 
 pter works with and uses the todo.txt file format and strictly adheres to the format
 as described at http://todotxt.org/. Additional special key/value tags are
```

### Comparing `pter-3.8.0/doc/qpter.png` & `pter-3.9.0/doc/qpter.png`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/extras/example.conf` & `pter-3.9.0/extras/example.conf`

 * *Files 7% similar despite different names*

```diff
@@ -99,14 +99,39 @@
 ;; This option only applies whene 'delete-is' is set to 'trash'.
 ;trash-file = ~/.config/pter/trash.txt
 
 ;; Whether or not to reuse the same task as the follow-up
 ;; when completing a recurring task.
 ;reuse-recurring = no
 
+;; How the archive functionality behaves
+;; Options are:
+;; relative (archive is relative to the todo.txt file),
+;; centralised (one archive for all your todo.txt files),
+;; disabled (archiving is disabled)
+;archive-is = centralised
+
+;; Where your archive file is, if 'archive-is' is set to 'centralised'
+;archive-file = ~/.config/pter/archive.txt
+
+;; How pter determines the filename of a task's note
+;; Options are:
+;; user-input (you will be asked for a filename),
+;; auto (the task's ID will be taken; an ID might be added if necessary),
+;; cancel (cancel task note editing if no note is defined)
+;note-naming = user-input
+
+;; Filename suffix for notes, if a suffix is not provided
+;note-suffix = .txt
+
+;; Where the notes for the tasks are stored. You may provide multiple
+;; paths here (separate with newlines). When creating notes, only the
+;; first path will be used
+;notes =
+
 [Symbols]
 ;; This text will be shown to indicate the selected task in the list.
 ;; If this is left empty but your terminal does not support colors pter
 ;; will show a ">" to indicate the selected task.
 ;selection =
 
 ;; This will be used to indicate tasks that are marked done
```

### Comparing `pter-3.8.0/man/pter.1` & `pter-3.9.0/man/pter.1`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/pter/common.py` & `pter-3.9.0/pter/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,16 +51,24 @@
 ARCHIVE_OPTION_RELATIVE = 'relative'
 ARCHIVE_OPTION_CENTRALISED = 'centralised'
 ARCHIVE_OPTION_DISABLED = 'disabled'
 ARCHIVE_OPTIONS = (ARCHIVE_OPTION_RELATIVE,
                    ARCHIVE_OPTION_CENTRALISED,
                    ARCHIVE_OPTION_DISABLED)
 
+NOTE_NAMING_AUTO = 'auto'
+NOTE_NAMING_USER = 'user-input'
+NOTE_NAMING_CANCEL = 'cancel'
+NOTE_NAMING_OPTIONS = (NOTE_NAMING_AUTO,
+                       NOTE_NAMING_USER,
+                       NOTE_NAMING_CANCEL)
+
 DEFAULT_SORT_ORDER = 'completed,due_in,priority,linenr'
 DEFAULT_INFO_TIMEOUT = 5
+DEFAULT_NOTE_SUFFIX = '.txt'
 
 SETTING_GROUP_GENERAL = 'General'
 SETTING_GROUP_SYMBOLS = 'Symbols'
 SETTING_GROUP_COLORS = 'Colors'
 SETTING_GROUP_HIGHLIGHT = 'Highlight'
 SETTING_GROUP_KEYS = 'Keys'
 SETTING_GROUP_EDITORKEYS = 'Editor:Keys'
@@ -94,14 +102,18 @@
 SETTING_CREATE_FROM_SEARCH = 'create-from-search'
 SETTING_AUTO_ID = 'auto-id'
 SETTING_HIDE_SEQUENTIAL = 'hide-sequential'
 SETTING_CLICKABLE = 'clickable'
 SETTING_DAILY_RELOAD = 'daily-reload'
 SETTING_DELETE_IS = 'delete-is'
 SETTING_TRASHFILE = 'trash-file'
+SETTING_FILES = 'files'
+SETTING_NOTES = 'notes'
+SETTING_NOTE_SUFFIX = 'note-suffix'
+SETTING_NOTE_NAMING = 'note-naming'
 SETTING_INFO_TIMEOUT = 'info-timeout'
 SETTING_ARCHIVE_FILE = 'archive-file'
 SETTING_ARCHIVE_IS = 'archive-is'
 SETTING_ICON_SELECTION = 'selection'
 SETTING_ICON_NOT_DONE = 'not-done'
 SETTING_ICON_DONE = 'done'
 SETTING_ICON_OVERFLOW_LEFT = 'overflow-left'
```

### Comparing `pter-3.8.0/pter/configuration.py` & `pter-3.9.0/pter/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
             common.SETTING_RELATED_SHOW_SELF: 'yes',
             common.SETTING_INFO_TIMEOUT: common.DEFAULT_INFO_TIMEOUT,
             common.SETTING_USE_COMPLETION: 'yes',
             common.SETTING_DELETE_IS: common.DELETE_OPTION_DISABLED,
             common.SETTING_TRASHFILE: common.DEFAULT_TRASHFILE,
             common.SETTING_ARCHIVE_IS: common.ARCHIVE_OPTION_CENTRALISED,
             common.SETTING_ARCHIVE_FILE: common.DEFAULT_ARCHIVE,
+            common.SETTING_NOTE_SUFFIX: common.DEFAULT_NOTE_SUFFIX,
+            common.SETTING_NOTE_NAMING: common.NOTE_NAMING_USER,
         },
         common.SETTING_GROUP_SYMBOLS: {
             common.SETTING_ICON_SELECTION: '',
             common.SETTING_ICON_NOT_DONE: '[ ]',
             common.SETTING_ICON_DONE: '[x]',
             common.SETTING_ICON_OVERFLOW_LEFT: '←',
             common.SETTING_ICON_OVERFLOW_RIGHT: '→',
@@ -130,15 +132,16 @@
         else:
             return default
 
     def bool(self, group, item, default='n'):
         return self.get(group, item, default).lower() in self.BOOL_TRUE
 
     def list(self, group, item, default='', sep=',', strip=True):
-        return [e.strip() if strip else e for e in self.get(group, item, default).split(sep)]
+        return [e.strip() if strip else e
+                for e in self.get(group, item, default).split(sep)]
 
     def number(self, group, item, default='0'):
         value = self.get(group, item, default)
         if value.isnumeric():
             return int(value)
         return None
 
@@ -183,13 +186,15 @@
     conf.optionxform = lambda o: o
     conf.read_dict(DEFAULT_CONFIG)
     conffile = pathlib.Path(args.config).expanduser().resolve()
 
     if conffile.exists() and conffile.is_file():
         conf.read([conffile])
 
-    if common.SETTING_GROUP_INCLUDE in conf and 'path' in conf[common.SETTING_GROUP_INCLUDE]:
-        path = pathlib.Path(conf[common.SETTING_GROUP_INCLUDE]['path']).expanduser().resolve()
+    has_group_include = common.SETTING_GROUP_INCLUDE in conf and \
+                        'path' in conf[common.SETTING_GROUP_INCLUDE]
+    if has_group_include:
+        path = pathlib.Path(conf[common.SETTING_GROUP_INCLUDE]['path']) \
+                      .expanduser().resolve()
         conf.read([path])
     
     return Configuration(conf)
-
```

### Comparing `pter-3.8.0/pter/curses.py` & `pter-3.9.0/pter/curses.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 import webbrowser
 import curses
 import traceback
 import tempfile
 import subprocess
 import shlex
 import shutil
+from pathlib import Path
 
 from pytodotxt import TodoTxt, Task, TodoTxtParser
 
-from cursedspace import Application, Panel, ScrollPanel, InputLine, ShellContext, Completion
+from cursedspace import Application, Panel, ScrollPanel, InputLine, \
+                        ShellContext, Completion
 
 from pter import common
 from pter import utils
-from pter import configuration
 from pter.searcher import Searcher
 from pter.key import Key
 from pter.tr import tr
 
 
 SHORT_NAMES = {'quit': 'Quit',
                'cancel': 'Cancel',
@@ -41,14 +42,15 @@
                'search-context': 'Search for context of this task',
                'search-project': 'Search for project of this task',
                'clear-search': 'Clear the search',
                'first-item': 'First item',
                'last-item': 'Last item',
                'edit-task': 'Edit task',
                'create-task': 'New task',
+               'edit-note': 'Edit note',
                'jump-to': 'Jump to item',
                'toggle-hidden': 'Set/unset hidden',
                'toggle-done': 'Set/unset done',
                'toggle-tracking': 'Start/stop tracking',
                'show-help': 'Help',
                'open-manual': 'Read the manual',
                'go-left': 'Go one character to the left',
@@ -74,14 +76,15 @@
                'prio-b': 'Set priority to (B)',
                'prio-c': 'Set priority to (C)',
                'prio-d': 'Set priority to (D)',
                'prio-none': 'Remove priority',
                'prio-up': 'Increase priority',
                'prio-down': 'Decrease priority',
                }
+TITLE_FRAME = '┤├'
 
 
 class Color:
     def __init__(self, fg, bg=None):
         self.fg = fg
         self.bg = bg
 
@@ -174,15 +177,16 @@
                                                   common.SETTING_INFO_TIMEOUT,
                                                   common.DEFAULT_INFO_TIMEOUT))
 
     def set_text(self, text, color=None, expire=True):
         self.text = text
         self.color = color or common.SETTING_COL_NORMAL
         if expire is True:
-            self.expire = datetime.datetime.now() + datetime.timedelta(seconds=self.blank_after)
+            self.expire = datetime.datetime.now() \
+                        + datetime.timedelta(seconds=self.blank_after)
         elif isinstance(expire, datetime.datetime):
             self.expire = expire
         else:
             self.expire = datetime.datetime.max
         self.paint()
 
     def is_expired(self):
@@ -210,15 +214,16 @@
     def paint(self, clear=False):
         self.border = Panel.BORDER_NONE
         super().paint(clear)
 
         mapping = self.app.key_mapping
         actions = ['show-help', 'quit', 'edit-task',
                    'create-task', 'search', 'load-search', 'save-search',
-                   'toggle-done', 'jump-to', 'next-item', 'prev-item']
+                   'toggle-done', 'jump-to', 'next-item', 'prev-item',
+                   'edit-note']
 
         if len(self.app.focus) == 0:
             pass
         elif isinstance(self.app.focus[-1], HelpScreen):
             actions = ['quit', 'cancel', 'refresh-screen']
         elif isinstance(self.app.focus[-1], Selector):
             actions = ['cancel', 'select-item']
@@ -299,18 +304,21 @@
 
     def rebuild_items(self):
         self.items = []
         self.max_widths = {}
 
         today = datetime.date.today()
 
-        self.update_max_width(common.TF_DONE, max(len(self.app.done_marker[0]), len(self.app.done_marker[1])))
+        self.update_max_width(common.TF_DONE,
+                              max(len(self.app.done_marker[0]),
+                                  len(self.app.done_marker[1])))
         self.update_max_width(common.TF_SELECTION, self.app.selection_indicator)
         self.update_max_width(common.TF_TRACKING, self.app.tracking_marker)
-        self.update_max_width(common.TF_DUE, max([len(m) for m in self.app.due_marker]))
+        self.update_max_width(common.TF_DUE,
+                              max([len(m) for m in self.app.due_marker]))
 
         for nr, pair in enumerate(self.tasks):
             task, _ = pair
             line = TaskLine(task, task.todotxt)
 
             # Selection indicator
             if len(self.app.selection_indicator) > 0:
@@ -477,16 +485,17 @@
                 elem = elem + extra_right
 
             elemlen = len(elem)
             if elemlen > maxwidth:
                 cut_off = True
                 elem = elem[:maxwidth]
 
+            color = self.app.color(element.color, is_selected, baseattrs)
             try:
-                self.win.addstr(y, x, elem, self.app.color(element.color, is_selected, baseattrs))
+                self.win.addstr(y, x, elem, color)
             except curses.error:
                 pass
 
             if cut_off:
                 attrs = common.SETTING_COL_OVERFLOW
                 try:
                     self.win.addstr(y, x+maxwidth-len(self.app.overflow_marker[1]),
@@ -496,33 +505,36 @@
                     pass
             return elem
 
         def print_group(y, x, maxwidth, group, align, extra):
             line = ''
 
             if extra is not None and extra[0] is not None:
-                self.win.addstr(y, x + len(line), extra[0], self.app.color(baseattrs, is_selected))
+                color = self.app.color(baseattrs, is_selected)
+                self.win.addstr(y, x + len(line), extra[0], color)
                 line = extra[0]
 
             if align is not None and align.endswith('>'):
                 group_width = len(' '.join([e.content for e in group.elements]))
                 spacing_width = min(maxwidth - len(line),
                                     self.max_widths[group.name] - group_width)
                 spacing = align[0] * spacing_width
+                color = self.app.color(baseattrs, is_selected)
                 try:
-                    self.win.addstr(y, x + len(line), spacing, self.app.color(baseattrs, is_selected))
+                    self.win.addstr(y, x + len(line), spacing, color)
                 except curses.error:
                     pass
                 line += spacing
 
             cut_off = False
             for elnr, element in enumerate(group.elements):
                 word = ''
 
-                if elnr > 0 and (element.space_around or group.elements[elnr-1].space_around):
+                if elnr > 0 and (element.space_around or
+                                 group.elements[elnr-1].space_around):
                     if len(line) + 1 >= maxwidth:
                         cut_off = True
                     else:
                         self.win.addstr(y, x + len(line), " ",
                                         self.app.color(baseattrs, is_selected))
                         line += " "
 
@@ -547,16 +559,18 @@
                     spacing = align[0] * min(maxwidth-len(line),
                                              self.max_widths[group.name]-len(line))
                     self.win.addstr(y, x + len(line),
                                     spacing,
                                     self.app.color(baseattrs, is_selected))
                     line += spacing
 
-            if not cut_off and extra is not None and extra[1] is not None and len(line) + 1 < maxwidth:
-                self.win.addstr(y, x + len(line), extra[1], self.app.color(baseattrs, is_selected))
+            if not cut_off and extra is not None and \
+               extra[1] is not None and len(line) + 1 < maxwidth:
+                color = self.app.color(baseattrs, is_selected)
+                self.win.addstr(y, x + len(line), extra[1], color)
             return line
 
         self.win.move(y, x)
         self.win.clrtoeol()
         self.win.noutrefresh()
 
         for token in self.app.task_format:
@@ -573,16 +587,17 @@
 
             x += len(print_element(y, x, maxwidth-x, token, align, extra))
 
             if x >= maxwidth:
                 break
 
         if x < maxwidth:
+            color = self.app.color(baseattrs, is_selected)
             try:
-                self.win.addstr(y, x, ' '*(maxwidth-x), self.app.color(baseattrs, is_selected))
+                self.win.addstr(y, x, ' '*(maxwidth-x), color)
             except curses.error:
                 pass
 
     def jump_to(self, item):
         if item in self.items:
             self.cursor = self.items.index(item)
 
@@ -731,14 +746,20 @@
             return
 
         word = self.inputline.text[span[0]:self.inputline.cursor].lower()
         if word.startswith('@'):
             options = self.app.known_contexts()
         elif word.startswith('+'):
             options = self.app.known_projects()
+        elif word.startswith('note:'):
+            options = set()
+            for path in self.app.notes:
+                options |= {'note:' + fn.name
+                            for fn in path.iterdir()
+                            if fn.is_file()}
         else:
             return
 
         options = [o for o in sorted(options)
                    if o.lower().startswith(word)]
 
         if len(options) == 0 or (len(options) == 1 and word in options):
@@ -759,15 +780,16 @@
     def paint(self, clear=False):
         self.border = Panel.BORDER_NONE
         if clear:
             self.win.erase()
         self.scroll()
 
         attr = 0
-        if len(self.text) == 0 and (len(self.app.focus) == 0 or self.app.focus[-1] is not self):
+        if len(self.text) == 0 and (len(self.app.focus) == 0 or
+                                    self.app.focus[-1] is not self):
             visible_text = tr('(no search active)')
             attr = self.app.color(common.SETTING_COL_INACTIVE)
         else:
             visible_text = self.text[self.offset:]
 
         visible_text = visible_text[:self.dim[1]]
         try:
@@ -866,43 +888,48 @@
         self.on_accept(self.editor.text)
         self.app.show_cursor(False)
         self.destroy()
 
 
 class TaskEditor(UserInput):
     def __init__(self, parent, task):
-        super().__init__(parent, None, None, 'Edit Task', '' if task is None else str(task.task))
+        super().__init__(parent, None, None, 'Edit Task',
+                         '' if task is None else str(task.task))
         self.task = task
         self.on_accept = self.save_changes
         self.on_cancel = lambda: self.app.show_cursor(False)
         if self.app.use_completion:
             self.editor.completion = ContextCompletion(self.editor)
 
     def save_changes(self, text):
         self.app.show_cursor(False)
         if self.has_changes() and not self.editor.read_only:
             text = self.processed_text
             self.app.modify_task(self.task, lambda t: t.parse(text))
 
     @property
     def processed_text(self):
-        return utils.dehumanize_dates(utils.auto_task_id(self.app.sources, self.editor.text))
+        return utils.dehumanize_dates(utils.auto_task_id(self.app.sources,
+                                                         self.editor.text))
 
     def has_changes(self):
         return str(self.task.task) != self.processed_text
 
 
 class TaskCreator(TaskEditor):
     def __init__(self, parent):
         super().__init__(parent, None)
         self.title = 'New task'
 
-        add_creation_date = self.app.conf.bool(common.SETTING_GROUP_GENERAL, common.SETTING_ADD_CREATED)
-        create_from_search = self.app.conf.bool(common.SETTING_GROUP_GENERAL, common.SETTING_CREATE_FROM_SEARCH)
-        self.auto_id = self.app.conf.bool(common.SETTING_GROUP_GENERAL, common.SETTING_AUTO_ID)
+        add_creation_date = self.app.conf.bool(common.SETTING_GROUP_GENERAL,
+                                               common.SETTING_ADD_CREATED)
+        create_from_search = self.app.conf.bool(common.SETTING_GROUP_GENERAL,
+                                                common.SETTING_CREATE_FROM_SEARCH)
+        self.auto_id = self.app.conf.bool(common.SETTING_GROUP_GENERAL,
+                                          common.SETTING_AUTO_ID)
         self.editor.cursor = 1
 
         initial = []
         if add_creation_date:
             create_date = datetime.datetime.now().strftime(Task.DATE_FMT)
             initial.append(create_date)
             self.editor.cursor += len(create_date)
@@ -966,15 +993,15 @@
             self.app.tasks.jump_to(self.task)
 
     def paint(self, clear=False):
         super().paint(clear)
 
         if len(self.app.sources) > 1:
             label = self.task.todotxt.displayname
-            self.win.addstr(2, self.dim[1]-len(label)-3, f"┤{label}├")
+            self.win.addstr(2, self.dim[1]-len(label)-3, title_frame(label))
             self.win.noutrefresh()
 
     def has_changes(self):
         return str(self.task) != self.processed_text
 
 
 class Selector(RemappedScrollPanel):
@@ -1081,15 +1108,15 @@
         super().__init__(*args, **kwargs)
 
         nav_fncs = ['next-item', 'prev-item', 'page-up', 'page-down',
                     'first-item', 'last-item', 'jump-to']
         edt_fncs = ['toggle-hidden', 'toggle-done', 'edit-task', 'create-task',
                     'toggle-tracking', 'delegate', 'save-template', 'load-template',
                     'delete-task', 'prio-a', 'prio-b', 'prio-c', 'prio-c',
-                    'prio-none', 'prio-up', 'prio-down']
+                    'prio-none', 'prio-up', 'prio-down', 'edit-note']
         search_fncs = ['search', 'load-search', 'save-search',
                        'search-context', 'search-project', 'clear-search']
         meta_fncs = ['show-help', 'open-manual', 'quit', 'cancel', 'refresh-screen',
                      'reload-tasks']
         other_fncs = ['open-url']
 
         lines = [(tr('TASK LIST'), ''), ('', ''), (tr('Program'), '')]
@@ -1316,14 +1343,31 @@
         if self.archive_is == common.ARCHIVE_OPTION_CENTRALISED:
             try:
                 self.archive_file.parent.mkdir(parents=True, exist_ok=True)
             except OSError as exc:
                 logging.error(f"Could not create path to archive file '{self.archive_file}': {exc}")
                 self.archive_is = common.ARCHIVE_OPTION_DISABLED
 
+        # notes
+        self.notes = [Path(nb.strip()).expanduser()
+                      for nb in self.conf.list(common.SETTING_GROUP_GENERAL,
+                                               common.SETTING_NOTES,
+                                               sep="\n")
+                      if len(nb.strip()) > 0]
+        self.note_suffix = self.conf.get(common.SETTING_GROUP_GENERAL,
+                                         common.SETTING_NOTE_SUFFIX,
+                                         common.DEFAULT_NOTE_SUFFIX)
+
+        self.note_naming = conf.get(common.SETTING_GROUP_GENERAL,
+                                    common.SETTING_NOTE_NAMING,
+                                    common.NOTE_NAMING_USER)
+        if self.note_naming not in common.NOTE_NAMING_OPTIONS:
+            logging.error(f"Configuration option 'note-naming' ('{self.note_naming}') is invalid.")
+            self.note_naming = common.NOTE_NAMING_USER
+
         # external editor
         self.external_editor = self.conf.get(common.SETTING_GROUP_GENERAL,
                                              common.SETTING_EXT_EDITOR)
 
         # protocols accepted to open with open-url
         self.protos = conf.list(common.SETTING_GROUP_GENERAL,
                                 common.SETTING_PROTOCOLS)
@@ -1347,14 +1391,15 @@
             ('r',): 'show-related',
             ('<return>',): 'select-item',
             ('h',): 'toggle-hidden',
             ('d',): 'toggle-done',
             ('e',): 'edit-task',
             ('E',): 'edit-external',
             ('n',): 'create-task',
+            ('N',): 'edit-note',
             (':',): 'jump-to',
             ('/',): 'search',
             ('^',): 'clear-search',
             ('c',): 'search-context',
             ('p',): 'search-project',
             ('<f6>',): 'select-project',
             ('<f7>',): 'select-context',
@@ -1418,14 +1463,15 @@
             'load-search': self.do_load_search,
             'save-search': self.do_save_search,
             'clear-search': self.do_clear_search,
             'edit-task': self.do_edit_task,
             'edit-external': self.do_edit_task_external,
             'edit-file-external': self.do_edit_file_external,
             'create-task': self.do_create_task,
+            'edit-note': self.do_edit_note,
             'jump-to': self.do_jump_to,
             'open-url': self.do_open_url,
             'toggle-tracking': self.do_toggle_tracking,
             'toggle-done': self.do_toggle_done,
             'toggle-hidden': self.do_toggle_hidden,
             'show-help': self.do_show_help,
             'delegate': self.do_delegate,
@@ -2002,15 +2048,15 @@
     def do_clear_search(self):
         self.set_search('')
 
     def do_save_search(self):
         self.focus.append(UserInput(self.tasks,
                                     self._do_save_search,
                                     lambda: self.show_cursor(False),
-                                    "Save Search"))
+                                    tr("Save Search")))
         self.paint(True)
 
     def _do_save_search(self, name):
         self.show_cursor(False)
 
         if len(name.strip()) == 0:
             self.error(tr("Not a valid name for a named search"))
@@ -2432,14 +2478,133 @@
             self.focus.append(Selector(self.tasks,
                                        projects,
                                        lambda p: self.add_to_search('+'+p),
                                        title="Select Project",
                                        numbered=True))
             self.paint(True)
 
+    def do_edit_note(self):
+        """Edit the note of the selected task, create note if it doesn't exist"""
+        if len(self.notes) == 0:
+            self.error(tr("No 'notes' directories defined."))
+            return
+
+        editor = self.resolve_editor()
+        if editor is None:
+            self.error(tr("Could not determine your external text editor"))
+            return
+
+        task = self.tasks.selected_item
+        if task is None:
+            return
+
+        filename = task.task.attributes.get('note', [])
+
+        if len(filename) == 0:
+            if self.note_naming == common.NOTE_NAMING_CANCEL:
+                self.error(tr("No 'note:' tag"))
+                return
+
+            if self.note_naming == common.NOTE_NAMING_USER:
+                self.focus.append(UserInput(self.tasks,
+                                            lambda n: self._append_note_tag(task, n),
+                                            lambda: self.show_cursor(False),
+                                            tr("Note filename")))
+                self.paint(True)
+                return
+
+            assert self.note_naming == common.NOTE_NAMING_AUTO
+            # does the task have a task id?
+            taskid = task.task.attributes.get('id', [])
+            if len(taskid) == 0:
+                # add a task id
+                newtask = utils.auto_task_id(self.sources,
+                                             str(task.task) + " id:#")
+                success, newtask = self.modify_task(task,
+                                                    lambda t: t.parse(newtask))
+                if not success:
+                    if newtask is not None:
+                        self.error(tr("Failed to add id"))
+                    return
+                task = self.tasks.selected_item
+                taskid = task.task.attributes.get('id')
+
+            # we use the taskid as the note's filename
+            taskid = taskid[0]
+
+            # make the new filename unique, so we don't overwrite existing files
+            counter = None
+            while True:
+                notefilename = taskid
+                if counter is not None:
+                    notefilename += '_' + str(counter)
+                notepath = self.resolve_note(notefilename)
+                if notepath.exists():
+                    if counter is None:
+                        counter = 1
+                    else:
+                        counter += 1
+                    continue
+                filename = [notepath.name]
+                break
+
+            # add the note: tag
+            newtask = str(task.task) + ' note:' + notefilename
+            success, _ = self.modify_task(task, lambda t: t.parse(newtask))
+            if not success:
+                return
+            self.paint(True)
+
+        filename = self.resolve_note(filename[0])
+
+        logging.debug(f"Edit note: {filename}")
+        with ShellContext(self.screen, True):
+            subprocess.run(editor + [str(filename)])
+        self.paint(True)
+
+    def _append_note_tag(self, task, name):
+        name = name.replace(' ', '_')
+        tasktext = str(task.task) + ' note:' + name
+        success, _ = self.modify_task(task,
+                                      lambda t: t.parse(tasktext))
+        if success:
+            self.do_edit_note()
+
+    def resolve_note(self, filename):
+        """Returns a path to a note file
+        The file may or may not exist"""
+        assert len(self.notes) > 0
+
+        # clean up the filename
+        while '..' in filename:
+            filename = filename.replace('..', '')
+        while '//' in filename:
+            filename = filename.replace('//', '/')
+        if filename.startswith('/'):
+            filename = filename[1:]
+
+        # add the suffix, if required
+        filename = Path(filename)
+        if len(filename.suffix) == 0:
+            filename = Path(str(filename) + self.note_suffix)
+
+        # see if the note exists already
+        location = None
+        for path in self.notes:
+            if (path / filename).is_file():
+                location = path / filename
+                break
+
+        # use the default location if the note doesn't exist yet
+        if location is None:
+            location = self.notes[0] / filename
+        filename = location.resolve()
+
+        return filename
+
 
 def parse_key_sequence(text):
     sequence = []
 
     pos = 0
     while pos < len(text):
         token = text[pos]
@@ -2475,36 +2640,38 @@
         w -= 1
 
     w -= 2  # the indicators left and right
     label = title[:min(w, len(title))]
     if label != title:
         label = label[:-1] + '…'
 
-    panel.win.addstr(0, 1, f"┤{label}├", attr)
+    panel.win.addstr(0, 1, title_frame(label), attr)
+
+
+def title_frame(label):
+    return TITLE_FRAME[0] + label + TITLE_FRAME[1]
 
 
-def run_cursesui(args):
+def run_cursesui(args, config):
     logging.basicConfig(format="[%(levelname)s] %(message)s", filename=args.log_file)
     logging.getLogger().setLevel(args.log_level.upper())
 
     success = 0
-    sources = utils.open_sources(args)
+    sources = utils.open_sources(args, config)
 
     if len(sources) == 0:
         success = -1
         print(tr("To start pter you must provide at least one todo.txt file. "
                  "See --help for more information."),
               file=sys.stderr)
     else:
         search = Searcher('', False)
         search.update_sources(sources)
 
-        window = CursesApplication(sources,
-                                   configuration.get_config(args),
-                                   args.search)
+        window = CursesApplication(sources, config, args.search)
 
         exception = None
 
         try:
             window.run()
         except Exception as exc:
             callstack = ''.join(traceback.format_tb(exc.__traceback__))
```

### Comparing `pter-3.8.0/pter/docs/pter.html` & `pter-3.9.0/pter/docs/pter.html`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/pter/icons/qpter_16x16.png` & `pter-3.9.0/pter/icons/qpter_16x16.png`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/pter/icons/qpter_32x32.png` & `pter-3.9.0/pter/icons/qpter_32x32.png`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/pter/key.py` & `pter-3.9.0/pter/key.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/pter/main.py` & `pter-3.9.0/pter/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 except ImportError as exc:
     run_qtui = None
     qterr = exc
 
 from pter import common
 from pter import version
 from pter import utils
+from pter import configuration
 from pter.tr import tr
 
 
 def parse_args(is_qtui):
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config',
                         type=str,
@@ -64,16 +65,14 @@
                         nargs='*',
                         help=tr('todo.txt file(s) to open'))
 
     return parser.parse_args()
 
 
 def run():
-    locale.setlocale(locale.LC_ALL, '')
-    code = locale.getpreferredencoding()
     is_qtui = pathlib.Path(sys.argv[0]).name == common.QTPROGRAMNAME
 
     args = parse_args(is_qtui)
 
     if args.check_for_updates:
         latest_version = utils.query_latest_version()
         if version.__version__ < latest_version:
@@ -84,50 +83,54 @@
         return 0
 
     # ensure logfile directory
     if args.log_file is not None:
         log_path = pathlib.Path(args.log_file).resolve().expanduser().parent
         log_path.mkdir(parents=True, exist_ok=True)
 
+    # obtain config
+    config = configuration.get_config(args)
+
     if args.new_task is not None:
-        if len(args.filename) != 1:
-            print(tr("You have to provide exactly one todo.txt file."), file=sys.stderr)
+        sources = utils.open_sources(args, config)
+        if len(sources) == 0:
+            print(tr("You have to provide at least one todo.txt file."), file=sys.stderr)
             return 1
 
-        filename = pathlib.Path(args.filename[0]).expanduser().resolve()
+        filename = sources[0].source.filename
 
         text = args.new_task
         if text == '-':
             text = sys.stdin.read()
 
         if len(text) == 0:
             return -1
 
         mode = "r+t"
         if not filename.exists():
             mode = "wt"
         
-        with open(args.filename[0], mode, encoding="utf-8") as fd:
+        with open(filename, mode, encoding="utf-8") as fd:
             fd.seek(0, io.SEEK_END)
             for line in text.split("\n"):
                 if len(line.strip()) == 0:
                     continue
                 fd.write(utils.dehumanize_dates(line) + "\n")
         return 0
 
     if is_qtui:
         success = -1
         if run_qtui is None:
             print(tr("PyQt5 is not installed or could otherwise not be imported: {}").format(qterr),
                   file=sys.stderr)
         else:
             success = 0
-            run_qtui(args)
+            run_qtui(args, config)
 
     elif run_cursesui is not None:
-        success = run_cursesui(args)
+        success = run_cursesui(args, config)
 
     else:
         print(tr("Neither PyQt5 nor curses are installed. To start the Qt version, please run 'qpter'."), file=sys.stderr)
         success = -2
 
     return success
```

### Comparing `pter-3.8.0/pter/qtui.py` & `pter-3.9.0/pter/qtui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import html
 import re
 import configparser
 import pathlib
 import getpass
 import sys
 import webbrowser
 import os
@@ -1766,15 +1765,15 @@
         utils.update_displaynames(self.sources)
         self.window.taskModel.reload()
 
     def do_quit(self):
         self.window.close()
 
 
-def run_qtui(args):
+def run_qtui(args, config):
     tmpdir = pathlib.Path(QtCore.QDir.tempPath())
     tmpdir.mkdir(parents=True, exist_ok=True)
     username = getpass.getuser().replace(' ', '_')
     fn = f"{common.QTPROGRAMNAME}-{username}.pid"
     fullpath = tmpdir / fn
 
     sock = None
@@ -1811,16 +1810,15 @@
 
     logging.basicConfig(format="[%(levelname)s] %(message)s", filename=args.log_file)
     logging.getLogger().setLevel(args.log_level.upper())
 
     app = QApplication([])
     app.setApplicationName(common.QTPROGRAMNAME)
     app.setApplicationVersion(version.__version__)
-    p = Program(configuration.get_config(args), utils.open_sources(args), fullpath)
+    p = Program(config, utils.open_sources(args), fullpath)
     p.window.actionShowAboutQt.triggered.connect(app.aboutQt)
     p.window.activateWindow()
 
     if args.add_task:
         p.window.actionNew.trigger()
 
     return app.exec_()
-
```

### Comparing `pter-3.8.0/pter/searcher.py` & `pter-3.9.0/pter/searcher.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/pter/source.py` & `pter-3.9.0/pter/source.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/pter/utils.py` & `pter-3.9.0/pter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -576,16 +576,26 @@
         if version.startswith('v'):
             version = version[1:]
         return version
     except:
         return ''
 
 
-def open_sources(args):
-    sources = [Source(TodoTxt(pathlib.Path(fn).expanduser().resolve())) for fn in args.filename]
+def open_sources(args, config):
+    files = [pathlib.Path(fn).expanduser().resolve() for fn in args.filename]
+    if len(files) == 0:
+        files = config.get(common.SETTING_GROUP_GENERAL,
+                           common.SETTING_FILES, [])
+        if "\n" in files:
+            files = [fn.strip()
+                     for fn in files.split("\n")
+                     if len(fn.strip()) > 0]
+        files = [pathlib.Path(fn.strip()).expanduser().resolve()
+                 for fn in files]
+    sources = [Source(TodoTxt(fn)) for fn in files]
     for source in sources:
         if source.filename.exists():
             source.parse()
     return sources
 
 
 def create_from_search(searcher):
```

### Comparing `pter-3.8.0/pter.egg-info/PKG-INFO` & `pter-3.9.0/pter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pter
-Version: 3.8.0
+Version: 3.9.0
 Summary: Console UI to manage your todo.txt file(s).
 Home-page: https://vonshednob.cc/pter
 Author: R
 Author-email: contact+pter@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pter-3.8.0/pter.egg-info/SOURCES.txt` & `pter-3.9.0/pter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/setup.py` & `pter-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/tests/test_displaynames.py` & `pter-3.9.0/tests/test_displaynames.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/tests/test_priochange.py` & `pter-3.9.0/tests/test_priochange.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/tests/test_pter.py` & `pter-3.9.0/tests/test_pter.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/tests/test_rec.py` & `pter-3.9.0/tests/test_rec.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/tests/test_searcher.py` & `pter-3.9.0/tests/test_searcher.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/tests/test_sorting.py` & `pter-3.9.0/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `pter-3.8.0/tests/test_taskid.py` & `pter-3.9.0/tests/test_taskid.py`

 * *Files identical despite different names*

