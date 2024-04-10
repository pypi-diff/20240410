# Comparing `tmp/pycotore-0.0.2.tar.gz` & `tmp/pycotore-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.0.2.tar", max compression
+gzip compressed data, was "pycotore-0.0.3.tar", max compression
```

## Comparing `pycotore-0.0.2.tar` & `pycotore-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.0.2/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.0.2/pycotore/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.0.2/pycotore/constants.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.0.2/pycotore/exceptions.py
--rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.0.2/pycotore/logger.py
--rw-r--r--   0        0        0     2874 2024-04-09 19:49:52.142541 pycotore-0.0.2/pycotore/progress.py
--rw-r--r--   0        0        0      598 2024-04-09 18:06:26.427901 pycotore-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 pycotore-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.0.3/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.0.3/pycotore/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.0.3/pycotore/constants.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.0.3/pycotore/exceptions.py
+-rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.0.3/pycotore/logger.py
+-rw-r--r--   0        0        0     4420 2024-04-10 14:20:50.041788 pycotore-0.0.3/pycotore/progress.py
+-rw-r--r--   0        0        0      599 2024-04-10 07:47:48.046176 pycotore-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.0.3/PKG-INFO
```

### Comparing `pycotore-0.0.2/LICENSE` & `pycotore-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.2/pycotore/logger.py` & `pycotore-0.0.3/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.2/pycotore/progress.py` & `pycotore-0.0.3/pycotore/progress.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,107 @@
 import sys
 import os
-from logging import getLogger, DEBUG, basicConfig
+from datetime import datetime
+from logging import getLogger
 
-basicConfig(level=DEBUG)
+# basicConfig(level=DEBUG)
 _logger = getLogger(__name__)
 
 
-class PorgressBar():
+class ProgressBar():
     """
     Progress bar class
     """
 
-    def __init__(self, base_marker: str = ".", done_marke: str = "#", current_marker: str = ">"):
+    def __init__(
+                self,
+                base_marker: str = ".",
+                done_marke: str = "#",
+                current_marker: str = ">",
+                show_percents: bool = True,
+                show_estimate: bool = True
+            ):
         self.preffix: str = ""
         self.suffix: str = ""
         self.bar_length: int = 0
         self.bar_size: int = 0
         self.terminal_size: int = os.get_terminal_size().columns
         self.progress: float = 0.00
         self.total: float = 100.00
-        self.done_marker = done_marke
-        self.in_progress_marker = base_marker
-        self.current_marker = current_marker
+        self.done_marker: str = done_marke
+        self.in_progress_marker: str = base_marker
+        self.current_marker: str = current_marker
+        self.percents: float = "|000.00%"
+        self.show_percents: bool = show_percents
+        self.show_numbers: bool = False
+        self.time_start = datetime.now()
+        self.show_estimate: bool = show_estimate
+        self.estimate = "|ETA: 00:00:00"
+
+    def flush_line(self) -> None:
+        sys.stdout.write("\n")
+        sys.stdout.flush()
 
     def __str__(self):
         bar = f"prefix: {self.preffix}\nsufix: {self.suffix}\nbar size: {self.bar_length}\ncurrent terminal: {self.terminal_size}\nbar size: {self.bar_size}\nMarker: {self.done_marker}\ntotal: {self.total}\nprogress: {self.progress}"
         return bar
 
+    def __calculate_estimate(self) -> None:
+        now = datetime.now()
+        run_time = now - self.time_start
+        left = self.total * run_time / self.progress - run_time
+        self.estimate = f"|ETA: {left.seconds//3600:0>2}:{left.seconds//60:0>2}:{left.seconds:0>2}"
+
+    def __update_percent_done(self) -> None:
+        percents = round(self.progress * 100 / self.total, 2)
+        self.percents = f"|{percents:0>6.2f}%"
+
     def __update_bar_length(self) -> None:
         """
         Updating progress bar total size
         """
-        self.bar_length = len(self.preffix) + len(self.suffix) + 1
+        self.bar_length = len(self.preffix) + len(self.suffix)
         self.__update_bar_size()
 
     def __update_bar_size(self) -> None:
         self.bar_size = self.terminal_size - self.bar_length - 3
+        if self.show_percents:
+            self.bar_size -= len(self.percents)
+        if self.show_estimate:
+            self.bar_size -= len(self.estimate)
 
-    def draw(self) -> None:
+    def __format_bar(self) -> str:
+        bar = ["\r"]
         finished = int(self.bar_size * self.progress / self.total)
         finished_mark = self.done_marker * finished
         in_progress_mark = self.in_progress_marker * (self.bar_size - finished - 1)
         if self.bar_size <= finished:
             self.current_marker = ""
-        if self.bar_length > self.terminal_size:
-            sys.stdout.write("\rDL:")
-        else:
-            sys.stdout.write(f"{self.preffix} [{finished_mark}{self.current_marker}{in_progress_mark}] {self.suffix}\r")
-            sys.stdout.flush()
+        if self.preffix:
+            bar.append(f"{self.preffix} ")
+        bar.append(f"[{finished_mark}{self.current_marker}{in_progress_mark}]")
+        if self.show_percents:
+            bar.append(self.percents)
+        if self.show_estimate:
+            bar.append(self.estimate)
+        if self.suffix:
+            bar.append(f"|{self.suffix}")
+        return "".join(bar)
+
+    def draw(self) -> None:
+        """
+        Draw a progress bar
+        """
+        if self.show_percents:
+            self.__update_percent_done()
+        if self.show_estimate:
+            self.__calculate_estimate()
+        bar = self.__format_bar()
+        sys.stdout.write(bar)
+        sys.stdout.flush()
 
     def set_prefix(self, preffix: str) -> None:
         """
         Change bar prefix
         """
         self.preffix = preffix
         self.__update_bar_length()
@@ -73,15 +123,14 @@
         except ValueError:
             _logger.warning("Unable to set bar size")
 
     def update_progress(self, done: float) -> None:
         """
         Update progress done percentage
         """
-        # self.progress = round(done * 100 / self.total, 2)
         self.progress = done
 
     def set_total(self, total) -> None:
         """
         Set progress bar total value
         """
         try:
```

### Comparing `pycotore-0.0.2/pyproject.toml` & `pycotore-0.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "pycotore"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
-description = "Genric classes for reuse"
+description = "Generic classes for reuse"
 version = "0.0.0a0"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pycotore"
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `pycotore-0.0.2/PKG-INFO` & `pycotore-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.0.2
-Summary: Genric classes for reuse
+Version: 0.0.3
+Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

