# Comparing `tmp/creaap-0.1.8.tar.gz` & `tmp/creaap-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creaap-0.1.8.tar", last modified: Wed Dec  6 16:48:21 2023, max compression
+gzip compressed data, was "creaap-0.1.9.tar", last modified: Tue Jan 23 11:35:56 2024, max compression
```

## Comparing `creaap-0.1.8.tar` & `creaap-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-06 16:48:21.855143 creaap-0.1.8/
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2023-12-06 16:47:33.000000 creaap-0.1.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       39 2023-12-06 16:47:33.000000 creaap-0.1.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    11797 2023-12-06 16:48:21.855143 creaap-0.1.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    11047 2023-12-06 16:47:33.000000 creaap-0.1.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-06 16:48:21.847143 creaap-0.1.8/creaap/
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4299 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/formats.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3131 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/io.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5848 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/models.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-06 16:48:21.851143 creaap-0.1.8/creaap/spatial/
--rw-r--r--   0 vsts      (1001) docker     (127)      271 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/spatial/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-06 16:48:21.851143 creaap-0.1.8/creaap/spatial/data/
--rw-r--r--   0 vsts      (1001) docker     (127)   114975 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/spatial/data/nuts0
--rw-r--r--   0 vsts      (1001) docker     (127)   169486 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/spatial/data/nuts1
--rw-r--r--   0 vsts      (1001) docker     (127)   236333 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/spatial/data/nuts2
--rw-r--r--   0 vsts      (1001) docker     (127)   456454 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/spatial/data/nuts3
--rw-r--r--   0 vsts      (1001) docker     (127)    10414 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/spatial/match.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7586 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/spatial/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-06 16:48:21.855143 creaap-0.1.8/creaap/storage/
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/storage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8318 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/storage/blob.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6705 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/storage/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10137 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/storage/table.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-06 16:48:21.855143 creaap-0.1.8/creaap/users/
--rw-r--r--   0 vsts      (1001) docker     (127)      281 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9799 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/users/aad.py
--rw-r--r--   0 vsts      (1001) docker     (127)      909 2023-12-06 16:47:33.000000 creaap-0.1.8/creaap/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-06 16:48:21.851143 creaap-0.1.8/creaap.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    11797 2023-12-06 16:48:21.000000 creaap-0.1.8/creaap.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      591 2023-12-06 16:48:21.000000 creaap-0.1.8/creaap.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-06 16:48:21.000000 creaap-0.1.8/creaap.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      146 2023-12-06 16:48:21.000000 creaap-0.1.8/creaap.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        7 2023-12-06 16:48:21.000000 creaap-0.1.8/creaap.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-12-06 16:48:21.855143 creaap-0.1.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1475 2023-12-06 16:47:33.000000 creaap-0.1.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-23 11:35:56.093291 creaap-0.1.9/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-01-23 11:35:10.000000 creaap-0.1.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       39 2024-01-23 11:35:10.000000 creaap-0.1.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    11797 2024-01-23 11:35:56.093291 creaap-0.1.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    11047 2024-01-23 11:35:10.000000 creaap-0.1.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-23 11:35:56.089291 creaap-0.1.9/creaap/
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4299 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/formats.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3101 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/io.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5848 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/models.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-23 11:35:56.089291 creaap-0.1.9/creaap/spatial/
+-rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/spatial/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-23 11:35:56.089291 creaap-0.1.9/creaap/spatial/data/
+-rw-r--r--   0 vsts      (1001) docker     (127)   114975 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/spatial/data/nuts0
+-rw-r--r--   0 vsts      (1001) docker     (127)   169486 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/spatial/data/nuts1
+-rw-r--r--   0 vsts      (1001) docker     (127)   236333 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/spatial/data/nuts2
+-rw-r--r--   0 vsts      (1001) docker     (127)   456454 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/spatial/data/nuts3
+-rw-r--r--   0 vsts      (1001) docker     (127)    10414 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/spatial/match.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7586 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/spatial/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-23 11:35:56.089291 creaap-0.1.9/creaap/storage/
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/storage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8318 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/storage/blob.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6705 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/storage/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10137 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/storage/table.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-23 11:35:56.089291 creaap-0.1.9/creaap/users/
+-rw-r--r--   0 vsts      (1001) docker     (127)      281 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9799 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/users/aad.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-01-23 11:35:10.000000 creaap-0.1.9/creaap/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-23 11:35:56.089291 creaap-0.1.9/creaap.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11797 2024-01-23 11:35:56.000000 creaap-0.1.9/creaap.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-01-23 11:35:56.000000 creaap-0.1.9/creaap.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-23 11:35:56.000000 creaap-0.1.9/creaap.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      146 2024-01-23 11:35:56.000000 creaap-0.1.9/creaap.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        7 2024-01-23 11:35:56.000000 creaap-0.1.9/creaap.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-01-23 11:35:56.093291 creaap-0.1.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1475 2024-01-23 11:35:10.000000 creaap-0.1.9/setup.py
```

### Comparing `creaap-0.1.8/LICENSE` & `creaap-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/PKG-INFO` & `creaap-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creaap
-Version: 0.1.8
+Version: 0.1.9
 Summary: CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.
 Home-page: https://dev.azure.com/dariodenart/_git/CREA%20Application%20Python%20toolkit
 Author: CREA
 Author-email: dario.denart@crea.gov.it
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `creaap-0.1.8/README.md` & `creaap-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/formats.py` & `creaap-0.1.9/creaap/formats.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/io.py` & `creaap-0.1.9/creaap/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 	return value
 
 def get_datetime_parameter_with_default(req, par_name:str, default_val:datetime, timezone_par:str = None, target_timezone = pytz.utc, **kwargs)->datetime:
 	'''
 	Parameters
 	----------
 	req:
-		an http request from an Azure Function
+		a http request from an Azure Function
 	par_name:str
 		how the datatime parameter is supposed to be named in the http request
 	default_val:datetime
 		a fallback datetime value
 	timezone_par:str
 		the name the timezone paramter has in the http request, if any.
 		If this paramter is not provided and the datetime in the htto request is naive,
@@ -110,13 +110,13 @@
 	# parse the timezone parameter, if any
 	if timezone_par:
 		tz = get_parameter_with_default(req, timezone_par, default_val = target_timezone)
 	else:
 		tz = target_timezone
 	if val:
 		try:
-			return to_tz_aware_datetime(val, origin_timezone = tz, target_timezone= target_timezone, **kwargs)
+			return to_tz_aware_datetime(val, timezone = tz, fallback=default_val)
 		except:
 			return default_val
 	return default_val
```

