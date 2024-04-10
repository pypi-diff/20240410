# Comparing `tmp/lineartest-0.1.2.tar.gz` & `tmp/lineartest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.1.2.tar", max compression
+gzip compressed data, was "lineartest-0.2.0.tar", max compression
```

## Comparing `lineartest-0.1.2.tar` & `lineartest-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.1.2/LICENSE
--rw-r--r--   0        0        0     2245 2024-04-09 02:47:37.099907 lineartest-0.1.2/README.md
--rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.1.2/lineartest/__init__.py
--rw-r--r--   0        0        0     1436 2024-04-08 09:41:54.891450 lineartest-0.1.2/lineartest/_log.py
--rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.1.2/lineartest/_type.py
--rw-r--r--   0        0        0     7650 2024-04-09 03:36:09.904701 lineartest-0.1.2/lineartest/client.py
--rw-r--r--   0        0        0     6291 2024-04-08 09:41:54.892408 lineartest-0.1.2/lineartest/schedule.py
--rw-r--r--   0        0        0     1178 2024-04-09 03:36:09.905046 lineartest-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 lineartest-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2237 2024-04-10 01:04:34.122025 lineartest-0.2.0/README.md
+-rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.2.0/lineartest/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-10 00:55:49.307063 lineartest-0.2.0/lineartest/_log.py
+-rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.2.0/lineartest/_type.py
+-rw-r--r--   0        0        0     7255 2024-04-10 00:57:52.049261 lineartest-0.2.0/lineartest/client.py
+-rw-r--r--   0        0        0     6288 2024-04-10 01:00:18.116728 lineartest-0.2.0/lineartest/schedule.py
+-rw-r--r--   0        0        0     1196 2024-04-10 01:03:55.785942 lineartest-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 lineartest-0.2.0/PKG-INFO
```

### Comparing `lineartest-0.1.2/LICENSE` & `lineartest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.2/README.md` & `lineartest-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # recommended
 httpx>=0.27.0   # for starlette.testclient
 ```
 
 ## Installing
 
-The package is published on https://pypi.org/project/lineartest.
+The package is published on https://pypi.org/lineartest.
 
 Use `pip` or `poetry` to install it.
 
 ```shell
 # pip
 pip install lineartest
```

### Comparing `lineartest-0.1.2/lineartest/client.py` & `lineartest-0.2.0/lineartest/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from collections.abc import Callable, Mapping
+from collections.abc import Mapping
 from typing import IO, Any
 
+import yaml
 from starlette.testclient import TestClient
 
 from ._log import LoggerBase
 from ._type import BaseModelType, DefaultResponse
 
 
 class LinearClient(LoggerBase):
@@ -14,24 +15,17 @@
         """
         Initialize the `LinearClient` instance.
         :param test_client: the Starlette TestClient instance
         """
         super().__init__()
         self.test_client = test_client
 
