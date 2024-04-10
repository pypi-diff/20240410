# Comparing `tmp/pyhelper_utils-0.0.7.tar.gz` & `tmp/pyhelper_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelper_utils-0.0.7.tar", max compression
+gzip compressed data, was "pyhelper_utils-0.0.8.tar", max compression
```

## Comparing `pyhelper_utils-0.0.7.tar` & `pyhelper_utils-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-09 09:04:47.085892 pyhelper_utils-0.0.7/LICENSE
--rw-r--r--   0        0        0      680 2024-04-09 09:04:47.085892 pyhelper_utils-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-04-09 09:04:47.085892 pyhelper_utils-0.0.7/pyhelper_utils/__init__.py
--rw-r--r--   0        0        0     1871 2024-04-09 09:04:47.085892 pyhelper_utils-0.0.7/pyhelper_utils/general.py
--rw-r--r--   0        0        0     1455 2024-04-09 09:04:47.086892 pyhelper_utils-0.0.7/pyhelper_utils/notifications.py
--rw-r--r--   0        0        0     1592 2024-04-09 09:04:47.086892 pyhelper_utils-0.0.7/pyhelper_utils/runners.py
--rw-r--r--   0        0        0     2324 2024-04-09 09:04:47.086892 pyhelper_utils-0.0.7/pyhelper_utils/shell.py
--rw-r--r--   0        0        0     1549 2024-04-09 09:04:51.211862 pyhelper_utils-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 11:34:42.614458 pyhelper_utils-0.0.8/LICENSE
+-rw-r--r--   0        0        0      680 2024-04-10 11:34:42.615458 pyhelper_utils-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/general.py
+-rw-r--r--   0        0        0     1455 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/notifications.py
+-rw-r--r--   0        0        0     1624 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/runners.py
+-rw-r--r--   0        0        0     2324 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/shell.py
+-rw-r--r--   0        0        0     1549 2024-04-10 11:34:46.935428 pyhelper_utils-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.8/PKG-INFO
```

### Comparing `pyhelper_utils-0.0.7/LICENSE` & `pyhelper_utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.7/README.md` & `pyhelper_utils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.7/pyhelper_utils/general.py` & `pyhelper_utils-0.0.8/pyhelper_utils/general.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.7/pyhelper_utils/notifications.py` & `pyhelper_utils-0.0.8/pyhelper_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.7/pyhelper_utils/runners.py` & `pyhelper_utils-0.0.8/pyhelper_utils/runners.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from typing import Callable, Any
 from simple_logger.logger import get_logger
 
 LOGGER = get_logger(name="runners")
 
 
-def function_runner_with_pdb(func: Callable, dry_run: bool = False) -> Any:
+def function_runner_with_pdb(func: Callable, dry_run: bool = False, *args, **kwargs) -> Any:
     """
     Run function with support to drop into pdb.
 
     In order to use this function you need to have --pdb in sys.argv
 
     Example:
         @click.option(
@@ -37,15 +37,15 @@
     Raises:
         SystemExit: If --pdb is not in sys.argv and execution failed
     """
     start_time = time.time()
     should_raise = False
 
     try:
-        return func()
+        return func(*args, **kwargs)
     except Exception as ex:
         if "--pdb" in sys.argv:
             _, _, tb = sys.exc_info()
             if not dry_run:
                 ipdb = __import__("ipdb")  # Bypass debug-statements pre-commit hook
                 ipdb.post_mortem(tb)
         else:
```

### Comparing `pyhelper_utils-0.0.7/pyhelper_utils/shell.py` & `pyhelper_utils-0.0.8/pyhelper_utils/shell.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.7/pyproject.toml` & `pyhelper_utils-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "pyhelper-utils"
-version = "0.0.7"
+version = "0.0.8"
 description = "Collective utility functions for python projects"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/pyhelper-utils"
 authors = [
   "Meni Yakove <myakove@gmail.com>",
   "Ruth Netser <rnetser@gmail.com>",
   "Debarati Basu-Nag <dbasunag@redhat.com>",
```

### Comparing `pyhelper_utils-0.0.7/PKG-INFO` & `pyhelper_utils-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelper-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collective utility functions for python projects
 Home-page: https://github.com/RedHatQE/pyhelper-utils
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

