# Comparing `tmp/osm-login-python-1.0.2.tar.gz` & `tmp/osm-login-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-login-python-1.0.2.tar", last modified: Wed Dec  6 04:00:39 2023, max compression
+gzip compressed data, was "osm-login-python-1.0.3.tar", last modified: Wed Apr 10 12:05:02 2024, max compression
```

## Comparing `osm-login-python-1.0.2.tar` & `osm-login-python-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    34523 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/LICENSE
--rw-r--r--   0        0        0     2109 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/README.md
--rw-r--r--   0        0        0      124 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/osm_login_python/__init__.py
--rw-r--r--   0        0        0       22 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/osm_login_python/__version__.py
--rw-r--r--   0        0        0     3610 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/osm_login_python/core.py
--rw-r--r--   0        0        0     2268 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-12-06 04:00:32.303607 osm-login-python-1.0.2/tests/test_app.py
--rw-r--r--   0        0        0     2952 1970-01-01 00:00:00.000000 osm-login-python-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-10 12:04:55.597015 osm-login-python-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2109 2024-04-10 12:04:55.597015 osm-login-python-1.0.3/README.md
+-rw-r--r--   0        0        0      124 2024-04-10 12:04:55.597015 osm-login-python-1.0.3/osm_login_python/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-10 12:04:55.601015 osm-login-python-1.0.3/osm_login_python/__version__.py
+-rw-r--r--   0        0        0     3587 2024-04-10 12:04:55.601015 osm-login-python-1.0.3/osm_login_python/core.py
+-rw-r--r--   0        0        0     2268 2024-04-10 12:04:55.601015 osm-login-python-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 12:04:55.601015 osm-login-python-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:04:55.601015 osm-login-python-1.0.3/tests/test_app.py
+-rw-r--r--   0        0        0     2952 1970-01-01 00:00:00.000000 osm-login-python-1.0.3/PKG-INFO
```

### Comparing `osm-login-python-1.0.2/LICENSE` & `osm-login-python-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osm-login-python-1.0.2/README.md` & `osm-login-python-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `osm-login-python-1.0.2/osm_login_python/core.py` & `osm-login-python-1.0.3/osm_login_python/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import base64
 import json
 import logging
 
 from itsdangerous import BadSignature, SignatureExpired
 from itsdangerous.url_safe import URLSafeSerializer
-from pydantic import ValidationError
 from requests_oauthlib import OAuth2Session
 
 from . import Login, Token
 
 log = logging.getLogger(__name__)
 
 
@@ -99,10 +98,10 @@
             log.error(f"Could not decode token: {access_token}")
             raise ValueError("Could not decode token") from e
 
         try:
             user_data = deserializer.loads(decoded_token)
         except (SignatureExpired, BadSignature) as e:
             log.error(e)
-            raise ValidationError("Invalid token") from e
+            raise ValueError("Auth token is invalid or expired") from e
 
         return user_data
```

### Comparing `osm-login-python-1.0.2/pyproject.toml` & `osm-login-python-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "osm-login-python"
-version = "1.0.2"
+version = "1.0.3"
 dynamic = []
 description = "Use OSM Token exchange with OAuth2.0 for python projects."
 readme = "README.md"
 authors = [
     { name = "Kshitij Raj Sharma", email = "skshitizraj@gmail.com" },
 ]
 requires-python = ">=3.9"
```

### Comparing `osm-login-python-1.0.2/PKG-INFO` & `osm-login-python-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-login-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Use OSM Token exchange with OAuth2.0 for python projects.
 License: GPL-3.0-only
 Keywords: osm,openstreetmap,oauth2,login,hot
 Author-email: Kshitij Raj Sharma <skshitizraj@gmail.com>
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

