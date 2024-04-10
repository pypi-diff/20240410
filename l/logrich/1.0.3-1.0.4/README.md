# Comparing `tmp/logrich-1.0.3.tar.gz` & `tmp/logrich-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrich-1.0.3.tar", max compression
+gzip compressed data, was "logrich-1.0.4.tar", max compression
```

## Comparing `logrich-1.0.3.tar` & `logrich-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-1.0.3/README.md
--rw-r--r--   0        0        0       21 2023-10-02 10:23:50.197687 logrich-1.0.3/logrich/__init__.py
--rw-r--r--   0        0        0     7266 2023-10-12 09:03:16.715453 logrich-1.0.3/logrich/app.py
--rw-r--r--   0        0        0     1427 2023-10-12 09:03:16.687453 logrich-1.0.3/logrich/config.py
--rw-r--r--   0        0        0     1168 2023-10-12 09:03:10.295443 logrich-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 logrich-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-1.0.4/README.md
+-rw-r--r--   0        0        0       21 2023-10-02 10:23:50.197687 logrich-1.0.4/logrich/__init__.py
+-rw-r--r--   0        0        0     7982 2024-04-10 03:54:37.054485 logrich-1.0.4/logrich/app.py
+-rw-r--r--   0        0        0     1505 2024-04-10 03:54:37.054485 logrich-1.0.4/logrich/config.py
+-rw-r--r--   0        0        0     1145 2024-04-10 03:54:37.054485 logrich-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 logrich-1.0.4/PKG-INFO
```

### Comparing `logrich-1.0.3/README.md` & `logrich-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `logrich-1.0.3/logrich/app.py` & `logrich-1.0.4/logrich/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import decimal
 import inspect
 import re
 from collections import deque
-from types import FrameType
+from datetime import datetime
+from functools import lru_cache
 from typing import Any, Deque
 
-from memoization import cached
 from rich.console import Console
 from rich.highlighter import ReprHighlighter
 from rich.pretty import pprint  # noqa
 from rich.table import Table
 from rich.theme import Theme
 
 from logrich.config import config
@@ -89,55 +89,76 @@
     markup=True,
     log_time=False,
     log_path=False,
     safe_box=True,
 )
 
 
-@cached
+@lru_cache
 class Log:
     """Extension log, use in tests."""
 
     def __init__(self, config: dict, **kwargs):
         self.deque: Deque = deque()
         self.config = config
         for k, v in kwargs.items():
             self.__setattr__(k, v)
 
-    def print(self, msg: str, frame: FrameType | None = None, **kwargs) -> None:
+    def print(
+        self,
+        # вызов логгера без параметров выведет текущую дату
+        msg: str | datetime = datetime.now().strftime("%H:%M:%S"),
+        frame=None,
+        **kwargs,
+    ) -> None:
         """Extension log."""
-        if not (level := self.deque.pop()):  # noqa WPS332
-            return
+        try:
+            if not (level := self.deque.pop()):  # noqa
+                return
+
+            level_key = f"LOG_LEVEL_{level.upper()}_TPL"
+            level_style = self.config.get(level_key, "").strip('"')
+            if not level_style:
+                return
+
+            frame = frame or inspect.currentframe().f_back
+            len_file_name_section = 30
+            file_name = kwargs.get("file_name", frame.f_code.co_filename)[-len_file_name_section:]
+            line = kwargs.get("line", frame.f_lineno)
+            divider = int(self.config.get("COLUMNS")) - len_file_name_section - 20
+            title = kwargs.get("title", "-" * divider)
 
-        frame = frame or inspect.currentframe().f_back  # type: ignore
-        file_name = kwargs.get("file_name", frame.f_code.co_filename)[-30:]  # type: ignore
-        line = kwargs.get("line", frame.f_lineno)  # type: ignore
-        title = kwargs.get("title", "---")
-
-        level_key = f"LOG_LEVEL_{level.upper()}_TPL"
-        level_style = self.config.get(level_key, "")
-        if level_style:
             if isinstance(msg, (str, int, float, bool, type(decimal), type(None))):
                 self.print_tbl(
-                    message=msg, file=file_name, line=line, level=level, level_style=level_style
+                    message=msg,
+                    file=file_name,
+                    line=line,
+                    level=level,
+                    level_style=level_style,
                 )
             elif isinstance(msg, (dict, tuple, list)):
                 # TODO add message for dict, tuple etc.
                 self.print_tbl(
-                    message=title, file=file_name, line=line, level=level, level_style=level_style
+                    message=title,
+                    file=file_name,
+                    line=line,
+                    level=level,
+                    level_style=level_style,
                 )
                 self.format_extra_obj(message=msg)
             else:
                 self.print_tbl(
                     message=msg,
                     file=file_name,
                     line=frame.f_lineno,
                     level=level,
                     level_style=level_style,
                 )
+        except Exception as err:
+            log.warning(err)
 
     def print_tbl(
         self,
         level_style: str,
         level: str,
         file: str,
         line: int,
@@ -223,16 +244,23 @@
 
         # MESSAGE
         table.add_row(self.print_message_for_table(message=message))
 
         console_dict.print(table, markup=True)
 
 
+class HashableDict(dict):  # noqa WPS600
+    """Add hash object."""
+
+    def __hash__(self):
+        return id(self)
+
+
 log = Log(
-    config=config,
     dev_style="blue",
     run_style="cyan",
     end_style="cyan",
     start_style="cyan",
     trace_style="turquoise2",
     debug_style="dark_orange3",
+    config=HashableDict(config),
 )
```

