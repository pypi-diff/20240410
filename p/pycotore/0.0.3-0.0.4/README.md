# Comparing `tmp/pycotore-0.0.3.tar.gz` & `tmp/pycotore-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.0.3.tar", max compression
+gzip compressed data, was "pycotore-0.0.4.tar", max compression
```

## Comparing `pycotore-0.0.3.tar` & `pycotore-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.0.3/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.0.3/pycotore/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.0.3/pycotore/constants.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.0.3/pycotore/exceptions.py
--rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.0.3/pycotore/logger.py
--rw-r--r--   0        0        0     4420 2024-04-10 14:20:50.041788 pycotore-0.0.3/pycotore/progress.py
--rw-r--r--   0        0        0      599 2024-04-10 07:47:48.046176 pycotore-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.0.4/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.0.4/pycotore/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.0.4/pycotore/constants.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.0.4/pycotore/exceptions.py
+-rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.0.4/pycotore/logger.py
+-rw-r--r--   0        0        0     4429 2024-04-10 14:42:29.019304 pycotore-0.0.4/pycotore/progress.py
+-rw-r--r--   0        0        0      599 2024-04-10 07:47:48.046176 pycotore-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.0.4/PKG-INFO
```

### Comparing `pycotore-0.0.3/LICENSE` & `pycotore-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.3/pycotore/logger.py` & `pycotore-0.0.4/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.3/pycotore/progress.py` & `pycotore-0.0.4/pycotore/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         bar = f"prefix: {self.preffix}\nsufix: {self.suffix}\nbar size: {self.bar_length}\ncurrent terminal: {self.terminal_size}\nbar size: {self.bar_size}\nMarker: {self.done_marker}\ntotal: {self.total}\nprogress: {self.progress}"
         return bar
 
     def __calculate_estimate(self) -> None:
         now = datetime.now()
         run_time = now - self.time_start
         left = self.total * run_time / self.progress - run_time
-        self.estimate = f"|ETA: {left.seconds//3600:0>2}:{left.seconds//60:0>2}:{left.seconds:0>2}"
+        self.estimate = f"|ETA: {left.seconds // 3600:0>2}:{left.seconds // 60:0>2}:{left.seconds % 60:0>2}"
 
     def __update_percent_done(self) -> None:
         percents = round(self.progress * 100 / self.total, 2)
         self.percents = f"|{percents:0>6.2f}%"
 
     def __update_bar_length(self) -> None:
         """
```

### Comparing `pycotore-0.0.3/pyproject.toml` & `pycotore-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.3/PKG-INFO` & `pycotore-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

