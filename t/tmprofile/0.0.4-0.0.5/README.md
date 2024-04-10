# Comparing `tmp/tmprofile-0.0.4.tar.gz` & `tmp/tmprofile-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmprofile-0.0.4.tar", last modified: Wed Apr  3 16:15:13 2024, max compression
+gzip compressed data, was "tmprofile-0.0.5.tar", last modified: Wed Apr 10 14:19:08 2024, max compression
```

## Comparing `tmprofile-0.0.4.tar` & `tmprofile-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 16:15:13.963051 tmprofile-0.0.4/
--rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.4/LICENSE
--rw-r--r--   0 vedrenne (271197) images    (7000)     2726 2024-04-03 16:15:13.963051 tmprofile-0.0.4/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)     2064 2024-04-03 16:11:58.000000 tmprofile-0.0.4/README.md
--rw-r--r--   0 vedrenne (271197) images    (7000)      835 2024-04-03 16:15:00.000000 tmprofile-0.0.4/pyproject.toml
--rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-03 16:15:13.963051 tmprofile-0.0.4/setup.cfg
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 16:15:13.963051 tmprofile-0.0.4/tmprofile/
--rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 14:04:17.000000 tmprofile-0.0.4/tmprofile/__init__.py
--rw-r--r--   0 vedrenne (271197) images    (7000)    13140 2024-04-03 16:09:27.000000 tmprofile-0.0.4/tmprofile/pyprofile.py
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-03 16:15:13.963051 tmprofile-0.0.4/tmprofile.egg-info/
--rw-r--r--   0 vedrenne (271197) images    (7000)     2726 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)      241 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/SOURCES.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/dependency_links.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)       50 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/requires.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-03 16:15:13.000000 tmprofile-0.0.4/tmprofile.egg-info/top_level.txt
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-10 14:19:08.649748 tmprofile-0.0.5/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1074 2024-04-03 14:04:43.000000 tmprofile-0.0.5/LICENSE
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2717 2024-04-10 14:19:08.649748 tmprofile-0.0.5/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2055 2024-04-10 14:18:24.000000 tmprofile-0.0.5/README.md
+-rw-r--r--   0 vedrenne (271197) images    (7000)      835 2024-04-10 14:18:06.000000 tmprofile-0.0.5/pyproject.toml
+-rw-r--r--   0 vedrenne (271197) images    (7000)       38 2024-04-10 14:19:08.649748 tmprofile-0.0.5/setup.cfg
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-10 14:19:08.645748 tmprofile-0.0.5/tmprofile/
+-rw-r--r--   0 vedrenne (271197) images    (7000)       40 2024-04-03 16:18:51.000000 tmprofile-0.0.5/tmprofile/__init__.py
+-rw-r--r--   0 vedrenne (271197) images    (7000)    13198 2024-04-09 15:14:47.000000 tmprofile-0.0.5/tmprofile/tmprofile.py
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2024-04-10 14:19:08.649748 tmprofile-0.0.5/tmprofile.egg-info/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     2717 2024-04-10 14:19:08.000000 tmprofile-0.0.5/tmprofile.egg-info/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)      241 2024-04-10 14:19:08.000000 tmprofile-0.0.5/tmprofile.egg-info/SOURCES.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)        1 2024-04-10 14:19:08.000000 tmprofile-0.0.5/tmprofile.egg-info/dependency_links.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       50 2024-04-10 14:19:08.000000 tmprofile-0.0.5/tmprofile.egg-info/requires.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       10 2024-04-10 14:19:08.000000 tmprofile-0.0.5/tmprofile.egg-info/top_level.txt
```

### Comparing `tmprofile-0.0.4/LICENSE` & `tmprofile-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tmprofile-0.0.4/PKG-INFO` & `tmprofile-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
-Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
-Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
+Project-URL: Homepage, https://github.com/ListIndexOutOfRange/tmprofile
+Project-URL: Issues, https://github.com/ListIndexOutOfRange/tmprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -27,15 +27,15 @@
 ## Usage
 
 ### 1. As a context manager
 
 ```python
 from tmprofile import Profile
 
-with Profile(name, ...) as profiler:
+with Profile() as profiler:
     f(...) # some intensive code
 # profile is automatically saved as a json file.
 # display elapsed time, RAM & VRAM consumption evolution
 profiler.print()
 profiler.plot()
 ```
```

### Comparing `tmprofile-0.0.4/README.md` & `tmprofile-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## Usage
 
 ### 1. As a context manager
 
 ```python
 from tmprofile import Profile
 
-with Profile(name, ...) as profiler:
+with Profile() as profiler:
     f(...) # some intensive code
 # profile is automatically saved as a json file.
 # display elapsed time, RAM & VRAM consumption evolution
 profiler.print()
 profiler.plot()
 ```
