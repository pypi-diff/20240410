# Comparing `tmp/lineartest-0.2.1.tar.gz` & `tmp/lineartest-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.2.1.tar", max compression
+gzip compressed data, was "lineartest-0.3.0.tar", max compression
```

## Comparing `lineartest-0.2.1.tar` & `lineartest-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.2.1/LICENSE
--rw-r--r--   0        0        0     2237 2024-04-10 07:28:02.170648 lineartest-0.2.1/README.md
--rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.2.1/lineartest/__init__.py
--rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.2.1/lineartest/_log.py
--rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.2.1/lineartest/_type.py
--rw-r--r--   0        0        0     7263 2024-04-10 07:28:02.171163 lineartest-0.2.1/lineartest/client.py
--rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.2.1/lineartest/schedule.py
--rw-r--r--   0        0        0     1196 2024-04-10 07:28:07.746983 lineartest-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 lineartest-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1963 2024-04-10 17:53:47.920014 lineartest-0.3.0/README.md
+-rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.3.0/lineartest/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.3.0/lineartest/_log.py
+-rw-r--r--   0        0        0     7281 2024-04-10 17:47:38.620517 lineartest-0.3.0/lineartest/client.py
+-rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.3.0/lineartest/schedule.py
+-rw-r--r--   0        0        0     1196 2024-04-10 17:54:53.051198 lineartest-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 lineartest-0.3.0/PKG-INFO
```

### Comparing `lineartest-0.2.1/LICENSE` & `lineartest-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.2.1/README.md` & `lineartest-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,45 +3,29 @@
 
 - **Source code**: https://github.com/fanyf22/lineartest/
 - **Documentation**: https://fanyf22.github.io/lineartest/
 
 ## Dependencies
 
 ```requirements
-# requried
 python>=3.10
 starlette>=0.37.2
 pydantic>=2.6.4
-
-# recommended
-httpx>=0.27.0   # for starlette.testclient
+pyyaml>=6.0.1
+httpx>=0.27.0
 ```
 
 ## Installing
 
 The package is published on https://pypi.org/lineartest.
 
-Use `pip` or `poetry` to install it.
+Use `pip` or similar commands to install it:
 
 ```shell
-# pip
 pip install lineartest
-
-# poetry
-poetry add lineartest
-```
-
-Also, if you are using the `LinearClient` feature, which is based on `starlette.testclient.TestClient`, you may need to install `httpx`:
-
-```shell
-# pip
-pip install httpx
-
-# poetry
-poetry add httpx
 ```
 
 ## Features
 
 - `lineartest.schedule` helps you run tests one-by-one in order, and the tests run later can retrieve the results from the tests run earlier.
 - `lineartest.client` helps you log the detail of a request and the response easily.
```

### Comparing `lineartest-0.2.1/lineartest/_log.py` & `lineartest-0.3.0/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.2.1/lineartest/client.py` & `lineartest-0.3.0/lineartest/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from collections.abc import Mapping
-from typing import IO, Any
+from typing import IO, Any, TypeVar
 
+import httpx
 import yaml
+from pydantic import BaseModel
 from starlette.testclient import TestClient
 
 from ._log import LoggerBase
-from ._type import BaseModelType, DefaultResponse
+
+BaseModelType = TypeVar('BaseModelType', bound=BaseModel)
 
 
 class LinearClient(LoggerBase):
     """The main entrypoint to use LinearTest."""
 
     def __init__(self, test_client: TestClient | None = None):
         """
@@ -34,15 +37,15 @@
         json: Mapping[str, Any] = None,
         headers: Mapping[str, str] | None = None,
         cookies: Mapping[str, str] | None = None,
         follow_redirects: bool | None = None,
         allow_redirects: bool | None = None,
         response_model: type[BaseModelType] | None = None,
         **extra,
-    ) -> BaseModelType | DefaultResponse:
+    ) -> BaseModelType | httpx.Response:
         """
         Perform a request using the `TestClient` instance.
         :param method: the HTTP method to use
         :param url: the URL to request
         :param params: the query parameters to send
         :param data: the form data to send
         :param files: the files to send
@@ -102,46 +105,46 @@
             headers=headers,
             cookies=cookies,
             follow_redirects=follow_redirects,
             allow_redirects=allow_redirects,
             **extra,
         )
 
