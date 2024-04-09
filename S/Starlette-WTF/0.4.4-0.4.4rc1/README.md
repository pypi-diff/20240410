# Comparing `tmp/Starlette-WTF-0.4.4.tar.gz` & `tmp/Starlette-WTF-0.4.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Starlette-WTF-0.4.4.tar", last modified: Tue Apr  9 07:46:02 2024, max compression
+gzip compressed data, was "Starlette-WTF-0.4.4rc1.tar", last modified: Tue Apr  9 06:22:30 2024, max compression
```

## Comparing `Starlette-WTF-0.4.4.tar` & `Starlette-WTF-0.4.4rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 07:46:02.640000 Starlette-WTF-0.4.4/
--rw-r--r--   0 andres     (501) staff       (20)     1079 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4/LICENSE.txt
--rw-r--r--   0 andres     (501) staff       (20)    14939 2024-04-09 07:46:02.639418 Starlette-WTF-0.4.4/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)    14016 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/README.md
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 07:46:02.637687 Starlette-WTF-0.4.4/Starlette_WTF.egg-info/
--rw-r--r--   0 andres     (501) staff       (20)    14939 2024-04-09 07:46:02.000000 Starlette-WTF-0.4.4/Starlette_WTF.egg-info/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)      470 2024-04-09 07:46:02.000000 Starlette-WTF-0.4.4/Starlette_WTF.egg-info/SOURCES.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-09 07:46:02.000000 Starlette-WTF-0.4.4/Starlette_WTF.egg-info/dependency_links.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-08 07:43:57.000000 Starlette-WTF-0.4.4/Starlette_WTF.egg-info/not-zip-safe
--rw-r--r--   0 andres     (501) staff       (20)       85 2024-04-09 07:46:02.000000 Starlette-WTF-0.4.4/Starlette_WTF.egg-info/requires.txt
--rw-r--r--   0 andres     (501) staff       (20)       14 2024-04-09 07:46:02.000000 Starlette-WTF-0.4.4/Starlette_WTF.egg-info/top_level.txt
--rw-r--r--   0 andres     (501) staff       (20)       79 2024-04-09 07:46:02.640773 Starlette-WTF-0.4.4/setup.cfg
--rw-r--r--   0 andres     (501) staff       (20)     1199 2024-04-09 07:44:24.000000 Starlette-WTF-0.4.4/setup.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 07:46:02.634705 Starlette-WTF-0.4.4/starlette_wtf/
--rw-r--r--   0 andres     (501) staff       (20)      293 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4/starlette_wtf/__init__.py
--rw-r--r--   0 andres     (501) staff       (20)     8945 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/starlette_wtf/csrf.py
--rw-r--r--   0 andres     (501) staff       (20)     6364 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/starlette_wtf/form.py
--rw-r--r--   0 andres     (501) staff       (20)     5445 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4/starlette_wtf/util.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 07:46:02.637067 Starlette-WTF-0.4.4/tests/
--rw-r--r--   0 andres     (501) staff       (20)     2971 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/tests/test_asyncvalidators.py
--rw-r--r--   0 andres     (501) staff       (20)    16461 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/tests/test_csrf.py
--rw-r--r--   0 andres     (501) staff       (20)     1492 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/tests/test_customvalidators.py
--rw-r--r--   0 andres     (501) staff       (20)     5009 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/tests/test_form.py
--rw-r--r--   0 andres     (501) staff       (20)     5134 2024-04-09 07:41:08.000000 Starlette-WTF-0.4.4/tests/test_util.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.451796 Starlette-WTF-0.4.4rc1/
+-rw-r--r--   0 andres     (501) staff       (20)     1079 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/LICENSE.txt
+-rw-r--r--   0 andres     (501) staff       (20)    15024 2024-04-09 06:22:30.451439 Starlette-WTF-0.4.4rc1/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)    14016 2024-04-08 10:13:11.000000 Starlette-WTF-0.4.4rc1/README.md
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.449977 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/
+-rw-r--r--   0 andres     (501) staff       (20)    15024 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)      470 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/SOURCES.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/dependency_links.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-08 07:43:57.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/not-zip-safe
+-rw-r--r--   0 andres     (501) staff       (20)       85 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/requires.txt
+-rw-r--r--   0 andres     (501) staff       (20)       14 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/top_level.txt
+-rw-r--r--   0 andres     (501) staff       (20)       79 2024-04-09 06:22:30.452557 Starlette-WTF-0.4.4rc1/setup.cfg
+-rw-r--r--   0 andres     (501) staff       (20)     1283 2024-04-09 06:22:23.000000 Starlette-WTF-0.4.4rc1/setup.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.447037 Starlette-WTF-0.4.4rc1/starlette_wtf/
+-rw-r--r--   0 andres     (501) staff       (20)      293 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/__init__.py
+-rw-r--r--   0 andres     (501) staff       (20)     8952 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/csrf.py
+-rw-r--r--   0 andres     (501) staff       (20)     6349 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/form.py
+-rw-r--r--   0 andres     (501) staff       (20)     5445 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/util.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.449439 Starlette-WTF-0.4.4rc1/tests/
+-rw-r--r--   0 andres     (501) staff       (20)     2971 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_asyncvalidators.py
+-rw-r--r--   0 andres     (501) staff       (20)    16461 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_csrf.py
+-rw-r--r--   0 andres     (501) staff       (20)     1492 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_customvalidators.py
+-rw-r--r--   0 andres     (501) staff       (20)     4679 2024-04-09 05:36:31.000000 Starlette-WTF-0.4.4rc1/tests/test_form.py
+-rw-r--r--   0 andres     (501) staff       (20)     5134 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_util.py
```

### Comparing `Starlette-WTF-0.4.4/LICENSE.txt` & `Starlette-WTF-0.4.4rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4/PKG-INFO` & `Starlette-WTF-0.4.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: Starlette-WTF
-Version: 0.4.4
+Version: 0.4.4rc1
 Summary: Simple integration of Starlette and WTForms.
