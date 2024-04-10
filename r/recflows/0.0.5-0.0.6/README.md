# Comparing `tmp/recflows-0.0.5.tar.gz` & `tmp/recflows-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recflows-0.0.5.tar", last modified: Wed Apr 10 20:14:40 2024, max compression
+gzip compressed data, was "recflows-0.0.6.tar", last modified: Wed Apr 10 20:17:56 2024, max compression
```

## Comparing `recflows-0.0.5.tar` & `recflows-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:14:40.077881 recflows-0.0.5/
--rwxrwxrwx   0     1000     1000     1065 2024-04-10 07:18:06.000000 recflows-0.0.5/LICENSE
--rwxrwxrwx   0     1000     1000      574 2024-04-10 20:14:40.071877 recflows-0.0.5/PKG-INFO
--rwxrwxrwx   0     1000     1000      186 2024-04-10 07:51:51.000000 recflows-0.0.5/README.md
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:14:39.844377 recflows-0.0.5/recflows/
--rwxrwxrwx   0     1000     1000        0 2024-04-09 18:00:48.000000 recflows-0.0.5/recflows/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:14:39.932375 recflows-0.0.5/recflows/decorators/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:16.000000 recflows-0.0.5/recflows/decorators/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:14:39.986184 recflows-0.0.5/recflows/resources/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:47.000000 recflows-0.0.5/recflows/resources/__init__.py
--rwxrwxrwx   0     1000     1000      370 2024-04-10 19:02:19.000000 recflows-0.0.5/recflows/resources/app.py
--rwxrwxrwx   0     1000     1000      411 2024-04-10 19:02:37.000000 recflows-0.0.5/recflows/resources/base.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:14:40.026877 recflows-0.0.5/recflows/services/
--rwxrwxrwx   0     1000     1000        0 2024-04-10 17:16:07.000000 recflows-0.0.5/recflows/services/__init__.py
--rwxrwxrwx   0     1000     1000     1648 2024-04-10 20:14:18.000000 recflows-0.0.5/recflows/services/database.py
--rwxrwxrwx   0     1000     1000      893 2024-04-10 19:52:02.000000 recflows-0.0.5/recflows/vars.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:14:40.062876 recflows-0.0.5/recflows.egg-info/
--rwxrwxrwx   0     1000     1000      574 2024-04-10 20:14:39.000000 recflows-0.0.5/recflows.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      417 2024-04-10 20:14:39.000000 recflows-0.0.5/recflows.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2024-04-10 20:14:39.000000 recflows-0.0.5/recflows.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       14 2024-04-10 20:14:39.000000 recflows-0.0.5/recflows.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        9 2024-04-10 20:14:39.000000 recflows-0.0.5/recflows.egg-info/top_level.txt
--rwxrwxrwx   0     1000     1000       38 2024-04-10 20:14:40.078876 recflows-0.0.5/setup.cfg
--rwxrwxrwx   0     1000     1000      738 2024-04-10 17:00:25.000000 recflows-0.0.5/setup.py
-drwxrwxrwx   0     1000     1000        0 2024-04-10 20:14:40.043876 recflows-0.0.5/tests/
--rwxrwxrwx   0     1000     1000       96 2024-04-10 07:05:40.000000 recflows-0.0.5/tests/test_app.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:17:56.759806 recflows-0.0.6/
+-rwxrwxrwx   0     1000     1000     1065 2024-04-10 07:18:06.000000 recflows-0.0.6/LICENSE
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 20:17:56.753809 recflows-0.0.6/PKG-INFO
+-rwxrwxrwx   0     1000     1000      186 2024-04-10 07:51:51.000000 recflows-0.0.6/README.md
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:17:56.537808 recflows-0.0.6/recflows/
+-rwxrwxrwx   0     1000     1000        0 2024-04-09 18:00:48.000000 recflows-0.0.6/recflows/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:17:56.622809 recflows-0.0.6/recflows/decorators/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:16.000000 recflows-0.0.6/recflows/decorators/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:17:56.672810 recflows-0.0.6/recflows/resources/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 06:37:47.000000 recflows-0.0.6/recflows/resources/__init__.py
+-rwxrwxrwx   0     1000     1000      370 2024-04-10 19:02:19.000000 recflows-0.0.6/recflows/resources/app.py
+-rwxrwxrwx   0     1000     1000      411 2024-04-10 19:02:37.000000 recflows-0.0.6/recflows/resources/base.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:17:56.710812 recflows-0.0.6/recflows/services/
+-rwxrwxrwx   0     1000     1000        0 2024-04-10 17:16:07.000000 recflows-0.0.6/recflows/services/__init__.py
+-rwxrwxrwx   0     1000     1000     1707 2024-04-10 20:17:44.000000 recflows-0.0.6/recflows/services/database.py
+-rwxrwxrwx   0     1000     1000      893 2024-04-10 19:52:02.000000 recflows-0.0.6/recflows/vars.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:17:56.744810 recflows-0.0.6/recflows.egg-info/
+-rwxrwxrwx   0     1000     1000      574 2024-04-10 20:17:56.000000 recflows-0.0.6/recflows.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      417 2024-04-10 20:17:56.000000 recflows-0.0.6/recflows.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2024-04-10 20:17:56.000000 recflows-0.0.6/recflows.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       14 2024-04-10 20:17:56.000000 recflows-0.0.6/recflows.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        9 2024-04-10 20:17:56.000000 recflows-0.0.6/recflows.egg-info/top_level.txt
+-rwxrwxrwx   0     1000     1000       38 2024-04-10 20:17:56.760810 recflows-0.0.6/setup.cfg
+-rwxrwxrwx   0     1000     1000      738 2024-04-10 17:00:25.000000 recflows-0.0.6/setup.py
+drwxrwxrwx   0     1000     1000        0 2024-04-10 20:17:56.726807 recflows-0.0.6/tests/
+-rwxrwxrwx   0     1000     1000       96 2024-04-10 07:05:40.000000 recflows-0.0.6/tests/test_app.py
```

### Comparing `recflows-0.0.5/LICENSE` & `recflows-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `recflows-0.0.5/PKG-INFO` & `recflows-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.5
+Version: 0.0.6
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recflows-0.0.5/recflows/services/database.py` & `recflows-0.0.6/recflows/services/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     VALUES({', '.join(["%s" for _ in record.keys()])})
     """
     values = tuple(record.values())
     run_query(query, values)
 
 
 def update_resouce(table_name, record):
+    id = record["id"]
+    record = {k: v for k, v in record.items() if k != "id"}
+    values = tuple(record.values())
     query = f"""
     UPDATE {table_name}
-    SET {', '.join([f"{k} = %s" for k in record.keys() if k != "id"])}
-    WHERE id = '{record["id"]}'
+    SET {', '.join([f"{k} = %s" for k in record.keys()])}
+    WHERE id = '{id}'
     """
-    values = tuple(record.values())
     print(query, values)
     run_query(query, values)
```

### Comparing `recflows-0.0.5/recflows/vars.py` & `recflows-0.0.6/recflows/vars.py`

 * *Files identical despite different names*

### Comparing `recflows-0.0.5/recflows.egg-info/PKG-INFO` & `recflows-0.0.6/recflows.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recflows
-Version: 0.0.5
+Version: 0.0.6
 Summary: Solution created to streamline the creation, programming, deployment and monitoring of recommendation systems.
 Home-page: https://github.com/cogdiver/recflows
 Author: cogdiver
 License: MIT
 Keywords: recommendation systems,programming
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recflows-0.0.5/setup.py` & `recflows-0.0.6/setup.py`

 * *Files identical despite different names*