### Comparing `creaap-0.1.8/creaap/models.py` & `creaap-0.1.9/creaap/models.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/spatial/data/nuts0` & `creaap-0.1.9/creaap/spatial/data/nuts0`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/spatial/data/nuts1` & `creaap-0.1.9/creaap/spatial/data/nuts1`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/spatial/data/nuts2` & `creaap-0.1.9/creaap/spatial/data/nuts2`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/spatial/data/nuts3` & `creaap-0.1.9/creaap/spatial/data/nuts3`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/spatial/match.py` & `creaap-0.1.9/creaap/spatial/match.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/spatial/utils.py` & `creaap-0.1.9/creaap/spatial/utils.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/storage/blob.py` & `creaap-0.1.9/creaap/storage/blob.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/storage/file.py` & `creaap-0.1.9/creaap/storage/file.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/storage/table.py` & `creaap-0.1.9/creaap/storage/table.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/users/aad.py` & `creaap-0.1.9/creaap/users/aad.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap/utils.py` & `creaap-0.1.9/creaap/utils.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/creaap.egg-info/PKG-INFO` & `creaap-0.1.9/creaap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creaap
-Version: 0.1.8
+Version: 0.1.9
 Summary: CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.
 Home-page: https://dev.azure.com/dariodenart/_git/CREA%20Application%20Python%20toolkit
 Author: CREA
 Author-email: dario.denart@crea.gov.it
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `creaap-0.1.8/creaap.egg-info/SOURCES.txt` & `creaap-0.1.9/creaap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creaap-0.1.8/setup.py` & `creaap-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
    name='creaap',
-   version='0.1.8',
+   version='0.1.9',
    description='CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.',
    author='CREA',
    author_email='dario.denart@crea.gov.it',
    packages=['creaap', 'creaap.spatial', 'creaap.storage', 'creaap.users'],
    classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