-Home-page: https://github.com/kubetail-org/starlette-wtf
+Home-page: https://github.com/muicss/starlette-wtf
 Author: Andres Morey
 License: MIT
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: itsdangerous
 Requires-Dist: python-multipart
 Requires-Dist: starlette
 Requires-Dist: WTForms
```

### Comparing `Starlette-WTF-0.4.4/README.md` & `Starlette-WTF-0.4.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4/Starlette_WTF.egg-info/PKG-INFO` & `Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: Starlette-WTF
-Version: 0.4.4
+Version: 0.4.4rc1
 Summary: Simple integration of Starlette and WTForms.
-Home-page: https://github.com/kubetail-org/starlette-wtf
+Home-page: https://github.com/muicss/starlette-wtf
 Author: Andres Morey
 License: MIT
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: itsdangerous
 Requires-Dist: python-multipart
 Requires-Dist: starlette
 Requires-Dist: WTForms
```

### Comparing `Starlette-WTF-0.4.4/starlette_wtf/csrf.py` & `Starlette-WTF-0.4.4rc1/starlette_wtf/csrf.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 DEFAULT_CSRF_SSL_STRICT = True
 
 
 class CSRFProtectMiddleware:
     def __init__(self,
                  app: ASGIApp,
                  enabled: bool=DEFAULT_ENABLED,
-                 csrf_secret: Optional[str]=DEFAULT_CSRF_SECRET,
+                 csrf_secret: Optional[ByteString]=DEFAULT_CSRF_SECRET,
                  csrf_field_name: str=DEFAULT_CSRF_FIELD_NAME,
                  csrf_time_limit: int=DEFAULT_CSRF_TIME_LIMIT,
                  csrf_headers: List[str]=DEFAULT_CSRF_HEADERS,
                  csrf_ssl_strict: bool=DEFAULT_CSRF_SSL_STRICT):
         """ASGI Middleware needed by Starlette-WTF to enable CSRF protection.
         
         Args:
```

### Comparing `Starlette-WTF-0.4.4/starlette_wtf/form.py` & `Starlette-WTF-0.4.4rc1/starlette_wtf/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             extra = {}
 
         async_validators = {}
             
         # use extra validators to check for StopValidation errors
         completed = []
         def record_status(form, field):
-            completed.append(form._prefix + field.name)
+            completed.append(field.name)
         
         for name, field in self._fields.items():
             func = getattr(self.__class__, f"async_validate_{name}", None)
             if func:
                 async_validators[name] = (func, field)
                 extra.setdefault(name, []).append(record_status)
```

### Comparing `Starlette-WTF-0.4.4/starlette_wtf/util.py` & `Starlette-WTF-0.4.4rc1/starlette_wtf/util.py`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4/tests/test_asyncvalidators.py` & `Starlette-WTF-0.4.4rc1/tests/test_asyncvalidators.py`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4/tests/test_csrf.py` & `Starlette-WTF-0.4.4rc1/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4/tests/test_customvalidators.py` & `Starlette-WTF-0.4.4rc1/tests/test_customvalidators.py`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4/tests/test_form.py` & `Starlette-WTF-0.4.4rc1/tests/test_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from io import BytesIO
 
 from starlette.datastructures import ImmutableMultiDict
 from starlette.responses import PlainTextResponse
+from wtforms.widgets import HiddenInput
 
 
 def test_populate_from_get_request(app, client, BasicForm):
     async def index(request):
         form = await BasicForm.from_formdata(request)
         assert form.name.data == None
         assert form.avatar.data == None
@@ -150,21 +151,7 @@
     assert client.get('/').text == 'False'
 
     # test is_submitted() == True and validate() == False
     assert client.post('/').text == 'True'
 
     # test is_submitted() == True and validate() == True
     assert client.post('/', data={'name': 'value'}).text == 'False'
-
-
-def test_form_with_prefix(app, client, BasicForm):
-    async def index(request):
-        form = await BasicForm.from_formdata(
-            request,
-            prefix="myprefix-",
-        )
-        assert form.name.data == 'x'
-        return PlainTextResponse()
-
-    app.add_route('/', methods=['POST'], route=index)
-
-    client.post('/', data={'myprefix-name': 'x'})
```

### Comparing `Starlette-WTF-0.4.4/tests/test_util.py` & `Starlette-WTF-0.4.4rc1/tests/test_util.py`

 * *Files identical despite different names*

