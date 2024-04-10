# Comparing `tmp/fewerai-1.0.2.tar.gz` & `tmp/fewerai-2.0.0.tar.gz`

## Comparing `fewerai-1.0.2.tar` & `fewerai-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fewerai-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 fewerai-1.0.2/src/fewerai/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fewerai-1.0.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 fewerai-1.0.2/LICENSE
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fewerai-1.0.2/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fewerai-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fewerai-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fewerai-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 fewerai-2.0.0/src/fewerai/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fewerai-2.0.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 fewerai-2.0.0/LICENSE
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fewerai-2.0.0/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fewerai-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fewerai-2.0.0/PKG-INFO
```

### Comparing `fewerai-1.0.2/.github/workflows/python-publish.yml` & `fewerai-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fewerai-1.0.2/src/fewerai/__init__.py` & `fewerai-2.0.0/src/fewerai/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # FewerAI | src.fewerai.__init__.py
 # This file is ruled by the license joined.
 
 import requests
 
-class LoginException(Exception):
+class AccessForbiddenException(Exception):
     """Raised when failed to login to the API server."""
     pass
 
 class BadRequestException(Exception):
     """Raised when the server can't decode the request."""
     pass
 
 class ServiceUnavailableException(Exception):
-    """Raised when the server get an internall exceptio, or when the server is not reachable"""
+    """Raised when the server get an internall exceptio, or when the server is not reachable."""
+
+class AccountBannedException(Exception):
+    """Raised when the provided account is suspended."""
 
 class API(object):
     def __init__(self, username:str, token:str):
         self.username = username
         self.token = token
         
     def generate(self, request:str):
@@ -28,14 +31,20 @@
             url = "http://n1.recloud-hosting.me:1123/api"
 
             response = requests.post(url, data=data)
 
             if response.text == "400":
                 raise BadRequestException("Bad Request. Please update the version of this client or post an issue here : https://github.com/FewerElk/FewerAI/issues")
             elif response.text == "403":
-                raise LoginException("Failed to login: incorrect username or password.")
+                raise AccessForbiddenException("Failed to login: incorrect username or password.")
+            elif response.text == "403-B":
+                try:
+                    raise AccountBannedException("The provided credentials are suspended by the server.")
+                except AccountBannedException as e:
+                    raise AccessForbiddenException("Could not log in to the server.") from e
+
             elif response.text == "503":
                 raise ServiceUnavailableException("An internal exception occured when performing the generation. Maybe the server couldn't decode your request. Did you used utf-8 caracters ?")
             else:
                 return response.text
         except requests.exceptions.ConnectionError:
             raise ServiceUnavailableException("Could not connect to the server. Please open an issue.")
```

### Comparing `fewerai-1.0.2/LICENSE` & `fewerai-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fewerai-1.0.2/pyproject.toml` & `fewerai-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fewerai"
-version = "1.0.2"
+version = "2.0.0"
 authors = [
   { name="FewerElk", email="fewerelk@gmail.com" },
 ]
 description = "A simple ai"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fewerai-1.0.2/PKG-INFO` & `fewerai-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fewerai
-Version: 1.0.2
+Version: 2.0.0
 Summary: A simple ai
 Project-URL: Homepage, https://github.com/FewerElk/FewerAI
 Project-URL: Issues, https://github.com/FewerElk/FewerAI/issues
 Author-email: FewerElk <fewerelk@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