-    def _log(self, func: Callable, prefix: str, dct: dict[str, Any]):
-        def inner(prefix: str, dct: dict[str, Any]):
-            for key, value in dct.items():
-                if isinstance(value, dict):
-                    func(f'{prefix}{key}:')
-                    inner(prefix + '  ', value)
-                else:
-                    func(f'{prefix}{key}={value!r}')
-
-        inner(prefix, dct)
+    def _log(self, prefix: str, dct: dict[str, Any]):
+        for line in yaml.dump(dct).split('\n'):
+            print(prefix, line, sep='')
 
     def request(
         self,
         method: str,
         url: str,
         *,
         params: Mapping[str, Any] | None = None,
@@ -58,50 +52,48 @@
         :param follow_redirects: whether to follow redirects
         :param allow_redirects: whether to allow redirects
         :param response_model: the Pydantic model to validate the response
         :param extra: extra arguments to pass to the `TestClient` request method
         :return: the parsed response data in the type of given model or a default one
         """
         # log the start of the request
-        self.info(f' REQUEST START: {method} {url} '.center(self.logging_width, '-'))
+        print(f' REQUEST START: {method} {url} '.center(self.logging_width, '-'))
 
         # log prefix
         prefix = '------+ '
 
         # log params
         if params:
-            self.info('>>> Request params:')
-            self._log(self.info, prefix, params)
+            print('>>> Request params:')
+            self._log(prefix, params)
 
         # log data
         if data:
-            self.info('>>> Request data:')
-            self._log(self.info, prefix, data)
+            print('>>> Request data:')
+            self._log(prefix, data)
 
         # log files
         if files:
-            self.info('>>> Request files:')
-            self._log(
-                self.info, prefix, {key: file.name for key, file in files.items()}
-            )
+            print('>>> Request files:')
+            self._log(prefix, {key: file.name for key, file in files.items()})
 
         # log json
         if json:
             self.info('>>> Request JSON:')
-            self._log(self.info, prefix, json)
+            self._log(prefix, json)
 
         # log headers
         if headers:
-            self.info('>>> Request headers:')
-            self._log(self.info, prefix, headers)
+            print('>>> Request headers:')
+            self._log(prefix, headers)
 
         # log cookies
         if cookies:
-            self.info('>>> Request cookies:')
-            self._log(self.info, prefix, cookies)
+            print('>>> Request cookies:')
+            self._log(prefix, cookies)
 
         # use TestClient to perform the request
         response = self.test_client.request(
             method,
             url,
             params=params,
             data=data,
@@ -117,26 +109,26 @@
         # check if response is JSON
         content_type = response.headers.get('Content-Type')
         error_message = f'expected response type to be "application/json", got {content_type} instead.'
         assert content_type == 'application/json', error_message
         response_dict = response.json()
 
         # log response
-        self.info('<<< Response JSON:')
-        self._log(self.info, prefix, response_dict)
+        print('<<< Response JSON:')
+        self._log(prefix, response_dict)
 
         # log the end of the request
-        self.info(f' REQUEST END: {method} {url} '.center(self.logging_width, '-'))
+        print(f' REQUEST END: {method} {url} '.center(self.logging_width, '-'))
 
         # use the default response model if response_model not speficied
         if response_model is None:
             response_model = DefaultResponse
 
         # parse the json dictionary to response_model
-        return response_model.parse_obj(response_dict)
+        return response_model.model_validate(response_dict)
 
     def get(
         self,
         url: str,
         *,
         params: Mapping[str, Any] | None = None,
         headers: Mapping[str, str] | None = None,
```

### Comparing `lineartest-0.1.2/lineartest/schedule.py` & `lineartest-0.2.0/lineartest/schedule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import sys
 import traceback
 from collections.abc import Callable
 from typing import Annotated, Any, ParamSpec, TypeVar, get_args, get_origin
 
 from ._log import LoggerBase
 
 P = ParamSpec('P')
@@ -131,39 +132,39 @@
         :return: whether the schedules are executed successfully
         """
         total = len(self._schedule)
         success = True
 
         for index, func in enumerate(self._schedule):
             # log the start of the schedule
-            self.info(
+            print(
                 f' SCHEDULE START ({index+1}/{total}): {func.__name__} '.center(
                     self.logging_width, '='
                 )
             )
 
             # execute the schedule
             try:
                 self._exec(func, *args, **kwargs)
             except Exception as e:
-                self.info('')
-                self.info(
+                print()
+                print(
                     f' ERROR: {e.__class__.__name__} '.center(self.logging_width, '-')
                 )
-                self.error(traceback.format_exc())
-                self.info(
+                print(traceback.format_exc(), file=sys.stderr)
+                print(
                     f' SCHEDULE ABORT ({index+1}/{total}): {func.__name__} '.center(
                         self.logging_width, '='
                     )
                 )
                 success = False
                 break
 
             # log the end of the schedule
-            self.info(
+            print(
                 f' SCHEDULE END ({index+1}/{total}): {func.__name__} '.center(
                     self.logging_width, '='
                 )
             )
-            self.info('')
+            print('')
 
         return success
```

### Comparing `lineartest-0.1.2/pyproject.toml` & `lineartest-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.1.2"
+version = "0.2.0"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -18,14 +18,15 @@
     "Programming Language :: Python :: 3.13"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 starlette = "^0.37.2"
 pydantic = "^2.6.4"
+pyyaml = "^6.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.21.3"
 ruff = "^0.3.5"
 pre-commit = "^3.7.0"
 isort = "^5.13.2"
```

### Comparing `lineartest-0.1.2/PKG-INFO` & `lineartest-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.1.2
+Version: 0.2.0
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.13
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: starlette (>=0.37.2,<0.38.0)
 Description-Content-Type: text/markdown
 
 # LinearTest
 A testing framework working with Starlette TestClient.
 
 - **Source code**: https://github.com/fanyf22/lineartest/
@@ -36,15 +37,15 @@
 
 # recommended
 httpx>=0.27.0   # for starlette.testclient
 ```
 
 ## Installing
 
-The package is published on https://pypi.org/project/lineartest.
+The package is published on https://pypi.org/lineartest.
 
 Use `pip` or `poetry` to install it.
 
 ```shell
 # pip
 pip install lineartest
```

