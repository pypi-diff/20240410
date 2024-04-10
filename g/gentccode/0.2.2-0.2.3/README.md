# Comparing `tmp/gentccode-0.2.2.tar.gz` & `tmp/gentccode-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentccode-0.2.2.tar", max compression
+gzip compressed data, was "gentccode-0.2.3.tar", max compression
```

## Comparing `gentccode-0.2.2.tar` & `gentccode-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.2/LICENSE
--rw-r--r--   0        0        0     1066 2024-04-10 03:12:23.157802 gentccode-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.2/gentccode/__init__.py
--rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.2/gentccode/cartesian_for_case.py
--rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.2/gentccode/check_version.py
--rw-r--r--   0        0        0     3014 2024-04-10 03:10:47.777166 gentccode-0.2.2/gentccode/cli.py
--rw-r--r--   0        0        0    20333 2024-04-10 03:04:41.206073 gentccode-0.2.2/gentccode/convert_to_jmx.py
--rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.2/gentccode/convert_to_locust.py
--rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.2/gentccode/generate_case_code.py
--rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.2/gentccode/merge_api.py
--rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.2/gentccode/produce_search_case.py
--rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.2/gentccode/produce_test_case.py
--rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.2/gentccode/read_swagger_rule.py
--rw-r--r--   0        0        0      612 2024-04-10 03:17:34.058423 gentccode-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 gentccode-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1066 2024-04-10 03:12:23.157802 gentccode-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.3/gentccode/__init__.py
+-rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.3/gentccode/cartesian_for_case.py
+-rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.3/gentccode/check_version.py
+-rw-r--r--   0        0        0     3068 2024-04-10 06:10:45.878017 gentccode-0.2.3/gentccode/cli.py
+-rw-r--r--   0        0        0    20333 2024-04-10 03:04:41.206073 gentccode-0.2.3/gentccode/convert_to_jmx.py
+-rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.3/gentccode/convert_to_locust.py
+-rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.3/gentccode/generate_case_code.py
+-rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.3/gentccode/merge_api.py
+-rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.3/gentccode/produce_search_case.py
+-rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.3/gentccode/produce_test_case.py
+-rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.3/gentccode/read_swagger_rule.py
+-rw-r--r--   0        0        0      612 2024-04-10 06:12:38.544960 gentccode-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 gentccode-0.2.3/PKG-INFO
```

### Comparing `gentccode-0.2.2/LICENSE` & `gentccode-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/README.md` & `gentccode-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/cartesian_for_case.py` & `gentccode-0.2.3/gentccode/cartesian_for_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/check_version.py` & `gentccode-0.2.3/gentccode/check_version.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/cli.py` & `gentccode-0.2.3/gentccode/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,20 +61,22 @@
     product_locust_code(curl_file_path=filename)
 
 
 @click.command(help="generate jmeter script by curl file")
 @click.argument("filename", type=click.Path(exists=True))
 @click.option(
     "-ja",
-    "--json-assert",
+    "--jsonAssert",
     required=True,
     help="json node, like: 'code','data.code','a.b.c'",
 )
-def jmeter(filename):
-    convert_payloads_of_curl_to_jmx_file(curl_file_path=filename)
+def jmeter(filename, jsonAssert):
+    convert_payloads_of_curl_to_jmx_file(
+        curl_file_path=filename, json_path_assert=jsonAssert
+    )
 
 
 @click.command(help="auto generate swagger2 document's test code")
 @click.argument("filename", type=click.Path(exists=True))
 def swagger_at(filename):
     ptc.produce_merged_case_for_swagger_and_curl(curl_file_path=filename)
```

### Comparing `gentccode-0.2.2/gentccode/convert_to_jmx.py` & `gentccode-0.2.3/gentccode/convert_to_jmx.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/convert_to_locust.py` & `gentccode-0.2.3/gentccode/convert_to_locust.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/generate_case_code.py` & `gentccode-0.2.3/gentccode/generate_case_code.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/merge_api.py` & `gentccode-0.2.3/gentccode/merge_api.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/produce_search_case.py` & `gentccode-0.2.3/gentccode/produce_search_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/produce_test_case.py` & `gentccode-0.2.3/gentccode/produce_test_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/gentccode/read_swagger_rule.py` & `gentccode-0.2.3/gentccode/read_swagger_rule.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.2/pyproject.toml` & `gentccode-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gentccode"
-version = "0.2.2"
+version = "0.2.3"
 description = "generate test case code"
 authors = ["Lei Su <lei.susl@shopee.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `gentccode-0.2.2/PKG-INFO` & `gentccode-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentccode
-Version: 0.2.2
+Version: 0.2.3
 Summary: generate test case code
 Author: Lei Su
 Author-email: lei.susl@shopee.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

