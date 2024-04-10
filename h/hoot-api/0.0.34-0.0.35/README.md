# Comparing `tmp/hoot-api-0.0.34.tar.gz` & `tmp/hoot-api-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoot-api-0.0.34.tar", last modified: Wed Mar 13 05:23:40 2024, max compression
+gzip compressed data, was "hoot-api-0.0.35.tar", last modified: Wed Apr 10 06:08:22 2024, max compression
```

## Comparing `hoot-api-0.0.34.tar` & `hoot-api-0.0.35.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:23:40.617885 hoot-api-0.0.34/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-13 05:23:21.000000 hoot-api-0.0.34/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-13 05:23:40.617885 hoot-api-0.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-13 05:23:21.000000 hoot-api-0.0.34/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-13 05:23:21.000000 hoot-api-0.0.34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 05:23:40.617885 hoot-api-0.0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-13 05:23:21.000000 hoot-api-0.0.34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:23:40.617885 hoot-api-0.0.34/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:23:40.617885 hoot-api-0.0.34/src/hoot_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-13 05:23:40.000000 hoot-api-0.0.34/src/hoot_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-13 05:23:40.000000 hoot-api-0.0.34/src/hoot_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 05:23:40.000000 hoot-api-0.0.34/src/hoot_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-13 05:23:40.000000 hoot-api-0.0.34/src/hoot_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 05:23:40.000000 hoot-api-0.0.34/src/hoot_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:23:40.617885 hoot-api-0.0.34/src/hoots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 05:23:21.000000 hoot-api-0.0.34/src/hoots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-03-13 05:23:21.000000 hoot-api-0.0.34/src/hoots/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:08:22.381586 hoot-api-0.0.35/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 06:08:11.000000 hoot-api-0.0.35/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-10 06:08:22.381586 hoot-api-0.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 06:08:11.000000 hoot-api-0.0.35/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 06:08:11.000000 hoot-api-0.0.35/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:08:22.381586 hoot-api-0.0.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-10 06:08:11.000000 hoot-api-0.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:08:22.377586 hoot-api-0.0.35/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:08:22.381586 hoot-api-0.0.35/src/hoot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-10 06:08:22.000000 hoot-api-0.0.35/src/hoot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-10 06:08:22.000000 hoot-api-0.0.35/src/hoot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:08:22.000000 hoot-api-0.0.35/src/hoot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 06:08:22.000000 hoot-api-0.0.35/src/hoot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 06:08:22.000000 hoot-api-0.0.35/src/hoot_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:08:22.381586 hoot-api-0.0.35/src/hoots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:08:11.000000 hoot-api-0.0.35/src/hoots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-04-10 06:08:11.000000 hoot-api-0.0.35/src/hoots/client.py
```

### Comparing `hoot-api-0.0.34/LICENSE.txt` & `hoot-api-0.0.35/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hoot-api-0.0.34/PKG-INFO` & `hoot-api-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoot-api
-Version: 0.0.34
+Version: 0.0.35
 Summary: A python client to access the Hoot API
 Home-page: https://github.com/OwlsAtWork/hoot-api
 Author: admin@owl.works
 Author-email: admin@owl.works
 Project-URL: Bug Tracker, https://github.com/OwlsAtWork/hoot-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hoot-api-0.0.34/setup.py` & `hoot-api-0.0.35/setup.py`

 * *Files identical despite different names*

### Comparing `hoot-api-0.0.34/src/hoot_api.egg-info/PKG-INFO` & `hoot-api-0.0.35/src/hoot_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoot-api
-Version: 0.0.34
+Version: 0.0.35
 Summary: A python client to access the Hoot API
 Home-page: https://github.com/OwlsAtWork/hoot-api
 Author: admin@owl.works
 Author-email: admin@owl.works
 Project-URL: Bug Tracker, https://github.com/OwlsAtWork/hoot-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hoot-api-0.0.34/src/hoots/client.py` & `hoot-api-0.0.35/src/hoots/client.py`

 * *Files identical despite different names*

