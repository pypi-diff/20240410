# Comparing `tmp/sqlalchemy-risingwave-1.0.1.tar.gz` & `tmp/sqlalchemy-risingwave-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-risingwave-1.0.1.tar", last modified: Mon Feb  5 20:52:37 2024, max compression
+gzip compressed data, was "sqlalchemy-risingwave-1.1.0.tar", last modified: Wed Apr 10 09:37:20 2024, max compression
```

## Comparing `sqlalchemy-risingwave-1.0.1.tar` & `sqlalchemy-risingwave-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kexiang    (501) staff       (20)        0 2024-02-05 20:52:37.546048 sqlalchemy-risingwave-1.0.1/
--rw-r--r--   0 kexiang    (501) staff       (20)    11325 2023-12-13 18:19:51.000000 sqlalchemy-risingwave-1.0.1/LICENSE
--rw-r--r--   0 kexiang    (501) staff       (20)     3010 2024-02-05 20:52:37.545962 sqlalchemy-risingwave-1.0.1/PKG-INFO
--rw-r--r--   0 kexiang    (501) staff       (20)     2026 2023-12-13 18:19:51.000000 sqlalchemy-risingwave-1.0.1/README.md
--rw-r--r--   0 kexiang    (501) staff       (20)      344 2024-02-05 20:52:37.546491 sqlalchemy-risingwave-1.0.1/setup.cfg
--rw-r--r--   0 kexiang    (501) staff       (20)     1831 2024-02-05 20:20:25.000000 sqlalchemy-risingwave-1.0.1/setup.py
-drwxr-xr-x   0 kexiang    (501) staff       (20)        0 2024-02-05 20:52:37.543650 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave/
--rw-r--r--   0 kexiang    (501) staff       (20)      359 2024-02-05 20:52:30.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave/__init__.py
--rw-r--r--   0 kexiang    (501) staff       (20)     9905 2024-02-05 20:52:30.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave/base.py
--rw-r--r--   0 kexiang    (501) staff       (20)      167 2023-12-27 00:37:52.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave/psycopg2.py
--rw-r--r--   0 kexiang    (501) staff       (20)     3318 2023-12-13 18:19:51.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave/requirements.py
-drwxr-xr-x   0 kexiang    (501) staff       (20)        0 2024-02-05 20:52:37.545666 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/
--rw-r--r--   0 kexiang    (501) staff       (20)     3010 2024-02-05 20:52:37.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/PKG-INFO
--rw-r--r--   0 kexiang    (501) staff       (20)      508 2024-02-05 20:52:37.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/SOURCES.txt
--rw-r--r--   0 kexiang    (501) staff       (20)        1 2024-02-05 20:52:37.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/dependency_links.txt
--rw-r--r--   0 kexiang    (501) staff       (20)      173 2024-02-05 20:52:37.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/entry_points.txt
--rw-r--r--   0 kexiang    (501) staff       (20)        1 2023-12-13 18:21:19.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/not-zip-safe
--rw-r--r--   0 kexiang    (501) staff       (20)       19 2024-02-05 20:52:37.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/requires.txt
--rw-r--r--   0 kexiang    (501) staff       (20)       22 2024-02-05 20:52:37.000000 sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/top_level.txt
-drwxr-xr-x   0 kexiang    (501) staff       (20)        0 2024-02-05 20:52:37.545258 sqlalchemy-risingwave-1.0.1/test/
--rw-r--r--   0 kexiang    (501) staff       (20)     2082 2024-01-07 22:38:29.000000 sqlalchemy-risingwave-1.0.1/test/test_schema.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-10 09:37:20.714430 sqlalchemy-risingwave-1.1.0/
+-rw-r--r--   0 dylan      (501) staff       (20)    11325 2023-09-06 08:34:30.000000 sqlalchemy-risingwave-1.1.0/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     3012 2024-04-10 09:37:20.714369 sqlalchemy-risingwave-1.1.0/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     2026 2023-09-06 08:50:44.000000 sqlalchemy-risingwave-1.1.0/README.md
+-rw-r--r--   0 dylan      (501) staff       (20)      344 2024-04-10 09:37:20.714673 sqlalchemy-risingwave-1.1.0/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1833 2024-04-10 09:30:15.000000 sqlalchemy-risingwave-1.1.0/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-10 09:37:20.712971 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave/
+-rw-r--r--   0 dylan      (501) staff       (20)      359 2024-04-10 09:30:15.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     9905 2024-04-10 09:30:15.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave/base.py
+-rw-r--r--   0 dylan      (501) staff       (20)      167 2023-09-06 08:34:30.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave/psycopg2.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3318 2023-09-06 08:34:30.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave/requirements.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-10 09:37:20.714178 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     3012 2024-04-10 09:37:20.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      508 2024-04-10 09:37:20.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-04-10 09:37:20.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      173 2024-04-10 09:37:20.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/entry_points.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-09-06 08:41:23.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/not-zip-safe
+-rw-r--r--   0 dylan      (501) staff       (20)       21 2024-04-10 09:37:20.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       22 2024-04-10 09:37:20.000000 sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-10 09:37:20.714002 sqlalchemy-risingwave-1.1.0/test/
+-rw-r--r--   0 dylan      (501) staff       (20)     2082 2024-04-10 09:30:15.000000 sqlalchemy-risingwave-1.1.0/test/test_schema.py
```

### Comparing `sqlalchemy-risingwave-1.0.1/LICENSE` & `sqlalchemy-risingwave-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-risingwave-1.0.1/PKG-INFO` & `sqlalchemy-risingwave-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-risingwave
-Version: 1.0.1
+Version: 1.1.0
 Summary: RisingWave dialect for SQLAlchemy
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Author-email: risingwave@dev.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/risingwavelabs/sqlalchemy-risingwave
 Project-URL: Tracker, https://github.com/risingwavelabs/sqlalchemy-risingwave/issues
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: SQLAlchemy<2,>=1.4
+Requires-Dist: SQLAlchemy<2.1,>=2.0
 
 # RisingWave dialect for SQLAlchemy
 
 SQLAlchemy is the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL. https://www.sqlalchemy.org/
 
 RisingWave is a cloud-native streaming database that uses SQL as the interface language. It is designed to reduce the complexity and cost of building real-time applications. https://www.risingwave.com
