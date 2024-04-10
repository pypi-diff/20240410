# Comparing `tmp/mecmitool-0.1.1.tar.gz` & `tmp/mecmitool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecmitool-0.1.1.tar", last modified: Mon Jan 15 07:20:47 2024, max compression
+gzip compressed data, was "mecmitool-0.1.2.tar", last modified: Wed Apr 10 16:28:14 2024, max compression
```

## Comparing `mecmitool-0.1.1.tar` & `mecmitool-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-01-15 07:20:47.210528 mecmitool-0.1.1/
--rw-rw-rw-   0        0        0        0 2023-10-23 07:06:45.000000 mecmitool-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1046 2024-01-15 07:20:47.209532 mecmitool-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      671 2024-01-15 07:20:18.000000 mecmitool-0.1.1/README.md
--rw-rw-rw-   0        0        0      469 2024-01-15 07:20:26.000000 mecmitool-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-15 07:20:47.210528 mecmitool-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-15 07:20:47.189936 mecmitool-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-15 07:20:47.200559 mecmitool-0.1.1/src/mecmitool/
--rw-rw-rw-   0        0        0      106 2024-01-15 07:12:58.000000 mecmitool-0.1.1/src/mecmitool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-15 07:20:47.207540 mecmitool-0.1.1/src/mecmitool/auto_upload/
--rw-rw-rw-   0        0        0       52 2023-11-22 10:14:07.000000 mecmitool-0.1.1/src/mecmitool/auto_upload/__init__.py
--rw-rw-rw-   0        0        0     1499 2023-11-22 06:44:52.000000 mecmitool-0.1.1/src/mecmitool/auto_upload/_twine_main.py
--rw-rw-rw-   0        0        0     1144 2023-11-22 09:56:10.000000 mecmitool-0.1.1/src/mecmitool/auto_upload/auto_upload.py
--rw-rw-rw-   0        0        0      893 2024-01-15 07:11:25.000000 mecmitool-0.1.1/src/mecmitool/decorator.py
--rw-rw-rw-   0        0        0      500 2023-12-03 12:09:01.000000 mecmitool-0.1.1/src/mecmitool/errors.py
--rw-rw-rw-   0        0        0     3526 2024-01-06 13:14:35.000000 mecmitool-0.1.1/src/mecmitool/path_checker.py
--rw-rw-rw-   0        0        0     9561 2023-09-24 13:44:25.000000 mecmitool-0.1.1/src/mecmitool/playsound.py
--rw-rw-rw-   0        0        0      170 2023-10-23 12:50:34.000000 mecmitool-0.1.1/src/mecmitool/playsound.pyi
--rw-rw-rw-   0        0        0     1270 2023-12-13 10:35:15.000000 mecmitool-0.1.1/src/mecmitool/timer.py
-drwxrwxrwx   0        0        0        0 2024-01-15 07:20:47.208536 mecmitool-0.1.1/src/mecmitool.egg-info/
--rw-rw-rw-   0        0        0     1046 2024-01-15 07:20:47.000000 mecmitool-0.1.1/src/mecmitool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-01-15 07:20:47.000000 mecmitool-0.1.1/src/mecmitool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-15 07:20:47.000000 mecmitool-0.1.1/src/mecmitool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-01-15 07:20:47.000000 mecmitool-0.1.1/src/mecmitool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 16:28:14.234670 mecmitool-0.1.2/
+-rw-rw-rw-   0        0        0        0 2023-10-23 07:06:45.000000 mecmitool-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1083 2024-04-10 16:28:14.233626 mecmitool-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2024-04-10 16:27:44.000000 mecmitool-0.1.2/README.md
+-rw-rw-rw-   0        0        0      469 2024-04-10 16:27:51.000000 mecmitool-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:28:14.234670 mecmitool-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 16:28:14.208881 mecmitool-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:28:14.222456 mecmitool-0.1.2/src/mecmitool/
+-rw-rw-rw-   0        0        0      106 2024-01-15 07:12:58.000000 mecmitool-0.1.2/src/mecmitool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:28:14.230423 mecmitool-0.1.2/src/mecmitool/auto_upload/
+-rw-rw-rw-   0        0        0       52 2023-11-22 10:14:07.000000 mecmitool-0.1.2/src/mecmitool/auto_upload/__init__.py
+-rw-rw-rw-   0        0        0     1499 2023-11-22 06:44:52.000000 mecmitool-0.1.2/src/mecmitool/auto_upload/_twine_main.py
+-rw-rw-rw-   0        0        0     1144 2023-11-22 09:56:10.000000 mecmitool-0.1.2/src/mecmitool/auto_upload/auto_upload.py
+-rw-rw-rw-   0        0        0      893 2024-01-15 07:11:25.000000 mecmitool-0.1.2/src/mecmitool/decorator.py
+-rw-rw-rw-   0        0        0      500 2023-12-03 12:09:01.000000 mecmitool-0.1.2/src/mecmitool/errors.py
+-rw-rw-rw-   0        0        0     3526 2024-01-06 13:14:35.000000 mecmitool-0.1.2/src/mecmitool/path_checker.py
+-rw-rw-rw-   0        0        0     9561 2023-09-24 13:44:25.000000 mecmitool-0.1.2/src/mecmitool/playsound.py
+-rw-rw-rw-   0        0        0      170 2023-10-23 12:50:34.000000 mecmitool-0.1.2/src/mecmitool/playsound.pyi
+-rw-rw-rw-   0        0        0     1003 2024-04-10 16:25:16.000000 mecmitool-0.1.2/src/mecmitool/rgb.py
+-rw-rw-rw-   0        0        0     1270 2024-04-10 16:01:30.000000 mecmitool-0.1.2/src/mecmitool/timer.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:28:14.232554 mecmitool-0.1.2/src/mecmitool.egg-info/
+-rw-rw-rw-   0        0        0     1083 2024-04-10 16:28:14.000000 mecmitool-0.1.2/src/mecmitool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-04-10 16:28:14.000000 mecmitool-0.1.2/src/mecmitool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:28:14.000000 mecmitool-0.1.2/src/mecmitool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-10 16:28:14.000000 mecmitool-0.1.2/src/mecmitool.egg-info/top_level.txt
```

### Comparing `mecmitool-0.1.1/PKG-INFO` & `mecmitool-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mecmitool
-Version: 0.1.1
+Version: 0.1.2
 Summary: some repetitive wheels
 Author-email: mechermit <mechermit@outlook.com>
 Project-URL: Homepage, https://github.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ###### this project contain some small tool which are use in my other project.  