### Comparing `logrich-1.0.3/logrich/config.py` & `logrich-1.0.4/logrich/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 
 from dotenv import load_dotenv
 
 load_dotenv(".env")
 
 config = dict(
+    # ширина вывода имени файла
+    RATIO_FILE_NAME=50,
     COLUMNS=110,  # type: ignore
     # https://rich.readthedocs.io/en/stable/appendix/colors.html
     LOG_LEVEL_ELAPCE_TPL="[reverse turquoise2] ELAPCE [/]",
     LOG_LEVEL_START_TPL="[reverse i aquamarine1] START  [/]",
     LOG_LEVEL_END_TPL="[reverse i green4] END    [/reverse i green4]",
     LOG_LEVEL_TEST_TPL="[reverse grey70] TEST   [/]",
     LOG_LEVEL_DATA_TPL="[reverse cornflower_blue] DATA   [/]",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `logrich-1.0.3/pyproject.toml` & `logrich-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logrich"
-version = "1.0.3"
+version = "1.0.4"
 description = "loguru + rich = logrich"
 authors = ["Dmitry Mavlin <mavlind@list.ru>"]
 license = "GPL"
 readme = "README.md"
 keywords = ["logger", "loguru", "rich"]
 
 [project.urls]
@@ -12,15 +12,14 @@
 "Bug Tracker" = "https://gitlab.com/mavlin74/logrich/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 toml = "0.10.2"
 rich = "^12.4.4"
 importlib-metadata = "^5.2.0"
-memoization = "^0.4.0"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "6.2.4"
 pytest-picked = "0.4.6"
 pytest-testmon = "1.1.1"
 pytest-watch = "4.2.0"
```

### Comparing `logrich-1.0.3/PKG-INFO` & `logrich-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: logrich
-Version: 1.0.3
+Version: 1.0.4
 Summary: loguru + rich = logrich
 License: GPL
 Keywords: logger,loguru,rich
 Author: Dmitry Mavlin
 Author-email: mavlind@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: importlib-metadata (>=5.2.0,<6.0.0)
-Requires-Dist: memoization (>=0.4.0,<0.5.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: toml (==0.10.2)
 Description-Content-Type: text/markdown
 
 ### Логгер
```

