# Comparing `tmp/elytra_ms-0.3.3.tar.gz` & `tmp/elytra_ms-0.4.0.tar.gz`

## Comparing `elytra_ms-0.3.3.tar` & `elytra_ms-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/const.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/core.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/protocols.py
--rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/retry_transport.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/bedrock_realms/__init__.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/bedrock_realms/models.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/scripts/auth_device_code.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/scripts/authenticate.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/__init__.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/core.py
--rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/rta.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/club/__init__.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/club/models.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/peoplehub/__init__.py
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/peoplehub/models.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/profile/__init__.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/profile/models.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/elytra/xbox/social/__init__.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/LICENSE
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/const.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/core.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/protocols.py
+-rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/retry_transport.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/bedrock_realms/__init__.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/bedrock_realms/models.py
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/scripts/auth_device_code.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/scripts/authenticate.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/__init__.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/core.py
+-rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/rta.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/club/__init__.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/club/models.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/message/__init__.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/message/models.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/peoplehub/__init__.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/peoplehub/models.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/profile/__init__.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/profile/models.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/social/__init__.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/PKG-INFO
```

### Comparing `elytra_ms-0.3.3/elytra/const.py` & `elytra_ms-0.4.0/elytra/const.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/core.py` & `elytra_ms-0.4.0/elytra/core.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/protocols.py` & `elytra_ms-0.4.0/elytra/protocols.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/retry_transport.py` & `elytra_ms-0.4.0/elytra/retry_transport.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/bedrock_realms/__init__.py` & `elytra_ms-0.4.0/elytra/bedrock_realms/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/bedrock_realms/models.py` & `elytra_ms-0.4.0/elytra/bedrock_realms/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/scripts/auth_device_code.py` & `elytra_ms-0.4.0/elytra/scripts/auth_device_code.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/scripts/authenticate.py` & `elytra_ms-0.4.0/elytra/scripts/authenticate.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/__init__.py` & `elytra_ms-0.4.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-"""
 MIT License
 
 Copyright (c) 2023-2024 AstreaTSS
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -16,14 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-"""
-
-from .club import *
-from .core import *
-from .peoplehub import *
-from .profile import *
-from .social import *
```

### Comparing `elytra_ms-0.3.3/elytra/xbox/core.py` & `elytra_ms-0.4.0/elytra/xbox/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 SOFTWARE.
 """
 
 from elytra import BaseMicrosoftAPI
 from elytra.const import XBOX_API_RELYING_PARTY
 
 from .club import ClubHandler
+from .message import MessageHandler
 from .peoplehub import PeopleHubHandler
 from .profile import ProfileHandler
 from .rta import RTA
 from .social import SocialHandler
 
 __all__ = ("XboxAPI", "RTA")
 
 
 class XboxAPI(
     BaseMicrosoftAPI,
     ProfileHandler,
     PeopleHubHandler,
     ClubHandler,
     SocialHandler,
+    MessageHandler,
 ):
     RELYING_PARTY: str = XBOX_API_RELYING_PARTY
 
     async def establish_rta(self) -> RTA:
         return await RTA.establish(self.base_headers)
```

### Comparing `elytra_ms-0.3.3/elytra/xbox/rta.py` & `elytra_ms-0.4.0/elytra/xbox/rta.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/club/__init__.py` & `elytra_ms-0.4.0/elytra/xbox/club/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/club/models.py` & `elytra_ms-0.4.0/elytra/xbox/club/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/peoplehub/__init__.py` & `elytra_ms-0.4.0/elytra/xbox/peoplehub/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/peoplehub/models.py` & `elytra_ms-0.4.0/elytra/xbox/peoplehub/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/profile/__init__.py` & `elytra_ms-0.4.0/elytra/xbox/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/profile/models.py` & `elytra_ms-0.4.0/elytra/xbox/profile/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/elytra/xbox/social/__init__.py` & `elytra_ms-0.4.0/elytra/xbox/social/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/.gitignore` & `elytra_ms-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/LICENSE` & `elytra_ms-0.4.0/elytra/xbox/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""
 MIT License
 
 Copyright (c) 2023-2024 AstreaTSS
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -15,7 +16,15 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+"""
+
+from .club import *
+from .core import *
+from .message import *
+from .peoplehub import *
+from .profile import *
+from .social import *
```

### Comparing `elytra_ms-0.3.3/README.md` & `elytra_ms-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/pyproject.toml` & `elytra_ms-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.3.3/PKG-INFO` & `elytra_ms-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: elytra-ms
-Version: 0.3.3
+Version: 0.4.0
 Summary: A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 Project-URL: Homepage, https://github.com/Astrea-Stellarium-Labs/elytra-ms
 Author: AstreaTSS
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AnyIO
```