```

### Comparing `tmprofile-0.0.4/pyproject.toml` & `tmprofile-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tmprofile"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Luc Vedrenne", email="vedrenneluc@gmail.com" },
 ]
 description = "A simple time, ram & vram python profiler."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -22,16 +22,16 @@
     "matplotlib",
     "psutil",
     "prettytable",
     "nvidia_ml_py3",
 ]
 
 [project.urls]
-Homepage = "https://github.com/ListIndexOutOfRange/pyprofile"
-Issues = "https://github.com/ListIndexOutOfRange/pyprofile/issues"
+Homepage = "https://github.com/ListIndexOutOfRange/tmprofile"
+Issues = "https://github.com/ListIndexOutOfRange/tmprofile/issues"
 
 
 # Usage
 # > python3 -m build
 # > twine check dist/*
 # > twine upload --repository testpypi dist/*
 # > twine upload dist/*
```

### Comparing `tmprofile-0.0.4/tmprofile/pyprofile.py` & `tmprofile-0.0.5/tmprofile/tmprofile.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         filename = Path(Path(filename).stem).with_suffix('.json')  # works w/ or w/o extension
         if (output_dir / filename).exists():
             idx = self.get_run_idx(output_dir)
             filename = f'run{idx}_{filename.stem}'
             filename = Path(Path(filename).stem).with_suffix('.json')
         return output_dir / filename
 
-    def print(self) -> None:
+    def _print(self) -> None:
         table = PrettyTable(["Memory", "Min", "Median", "Max", "Average"])
         for memory in ('ram', 'vram'):
             total = self.data[f'total_{memory}']
             usage = np.array(self.data[memory])
             values = np.quantile(usage, np.array([0, 0.5, 1]))
             percents = values / total
             row = [memory.upper()]
@@ -226,14 +226,20 @@
         time = str(timedelta(seconds=self.data["elapsed_time"])).split(':')
         time_string = f'{time[0]} h {time[1]} m {time[2]} s'
         table.title = f'PROFILE : {self._name} | elapsed time: {time_string} s'
         print('\n' + str(table))
         with open(self._output_file.with_suffix('.txt'), 'w') as openfile:
             openfile.write(str(table))
 
+    def print(self) -> None:
+        try:
+            self._print()
+        except IndexError:  # wrapped function crashed before any values was recorded
+            print('No values recorded.')
+
     def plot(self, percent: bool = False):
         t = len(self.data['ram']) * self.data['time_delta']
         x = np.arange(0, t, self.data['timedelta'])
         ram, vram = np.array(self.data['ram']), np.array(self.data['vram'])
         if percent:
             ram /= self.data['total_ram']
             vram /= self.data['total_vram']
@@ -257,20 +263,16 @@
 
     def __exit__(self, exception_type, exception_value, exception_traceback) -> None:
         self._stop_event.set()  # Signal the monitor process to stop
         assert self._monitor_process is not None
         self._monitor_process.join()
         with open(self._output_file, 'r') as openfile:
             self.data = json.load(openfile)
-        if not self._verbose:
-            return
-        try:
+        if self._verbose:
             self.print()
-        except IndexError:  # wrapped function crashed before any values was recorded
-            pass
 
 
 # __________________________________________ Decorator __________________________________________ #
 
 def is_notebook() -> bool:
     try:
         shell = get_ipython().__class__.__name__
```

### Comparing `tmprofile-0.0.4/tmprofile.egg-info/PKG-INFO` & `tmprofile-0.0.5/tmprofile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tmprofile
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple time, ram & vram python profiler.
 Author-email: Luc Vedrenne <vedrenneluc@gmail.com>
-Project-URL: Homepage, https://github.com/ListIndexOutOfRange/pyprofile
-Project-URL: Issues, https://github.com/ListIndexOutOfRange/pyprofile/issues
+Project-URL: Homepage, https://github.com/ListIndexOutOfRange/tmprofile
+Project-URL: Issues, https://github.com/ListIndexOutOfRange/tmprofile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -27,15 +27,15 @@
 ## Usage
 
 ### 1. As a context manager
 
 ```python
 from tmprofile import Profile
 
-with Profile(name, ...) as profiler:
+with Profile() as profiler:
     f(...) # some intensive code
 # profile is automatically saved as a json file.
 # display elapsed time, RAM & VRAM consumption evolution
 profiler.print()
 profiler.plot()
 ```
```

