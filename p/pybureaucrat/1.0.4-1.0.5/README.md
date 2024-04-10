# Comparing `tmp/pybureaucrat-1.0.4.tar.gz` & `tmp/pybureaucrat-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybureaucrat-1.0.4.tar", last modified: Sat Apr  6 04:10:32 2024, max compression
+gzip compressed data, was "pybureaucrat-1.0.5.tar", last modified: Wed Apr 10 15:12:55 2024, max compression
```

## Comparing `pybureaucrat-1.0.4.tar` & `pybureaucrat-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/README.MD
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/client/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/client/common/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2634 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/base.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1244 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/blobs.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      348 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/bureaucrat_connection.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/deserializers.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      813 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/queues.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1795 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/client/common/tables.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      426 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        7 2024-04-06 04:10:32.000000 pybureaucrat-1.0.4/client/pybureaucrat.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2024-04-06 04:10:32.565198 pybureaucrat-1.0.4/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1151 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/setup.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2024-04-06 03:57:44.000000 pybureaucrat-1.0.4/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:12:55.558035 pybureaucrat-1.0.5/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2024-04-06 03:57:44.000000 pybureaucrat-1.0.5/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2024-04-06 03:57:44.000000 pybureaucrat-1.0.5/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-10 15:12:55.558035 pybureaucrat-1.0.5/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.5/README.MD
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:12:55.546036 pybureaucrat-1.0.5/client/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:12:55.554036 pybureaucrat-1.0.5/client/pybureaucrat/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/client/pybureaucrat/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2634 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/client/pybureaucrat/base.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1244 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/client/pybureaucrat/blobs.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      348 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/client/pybureaucrat/bureaucrat_connection.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/client/pybureaucrat/deserializers.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      813 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/client/pybureaucrat/queues.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1795 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/client/pybureaucrat/tables.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:12:55.558035 pybureaucrat-1.0.5/client/pybureaucrat.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-10 15:12:55.000000 pybureaucrat-1.0.5/client/pybureaucrat.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      468 2024-04-10 15:12:55.000000 pybureaucrat-1.0.5/client/pybureaucrat.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2024-04-10 15:12:55.000000 pybureaucrat-1.0.5/client/pybureaucrat.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2024-04-10 15:12:55.000000 pybureaucrat-1.0.5/client/pybureaucrat.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2024-04-06 03:57:44.000000 pybureaucrat-1.0.5/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2024-04-10 15:12:55.558035 pybureaucrat-1.0.5/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1163 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/setup.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2024-04-10 15:11:05.000000 pybureaucrat-1.0.5/version.txt
```

### Comparing `pybureaucrat-1.0.4/LICENSE` & `pybureaucrat-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.4/PKG-INFO` & `pybureaucrat-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybureaucrat-1.0.4/client/common/base.py` & `pybureaucrat-1.0.5/client/pybureaucrat/base.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.4/client/common/blobs.py` & `pybureaucrat-1.0.5/client/pybureaucrat/blobs.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.4/client/common/queues.py` & `pybureaucrat-1.0.5/client/pybureaucrat/queues.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.4/client/common/tables.py` & `pybureaucrat-1.0.5/client/pybureaucrat/tables.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.4/client/pybureaucrat.egg-info/PKG-INFO` & `pybureaucrat-1.0.5/client/pybureaucrat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybureaucrat-1.0.4/setup.py` & `pybureaucrat-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "Examples": "https://dev.moradev.dev/pybureaucrat/examples",
     },
     package_data={
         "":["*.txt"]
     },
     classifiers=[
     "Programming Language :: Python :: 3",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     ],
     package_dir={"": "client"},
     packages=setuptools.find_packages(where="client"),
     python_requires=">=3.6"
 )
```

