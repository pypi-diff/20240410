# Comparing `tmp/xarg-python-1.4.4.tar.gz` & `tmp/xarg-python-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-1.4.4.tar", last modified: Mon Apr  8 16:20:14 2024, max compression
+gzip compressed data, was "xarg-python-1.4.5.tar", last modified: Wed Apr 10 05:09:47 2024, max compression
```

## Comparing `xarg-python-1.4.4.tar` & `xarg-python-1.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:20:14.108264 xarg-python-1.4.4/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-08 16:20:14.108264 xarg-python-1.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.4/README.md
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-08 16:20:14.108264 xarg-python-1.4.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:20:14.098264 xarg-python-1.4.4/xarg/
--rw-r--r--   0 root         (0) root         (0)      490 2024-04-06 10:39:58.000000 xarg-python-1.4.4/xarg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22139 2024-04-08 16:13:46.000000 xarg-python-1.4.4/xarg/actuator.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-08 16:17:56.000000 xarg-python-1.4.4/xarg/attribute.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-04-06 18:33:10.000000 xarg-python-1.4.4/xarg/colorful.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.4/xarg/complete.py
--rw-r--r--   0 root         (0) root         (0)     4211 2024-04-08 16:15:15.000000 xarg-python-1.4.4/xarg/logger.py
--rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.4/xarg/parser.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.4/xarg/safefile.py
--rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.4/xarg/scanner.py
--rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.4/xarg/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:20:14.108264 xarg-python-1.4.4/xarg_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:20:14.000000 xarg-python-1.4.4/xarg_python.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 05:09:47.720985 xarg-python-1.4.5/
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-12-26 08:19:24.000000 xarg-python-1.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1424 2024-04-10 05:09:47.720985 xarg-python-1.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-12-26 08:19:24.000000 xarg-python-1.4.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-10 05:09:47.720985 xarg-python-1.4.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      779 2024-03-28 12:58:33.000000 xarg-python-1.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 05:09:47.720985 xarg-python-1.4.5/xarg/
+-rw-r--r--   0 root         (0) root         (0)      490 2024-04-07 12:41:34.000000 xarg-python-1.4.5/xarg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22137 2024-04-09 12:36:04.000000 xarg-python-1.4.5/xarg/actuator.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-10 05:09:21.000000 xarg-python-1.4.5/xarg/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-04-07 12:41:34.000000 xarg-python-1.4.5/xarg/colorful.py
+-rw-r--r--   0 root         (0) root         (0)     8184 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/complete.py
+-rw-r--r--   0 root         (0) root         (0)     4359 2024-04-09 12:43:23.000000 xarg-python-1.4.5/xarg/logger.py
+-rw-r--r--   0 root         (0) root         (0)     8479 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/safefile.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2023-12-28 08:08:34.000000 xarg-python-1.4.5/xarg/scanner.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 05:09:47.720985 xarg-python-1.4.5/xarg_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1424 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/zip-safe
```

### Comparing `xarg-python-1.4.4/LICENSE` & `xarg-python-1.4.5/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Mingzhe Zou <zoumingzhe@outlook.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Mingzhe Zou <zoumingzhe@outlook.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `xarg-python-1.4.4/README.md` & `xarg-python-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/setup.cfg` & `xarg-python-1.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/setup.py` & `xarg-python-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/xarg/actuator.py` & `xarg-python-1.4.5/xarg/actuator.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,16 +426,16 @@
 
             option_level = filter_optional_name("--level", "--log-level")
             if isinstance(option_level, str):
                 group_level.add_argument(
                     option_level,
                     type=str,
                     nargs="?",
-                    const=self.LOG_LEVEL_INFO.lower(),
-                    default=self.LOG_LEVEL_INFO.lower(),
+                    const=self.LOG_LEVELS.INFO.value,
+                    default=self.LOG_LEVELS.INFO.value,
                     choices=self.ALLOWED_LOG_LEVELS,
                     dest="_log_level_str_",
                     help="Logger output level, default info.")
 
             for level in self.ALLOWED_LOG_LEVELS:
                 options = []
                 if isinstance(filter_optional_name(f"-{level[0]}"), str):
```

### Comparing `xarg-python-1.4.4/xarg/colorful.py` & `xarg-python-1.4.5/xarg/colorful.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/xarg/complete.py` & `xarg-python-1.4.5/xarg/complete.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/xarg/logger.py` & `xarg-python-1.4.5/xarg/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding:utf-8
 
+from enum import Enum
 import logging
 import os
 import sys
 from time import time
 from typing import Iterable
 from typing import List
 from typing import Optional
@@ -42,30 +43,35 @@
 
     @property
     def timeout(self) -> bool:
         return self.interval_seconds > self.max_interval_seconds
 
 
 class log:
-    LOG_LEVEL_FATAL: str = "FATAL"
-    LOG_LEVEL_ERROR: str = "ERROR"
-    LOG_LEVEL_WARN: str = "WARN"
-    LOG_LEVEL_INFO: str = "INFO"
-    LOG_LEVEL_DEBUG: str = "DEBUG"
+    class LOG_LEVELS(Enum):
+        CRITICAL = "fatal"
+        ERROR = "error"
+        WARNING = "warn"
+        INFO = "info"
+        DEBUG = "debug"
+    ALLOWED_LOG_LEVELS: List[str] = [
+        LOG_LEVELS.CRITICAL.value,
+        LOG_LEVELS.ERROR.value,
+        LOG_LEVELS.WARNING.value,
+        LOG_LEVELS.INFO.value,
+        LOG_LEVELS.DEBUG.value,
+    ]
     DEFAULT_LOG_FORMAT: str = "%(log_color)s%(message)s"
     DEFAULT_LOG_COLORS: LogColors = {
-        LOG_LEVEL_FATAL: "light_red",
-        LOG_LEVEL_ERROR: "red",
-        LOG_LEVEL_WARN: "yellow",
-        LOG_LEVEL_INFO: "white",
-        LOG_LEVEL_DEBUG: "black",
+        LOG_LEVELS.CRITICAL.name: "light_red",
+        LOG_LEVELS.ERROR.name: "red",
+        LOG_LEVELS.WARNING.name: "yellow",
+        LOG_LEVELS.INFO.name: "white",
+        LOG_LEVELS.DEBUG.name: "black",
     }
-    ALLOWED_LOG_LEVELS: List[str] = [
-        k.lower() for k in DEFAULT_LOG_COLORS.keys()
-    ]
 
     def __init__(self):
         self.__initiated_names: Set[str] = set()
 
     def logger_initiated(self, name: str) -> bool:
         return name in self.__initiated_names
```

### Comparing `xarg-python-1.4.4/xarg/parser.py` & `xarg-python-1.4.5/xarg/parser.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/xarg/safefile.py` & `xarg-python-1.4.5/xarg/safefile.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/xarg/scanner.py` & `xarg-python-1.4.5/xarg/scanner.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.4/xarg/util.py` & `xarg-python-1.4.5/xarg/util.py`

 * *Files identical despite different names*

