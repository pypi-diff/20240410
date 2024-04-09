# Comparing `tmp/mpcontribs-client-5.8.1.tar.gz` & `tmp/mpcontribs-client-5.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.8.1.tar", last modified: Mon Apr  8 22:10:06 2024, max compression
+gzip compressed data, was "mpcontribs-client-5.8.2.tar", last modified: Tue Apr  9 23:44:44 2024, max compression
```

## Comparing `mpcontribs-client-5.8.1.tar` & `mpcontribs-client-5.8.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.079616 mpcontribs-client-5.8.1/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.079616 mpcontribs-client-5.8.1/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    96520 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 22:10:06.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.145999 mpcontribs-client-5.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.137999 mpcontribs-client-5.8.2/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    96696 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-09 23:44:44.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:44:44.145999 mpcontribs-client-5.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/tests/test_client.py
```

### Comparing `mpcontribs-client-5.8.1/LICENSE` & `mpcontribs-client-5.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/PKG-INFO` & `mpcontribs-client-5.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.8.1
+Version: 5.8.2
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.8.1/README.md` & `mpcontribs-client-5.8.2/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/mpcontribs/client/__init__.py` & `mpcontribs-client-5.8.2/mpcontribs/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2162,22 +2162,24 @@
                 in existing.get(project_name, {}).get("identifiers", {})
             ):
                 continue
 
             contrib_copy = {}
             for k in fields:
                 if k in contrib:
-                    flat = {}
-                    for kk, vv in flatten(contrib[k], reducer="dot").items():
-                        if isinstance(vv, bool):
-                            flat[kk] = "Yes" if vv else "No"
-                        elif isinstance(vv, str):
-                            flat[kk] = vv
-
-                    contrib_copy[k] = deepcopy(unflatten(flat, splitter="dot"))
+                    if isinstance(contrib[k], dict):
+                        flat = {}
+                        for kk, vv in flatten(contrib[k], reducer="dot").items():
+                            if isinstance(vv, bool):
+                                flat[kk] = "Yes" if vv else "No"
+                            elif isinstance(vv, str) and vv:
+                                flat[kk] = vv
+                        contrib_copy[k] = deepcopy(unflatten(flat, splitter="dot"))
+                    else:
+                        contrib_copy[k] = deepcopy(contrib[k])
 
             contribs[project_name].append(contrib_copy)
 
             for component in COMPONENTS:
                 elements = contrib.get(component, [])
                 nelems = len(elements)
```

### Comparing `mpcontribs-client-5.8.1/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.8.2/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.8.1
+Version: 5.8.2
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.8.1/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.8.2/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/requirements/deployment.txt` & `mpcontribs-client-5.8.2/requirements/deployment.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/setup.py` & `mpcontribs-client-5.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.1/tests/test_client.py` & `mpcontribs-client-5.8.2/tests/test_client.py`

 * *Files identical despite different names*

