# Comparing `tmp/Starlette-WTF-0.4.4rc1.tar.gz` & `tmp/Starlette-WTF-0.4.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Starlette-WTF-0.4.4rc1.tar", last modified: Tue Apr  9 06:22:30 2024, max compression
+gzip compressed data, was "Starlette-WTF-0.4.5rc1.tar", last modified: Tue Apr  9 22:00:58 2024, max compression
```

## Comparing `Starlette-WTF-0.4.4rc1.tar` & `Starlette-WTF-0.4.5rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.451796 Starlette-WTF-0.4.4rc1/
--rw-r--r--   0 andres     (501) staff       (20)     1079 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/LICENSE.txt
--rw-r--r--   0 andres     (501) staff       (20)    15024 2024-04-09 06:22:30.451439 Starlette-WTF-0.4.4rc1/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)    14016 2024-04-08 10:13:11.000000 Starlette-WTF-0.4.4rc1/README.md
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.449977 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/
--rw-r--r--   0 andres     (501) staff       (20)    15024 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)      470 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/SOURCES.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/dependency_links.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-08 07:43:57.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/not-zip-safe
--rw-r--r--   0 andres     (501) staff       (20)       85 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/requires.txt
--rw-r--r--   0 andres     (501) staff       (20)       14 2024-04-09 06:22:30.000000 Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/top_level.txt
--rw-r--r--   0 andres     (501) staff       (20)       79 2024-04-09 06:22:30.452557 Starlette-WTF-0.4.4rc1/setup.cfg
--rw-r--r--   0 andres     (501) staff       (20)     1283 2024-04-09 06:22:23.000000 Starlette-WTF-0.4.4rc1/setup.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.447037 Starlette-WTF-0.4.4rc1/starlette_wtf/
--rw-r--r--   0 andres     (501) staff       (20)      293 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/__init__.py
--rw-r--r--   0 andres     (501) staff       (20)     8952 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/csrf.py
--rw-r--r--   0 andres     (501) staff       (20)     6349 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/form.py
--rw-r--r--   0 andres     (501) staff       (20)     5445 2024-04-08 07:42:57.000000 Starlette-WTF-0.4.4rc1/starlette_wtf/util.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 06:22:30.449439 Starlette-WTF-0.4.4rc1/tests/
--rw-r--r--   0 andres     (501) staff       (20)     2971 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_asyncvalidators.py
--rw-r--r--   0 andres     (501) staff       (20)    16461 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_csrf.py
--rw-r--r--   0 andres     (501) staff       (20)     1492 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_customvalidators.py
--rw-r--r--   0 andres     (501) staff       (20)     4679 2024-04-09 05:36:31.000000 Starlette-WTF-0.4.4rc1/tests/test_form.py
--rw-r--r--   0 andres     (501) staff       (20)     5134 2024-04-08 10:33:23.000000 Starlette-WTF-0.4.4rc1/tests/test_util.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 22:00:58.728331 Starlette-WTF-0.4.5rc1/
+-rw-r--r--   0 andres     (501) staff       (20)     1079 2024-04-08 20:52:25.000000 Starlette-WTF-0.4.5rc1/LICENSE.txt
+-rw-r--r--   0 andres     (501) staff       (20)    14942 2024-04-09 22:00:58.727834 Starlette-WTF-0.4.5rc1/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)    14016 2024-04-09 21:02:12.000000 Starlette-WTF-0.4.5rc1/README.md
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 22:00:58.726461 Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/
+-rw-r--r--   0 andres     (501) staff       (20)    14942 2024-04-09 22:00:58.000000 Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)      470 2024-04-09 22:00:58.000000 Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/SOURCES.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-09 22:00:58.000000 Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/dependency_links.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2024-04-08 20:54:49.000000 Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/not-zip-safe
+-rw-r--r--   0 andres     (501) staff       (20)       85 2024-04-09 22:00:58.000000 Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/requires.txt
+-rw-r--r--   0 andres     (501) staff       (20)       14 2024-04-09 22:00:58.000000 Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/top_level.txt
+-rw-r--r--   0 andres     (501) staff       (20)       79 2024-04-09 22:00:58.729109 Starlette-WTF-0.4.5rc1/setup.cfg
+-rw-r--r--   0 andres     (501) staff       (20)     1203 2024-04-09 22:00:13.000000 Starlette-WTF-0.4.5rc1/setup.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 22:00:58.720438 Starlette-WTF-0.4.5rc1/starlette_wtf/
+-rw-r--r--   0 andres     (501) staff       (20)      293 2024-04-08 20:52:25.000000 Starlette-WTF-0.4.5rc1/starlette_wtf/__init__.py
+-rw-r--r--   0 andres     (501) staff       (20)     8945 2024-04-09 21:02:12.000000 Starlette-WTF-0.4.5rc1/starlette_wtf/csrf.py
+-rw-r--r--   0 andres     (501) staff       (20)     6241 2024-04-09 21:59:06.000000 Starlette-WTF-0.4.5rc1/starlette_wtf/form.py
+-rw-r--r--   0 andres     (501) staff       (20)     5445 2024-04-08 20:52:25.000000 Starlette-WTF-0.4.5rc1/starlette_wtf/util.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-04-09 22:00:58.725274 Starlette-WTF-0.4.5rc1/tests/
+-rw-r--r--   0 andres     (501) staff       (20)     4741 2024-04-09 21:59:06.000000 Starlette-WTF-0.4.5rc1/tests/test_asyncvalidators.py
+-rw-r--r--   0 andres     (501) staff       (20)    16461 2024-04-09 21:02:12.000000 Starlette-WTF-0.4.5rc1/tests/test_csrf.py
+-rw-r--r--   0 andres     (501) staff       (20)     1492 2024-04-09 21:02:12.000000 Starlette-WTF-0.4.5rc1/tests/test_customvalidators.py
+-rw-r--r--   0 andres     (501) staff       (20)     5284 2024-04-09 21:59:06.000000 Starlette-WTF-0.4.5rc1/tests/test_form.py
+-rw-r--r--   0 andres     (501) staff       (20)     5134 2024-04-09 21:02:12.000000 Starlette-WTF-0.4.5rc1/tests/test_util.py
```

### Comparing `Starlette-WTF-0.4.4rc1/LICENSE.txt` & `Starlette-WTF-0.4.5rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4rc1/PKG-INFO` & `Starlette-WTF-0.4.5rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: Starlette-WTF
-Version: 0.4.4rc1
+Version: 0.4.5rc1
 Summary: Simple integration of Starlette and WTForms.
