# Comparing `tmp/rich-click-1.8.0.dev0.tar.gz` & `tmp/rich-click-1.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-click-1.8.0.dev0.tar", last modified: Tue Apr  9 11:19:35 2024, max compression
+gzip compressed data, was "rich-click-1.8.0.dev1.tar", last modified: Tue Apr  9 13:13:34 2024, max compression
```

## Comparing `rich-click-1.8.0.dev0.tar` & `rich-click-1.8.0.dev1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.708014 rich-click-1.8.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27385 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.008108 rich-click-1.8.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.012108 rich-click-1.8.0.dev1/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27385 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.012108 rich-click-1.8.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_rich_click_cli.py
```

### Comparing `rich-click-1.8.0.dev0/LICENSE` & `rich-click-1.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/PKG-INFO` & `rich-click-1.8.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev0
+Version: 1.8.0.dev1
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -79,15 +79,15 @@
     <img src="https://github.com/ewels/rich-click/workflows/Test%20Coverage/badge.svg" alt="Test Coverage badge">
     <img src="https://github.com/ewels/rich-click/workflows/Lint%20code/badge.svg" alt="Lint code badge">
 </p>
 
 ---
 
 <p align="center">
-    <a href="https://ewels.github.io/rich-click">Documentation</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Source Code</a>&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Changelog</a>
+    <a href="https://ewels.github.io/rich-click">Documentation</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Source Code</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Changelog</a>
 </p>
 
 ---
 
 **rich-click** is a shim around [Click](https://click.palletsprojects.com/) that renders help output nicely using [Rich](https://github.com/Textualize/rich).
 
 - Click is a _"Python package for creating beautiful command line interfaces"_.
```

### Comparing `rich-click-1.8.0.dev0/README.md` & `rich-click-1.8.0.dev1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <img src="https://github.com/ewels/rich-click/workflows/Test%20Coverage/badge.svg" alt="Test Coverage badge">
     <img src="https://github.com/ewels/rich-click/workflows/Lint%20code/badge.svg" alt="Lint code badge">
 </p>
 
 ---
 
 <p align="center">
-    <a href="https://ewels.github.io/rich-click">Documentation</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Source Code</a>&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Changelog</a>
+    <a href="https://ewels.github.io/rich-click">Documentation</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Source Code</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Changelog</a>
 </p>
 
 ---
 
 **rich-click** is a shim around [Click](https://click.palletsprojects.com/) that renders help output nicely using [Rich](https://github.com/Textualize/rich).
 
 - Click is a _"Python package for creating beautiful command line interfaces"_.
```

### Comparing `rich-click-1.8.0.dev0/pyproject.toml` & `rich-click-1.8.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/__init__.py` & `rich-click-1.8.0.dev1/src/rich_click/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.0dev0"
+__version__ = "1.8.0dev1"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich-click-1.8.0.dev0/src/rich_click/_compat_click.py` & `rich-click-1.8.0.dev1/src/rich_click/_compat_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/cli.py` & `rich-click-1.8.0.dev1/src/rich_click/cli.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/decorators.py` & `rich-click-1.8.0.dev1/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/patch.py` & `rich-click-1.8.0.dev1/src/rich_click/patch.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/rich_click.py` & `rich-click-1.8.0.dev1/src/rich_click/rich_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/rich_command.py` & `rich-click-1.8.0.dev1/src/rich_click/rich_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,9 +402,7 @@
             getattr(RichCommand, method_name)(cmd, ctx, formatter)
         else:
             getattr(cmd, method_name)(ctx, formatter)
 
     if hasattr(cmd.__class__, "format_commands"):
         if method_is_from_subclass_of(cmd.__class__, cls, "format_commands"):
             getattr(RichMultiCommand, "format_commands")(cmd, ctx, formatter)
-        else:
-            getattr(cmd, "format_commands")(ctx, formatter)
```

### Comparing `rich-click-1.8.0.dev0/src/rich_click/rich_context.py` & `rich-click-1.8.0.dev1/src/rich_click/rich_context.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/rich_help_configuration.py` & `rich-click-1.8.0.dev1/src/rich_click/rich_help_configuration.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/rich_help_formatter.py` & `rich-click-1.8.0.dev1/src/rich_click/rich_help_formatter.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/rich_help_rendering.py` & `rich-click-1.8.0.dev1/src/rich_click/rich_help_rendering.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click/utils.py` & `rich-click-1.8.0.dev1/src/rich_click/utils.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/src/rich_click.egg-info/PKG-INFO` & `rich-click-1.8.0.dev1/src/rich_click.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev0
+Version: 1.8.0.dev1
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -79,15 +79,15 @@
     <img src="https://github.com/ewels/rich-click/workflows/Test%20Coverage/badge.svg" alt="Test Coverage badge">
     <img src="https://github.com/ewels/rich-click/workflows/Lint%20code/badge.svg" alt="Lint code badge">
 </p>
 
 ---
 
 <p align="center">
-    <a href="https://ewels.github.io/rich-click">Documentation</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Source Code</a>&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Changelog</a>
+    <a href="https://ewels.github.io/rich-click">Documentation</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Source Code</a>&nbsp&nbsp·&nbsp&nbsp<a href="https://github.com/ewels/rich-click">Changelog</a>
 </p>
 
 ---
 
 **rich-click** is a shim around [Click](https://click.palletsprojects.com/) that renders help output nicely using [Rich](https://github.com/Textualize/rich).
 
 - Click is a _"Python package for creating beautiful command line interfaces"_.
```

### Comparing `rich-click-1.8.0.dev0/src/rich_click.egg-info/SOURCES.txt` & `rich-click-1.8.0.dev1/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/tests/test_config.py` & `rich-click-1.8.0.dev1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/tests/test_exit_code.py` & `rich-click-1.8.0.dev1/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/tests/test_help.py` & `rich-click-1.8.0.dev1/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev0/tests/test_rich_click_cli.py` & `rich-click-1.8.0.dev1/tests/test_rich_click_cli.py`

 * *Files identical despite different names*

