# Comparing `tmp/PyProfQueue-0.1.tar.gz` & `tmp/PyProfQueue-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.tar", last modified: Tue Apr  9 13:37:01 2024, max compression
+gzip compressed data, was "PyProfQueue-0.1.1.tar", last modified: Tue Apr  9 14:34:15 2024, max compression
```

## Comparing `PyProfQueue-0.1.tar` & `PyProfQueue-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 13:37:01.318337 PyProfQueue-0.1/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     3813 2024-04-09 13:37:01.318337 PyProfQueue-0.1/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 13:37:01.318337 PyProfQueue-0.1/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 13:37:01.318337 PyProfQueue-0.1/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1435 2024-03-27 13:45:25.000000 PyProfQueue-0.1/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      732 2024-04-04 13:48:15.000000 PyProfQueue-0.1/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4517 2024-04-09 09:21:10.000000 PyProfQueue-0.1/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    33249 2024-04-09 11:30:09.000000 PyProfQueue-0.1/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 13:37:01.318337 PyProfQueue-0.1/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     3813 2024-04-09 13:37:01.000000 PyProfQueue-0.1/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-09 13:37:01.000000 PyProfQueue-0.1/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-09 13:37:01.000000 PyProfQueue-0.1/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-09 13:37:01.000000 PyProfQueue-0.1/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-09 13:37:01.000000 PyProfQueue-0.1/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     3115 2024-04-09 09:02:52.000000 PyProfQueue-0.1/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-09 13:37:01.318337 PyProfQueue-0.1/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1194 2024-04-09 13:36:50.000000 PyProfQueue-0.1/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     3815 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.1/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PyProfQueue/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1435 2024-03-27 13:45:25.000000 PyProfQueue-0.1.1/PyProfQueue/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      732 2024-04-04 13:48:15.000000 PyProfQueue-0.1.1/PyProfQueue/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4517 2024-04-09 09:21:10.000000 PyProfQueue-0.1.1/PyProfQueue/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    33503 2024-04-09 14:32:49.000000 PyProfQueue-0.1.1/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.1/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     3815 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     3115 2024-04-09 09:02:52.000000 PyProfQueue-0.1.1/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-09 14:34:10.000000 PyProfQueue-0.1.1/setup.py
```

### Comparing `PyProfQueue-0.1/PKG-INFO` & `PyProfQueue-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1
+Version: 0.1.1
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.1.1/PyProfQueue/data/likwid_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1/PyProfQueue/data/prometheus_commands.txt` & `PyProfQueue-0.1.1/PyProfQueue/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1/PyProfQueue/data/read_prometheus.py` & `PyProfQueue-0.1.1/PyProfQueue/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1/PyProfQueue/script.py` & `PyProfQueue-0.1.1/PyProfQueue/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,25 +184,31 @@
         self.likwid_file = impresources.files(data) / "likwid_commands.txt"
         self.likwid_initEndSplit = -1
         self.likwid_location = likwid_output
         self.likwid_req = likwid_req
 
     def add_prometheus(self, prometheus_req, prometheus_output='./'):
         contains_ps = False
+        contains_pp = False
         for req in prometheus_req:
             if 'PROMETHEUS_SOFTWARE' in req:
                 contains_ps = True
                 continue
             if 'PROMPYTHON' in req:
+                contains_pp = True
                 continue
             else:
                 prometheus_req += ['export PROMPYTHON={}'.format(sys.executable)]
+                contains_pp = True
                 continue
+        if not contains_pp:
+            prometheus_req += ['export PROMPYTHON={}'.format(sys.executable)]
+            contains_pp = True
 
-        if not contains_ps:
+        if not contains_ps or not contains_pp:
             exit('When requesting prometheus profiling, prometheus_req must include "export PROMETHEUS_SOFTWARE=".')
         self.prometheus = True
         self.prometheus_file = impresources.files(data) / "prometheus_commands.txt"
         self.prometheus_initEndSplit = -1
         self.prometheus_location = prometheus_output
         self.prometheus_req = prometheus_req
```

### Comparing `PyProfQueue-0.1/PyProfQueue/submission.py` & `PyProfQueue-0.1.1/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.1.1/PyProfQueue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1
+Version: 0.1.1
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1/ReadMe.md` & `PyProfQueue-0.1.1/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1/setup.py` & `PyProfQueue-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1',
+    version='0.1.1',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
```

