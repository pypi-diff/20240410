# Comparing `tmp/recflows-0.0.3.tar.gz` & `tmp/recflows-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recflows-0.0.3.tar", last modified: Wed Apr 10 19:42:21 2024, max compression
+gzip compressed data, was "recflows-0.0.4.tar", last modified: Wed Apr 10 19:50:27 2024, max compression
```

## Comparing `recflows-0.0.3.tar` & `recflows-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0     1000     1000        0 2024-04-10 19:42:21.626121 recflows-0.0.3/
--rwxrwxrwx   0     1000     1000     1065 2024-04-10 07:18:06.000000 recflows-0.0.3/LICENSE
--rwxrwxrwx   0     1000     1000      574 2024-04-10 19:42:21.618120 recflows-0.0.3/PKG-INFO
--rwxrwxrwx   0     1000     1000      186 2024-04-10 07:51:51.000000 recflows-0.0.3/README.md
-drwxrwxrwx   0     1000     1000        0 2024-04-10 19:42:21.382085 recflows-0.0.3/recflows/
--rwxrwxrwx   0     1000     1000        0 2024-04-09 18:00:48.000000 recflows-0.0.3/recflows/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 19:42:21.475111 recflows-0.0.3/recflows/decorators/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:16.000000 recflows-0.0.3/recflows/decorators/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 19:42:21.528121 recflows-0.0.3/recflows/resources/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:47.000000 recflows-0.0.3/recflows/resources/__init__.py
--rwxrwxrwx   0     1000     1000      370 2024-04-10 19:02:19.000000 recflows-0.0.3/recflows/resources/app.py
--rwxrwxrwx   0     1000     1000      411 2024-04-10 19:02:37.000000 recflows-0.0.3/recflows/resources/base.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 19:42:21.564121 recflows-0.0.3/recflows/services/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 17:16:07.000000 recflows-0.0.3/recflows/services/__init__.py
--rwxrwxrwx   0     1000     1000     1623 2024-04-10 17:30:23.000000 recflows-0.0.3/recflows/services/database.py
--rwxrwxrwx   0     1000     1000      236 2024-04-10 19:32:29.000000 recflows-0.0.3/recflows/vars.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 19:42:21.609125 recflows-0.0.3/recflows.egg-info/
--rwxrwxrwx   0     1000     1000      574 2024-04-10 19:42:21.000000 recflows-0.0.3/recflows.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      417 2024-04-10 19:42:21.000000 recflows-0.0.3/recflows.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2024-04-10 19:42:21.000000 recflows-0.0.3/recflows.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       14 2024-04-10 19:42:21.000000 recflows-0.0.3/recflows.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        9 2024-04-10 19:42:21.000000 recflows-0.0.3/recflows.egg-info/top_level.txt
--rwxrwxrwx   0     1000     1000       38 2024-04-10 19:42:21.627119 recflows-0.0.3/setup.cfg
--rwxrwxrwx   0     1000     1000      738 2024-04-10 17:00:25.000000 recflows-0.0.3/setup.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 19:42:21.582125 recflows-0.0.3/tests/
--rwxrwxrwx   0     1000     1000       96 2024-04-10 07:05:40.000000 recflows-0.0.3/tests/test_app.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 19:50:27.938286 recflows-0.0.4/
+-rwxrwxrwx   0     1000     1000     1065 2024-04-10 07:18:06.000000 recflows-0.0.4/LICENSE
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 19:50:27.933286 recflows-0.0.4/PKG-INFO
+-rwxrwxrwx   0     1000     1000      186 2024-04-10 07:51:51.000000 recflows-0.0.4/README.md
+drwxrwxrwx   0     1000     1000        0 2024-04-10 19:50:27.739503 recflows-0.0.4/recflows/
+-rwxrwxrwx   0     1000     1000        0 2024-04-09 18:00:48.000000 recflows-0.0.4/recflows/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 19:50:27.821503 recflows-0.0.4/recflows/decorators/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:16.000000 recflows-0.0.4/recflows/decorators/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 19:50:27.872504 recflows-0.0.4/recflows/resources/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:47.000000 recflows-0.0.4/recflows/resources/__init__.py
+-rwxrwxrwx   0     1000     1000      370 2024-04-10 19:02:19.000000 recflows-0.0.4/recflows/resources/app.py
+-rwxrwxrwx   0     1000     1000      411 2024-04-10 19:02:37.000000 recflows-0.0.4/recflows/resources/base.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 19:50:27.899285 recflows-0.0.4/recflows/services/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 17:16:07.000000 recflows-0.0.4/recflows/services/__init__.py
+-rwxrwxrwx   0     1000     1000     1623 2024-04-10 17:30:23.000000 recflows-0.0.4/recflows/services/database.py
+-rwxrwxrwx   0     1000     1000      893 2024-04-10 19:48:32.000000 recflows-0.0.4/recflows/vars.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 19:50:27.926283 recflows-0.0.4/recflows.egg-info/
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 19:50:27.000000 recflows-0.0.4/recflows.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      417 2024-04-10 19:50:27.000000 recflows-0.0.4/recflows.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2024-04-10 19:50:27.000000 recflows-0.0.4/recflows.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       14 2024-04-10 19:50:27.000000 recflows-0.0.4/recflows.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        9 2024-04-10 19:50:27.000000 recflows-0.0.4/recflows.egg-info/top_level.txt
+-rwxrwxrwx   0     1000     1000       38 2024-04-10 19:50:27.939288 recflows-0.0.4/setup.cfg
+-rwxrwxrwx   0     1000     1000      738 2024-04-10 17:00:25.000000 recflows-0.0.4/setup.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 19:50:27.910282 recflows-0.0.4/tests/
+-rwxrwxrwx   0     1000     1000       96 2024-04-10 07:05:40.000000 recflows-0.0.4/tests/test_app.py
```

### Comparing `recflows-0.0.3/LICENSE` & `recflows-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `recflows-0.0.3/PKG-INFO` & `recflows-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.3
+Version: 0.0.4
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recflows-0.0.3/recflows/services/database.py` & `recflows-0.0.4/recflows/services/database.py`

 * *Files identical despite different names*

### Comparing `recflows-0.0.3/recflows.egg-info/PKG-INFO` & `recflows-0.0.4/recflows.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.3
+Version: 0.0.4
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recflows-0.0.3/setup.py` & `recflows-0.0.4/setup.py`

 * *Files identical despite different names*