+        # return if not response model specified
+        if response_model is None:
+            return response
+
         # check if response is JSON
         content_type = response.headers.get('Content-Type')
         error_message = f'expected response type to be "application/json", got {content_type} instead.'
         assert content_type == 'application/json', error_message
         response_dict = response.json()
 
         # log response
         print('<<< Response JSON:')
         self._log(prefix, response_dict)
 
         # log the end of the request
         print(f' REQUEST END: {method} {url} '.center(self.logging_width, '-'))
 
-        # use the default response model if response_model not speficied
-        if response_model is None:
-            response_model = DefaultResponse
-
         # parse the json dictionary to response_model
         return response_model.model_validate(response_dict)
 
     def get(
         self,
         url: str,
         *,
         params: Mapping[str, Any] | None = None,
         headers: Mapping[str, str] | None = None,
         cookies: Mapping[str, str] | None = None,
         follow_redirects: bool | None = None,
         allow_redirects: bool | None = None,
         response_model: type[BaseModelType] | None = None,
         **extra,
-    ) -> BaseModelType | DefaultResponse:
+    ) -> BaseModelType | httpx.Response:
         """
         Perform a GET request using the `TestClient` instance.
         :param url: the URL to request
         :param params: the query parameters to send
         :param headers: the headers to send
         :param cookies: the cookies to send
         :param follow_redirects: whether to follow redirects
@@ -172,15 +175,15 @@
         json: Mapping[str, Any] = None,
         headers: Mapping[str, str] | None = None,
         cookies: Mapping[str, str] | None = None,
         follow_redirects: bool | None = None,
         allow_redirects: bool | None = None,
         response_model: type[BaseModelType] | None = None,
         **extra,
-    ) -> BaseModelType | DefaultResponse:
+    ) -> BaseModelType | httpx.Response:
         """
         Perform a POST request using the `TestClient` instance.
         :param url: the URL to request
         :param params: the query parameters to send
         :param data: the form data to send
         :param files: the files to send
         :param json: the JSON data to send
```

### Comparing `lineartest-0.2.1/lineartest/schedule.py` & `lineartest-0.3.0/lineartest/schedule.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.2.1/pyproject.toml` & `lineartest-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.2.1"
+version = "0.3.0"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -19,22 +19,22 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 starlette = "^0.37.2"
 pydantic = "^2.6.4"
 pyyaml = "^6.0.1"
+httpx = "^0.27.0"
 
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.21.3"
 ruff = "^0.3.5"
 pre-commit = "^3.7.0"
 isort = "^5.13.2"
-httpx = "^0.27.0"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.17"
 
 
 [tool.poetry.group.test.dependencies]
 fastapi = "^0.110.1"
 python-multipart = "^0.0.9"
```

### Comparing `lineartest-0.2.1/PKG-INFO` & `lineartest-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.2.1
+Version: 0.3.0
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,59 +12,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.13
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: starlette (>=0.37.2,<0.38.0)
 Description-Content-Type: text/markdown
 
 # LinearTest
 A testing framework working with Starlette TestClient.
 
 - **Source code**: https://github.com/fanyf22/lineartest/
 - **Documentation**: https://fanyf22.github.io/lineartest/
 
 ## Dependencies
 
 ```requirements
-# requried
 python>=3.10
 starlette>=0.37.2
 pydantic>=2.6.4
-
-# recommended
-httpx>=0.27.0   # for starlette.testclient
+pyyaml>=6.0.1
+httpx>=0.27.0
 ```
 
 ## Installing
 
 The package is published on https://pypi.org/lineartest.
 
-Use `pip` or `poetry` to install it.
+Use `pip` or similar commands to install it:
 
 ```shell
-# pip
 pip install lineartest
-
-# poetry
-poetry add lineartest
-```
-
-Also, if you are using the `LinearClient` feature, which is based on `starlette.testclient.TestClient`, you may need to install `httpx`:
-
-```shell
-# pip
-pip install httpx
-
-# poetry
-poetry add httpx
 ```
 
 ## Features
 
 - `lineartest.schedule` helps you run tests one-by-one in order, and the tests run later can retrieve the results from the tests run earlier.
 - `lineartest.client` helps you log the detail of a request and the response easily.
```

