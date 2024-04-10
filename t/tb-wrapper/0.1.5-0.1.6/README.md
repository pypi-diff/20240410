# Comparing `tmp/tb_wrapper-0.1.5.tar.gz` & `tmp/tb_wrapper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb_wrapper-0.1.5.tar", last modified: Wed Apr 10 09:39:58 2024, max compression
+gzip compressed data, was "tb_wrapper-0.1.6.tar", last modified: Wed Apr 10 09:52:46 2024, max compression
```

## Comparing `tb_wrapper-0.1.5.tar` & `tb_wrapper-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11357 2023-11-21 13:34:49.000000 tb_wrapper-0.1.5/LICENSE
--rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1050 2023-12-12 14:30:11.000000 tb_wrapper-0.1.5/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      672 2024-04-10 09:39:43.000000 tb_wrapper-0.1.5/pyproject.toml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/setup.cfg
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/tb_wrapper/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1517 2024-03-15 16:23:18.000000 tb_wrapper-0.1.5/tb_wrapper/AlarmController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2475 2024-04-09 14:26:35.000000 tb_wrapper-0.1.5/tb_wrapper/AssetController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5247 2024-04-10 09:21:34.000000 tb_wrapper-0.1.5/tb_wrapper/DeviceController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1706 2024-04-09 14:25:14.000000 tb_wrapper-0.1.5/tb_wrapper/MainController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3142 2024-04-09 14:26:33.000000 tb_wrapper-0.1.5/tb_wrapper/QueryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1456 2024-04-09 14:26:31.000000 tb_wrapper-0.1.5/tb_wrapper/TelemetryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      755 2024-04-09 14:26:28.000000 tb_wrapper-0.1.5/tb_wrapper/UserController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tb_wrapper/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1343 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tb_wrapper/handle_exception.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/tb_wrapper.egg-info/
--rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      647 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       49 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       11 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/top_level.txt
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7437 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_AlarmController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18776 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_AssetController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    16871 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_DeviceController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1301 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_MainController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4190 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_QueryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6763 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_UserController.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:52:46.341334 tb_wrapper-0.1.6/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11357 2023-11-21 13:34:49.000000 tb_wrapper-0.1.6/LICENSE
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-10 09:52:46.341334 tb_wrapper-0.1.6/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1050 2023-12-12 14:30:11.000000 tb_wrapper-0.1.6/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      672 2024-04-10 09:52:06.000000 tb_wrapper-0.1.6/pyproject.toml
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-04-10 09:52:46.341334 tb_wrapper-0.1.6/setup.cfg
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:52:46.341334 tb_wrapper-0.1.6/tb_wrapper/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1517 2024-03-15 16:23:18.000000 tb_wrapper-0.1.6/tb_wrapper/AlarmController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2475 2024-04-09 14:26:35.000000 tb_wrapper-0.1.6/tb_wrapper/AssetController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5247 2024-04-10 09:21:34.000000 tb_wrapper-0.1.6/tb_wrapper/DeviceController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1821 2024-04-10 09:49:32.000000 tb_wrapper-0.1.6/tb_wrapper/MainController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3142 2024-04-09 14:26:33.000000 tb_wrapper-0.1.6/tb_wrapper/QueryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1456 2024-04-09 14:26:31.000000 tb_wrapper-0.1.6/tb_wrapper/TelemetryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      755 2024-04-09 14:26:28.000000 tb_wrapper-0.1.6/tb_wrapper/UserController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tb_wrapper/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1343 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tb_wrapper/handle_exception.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:52:46.341334 tb_wrapper-0.1.6/tb_wrapper.egg-info/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-10 09:52:46.000000 tb_wrapper-0.1.6/tb_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      647 2024-04-10 09:52:46.000000 tb_wrapper-0.1.6/tb_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-04-10 09:52:46.000000 tb_wrapper-0.1.6/tb_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       49 2024-04-10 09:52:46.000000 tb_wrapper-0.1.6/tb_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       11 2024-04-10 09:52:46.000000 tb_wrapper-0.1.6/tb_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:52:46.341334 tb_wrapper-0.1.6/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7437 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tests/test_AlarmController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18776 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tests/test_AssetController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    16871 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tests/test_DeviceController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1301 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tests/test_MainController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4190 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tests/test_QueryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6763 2023-12-07 10:30:45.000000 tb_wrapper-0.1.6/tests/test_UserController.py
```

### Comparing `tb_wrapper-0.1.5/LICENSE` & `tb_wrapper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/PKG-INFO` & `tb_wrapper-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb_wrapper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Wrapper for Zoe Project
 Author-email: GolDAndy <author@example.com>
 Project-URL: Homepage, https://github.com/GolDandy7/tb_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `tb_wrapper-0.1.5/README.md` & `tb_wrapper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/pyproject.toml` & `tb_wrapper-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.2.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tb_wrapper"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="GolDAndy", email="author@example.com" },
 ]
 description = "Wrapper for Zoe Project"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tb_wrapper-0.1.5/tb_wrapper/AlarmController.py` & `tb_wrapper-0.1.6/tb_wrapper/AlarmController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tb_wrapper/AssetController.py` & `tb_wrapper-0.1.6/tb_wrapper/AssetController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tb_wrapper/DeviceController.py` & `tb_wrapper-0.1.6/tb_wrapper/DeviceController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tb_wrapper/MainController.py` & `tb_wrapper-0.1.6/tb_wrapper/MainController.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 # tb_client.token_login(token=token,refresh_token=refresh_token)
 
 
 class MainController:
     tb_client = None
 
     def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None, token=None, refresh_token=None):