-Home-page: https://github.com/muicss/starlette-wtf
+Home-page: https://github.com/kubetail-org/starlette-wtf
 Author: Andres Morey
 License: MIT
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: itsdangerous
 Requires-Dist: python-multipart
 Requires-Dist: starlette
 Requires-Dist: WTForms
```

### Comparing `Starlette-WTF-0.4.4rc1/README.md` & `Starlette-WTF-0.4.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4rc1/Starlette_WTF.egg-info/PKG-INFO` & `Starlette-WTF-0.4.5rc1/Starlette_WTF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: Starlette-WTF
-Version: 0.4.4rc1
+Version: 0.4.5rc1
 Summary: Simple integration of Starlette and WTForms.
-Home-page: https://github.com/muicss/starlette-wtf
+Home-page: https://github.com/kubetail-org/starlette-wtf
 Author: Andres Morey
 License: MIT
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: itsdangerous
 Requires-Dist: python-multipart
 Requires-Dist: starlette
 Requires-Dist: WTForms
```

### Comparing `Starlette-WTF-0.4.4rc1/starlette_wtf/csrf.py` & `Starlette-WTF-0.4.5rc1/starlette_wtf/csrf.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 DEFAULT_CSRF_SSL_STRICT = True
 
 
 class CSRFProtectMiddleware:
     def __init__(self,
                  app: ASGIApp,
                  enabled: bool=DEFAULT_ENABLED,
-                 csrf_secret: Optional[ByteString]=DEFAULT_CSRF_SECRET,
+                 csrf_secret: Optional[str]=DEFAULT_CSRF_SECRET,
                  csrf_field_name: str=DEFAULT_CSRF_FIELD_NAME,
                  csrf_time_limit: int=DEFAULT_CSRF_TIME_LIMIT,
                  csrf_headers: List[str]=DEFAULT_CSRF_HEADERS,
                  csrf_ssl_strict: bool=DEFAULT_CSRF_SSL_STRICT):
         """ASGI Middleware needed by Starlette-WTF to enable CSRF protection.
         
         Args:
```

### Comparing `Starlette-WTF-0.4.4rc1/starlette_wtf/form.py` & `Starlette-WTF-0.4.5rc1/starlette_wtf/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,30 +69,29 @@
               .Request`
           **kwargs: Arbitrary keyword arguments for :class:`starlette.requests
               .Request`
 
         """
         # cache request
         self._request = request
