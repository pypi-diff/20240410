# Comparing `tmp/jsm_user_services-1.3.7.tar.gz` & `tmp/jsm_user_services-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_user_services-1.3.7.tar", max compression
+gzip compressed data, was "jsm_user_services-1.4.0.tar", max compression
```

## Comparing `jsm_user_services-1.3.7.tar` & `jsm_user_services-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/LICENSE
--rw-r--r--   0        0        0    10306 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/README.md
--rw-r--r--   0        0        0       54 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/__init__.py
--rw-r--r--   0        0        0      107 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/apps.py
--rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/decorators/__init__.py
--rw-r--r--   0        0        0     3795 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd.py
--rw-r--r--   0        0        0     5933 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd_utils.py
--rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/drf_tools/__init__.py
--rw-r--r--   0        0        0     2475 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/drf_tools/helpers.py
--rw-r--r--   0        0        0    14221 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/drf_tools/permissions.py
--rw-r--r--   0        0        0      692 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/exception.py
--rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/flask/__init__.py
--rw-r--r--   0        0        0     3462 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/flask/middleware.py
--rw-r--r--   0        0        0     3292 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/middleware.py
--rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/__init__.py
--rw-r--r--   0        0        0     4247 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/everest.py
--rw-r--r--   0        0        0     1996 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/google.py
--rw-r--r--   0        0        0     4657 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/user.py
--rw-r--r--   0        0        0     1840 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/settings.py
--rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/__init__.py
--rw-r--r--   0        0        0     1007 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/auth_jwt.py
--rw-r--r--   0        0        0      866 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/email_utils.py
--rw-r--r--   0        0        0     2333 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/http_utils.py
--rw-r--r--   0        0        0      304 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/import_utils.py
--rw-r--r--   0        0        0      415 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/local_threading_utils.py
--rw-r--r--   0        0        0      268 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/logging_utils.py
--rw-r--r--   0        0        0     2185 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/request_id.py
--rw-r--r--   0        0        0      618 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/settings_utils.py
--rw-r--r--   0        0        0      237 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/string_utils.py
--rw-r--r--   0        0        0     1574 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/pyproject.toml
--rw-r--r--   0        0        0    11293 1970-01-01 00:00:00.000000 jsm_user_services-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/LICENSE
+-rw-r--r--   0        0        0    10306 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/README.md
+-rw-r--r--   0        0        0       54 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/__init__.py
+-rw-r--r--   0        0        0      107 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/apps.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/decorators/__init__.py
+-rw-r--r--   0        0        0     3795 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd.py
+-rw-r--r--   0        0        0     5933 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd_utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/drf_tools/__init__.py
+-rw-r--r--   0        0        0     2475 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/drf_tools/helpers.py
+-rw-r--r--   0        0        0    14221 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/drf_tools/permissions.py
+-rw-r--r--   0        0        0      692 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/exception.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/flask/__init__.py
+-rw-r--r--   0        0        0     3462 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/flask/middleware.py
+-rw-r--r--   0        0        0     3292 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/__init__.py
+-rw-r--r--   0        0        0     4247 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/everest.py
+-rw-r--r--   0        0        0     1996 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/google.py
+-rw-r--r--   0        0        0     5640 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/user.py
+-rw-r--r--   0        0        0     1840 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/settings.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/__init__.py
+-rw-r--r--   0        0        0     1262 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/auth_jwt.py
+-rw-r--r--   0        0        0      866 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/email_utils.py
+-rw-r--r--   0        0        0     2333 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/http_utils.py
+-rw-r--r--   0        0        0      304 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/import_utils.py
+-rw-r--r--   0        0        0      415 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/local_threading_utils.py
+-rw-r--r--   0        0        0      268 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/logging_utils.py
+-rw-r--r--   0        0        0     2185 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/request_id.py
+-rw-r--r--   0        0        0      618 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/settings_utils.py
+-rw-r--r--   0        0        0      237 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/string_utils.py
+-rw-r--r--   0        0        0     1574 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11293 1970-01-01 00:00:00.000000 jsm_user_services-1.4.0/PKG-INFO
```

### Comparing `jsm_user_services-1.3.7/LICENSE` & `jsm_user_services-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/README.md` & `jsm_user_services-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd.py` & `jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd_utils.py` & `jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/drf_tools/helpers.py` & `jsm_user_services-1.4.0/jsm_user_services/drf_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/drf_tools/permissions.py` & `jsm_user_services-1.4.0/jsm_user_services/drf_tools/permissions.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/exception.py` & `jsm_user_services-1.4.0/jsm_user_services/exception.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/flask/middleware.py` & `jsm_user_services-1.4.0/jsm_user_services/flask/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/middleware.py` & `jsm_user_services-1.4.0/jsm_user_services/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/services/everest.py` & `jsm_user_services-1.4.0/jsm_user_services/services/everest.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/services/google.py` & `jsm_user_services-1.4.0/jsm_user_services/services/google.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/services/user.py` & `jsm_user_services-1.4.0/jsm_user_services/services/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import hashlib
 
 from importlib import import_module