-        if token is not None and refresh_token is not None:
+        if token is not None:
             self.tb_client = RestClientCE(base_url=tb_url)
-            self.tb_client.token_login(
-                token=token, refresh_token=refresh_token)
+            if refresh_token is not None:
+                self.tb_client.token_login(
+                    token=token, refresh_token=refresh_token)
+            else:
+                self.tb_client.token_login(
+                    token=token)
         elif connection is not None:
             self.tb_client = connection
         else:
             self.__check_valid_parameters(tb_url, userfile, passwordfile)
             self.tb_client = RestClientCE(base_url=tb_url)
             with open(userfile) as f:
                 USERNAME = f.readline().strip()
```

### Comparing `tb_wrapper-0.1.5/tb_wrapper/QueryController.py` & `tb_wrapper-0.1.6/tb_wrapper/QueryController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tb_wrapper/TelemetryController.py` & `tb_wrapper-0.1.6/tb_wrapper/TelemetryController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tb_wrapper/UserController.py` & `tb_wrapper-0.1.6/tb_wrapper/UserController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tb_wrapper/handle_exception.py` & `tb_wrapper-0.1.6/tb_wrapper/handle_exception.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tb_wrapper.egg-info/PKG-INFO` & `tb_wrapper-0.1.6/tb_wrapper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb_wrapper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Wrapper for Zoe Project
 Author-email: GolDAndy <author@example.com>
 Project-URL: Homepage, https://github.com/GolDandy7/tb_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `tb_wrapper-0.1.5/tb_wrapper.egg-info/SOURCES.txt` & `tb_wrapper-0.1.6/tb_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tests/test_AlarmController.py` & `tb_wrapper-0.1.6/tests/test_AlarmController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tests/test_AssetController.py` & `tb_wrapper-0.1.6/tests/test_AssetController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tests/test_DeviceController.py` & `tb_wrapper-0.1.6/tests/test_DeviceController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tests/test_MainController.py` & `tb_wrapper-0.1.6/tests/test_MainController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tests/test_QueryController.py` & `tb_wrapper-0.1.6/tests/test_QueryController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.5/tests/test_UserController.py` & `tb_wrapper-0.1.6/tests/test_UserController.py`

 * *Files identical despite different names*

