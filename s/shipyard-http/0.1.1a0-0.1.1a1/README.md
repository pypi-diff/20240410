# Comparing `tmp/shipyard_http-0.1.1a0.tar.gz` & `tmp/shipyard_http-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_http-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_http-0.1.1a1.tar", max compression
```

## Comparing `shipyard_http-0.1.1a0.tar` & `shipyard_http-0.1.1a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.742554 shipyard_http-0.1.1a0/README.md
--rw-r--r--   0        0        0      482 2024-04-09 22:36:52.664197 shipyard_http-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743381 shipyard_http-0.1.1a0/shipyard_http/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743456 shipyard_http-0.1.1a0/shipyard_http/cli/__init__.py
--rw-r--r--   0        0        0     3694 2024-04-09 21:08:58.774558 shipyard_http-0.1.1a0/shipyard_http/cli/download_file.py
--rw-r--r--   0        0        0     3568 2024-04-09 21:08:58.774913 shipyard_http-0.1.1a0/shipyard_http/cli/execute_request.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 shipyard_http-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.742554 shipyard_http-0.1.1a1/README.md
+-rw-r--r--   0        0        0      482 2024-04-09 22:45:50.318648 shipyard_http-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743381 shipyard_http-0.1.1a1/shipyard_http/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.743456 shipyard_http-0.1.1a1/shipyard_http/cli/__init__.py
+-rw-r--r--   0        0        0     3694 2024-04-09 21:08:58.774558 shipyard_http-0.1.1a1/shipyard_http/cli/download_file.py
+-rw-r--r--   0        0        0     3604 2024-04-09 22:45:14.825369 shipyard_http-0.1.1a1/shipyard_http/cli/execute_request.py
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 shipyard_http-0.1.1a1/PKG-INFO
```

### Comparing `shipyard_http-0.1.1a0/shipyard_http/cli/download_file.py` & `shipyard_http-0.1.1a1/shipyard_http/cli/download_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_http-0.1.1a0/shipyard_http/cli/execute_request.py` & `shipyard_http-0.1.1a1/shipyard_http/cli/execute_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,16 @@
         headers["Content-Type"] = args.content_type
 
     message = args.message
     print_response = shipyard_utils.args.convert_to_boolean(args.print_response)
     artifact = Artifact("httprequest")
 
     destination_folder_name = shipyard_utils.files.clean_folder_name(args.destination_folder_name)
-    shipyard_utils.files.create_folder_if_dne(destination_folder_name)
+    if destination_folder_name:
+        shipyard_utils.files.create_folder_if_dne(destination_folder_name)
 
     destination_name = shipyard_utils.files.combine_folder_and_file_name(
         destination_folder_name, args.destination_file_name
     )
 
     request = execute_request(method, url, headers, message)
     write_response_to_file(request, destination_name)
```

### Comparing `shipyard_http-0.1.1a0/PKG-INFO` & `shipyard_http-0.1.1a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-http
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: 
 Author: johnathan-rodriguez
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