-
+##### 0.1.02:  
+add rgb; refix timer
 ##### 0.1.01:  
 add functimer 
 ##### 0.1.00:  
 refix pathchecker with @classmethod 
 ##### 0.0.12:  
 add checkpoint  
 ##### 0.0.11:
```

### Comparing `mecmitool-0.1.1/README.md` & `mecmitool-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ###### this project contain some small tool which are use in my other project.  
-
+##### 0.1.02:  
+add rgb; refix timer
 ##### 0.1.01:  
 add functimer 
 ##### 0.1.00:  
 refix pathchecker with @classmethod 
 ##### 0.0.12:  
 add checkpoint  
 ##### 0.0.11:
```

### Comparing `mecmitool-0.1.1/src/mecmitool/auto_upload/_twine_main.py` & `mecmitool-0.1.2/src/mecmitool/auto_upload/_twine_main.py`

 * *Files identical despite different names*

### Comparing `mecmitool-0.1.1/src/mecmitool/auto_upload/auto_upload.py` & `mecmitool-0.1.2/src/mecmitool/auto_upload/auto_upload.py`

 * *Files identical despite different names*

### Comparing `mecmitool-0.1.1/src/mecmitool/decorator.py` & `mecmitool-0.1.2/src/mecmitool/decorator.py`

 * *Files identical despite different names*

### Comparing `mecmitool-0.1.1/src/mecmitool/path_checker.py` & `mecmitool-0.1.2/src/mecmitool/path_checker.py`

 * *Files identical despite different names*

### Comparing `mecmitool-0.1.1/src/mecmitool/playsound.py` & `mecmitool-0.1.2/src/mecmitool/playsound.py`

 * *Files identical despite different names*

### Comparing `mecmitool-0.1.1/src/mecmitool/timer.py` & `mecmitool-0.1.2/src/mecmitool/timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 import mecmitool.errors
 
 
-class timer:
+class Timer:
     def __init__(self, timer_name= "timer_name") -> None:
         self.timer_name = timer_name
         self.time_start = time.time()
         self.start_status= 0
         self.accumulate_time = 0
     def reset(self):
         self.time_start = time.time()
```

### Comparing `mecmitool-0.1.1/src/mecmitool.egg-info/PKG-INFO` & `mecmitool-0.1.2/src/mecmitool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mecmitool
-Version: 0.1.1
+Version: 0.1.2
 Summary: some repetitive wheels
 Author-email: mechermit <mechermit@outlook.com>
 Project-URL: Homepage, https://github.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ###### this project contain some small tool which are use in my other project.  
-
+##### 0.1.02:  
+add rgb; refix timer
 ##### 0.1.01:  
 add functimer 
 ##### 0.1.00:  
 refix pathchecker with @classmethod 
 ##### 0.0.12:  
 add checkpoint  
 ##### 0.0.11:
```

