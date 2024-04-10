# Comparing `tmp/sdkgen-client-0.1.2.tar.gz` & `tmp/sdkgen-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkgen-client-0.1.2.tar", last modified: Mon Apr  8 20:28:00 2024, max compression
+gzip compressed data, was "sdkgen-client-0.2.0.tar", last modified: Wed Apr 10 17:33:11 2024, max compression
```

## Comparing `sdkgen-client-0.1.2.tar` & `sdkgen-client-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:28:00.376315 sdkgen-client-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 20:28:00.376315 sdkgen-client-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:28:00.376315 sdkgen-client-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:28:00.372315 sdkgen-client-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:28:00.372315 sdkgen-client-0.1.2/src/sdkgen/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/client_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/src/sdkgen/token_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:28:00.376315 sdkgen-client-0.1.2/src/sdkgen_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 20:28:00.000000 sdkgen-client-0.1.2/src/sdkgen_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 20:28:00.000000 sdkgen-client-0.1.2/src/sdkgen_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:28:00.000000 sdkgen-client-0.1.2/src/sdkgen_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 20:28:00.000000 sdkgen-client-0.1.2/src/sdkgen_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:28:00.000000 sdkgen-client-0.1.2/src/sdkgen_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:28:00.376315 sdkgen-client-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-08 20:27:56.000000 sdkgen-client-0.1.2/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:33:11.519335 sdkgen-client-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/src/sdkgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/client_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/token_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/tests/test_serialize.py
```

### Comparing `sdkgen-client-0.1.2/LICENSE` & `sdkgen-client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.1.2/PKG-INFO` & `sdkgen-client-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sdkgen-client
-Version: 0.1.2
+Version: 0.2.0
 Summary: SDKgen is a powerful code generator to automatically build client SDKs for your REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/sdkgen-python
 Project-URL: Issues, https://github.com/apioo/sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: dataclasses-json
+Requires-Dist: pydantic
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 SDKgen client
 ===
 
 Python implementation of the SDKgen client library. This library is used at our automatically generated Python
```

### Comparing `sdkgen-client-0.1.2/pyproject.toml` & `sdkgen-client-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkgen-client"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDKgen is a powerful code generator to automatically build client SDKs for your REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
@@ -12,15 +12,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Code Generators",
 ]
 dependencies = [
     "requests",
-    "dataclasses-json",
+    "pydantic",
 ]
 
 [project.urls]
 Homepage = "https://github.com/apioo/sdkgen-python"
 Issues = "https://github.com/apioo/sdkgen-python/issues"
 
 [project.optional-dependencies]
```

### Comparing `sdkgen-client-0.1.2/src/sdkgen/__init__.py` & `sdkgen-client-0.2.0/src/sdkgen/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.1.2/src/sdkgen/access_token.py` & `sdkgen-client-0.2.0/src/sdkgen/access_token.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 class AccessToken:
     access_token: Optional[str] = data_field(default=None, metadata=json_config(field_name="access_token"))
     token_type: Optional[str] = data_field(default=None, metadata=json_config(field_name="token_type"))
     expires_in: Optional[int] = data_field(default=None, metadata=json_config(field_name="expires_in"))
     refresh_token: Optional[str] = data_field(default=None, metadata=json_config(field_name="refresh_token"))
     scope: Optional[str] = data_field(default=None, metadata=json_config(field_name="scope"))
 
-    def get_expires_in_timestamp(self):
+    @classmethod
+    def get_expires_in_timestamp(cls):
         now = time.time()
 
-        expires_in = self.expires_in
-        if self.expires_in < 529196400:
+        expires_in = cls.expires_in
+        if cls.expires_in < 529196400:
             expires_in = now + expires_in
 
         return expires_in
```

### Comparing `sdkgen-client-0.1.2/src/sdkgen/parser.py` & `sdkgen-client-0.2.0/src/sdkgen/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import string
 import datetime
 
 
 class Parser:
-    def __init__(self, base_url: str):
-        self.base_url = self.normalize_url(base_url)
+    base_url: str = None
 
-    def url(self, path: str, parameters: dict[str, any]) -> str:
-        return self.base_url + "/" + self.substitute_parameters(path, parameters)
+    @classmethod
+    def __init__(cls, base_url: str):
+        cls.base_url = cls.normalize_url(base_url)
+
+    @classmethod
+    def url(cls, path: str, parameters: dict[str, any]) -> str:
+        return cls.base_url + "/" + cls.substitute_parameters(path, parameters)
 
-    def substitute_parameters(self, path: str, parameters: dict[str, any]) -> str:
+    @classmethod
+    def substitute_parameters(cls, path: str, parameters: dict[str, any]) -> str:
         parts = path.split("/")
         result = []
 
         for part in parts:
             if part is None or part == "":
                 continue
 
@@ -26,34 +31,36 @@
                     name = part[1:pos]
                 except ValueError:
                     name = part[1:]
             elif part.startswith("{") and part.endswith("}"):
                 name = part[1:len(part) - 1]
 
             if name in parameters:
-                part = self.to_string(parameters[name])
+                part = cls.to_string(parameters[name])
 
             result.append(part)
 
         return "/".join(result)
 
-    def query(self, parameters: dict[str, any], struct_names: list[str] = None) -> dict[str, any]:
+    @classmethod
+    def query(cls, parameters: dict[str, any], struct_names: list[str] = None) -> dict[str, any]:
         result: dict[str, any] = {}
         for name, value in parameters.items():
             if value is None:
                 continue
 
             if struct_names and name in struct_names:
-                result = result | self.query(value.to_dict())
+                result = result | cls.query(value.to_dict())
             else:
-                result[name] = self.to_string(value)
+                result[name] = cls.to_string(value)
 
         return result
 
-    def to_string(self, value: any) -> string:
+    @classmethod
+    def to_string(cls, value: any) -> string:
         t = type(value)
         if t is int:
             return str(value)
         elif t is float:
             return str(value)
         elif t is bool:
             return "1" if value else "0"
@@ -64,11 +71,12 @@
         elif t is datetime.datetime:
             return value.isoformat() + "Z"
         elif t is datetime.time:
             return value.isoformat()
         else:
             return ""
 
-    def normalize_url(self, value: string) -> string:
+    @classmethod
+    def normalize_url(cls, value: string) -> string:
         if value.endswith("/"):
             value = value[0:len(value) - 1]
         return value
```

### Comparing `sdkgen-client-0.1.2/src/sdkgen_client.egg-info/PKG-INFO` & `sdkgen-client-0.2.0/src/sdkgen_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sdkgen-client
-Version: 0.1.2
+Version: 0.2.0
 Summary: SDKgen is a powerful code generator to automatically build client SDKs for your REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/sdkgen-python
 Project-URL: Issues, https://github.com/apioo/sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: dataclasses-json
+Requires-Dist: pydantic
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 SDKgen client
 ===
 
 Python implementation of the SDKgen client library. This library is used at our automatically generated Python
```

### Comparing `sdkgen-client-0.1.2/tests/test_integration.py` & `sdkgen-client-0.2.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.1.2/tests/test_parser.py` & `sdkgen-client-0.2.0/tests/test_parser.py`

 * *Files identical despite different names*