-        
+
         # for WTForms CSRF handling
         if hasattr(request.state, 'csrf_config'):
             config = request.state.csrf_config
             kwargs['meta'] = {
                 'csrf': config['enabled'],
                 'csrf_secret': str(config['csrf_secret']).encode('utf-8'),
                 'csrf_class': config['csrf_class'],
                 'csrf_context': request,
                 'csrf_field_name': config['csrf_field_name'],
                 'csrf_time_limit': config['csrf_time_limit']
             }
 
         super().__init__(*args, **kwargs)
 
-        
     @classmethod
     async def from_formdata(cls, request: StarletteRequest, formdata=_Auto,
                             **kwargs):
         """Method to support initializing class from submitted formdata. If
         request is a POST, PUT, PATCH or DELETE, form will be initialized using
         formdata. Otherwise, it will be initialized using defaults.
 
@@ -107,72 +106,69 @@
         """
         if formdata is _Auto:
             if request.method in SUBMIT_METHODS:
                 # get formdata from request.form() or request.json()
                 formdata = await get_formdata(request)
             else:
                 formdata = None
-            
+
         # return new instance
         return cls(request, formdata=formdata, **kwargs)
 
-    
     async def _validate_async(self, validator, field):
         """Execute async validator
         """
         try:
             await validator(self, field)
         except ValidationError as e:
             field.errors.append(e.args[0])
             return False
         return True
 
-    
     async def validate(self, extra_validators=None):
         """Overload :meth:`validate` to handle custom async validators
         """
         if extra_validators is not None:
             extra = extra_validators.copy()
         else:
             extra = {}
 
         async_validators = {}
-            
+
         # use extra validators to check for StopValidation errors
         completed = []
-        def record_status(form, field):
+
+        def record_status(_, field):
             completed.append(field.name)
-        
+
         for name, field in self._fields.items():
             func = getattr(self.__class__, f"async_validate_{name}", None)
             if func:
-                async_validators[name] = (func, field)
+                async_validators[field.name] = (func, field)
                 extra.setdefault(name, []).append(record_status)
-                
+
         # execute non-async validators
         success = super().validate(extra_validators=extra)
 
         # execute async validators
