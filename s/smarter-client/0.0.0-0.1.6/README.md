# Comparing `tmp/smarter_client-0.0.0.tar.gz` & `tmp/smarter_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarter_client-0.0.0.tar", last modified: Wed Apr 10 02:14:24 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `smarter_client-0.0.0.tar` & `smarter_client-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,30 @@
--rw-r--r--   0        0        0     1070 2024-04-10 02:13:50.488636 smarter_client-0.0.0/LICENSE
--rw-r--r--   0        0        0     1165 2024-04-10 02:13:50.488636 smarter_client-0.0.0/README.md
--rw-r--r--   0        0        0     1360 2024-04-10 02:14:24.788866 smarter_client-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 02:13:50.492636 smarter_client-0.0.0/src/smarter_kettle_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 02:13:50.492636 smarter_client-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3694 2024-04-10 02:13:50.492636 smarter_client-0.0.0/tests/dict_util_test.py
--rw-r--r--   0        0        0        0 2024-04-10 02:13:50.492636 smarter_client-0.0.0/tests/domain/__init__.py
--rw-r--r--   0        0        0     3644 2024-04-10 02:13:50.492636 smarter_client-0.0.0/tests/domain/models_test.py
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 smarter_client-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 smarter_client-0.1.6/.pylintrc
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 smarter_client-0.1.6/conftest.py
+-rw-r--r--   0        0        0    52843 2020-02-02 00:00:00.000000 smarter_client-0.1.6/pdm.lock
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 smarter_client-0.1.6/requirements.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 smarter_client-0.1.6/setup.cfg
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 smarter_client-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 smarter_client-0.1.6/.vscode/launch.json
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 smarter_client-0.1.6/.vscode/settings.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/_consts.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/dict_util.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/version.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/domain/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/domain/identity_toolkit_client.py
+-rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/domain/models.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/domain/smarter_client.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/domain/decorators/session.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/managed_devices/__init__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/managed_devices/base.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 smarter_client-0.1.6/smarter_client/managed_devices/kettle_v3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.6/src/smarter_kettle_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 smarter_client-0.1.6/tests/dict_util_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.6/tests/domain/__init__.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 smarter_client-0.1.6/tests/domain/models_test.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 smarter_client-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 smarter_client-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 smarter_client-0.1.6/README.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 smarter_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 smarter_client-0.1.6/PKG-INFO
```

### Comparing `smarter_client-0.0.0/LICENSE` & `smarter_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `smarter_client-0.0.0/README.md` & `smarter_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `smarter_client-0.0.0/pyproject.toml` & `smarter_client-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,55 @@
-[project]
-name = "smarter-client"
-description = "Smarter Kettle client library"
-authors = [
-    { name = "Kirill Birger", email = "kbirger@gmail.com" },
-    { name = "@kbirger" },
-]
-dependencies = [
-    "astroid==3.1.0",
-    "pylint==3.1.0",
-    "pytest>=6.2.0",
-    "pytest-cov>=2.4.0",
-    "pytest-localserver>=0.4.1",
-    "pytest-asyncio>=0.16.0",
-    "pytest-mock>=3.6.1",
-    "aiohttp>=3.9.3",
-    "pyrebase4==4.7.1",
-    "setuptools>=69.2.0",
-]
-dynamic = []
-requires-python = ">=3.12.2"
-readme = "README.md"
-keywords = [
-    "smarter kettle python",
-]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.12",
-]
-version = "0.0.0"
-
-[project.license]
-text = "MIT"
-
-[project.urls]
-Homepage = "https://www.github.com/kbirger/smarter-kettle-client"
-"Release Notes" = "https://www.github.com/kbirger/smarter-kettle-client"
-Source = "https://www.github.com/kbirger/smarter-kettle-client"
-
-[tool.pdm]
-distribution = false
-
-[tool.pdm.dev-dependencies]
-testing = [
-    "pytest>=6.2.0",
-    "pytest-cov>=2.4.0",
-    "pytest-localserver>=0.4.1",
-    "pytest-asyncio>=0.16.0",
-    "pytest-mock>=3.6.1",
-]
-build = [
-    "build",
-]
-
-[tool.hatch.version]
-path = "smarter_kettle_client/version.py"
-
-[build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
+[project]
+name = "smarter-client"
+description = "Smarter Kettle client library"
+authors = [
+    { name = "Kirill Birger", email = "kbirger@gmail.com" },
+    { name = "@kbirger" },
+]
+dependencies = [
+    "astroid==3.1.0",
+    "pylint==3.1.0",
+    "pytest>=6.2.0",
+    "pytest-cov>=2.4.0",
+    "pytest-localserver>=0.4.1",
+    "pytest-asyncio>=0.16.0",
+    "pytest-mock>=3.6.1",
+    "aiohttp>=3.9.3",
+    "pyrebase4==4.7.1",
+    "setuptools>=69.2.0",
+]
+dynamic = ['version']
+requires-python = ">=3.12.2"
+readme = "README.md"
+license = { text = "MIT" }
+keywords = ["smarter kettle python"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.12",
+]
+[tool.pdm]
+distribution = false
+
+[tool.hatch.version]
+path = 'smarter_client/version.py'
+
+[tool.pdm.dev-dependencies]
+testing = [
+    "pytest>=6.2.0",
+    "pytest-cov>=2.4.0",
+    "pytest-localserver>=0.4.1",
+    "pytest-asyncio>=0.16.0",
+    "pytest-mock>=3.6.1",
+]
+
+
+build = ["build"]
+
+[project.urls]
+Homepage = "https://www.github.com/kbirger/smarter-kettle-client"
+"Release Notes" = "https://www.github.com/kbirger/smarter-kettle-client"
+Source = "https://www.github.com/kbirger/smarter-kettle-client"
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

### Comparing `smarter_client-0.0.0/tests/dict_util_test.py` & `smarter_client-0.1.6/tests/dict_util_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 from typing import Generator
 import pytest
-from smarter_kettle_client.dict_util import delete_dict, patch_dict, put_dict
+from smarter_client.dict_util import delete_dict, patch_dict, put_dict
 
 
 @pytest.fixture()
 def original_state() -> Generator[dict, None, None]:
     yield {
         'commands': {
             'test_command': {
```

### Comparing `smarter_client-0.0.0/tests/domain/models_test.py` & `smarter_client-0.1.6/tests/domain/models_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 import pytest_mock
 
 
 import sys
 import types
 
-from smarter_kettle_client.domain.models import Command, CommandInstance, Commands, LoginSession
+from smarter_client.domain.models import Command, CommandInstance, Commands, LoginSession
 
 
 # module_name = 'smarter_client'
 # bogus_module = types.ModuleType(module_name)
 # sys.modules[module_name] = bogus_module
 # bogus_module.SmarterClient = MagicMock(name=module_name+'.SmarterClient')
 # SmarterClient
```

### Comparing `smarter_client-0.0.0/PKG-INFO` & `smarter_client-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: smarter-client
-Version: 0.0.0
+Version: 0.1.6
 Summary: Smarter Kettle client library
-Keywords: smarter kettle python
+Project-URL: Homepage, https://www.github.com/kbirger/smarter-kettle-client
+Project-URL: Release Notes, https://www.github.com/kbirger/smarter-kettle-client
+Project-URL: Source, https://www.github.com/kbirger/smarter-kettle-client
 Author: @kbirger
-Author-Email: Kirill Birger <kbirger@gmail.com>
+Author-email: Kirill Birger <kbirger@gmail.com>
 License: MIT
+License-File: LICENSE
+Keywords: smarter kettle python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Project-URL: Homepage, https://www.github.com/kbirger/smarter-kettle-client
-Project-URL: Release notes, https://www.github.com/kbirger/smarter-kettle-client
-Project-URL: Source, https://www.github.com/kbirger/smarter-kettle-client
 Requires-Python: >=3.12.2
+Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: astroid==3.1.0
 Requires-Dist: pylint==3.1.0
-Requires-Dist: pytest>=6.2.0
+Requires-Dist: pyrebase4==4.7.1
+Requires-Dist: pytest-asyncio>=0.16.0
 Requires-Dist: pytest-cov>=2.4.0
 Requires-Dist: pytest-localserver>=0.4.1
-Requires-Dist: pytest-asyncio>=0.16.0
 Requires-Dist: pytest-mock>=3.6.1
-Requires-Dist: aiohttp>=3.9.3
-Requires-Dist: pyrebase4==4.7.1
+Requires-Dist: pytest>=6.2.0
 Requires-Dist: setuptools>=69.2.0
 Description-Content-Type: text/markdown
 
 # smarter-kettle-client
 Python client for Smarter Kettle integration
 
 [![CI](https://github.com/kbirger/smarter-kettle-client/actions/workflows/ci.yml/badge.svg)](https://github.com/kbirger/smarter-kettle-client/actions/workflows/ci.yml)
```

