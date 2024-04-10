# Comparing `tmp/tb_wrapper-0.1.4.tar.gz` & `tmp/tb_wrapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb_wrapper-0.1.4.tar", last modified: Mon Apr  8 14:14:05 2024, max compression
+gzip compressed data, was "tb_wrapper-0.1.5.tar", last modified: Wed Apr 10 09:39:58 2024, max compression
```

## Comparing `tb_wrapper-0.1.4.tar` & `tb_wrapper-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-08 14:14:05.980695 tb_wrapper-0.1.4/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11357 2023-11-21 13:34:49.000000 tb_wrapper-0.1.4/LICENSE
--rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-08 14:14:05.980695 tb_wrapper-0.1.4/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1050 2023-12-12 14:30:11.000000 tb_wrapper-0.1.4/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      672 2024-04-08 14:13:59.000000 tb_wrapper-0.1.4/pyproject.toml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-04-08 14:14:05.980695 tb_wrapper-0.1.4/setup.cfg
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-08 14:14:05.980695 tb_wrapper-0.1.4/tb_wrapper/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1517 2024-03-15 16:23:18.000000 tb_wrapper-0.1.4/tb_wrapper/AlarmController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2421 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tb_wrapper/AssetController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9829 2024-04-08 14:13:22.000000 tb_wrapper-0.1.4/tb_wrapper/DeviceController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1386 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tb_wrapper/MainController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3088 2024-02-16 12:09:09.000000 tb_wrapper-0.1.4/tb_wrapper/QueryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1402 2024-02-09 14:10:28.000000 tb_wrapper-0.1.4/tb_wrapper/TelemetryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      701 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tb_wrapper/UserController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tb_wrapper/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1343 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tb_wrapper/handle_exception.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-08 14:14:05.980695 tb_wrapper-0.1.4/tb_wrapper.egg-info/
--rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-08 14:14:05.000000 tb_wrapper-0.1.4/tb_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      647 2024-04-08 14:14:05.000000 tb_wrapper-0.1.4/tb_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-04-08 14:14:05.000000 tb_wrapper-0.1.4/tb_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       49 2024-04-08 14:14:05.000000 tb_wrapper-0.1.4/tb_wrapper.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       11 2024-04-08 14:14:05.000000 tb_wrapper-0.1.4/tb_wrapper.egg-info/top_level.txt
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-08 14:14:05.980695 tb_wrapper-0.1.4/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7437 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tests/test_AlarmController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18776 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tests/test_AssetController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    16871 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tests/test_DeviceController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1301 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tests/test_MainController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4190 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tests/test_QueryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6763 2023-12-07 10:30:45.000000 tb_wrapper-0.1.4/tests/test_UserController.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11357 2023-11-21 13:34:49.000000 tb_wrapper-0.1.5/LICENSE
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1050 2023-12-12 14:30:11.000000 tb_wrapper-0.1.5/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      672 2024-04-10 09:39:43.000000 tb_wrapper-0.1.5/pyproject.toml
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/setup.cfg
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/tb_wrapper/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1517 2024-03-15 16:23:18.000000 tb_wrapper-0.1.5/tb_wrapper/AlarmController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2475 2024-04-09 14:26:35.000000 tb_wrapper-0.1.5/tb_wrapper/AssetController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5247 2024-04-10 09:21:34.000000 tb_wrapper-0.1.5/tb_wrapper/DeviceController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1706 2024-04-09 14:25:14.000000 tb_wrapper-0.1.5/tb_wrapper/MainController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3142 2024-04-09 14:26:33.000000 tb_wrapper-0.1.5/tb_wrapper/QueryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1456 2024-04-09 14:26:31.000000 tb_wrapper-0.1.5/tb_wrapper/TelemetryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      755 2024-04-09 14:26:28.000000 tb_wrapper-0.1.5/tb_wrapper/UserController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tb_wrapper/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1343 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tb_wrapper/handle_exception.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/tb_wrapper.egg-info/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      647 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       49 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       11 2024-04-10 09:39:58.000000 tb_wrapper-0.1.5/tb_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-10 09:39:58.351458 tb_wrapper-0.1.5/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7437 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_AlarmController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18776 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_AssetController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    16871 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_DeviceController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1301 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_MainController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4190 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_QueryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6763 2023-12-07 10:30:45.000000 tb_wrapper-0.1.5/tests/test_UserController.py
```

### Comparing `tb_wrapper-0.1.4/LICENSE` & `tb_wrapper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/PKG-INFO` & `tb_wrapper-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb_wrapper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Wrapper for Zoe Project
 Author-email: GolDAndy <author@example.com>
 Project-URL: Homepage, https://github.com/GolDandy7/tb_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `tb_wrapper-0.1.4/README.md` & `tb_wrapper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/pyproject.toml` & `tb_wrapper-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.2.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tb_wrapper"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GolDAndy", email="author@example.com" },
 ]
 description = "Wrapper for Zoe Project"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tb_wrapper-0.1.4/tb_wrapper/AlarmController.py` & `tb_wrapper-0.1.5/tb_wrapper/AlarmController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tb_wrapper/AssetController.py` & `tb_wrapper-0.1.5/tb_wrapper/AssetController.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from tb_wrapper.handle_exception import *
 from tb_wrapper.MainController import *
 
 
 @handle_tb_wrapper_exception
 class AssetController(MainController):
 
