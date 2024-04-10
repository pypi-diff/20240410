# Comparing `tmp/recflows-0.0.7.tar.gz` & `tmp/recflows-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recflows-0.0.7.tar", last modified: Wed Apr 10 20:22:25 2024, max compression
+gzip compressed data, was "recflows-0.0.8.tar", last modified: Wed Apr 10 20:31:04 2024, max compression
```

## Comparing `recflows-0.0.7.tar` & `recflows-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:22:25.476940 recflows-0.0.7/
--rwxrwxrwx   0     1000     1000     1065 2024-04-10 07:18:06.000000 recflows-0.0.7/LICENSE
--rwxrwxrwx   0     1000     1000      574 2024-04-10 20:22:25.468935 recflows-0.0.7/PKG-INFO
--rwxrwxrwx   0     1000     1000      186 2024-04-10 07:51:51.000000 recflows-0.0.7/README.md
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:22:25.246309 recflows-0.0.7/recflows/
--rwxrwxrwx   0     1000     1000        0 2024-04-09 18:00:48.000000 recflows-0.0.7/recflows/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:22:25.335870 recflows-0.0.7/recflows/decorators/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:16.000000 recflows-0.0.7/recflows/decorators/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:22:25.385903 recflows-0.0.7/recflows/resources/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:47.000000 recflows-0.0.7/recflows/resources/__init__.py
--rwxrwxrwx   0     1000     1000      370 2024-04-10 19:02:19.000000 recflows-0.0.7/recflows/resources/app.py
--rwxrwxrwx   0     1000     1000      411 2024-04-10 19:02:37.000000 recflows-0.0.7/recflows/resources/base.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:22:25.424421 recflows-0.0.7/recflows/services/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 17:16:07.000000 recflows-0.0.7/recflows/services/__init__.py
--rwxrwxrwx   0     1000     1000     1802 2024-04-10 20:22:11.000000 recflows-0.0.7/recflows/services/database.py
--rwxrwxrwx   0     1000     1000      893 2024-04-10 19:52:02.000000 recflows-0.0.7/recflows/vars.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:22:25.460938 recflows-0.0.7/recflows.egg-info/
--rwxrwxrwx   0     1000     1000      574 2024-04-10 20:22:24.000000 recflows-0.0.7/recflows.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      417 2024-04-10 20:22:25.000000 recflows-0.0.7/recflows.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2024-04-10 20:22:24.000000 recflows-0.0.7/recflows.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       14 2024-04-10 20:22:25.000000 recflows-0.0.7/recflows.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        9 2024-04-10 20:22:25.000000 recflows-0.0.7/recflows.egg-info/top_level.txt
--rwxrwxrwx   0     1000     1000       38 2024-04-10 20:22:25.477937 recflows-0.0.7/setup.cfg
--rwxrwxrwx   0     1000     1000      738 2024-04-10 17:00:25.000000 recflows-0.0.7/setup.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:22:25.440935 recflows-0.0.7/tests/
--rwxrwxrwx   0     1000     1000       96 2024-04-10 07:05:40.000000 recflows-0.0.7/tests/test_app.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:31:04.165949 recflows-0.0.8/
+-rwxrwxrwx   0     1000     1000     1065 2024-04-10 07:18:06.000000 recflows-0.0.8/LICENSE
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 20:31:04.158620 recflows-0.0.8/PKG-INFO
+-rwxrwxrwx   0     1000     1000      186 2024-04-10 07:51:51.000000 recflows-0.0.8/README.md
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:31:03.943582 recflows-0.0.8/recflows/
+-rwxrwxrwx   0     1000     1000        0 2024-04-09 18:00:48.000000 recflows-0.0.8/recflows/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:31:04.032100 recflows-0.0.8/recflows/decorators/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:16.000000 recflows-0.0.8/recflows/decorators/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:31:04.082617 recflows-0.0.8/recflows/resources/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:47.000000 recflows-0.0.8/recflows/resources/__init__.py
+-rwxrwxrwx   0     1000     1000      370 2024-04-10 19:02:19.000000 recflows-0.0.8/recflows/resources/app.py
+-rwxrwxrwx   0     1000     1000      411 2024-04-10 19:02:37.000000 recflows-0.0.8/recflows/resources/base.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:31:04.117617 recflows-0.0.8/recflows/services/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 17:16:07.000000 recflows-0.0.8/recflows/services/__init__.py
+-rwxrwxrwx   0     1000     1000     1807 2024-04-10 20:30:39.000000 recflows-0.0.8/recflows/services/database.py
+-rwxrwxrwx   0     1000     1000      893 2024-04-10 19:52:02.000000 recflows-0.0.8/recflows/vars.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:31:04.150620 recflows-0.0.8/recflows.egg-info/
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 20:31:03.000000 recflows-0.0.8/recflows.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      417 2024-04-10 20:31:03.000000 recflows-0.0.8/recflows.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2024-04-10 20:31:03.000000 recflows-0.0.8/recflows.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       14 2024-04-10 20:31:03.000000 recflows-0.0.8/recflows.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        9 2024-04-10 20:31:03.000000 recflows-0.0.8/recflows.egg-info/top_level.txt
+-rwxrwxrwx   0     1000     1000       38 2024-04-10 20:31:04.167622 recflows-0.0.8/setup.cfg
+-rwxrwxrwx   0     1000     1000      738 2024-04-10 17:00:25.000000 recflows-0.0.8/setup.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:31:04.132618 recflows-0.0.8/tests/
+-rwxrwxrwx   0     1000     1000       96 2024-04-10 07:05:40.000000 recflows-0.0.8/tests/test_app.py
```

### Comparing `recflows-0.0.7/LICENSE` & `recflows-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `recflows-0.0.7/PKG-INFO` & `recflows-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.7
+Version: 0.0.8
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recflows-0.0.7/recflows/services/database.py` & `recflows-0.0.8/recflows/services/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     WHERE id = '{id}'
     """
 
     run_query(query, values)
 
 
 def delete_resouce_by_id(table_name, id):
-    query = f"DELETE {table_name} WHERE id = '{id}'"
+    query = f"DELETE FROM {table_name} WHERE id = '{id}'"
 
     run_query(query)
```

### Comparing `recflows-0.0.7/recflows/vars.py` & `recflows-0.0.8/recflows/vars.py`

 * *Files identical despite different names*

### Comparing `recflows-0.0.7/recflows.egg-info/PKG-INFO` & `recflows-0.0.8/recflows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.7
+Version: 0.0.8
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recflows-0.0.7/setup.py` & `recflows-0.0.8/setup.py`

 * *Files identical despite different names*