+from typing import Any
 from typing import List
 from typing import Optional
 
 from jsm_user_services.support.auth_jwt import get_decoded_jwt_token
+from jsm_user_services.support.auth_jwt import get_decoded_oauth_token
 from jsm_user_services.support.http_utils import get_response_body
 from jsm_user_services.support.http_utils import request
 from jsm_user_services.support.local_threading_utils import get_from_local_threading
 from jsm_user_services.support.request_id import current_request_id
 from jsm_user_services.support.request_id import request_id_header_name
 
 
@@ -43,14 +45,25 @@
     token = current_jwt_token()
     if token:
         return get_decoded_jwt_token(token)["jsm_identity"]
 
     return None
 
 
+def get_oauth_token() -> Optional[dict[Any, Any]]:
+    """
+    This function retrieves the OAuth token from the local threading.
+    If the token is not present, it returns None.
+    """
+    token = current_jwt_token()
+    if token:
+        return get_decoded_oauth_token(token)
+    return None
+
+
 def get_ltm_token() -> Optional[str]:
     token = current_jwt_token()
     if token:
         return get_decoded_jwt_token(token)["yuntiandu"]
 
     return None
 
@@ -156,7 +169,29 @@
 
 def get_session_id_from_bearer_token(bearer_token: str) -> str:
     return hashlib.sha1(bearer_token.encode("utf-8")).hexdigest()
 
 
 def get_user_session_id() -> Optional[str]:
     return get_from_local_threading("user_session_id")
+
+
+def get_user_id_auth() -> Optional[str]:
+    """
+    This function retrieves the user's ID from an OAuth JWT token.
+    If the "sub" field is not present, it returns None.
+    """
+    user_data = get_oauth_token()
+    if user_data:
+        return user_data.get("sub")
+    return None
+
+
+def get_user_email_from_oauth_jwt() -> Optional[str]:
+    """
+    This function retrieves the user's email from an OAuth JWT token.
+    If the "email" field is not present, it returns None.
+    """
+    user_data = get_oauth_token()
+    if user_data:
+        return user_data.get("email")
+    return None
```

### Comparing `jsm_user_services-1.3.7/jsm_user_services/settings.py` & `jsm_user_services-1.4.0/jsm_user_services/settings.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/support/auth_jwt.py` & `jsm_user_services-1.4.0/jsm_user_services/support/auth_jwt.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,27 @@
 from typing import Optional
 
 import jwt
 
 
 def get_decoded_jwt_token(jwt_token: str) -> dict:
     """
-    Gets a decoded JWT token.
+    Gets a decoded JWT token with the HS256 algorithm.
     """
 
     return jwt.decode(jwt_token, algorithms=["HS256"], options={"verify_signature": False})
 
 
+def get_decoded_oauth_token(oauth_jwt_token: str) -> dict:
+    """
+    Gets a decoded JWT token with the RS256 algorithm.
+    """
+    return jwt.decode(oauth_jwt_token, algorithms=["RS256"], options={"verify_signature": False})
+
+
 def get_bearer_authorization_token(authorization_value: str) -> Optional[str]:
     """
     Retrieve a bearer authorization token from an Authorization header value.
 
     It expects the header value to be something on the lines of: "Bearer token".
 
     Examples:
```

### Comparing `jsm_user_services-1.3.7/jsm_user_services/support/email_utils.py` & `jsm_user_services-1.4.0/jsm_user_services/support/email_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/support/http_utils.py` & `jsm_user_services-1.4.0/jsm_user_services/support/http_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/support/request_id.py` & `jsm_user_services-1.4.0/jsm_user_services/support/request_id.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/jsm_user_services/support/settings_utils.py` & `jsm_user_services-1.4.0/jsm_user_services/support/settings_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.7/pyproject.toml` & `jsm_user_services-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsm-user-services"
-version = "1.3.7"
+version = "1.4.0"
 description = "Middleware to intercept JWT auth token and more utils functions"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "jsm_user_services"}]
 classifiers=[
     "Programming Language :: Python",
```

### Comparing `jsm_user_services-1.3.7/PKG-INFO` & `jsm_user_services-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-user-services
-Version: 1.3.7
+Version: 1.4.0
 Summary: Middleware to intercept JWT auth token and more utils functions
 License: MIT
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