-    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None):
-        super().__init__(tb_url, userfile, passwordfile, connection)
+    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None, token=None, refresh_token=None):
+        super().__init__(tb_url, userfile, passwordfile, connection, token, refresh_token)
 
     def get_default_asset_profile_info(self):
         return self.tb_client.get_default_asset_profile_info()
 
     def create_asset(self, asset_profile_id, asset_name, customer_obj_id):
         asset = Asset(
             name=asset_name, asset_profile_id=asset_profile_id, customer_id=customer_obj_id)
```

### Comparing `tb_wrapper-0.1.4/tb_wrapper/MainController.py` & `tb_wrapper-0.1.5/tb_wrapper/MainController.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from tb_wrapper.handle_exception import handle_tb_wrapper_exception
 from tb_rest_client.rest_client_ce import *
+# tb_client.token_login(token=token,refresh_token=refresh_token)
 
 
 class MainController:
     tb_client = None
 
-    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None):
-        if connection is None:
+    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None, token=None, refresh_token=None):
+        if token is not None and refresh_token is not None:
+            self.tb_client = RestClientCE(base_url=tb_url)
+            self.tb_client.token_login(
+                token=token, refresh_token=refresh_token)
+        elif connection is not None:
+            self.tb_client = connection
+        else:
             self.__check_valid_parameters(tb_url, userfile, passwordfile)
             self.tb_client = RestClientCE(base_url=tb_url)
             with open(userfile) as f:
                 USERNAME = f.readline().strip()
             with open(passwordfile) as f:
                 PASSWORD = f.readline().strip()
             self.tb_client.login(
                 username=USERNAME, password=PASSWORD)
-        else:
-            self.tb_client = connection
 
     def destroyConnection(self):
         return self.tb_client.logout()
 
     @handle_tb_wrapper_exception
     def __check_valid_parameters(self, tb_url, userfile, passwordfile):
         if tb_url is None or tb_url is "":
```

### Comparing `tb_wrapper-0.1.4/tb_wrapper/QueryController.py` & `tb_wrapper-0.1.5/tb_wrapper/QueryController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tb_wrapper.handle_exception import *
 from tb_wrapper.MainController import *
 
 
 class QueryController(MainController):
 
-    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None):
-        super().__init__(tb_url, userfile, passwordfile, connection)
+    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None, token=None, refresh_token=None):
+        super().__init__(tb_url, userfile, passwordfile, connection, token, refresh_token)
 
     @handle_tb_wrapper_exception
     def query_body_attribute(self, filter_key_scope, filter_key_name, filter_key_value, filter_key_type):
         predicate = {"operation": "EQUAL",
                      "value": {"defaultValue": filter_key_value},
                      "type": filter_key_type}
         ef = EntityFilter(entity_type="CUSTOMER",
```

### Comparing `tb_wrapper-0.1.4/tb_wrapper/TelemetryController.py` & `tb_wrapper-0.1.5/tb_wrapper/TelemetryController.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from tb_wrapper.handle_exception import *
 from tb_wrapper.MainController import *
 
 
 @handle_tb_wrapper_exception
 class TelemetryController(MainController):
 
-    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None):
-        super().__init__(tb_url, userfile, passwordfile, connection)
+    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None, token=None, refresh_token=None):
+        super().__init__(tb_url, userfile, passwordfile, connection, token, refresh_token)
 
     # this method manages one entity id and a list of keys
 
     def get_timeseries(self, entities_keys=None, start_ts=None, end_ts=None):
         if entities_keys is None:
             raise ValueError(
                 "Entity IDs and Keys must be specified")
```

### Comparing `tb_wrapper-0.1.4/tb_wrapper/UserController.py` & `tb_wrapper-0.1.5/tb_wrapper/UserController.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from tb_wrapper.handle_exception import *
 from tb_wrapper.MainController import *
 
 
 @handle_tb_wrapper_exception
 class UserController(MainController):
 
-    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None):
-        super().__init__(tb_url, userfile, passwordfile, connection)
+    def __init__(self, tb_url=None, userfile=None, passwordfile=None, connection=None, token=None, refresh_token=None):
+        super().__init__(tb_url, userfile, passwordfile, connection, token, refresh_token)
 
     def actual_user(self):
         return self.tb_client.get_user()
 
     def get_users_from_customer(self, customer_id):
         return self.tb_client.get_customer_users(customer_id=customer_id, page_size=1000, page=0)
```

### Comparing `tb_wrapper-0.1.4/tb_wrapper/handle_exception.py` & `tb_wrapper-0.1.5/tb_wrapper/handle_exception.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tb_wrapper.egg-info/PKG-INFO` & `tb_wrapper-0.1.5/tb_wrapper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb_wrapper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Wrapper for Zoe Project
 Author-email: GolDAndy <author@example.com>
 Project-URL: Homepage, https://github.com/GolDandy7/tb_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `tb_wrapper-0.1.4/tb_wrapper.egg-info/SOURCES.txt` & `tb_wrapper-0.1.5/tb_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tests/test_AlarmController.py` & `tb_wrapper-0.1.5/tests/test_AlarmController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tests/test_AssetController.py` & `tb_wrapper-0.1.5/tests/test_AssetController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tests/test_DeviceController.py` & `tb_wrapper-0.1.5/tests/test_DeviceController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tests/test_MainController.py` & `tb_wrapper-0.1.5/tests/test_MainController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tests/test_QueryController.py` & `tb_wrapper-0.1.5/tests/test_QueryController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.4/tests/test_UserController.py` & `tb_wrapper-0.1.5/tests/test_UserController.py`

 * *Files identical despite different names*

