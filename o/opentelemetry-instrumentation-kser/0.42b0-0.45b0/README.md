# Comparing `tmp/opentelemetry-instrumentation-kser-0.42b0.tar.gz` & `tmp/opentelemetry-instrumentation-kser-0.45b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry-instrumentation-kser-0.42b0.tar", last modified: Tue Nov 14 14:21:02 2023, max compression
+gzip compressed data, was "opentelemetry-instrumentation-kser-0.45b0.tar", last modified: Wed Apr 10 09:59:14 2024, max compression
```

## Comparing `opentelemetry-instrumentation-kser-0.42b0.tar` & `opentelemetry-instrumentation-kser-0.45b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2023-11-14 14:21:02.809240 opentelemetry-instrumentation-kser-0.42b0/
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)       60 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.42b0/MANIFEST.in
--rw-r--r--   0 cdumay    (1000) ovh       (1000)     1727 2023-11-14 14:21:02.809240 opentelemetry-instrumentation-kser-0.42b0/PKG-INFO
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)      716 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.42b0/README.rst
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)      144 2023-11-14 14:19:33.000000 opentelemetry-instrumentation-kser-0.42b0/requirements.txt
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)     1055 2023-11-14 14:21:02.809240 opentelemetry-instrumentation-kser-0.42b0/setup.cfg
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)     1983 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.42b0/setup.py
-drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2023-11-14 14:21:02.805240 opentelemetry-instrumentation-kser-0.42b0/src/
-drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2023-11-14 14:21:02.805240 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry/
-drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2023-11-14 14:21:02.805240 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry/instrumentation/
-drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2023-11-14 14:21:02.809240 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry/instrumentation/kser/
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)     5713 2023-05-19 08:45:43.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry/instrumentation/kser/__init__.py
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)      147 2022-05-24 16:12:37.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry/instrumentation/kser/package.py
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)      134 2023-11-14 14:19:33.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry/instrumentation/kser/version.py
-drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2023-11-14 14:21:02.809240 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/
--rw-r--r--   0 cdumay    (1000) ovh       (1000)     1727 2023-11-14 14:21:02.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)      583 2023-11-14 14:21:02.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)        1 2023-11-14 14:21:02.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/dependency_links.txt
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)       88 2023-11-14 14:21:02.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/entry_points.txt
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)      151 2023-11-14 14:21:02.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/requires.txt
--rw-rw-r--   0 cdumay    (1000) ovh       (1000)       14 2023-11-14 14:21:02.000000 opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/top_level.txt
+drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2024-04-10 09:59:14.254612 opentelemetry-instrumentation-kser-0.45b0/
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)       60 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.45b0/MANIFEST.in
+-rw-r--r--   0 cdumay    (1000) ovh       (1000)     1727 2024-04-10 09:59:14.254612 opentelemetry-instrumentation-kser-0.45b0/PKG-INFO
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)      716 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.45b0/README.rst
+-rw-r--r--   0 cdumay    (1000) ovh       (1000)      138 2024-04-10 09:54:34.000000 opentelemetry-instrumentation-kser-0.45b0/requirements.txt
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)     1055 2024-04-10 09:59:14.254612 opentelemetry-instrumentation-kser-0.45b0/setup.cfg
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)     1983 2021-08-18 19:53:31.000000 opentelemetry-instrumentation-kser-0.45b0/setup.py
+drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2024-04-10 09:59:14.254612 opentelemetry-instrumentation-kser-0.45b0/src/
+drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2024-04-10 09:59:14.250612 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry/
+drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2024-04-10 09:59:14.250612 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry/instrumentation/
+drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2024-04-10 09:59:14.254612 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry/instrumentation/kser/
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)     5713 2023-05-19 08:45:43.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry/instrumentation/kser/__init__.py
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)      147 2022-05-24 16:12:37.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry/instrumentation/kser/package.py
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)      134 2024-04-10 09:56:09.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry/instrumentation/kser/version.py
+drwxr-xr-x   0 cdumay    (1000) ovh       (1000)        0 2024-04-10 09:59:14.254612 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/
+-rw-r--r--   0 cdumay    (1000) ovh       (1000)     1727 2024-04-10 09:59:13.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)      583 2024-04-10 09:59:14.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)        1 2024-04-10 09:59:13.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/dependency_links.txt
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)       88 2024-04-10 09:59:13.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/entry_points.txt
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)      151 2024-04-10 09:59:13.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/requires.txt
+-rw-rw-r--   0 cdumay    (1000) ovh       (1000)       14 2024-04-10 09:59:13.000000 opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/top_level.txt
```

### Comparing `opentelemetry-instrumentation-kser-0.42b0/PKG-INFO` & `opentelemetry-instrumentation-kser-0.45b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-kser
-Version: 0.42b0
+Version: 0.45b0
 Summary: OpenTelemetry kser instrumentation
 Home-page: https://github.com/cdumay/opentelemetry-instrumentation-kser
 Author: Cédric Dumay
 Author-email: cedric.dumay@gmail.com
 License: BSD 3-Clause License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `opentelemetry-instrumentation-kser-0.42b0/README.rst` & `opentelemetry-instrumentation-kser-0.45b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-instrumentation-kser-0.42b0/setup.cfg` & `opentelemetry-instrumentation-kser-0.45b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `opentelemetry-instrumentation-kser-0.42b0/setup.py` & `opentelemetry-instrumentation-kser-0.45b0/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry/instrumentation/kser/__init__.py` & `opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry/instrumentation/kser/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO` & `opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-kser
-Version: 0.42b0
+Version: 0.45b0
 Summary: OpenTelemetry kser instrumentation
 Home-page: https://github.com/cdumay/opentelemetry-instrumentation-kser
 Author: Cédric Dumay
 Author-email: cedric.dumay@gmail.com
 License: BSD 3-Clause License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `opentelemetry-instrumentation-kser-0.42b0/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt` & `opentelemetry-instrumentation-kser-0.45b0/src/opentelemetry_instrumentation_kser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