```

### Comparing `sqlalchemy-risingwave-1.0.1/README.md` & `sqlalchemy-risingwave-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-risingwave-1.0.1/setup.py` & `sqlalchemy-risingwave-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     keywords="SQLAlchemy RisingWave",
     project_urls={
         "Source": "https://github.com/risingwavelabs/sqlalchemy-risingwave",
         "Tracker": "https://github.com/risingwavelabs/sqlalchemy-risingwave/issues",
     },
     packages=find_packages(include=["sqlalchemy_risingwave"]),
     include_package_data=True,
-    install_requires=["SQLAlchemy>=1.4,<2"],
+    install_requires=["SQLAlchemy>=2.0,<2.1"],
     zip_safe=False,
     # # Do not support dialects now.
     entry_points={
         "sqlalchemy.dialects": [
             "risingwave = sqlalchemy_risingwave.psycopg2:RisingWaveDialect_psycopg2",
             "risingwave.psycopg2 = sqlalchemy_risingwave.psycopg2:RisingWaveDialect_psycopg2",
         ],
```

### Comparing `sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave/base.py` & `sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave/requirements.py` & `sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-risingwave-1.0.1/sqlalchemy_risingwave.egg-info/PKG-INFO` & `sqlalchemy-risingwave-1.1.0/sqlalchemy_risingwave.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-risingwave
-Version: 1.0.1
+Version: 1.1.0
 Summary: RisingWave dialect for SQLAlchemy
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Author-email: risingwave@dev.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/risingwavelabs/sqlalchemy-risingwave
 Project-URL: Tracker, https://github.com/risingwavelabs/sqlalchemy-risingwave/issues
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: SQLAlchemy<2,>=1.4
+Requires-Dist: SQLAlchemy<2.1,>=2.0
 
 # RisingWave dialect for SQLAlchemy
 
 SQLAlchemy is the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL. https://www.sqlalchemy.org/
 
 RisingWave is a cloud-native streaming database that uses SQL as the interface language. It is designed to reduce the complexity and cost of building real-time applications. https://www.risingwave.com
```

### Comparing `sqlalchemy-risingwave-1.0.1/test/test_schema.py` & `sqlalchemy-risingwave-1.1.0/test/test_schema.py`

 * *Files identical despite different names*