-        tasks = [self._validate_async(*async_validators[name]) for name in \
+        tasks = [self._validate_async(*async_validators[field_name]) for field_name in
                  completed]
         async_results = await asyncio.gather(*tasks)
 
         # check results
         if False in async_results:
             success = False
-                         
+
         return success
-    
-    
+
     def is_submitted(self):
         """Consider the form submitted if there is an active request and
         the method is ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
         """
         return self._request.method in SUBMIT_METHODS
-    
-        
+
     async def validate_on_submit(self, extra_validators=None):
         """Call :meth:`validate` only if the form is submitted.
         This is a shortcut for ``form.is_submitted() and form.validate()``.
         """
         return self.is_submitted() and \
             await self.validate(extra_validators=extra_validators)
```

### Comparing `Starlette-WTF-0.4.4rc1/starlette_wtf/util.py` & `Starlette-WTF-0.4.5rc1/starlette_wtf/util.py`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4rc1/tests/test_asyncvalidators.py` & `Starlette-WTF-0.4.5rc1/tests/test_asyncvalidators.py`

 * *Files 19% similar despite different names*

```diff
@@ -87,7 +87,63 @@
             assert False
 
         return PlainTextResponse()
 
     app.add_route('/', methods=['POST'], route=index)
 
     client.post('/', data={'field1': 'xxx1', 'field2': 'xxx2'})
+
+
+def test_async_validator_with_prefix_success(app, client, FormWithAsyncValidators):
+    async def index(request):
+        form = await FormWithAsyncValidators.from_formdata(
+            request,
+            prefix="myprefix-",
+        )
+        assert form.field1.data == 'value1'
+        assert form.field2.data == 'value2'
+
+        # validate and check again
+        success = await form.validate()
+        assert success == True
+
+        # check values and errors
+        assert form.field1.data == 'value1'
+        assert 'field1' not in form.errors
+
+        assert form.field2.data == 'value2'
+        assert 'field2' not in form.errors
+
+        return PlainTextResponse()
+
+    app.add_route('/', methods=['POST'], route=index)
+
+    client.post('/', data={'myprefix-field1': 'value1', 'myprefix-field2': 'value2'})
+
+
+def test_async_validator_with_prefix_error(app, client, FormWithAsyncValidators):
+    async def index(request):
+        form = await FormWithAsyncValidators.from_formdata(
+            request,
+            prefix="myprefix-",
+        )
+        assert form.field1.data == 'xxx1'
+        assert form.field2.data == 'xxx2'
+
+        # validate and check again
+        success = await form.validate()
+        assert success == False
+        assert form.field1.data == 'xxx1'
+        assert form.field2.data == 'xxx2'
+
+        # check errors
+        assert len(form.errors['field1']) == 1
+        assert form.errors['field1'][0] == 'Field value is incorrect.'
+
+        assert len(form.errors['field2']) == 1
+        assert form.errors['field2'][0] == 'Field value is incorrect.'
+
+        return PlainTextResponse()
+
+    app.add_route('/', methods=['POST'], route=index)
+
+    client.post('/', data={'myprefix-field1': 'xxx1', 'myprefix-field2': 'xxx2'})
```

### Comparing `Starlette-WTF-0.4.4rc1/tests/test_csrf.py` & `Starlette-WTF-0.4.5rc1/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4rc1/tests/test_customvalidators.py` & `Starlette-WTF-0.4.5rc1/tests/test_customvalidators.py`

 * *Files identical despite different names*

### Comparing `Starlette-WTF-0.4.4rc1/tests/test_form.py` & `Starlette-WTF-0.4.5rc1/tests/test_form.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from io import BytesIO
 
 from starlette.datastructures import ImmutableMultiDict
 from starlette.responses import PlainTextResponse
-from wtforms.widgets import HiddenInput
 
 
 def test_populate_from_get_request(app, client, BasicForm):
     async def index(request):
         form = await BasicForm.from_formdata(request)
         assert form.name.data == None
         assert form.avatar.data == None
@@ -151,7 +150,27 @@
     assert client.get('/').text == 'False'
 
     # test is_submitted() == True and validate() == False
     assert client.post('/').text == 'True'
 
     # test is_submitted() == True and validate() == True
     assert client.post('/', data={'name': 'value'}).text == 'False'
+
+
+def test_validate_form_with_prefix(app, client, BasicForm):
+    async def index(request):
+        form = await BasicForm.from_formdata(
+            request,
+            prefix="myprefix-",
+        )
+
+        if await form.validate_on_submit():
+            assert request.method == 'POST'
+
+        return PlainTextResponse(str('name' in form.errors))
+
+    app.add_route('/', methods=['GET', 'POST'], route=index)
+
+    assert client.get('/').text == 'False'
+    assert client.post('/').text == 'True'
+    assert client.post('/', data={'name': 'value'}).text == 'True'
+    assert client.post('/', data={'myprefix-name': 'value'}).text == 'False'
```

### Comparing `Starlette-WTF-0.4.4rc1/tests/test_util.py` & `Starlette-WTF-0.4.5rc1/tests/test_util.py`

 * *Files identical despite different names*

