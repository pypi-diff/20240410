# Comparing `tmp/pyegeria-0.3.2.tar.gz` & `tmp/pyegeria-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegeria-0.3.2.tar", last modified: Tue Apr  9 02:29:41 2024, max compression
+gzip compressed data, was "pyegeria-0.3.3.tar", last modified: Wed Apr 10 02:48:17 2024, max compression
```

## Comparing `pyegeria-0.3.2.tar` & `pyegeria-0.3.3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 02:29:41.843562 pyegeria-0.3.2/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-02-13 19:55:10.000000 pyegeria-0.3.2/LICENSE
--rw-r--r--   0 dwolfson   (501) staff       (20)        0 2024-02-13 19:55:10.000000 pyegeria-0.3.2/MANIFEST.in
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-09 02:29:41.843375 pyegeria-0.3.2/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-09 02:21:44.000000 pyegeria-0.3.2/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)     1016 2024-04-09 02:29:05.000000 pyegeria-0.3.2/pyproject.toml
--rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-09 02:29:41.843603 pyegeria-0.3.2/setup.cfg
--rw-r--r--   0 dwolfson   (501) staff       (20)     1165 2024-04-09 02:29:05.000000 pyegeria-0.3.2/setup.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 02:29:41.838132 pyegeria-0.3.2/src/
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 02:29:41.840702 pyegeria-0.3.2/src/pyegeria/
--rw-r--r--   0 dwolfson   (501) staff       (20)     1601 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/_exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-02-09 22:22:39.000000 pyegeria-0.3.2/src/pyegeria/_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/_validators.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    99125 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    93697 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    46147 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    35897 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    19930 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6272 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/governance_author.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    42436 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    43011 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     7502 2024-03-18 16:53:12.000000 pyegeria-0.3.2/src/pyegeria/registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    16273 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-09 02:21:44.000000 pyegeria-0.3.2/src/pyegeria/utils.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 02:29:41.843074 pyegeria-0.3.2/src/pyegeria.egg-info/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-09 02:29:41.000000 pyegeria-0.3.2/src/pyegeria.egg-info/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1130 2024-04-09 02:29:41.000000 pyegeria-0.3.2/src/pyegeria.egg-info/SOURCES.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-09 02:29:41.000000 pyegeria-0.3.2/src/pyegeria.egg-info/dependency_links.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-09 02:29:41.000000 pyegeria-0.3.2/src/pyegeria.egg-info/requires.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-09 02:29:41.000000 pyegeria-0.3.2/src/pyegeria.egg-info/top_level.txt
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 02:29:41.842882 pyegeria-0.3.2/tests/
--rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_automated_curation_omvs_cray.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     9624 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    40009 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3836 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_util_exp.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-09 02:21:44.000000 pyegeria-0.3.2/tests/test_validators.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.292011 pyegeria-0.3.3/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-02-13 19:55:10.000000 pyegeria-0.3.3/LICENSE
+-rw-r--r--   0 dwolfson   (501) staff       (20)        0 2024-02-13 19:55:10.000000 pyegeria-0.3.3/MANIFEST.in
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-10 02:48:17.291821 pyegeria-0.3.3/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-09 02:21:44.000000 pyegeria-0.3.3/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1016 2024-04-09 22:07:39.000000 pyegeria-0.3.3/pyproject.toml
+-rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-10 02:48:17.292048 pyegeria-0.3.3/setup.cfg
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1165 2024-04-09 22:07:39.000000 pyegeria-0.3.3/setup.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.279264 pyegeria-0.3.3/src/
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.287207 pyegeria-0.3.3/src/pyegeria/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1612 2024-04-09 21:54:17.000000 pyegeria-0.3.3/src/pyegeria/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/_exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-02-09 22:22:39.000000 pyegeria-0.3.3/src/pyegeria/_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/_validators.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    99769 2024-04-09 12:36:45.000000 pyegeria-0.3.3/src/pyegeria/automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    93697 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-09 15:45:59.000000 pyegeria-0.3.3/src/pyegeria/exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    46147 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    35897 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    19930 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6272 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/governance_author.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42436 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    43011 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8713 2024-04-09 22:07:10.000000 pyegeria-0.3.3/src/pyegeria/registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    16273 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/utils.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.291543 pyegeria-0.3.3/src/pyegeria.egg-info/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1157 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/SOURCES.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/dependency_links.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/requires.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/top_level.txt
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.291317 pyegeria-0.3.3/tests/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_automated_curation_omvs_cray.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-09 20:58:51.000000 pyegeria-0.3.3/tests/test_core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     9624 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    40009 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4728 2024-04-09 21:23:08.000000 pyegeria-0.3.3/tests/test_registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_util_exp.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_validators.py
```

### Comparing `pyegeria-0.3.2/LICENSE` & `pyegeria-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/PKG-INFO` & `pyegeria-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.2/README.md` & `pyegeria-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/pyproject.toml` & `pyegeria-0.3.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #requires = ["hatchling"]
 requires = ["setuptools", "wheel"]
 #build-backend = "hatchling.build"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyegeria"
-version = "0.3.2"
+version = "0.3.3"
 #license = 'Apache 2.0'
 authors = [
     {name ="Dan Wolfson", email= "dan.wolfson@pdr-associates.com"},
 ]
 description = "A python client for Egeria"
 readme= "README.md"
 requires-python = ">=3.10"
```

### Comparing `pyegeria-0.3.2/setup.py` & `pyegeria-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pyegeria',
     extras_require=dict(tests=["pytest"]),
     # packages=find_packages(where="src"),
     package_dir={"": "src"},
-    version='0.3.2',
+    version='0.3.3',
     packages=find_packages(where="src"),
     url="https://egeria-project.org/egeria-python",
     project_urls={
         "Issues": "https://github.com/odpi/egeria-python/issues",
     },
     #license='Apache 2.0',
     author='Dan Wolfson',
```

### Comparing `pyegeria-0.3.2/src/pyegeria/__init__.py` & `pyegeria-0.3.3/src/pyegeria/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 if disable_ssl_warnings:
     from urllib3.exceptions import InsecureRequestWarning
     from urllib3 import disable_warnings
     disable_warnings(InsecureRequestWarning)
 
 from ._exceptions import (InvalidParameterException, PropertyServerException, UserNotAuthorizedException,
                           print_exception_response)
-from .utils import print_response, body_slimmer
+from .utils import print_response, body_slimmer, wrap_text
 from ._client import Client
 from .automated_curation_omvs import AutomatedCuration
 from .core_omag_server_config import CoreServerConfig
 from .platform_services import Platform
 from .registered_info import RegisteredInfo
 from .glossary_omvs import GlossaryBrowser
 from ._validators import (validate_user_id, validate_name, validate_guid, validate_server_name, validate_search_string,
```

### Comparing `pyegeria-0.3.2/src/pyegeria/_client.py` & `pyegeria-0.3.3/src/pyegeria/_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/_exceptions.py` & `pyegeria-0.3.3/src/pyegeria/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/_globals.py` & `pyegeria-0.3.3/src/pyegeria/_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/_validators.py` & `pyegeria-0.3.3/src/pyegeria/_validators.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/automated_curation_omvs.py` & `pyegeria-0.3.3/src/pyegeria/automated_curation_omvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
  Automated Curation View Service Methods - this file is in active development...
 
 """
 import asyncio
-import json
 from datetime import datetime
-from httpx import AsyncClient, Response
+
+from httpx import Response
 
 from pyegeria import Client, max_paging_size, body_slimmer
-from ._validators import validate_name, validate_guid, validate_search_string
 from pyegeria._exceptions import (
     InvalidParameterException,
 )
+from ._validators import validate_name, validate_guid, validate_search_string
 
 
 class AutomatedCuration(Client):
     """ Set up and maintain automation services in Egeria.
     class AutomatedCuration(Platform):
 
         def __init__(
@@ -88,15 +88,15 @@
                 }
                 """
 
         server = self.server_name if server is None else server
 
         url = f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/catalog-templates/new-element"
         response = await self._async_make_request("POST", url, body)
-        return response.json().get("guid","GUID failed to be returned")
+        return response.json().get("guid", "GUID failed to be returned")
 
     def create_element_from_template(self, body: dict, server: str = None) -> str:
         """ Create a new metadata element from a template.  Async version.
            Parameters
            ----------
            body : str
                 The json body used to instantiate the template.
@@ -141,16 +141,16 @@
         """
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_create_element_from_template(body, server)
         )
         return response
 
-    async def _async_create_kafka_server_element_from_template(self, kafka_server:str, host_name: str, port: str,
-                                                               server:str = None) -> str:
+    async def _async_create_kafka_server_element_from_template(self, kafka_server: str, host_name: str, port: str,
+                                                               server: str = None) -> str:
         """ Create a Kafka server element from a template. Async version.
 
             Parameters
             ----------
             kafka_server : str
                 The name of the Kafka server.
 
@@ -206,15 +206,14 @@
             """
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_create_kafka_server_element_from_template(kafka_server, host_name, port, server)
         )
         return response
 
-
     async def _async_create_postgres_server_element_from_template(self, postgres_server: str, host_name: str, port: str,
                                                                   db_user: str, db_pwd: str, server: str = None) -> str:
         """ Create a Postgres server element from a template. Async version.
 
             Parameters
             ----------
             postgres_server : str
@@ -243,15 +242,15 @@
         body = {
             "templateGUID": "542134e6-b9ce-4dce-8aef-22e8daf34fdb",
             "isOwnAnchor": 'true',
             "placeholderPropertyValues": {
                 "serverName": postgres_server,
                 "hostIdentifier": host_name,
                 "portNumber": port,
-                "databaseUserId" : db_user,
+                "databaseUserId": db_user,
                 "databasePassword": db_pwd
             }
         }
         response = await self._async_create_element_from_template(body, server)
         return response
 
     def create_postgres_server_element_from_template(self, postgres_server: str, host_name: str, port: str,
@@ -281,22 +280,22 @@
             Returns
             -------
             str
                 The GUID of the Postgres server element.
             """
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
-            self._async_create_postgres_server_element_from_template(postgres_server,host_name,
-                                                                     port, db_user,db_pwd,server)
+            self._async_create_postgres_server_element_from_template(postgres_server, host_name,
+                                                                     port, db_user, db_pwd, server)
         )
         return response
 
     #
-# Engine Actions
-#
+    # Engine Actions
+    #
     async def _async_get_engine_actions(self, server: str = None, start_from: int = 0,
                                         page_size: int = max_paging_size) -> list:
         """ Retrieve the engine actions that are known to the server. Async version.
         Parameters
         ----------
         server : str, optional
             The name of the server. If not provided, it uses the default server name.
@@ -558,24 +557,27 @@
         """ Retrieve the list of engine action metadata elements with a matching qualified or display name.
         There are no wildcards supported on this request. Async Version.
         Parameters
         ----------
         name : str
             The name of the engine action to retrieve.
         server : str, optional
-            The name of the server to retrieve the engine action from. If not provided, the default server specified in the instance will be used.
+             The name of the server to retrieve the engine action from. If not provided, the default server specified in
+             the instance will be used.
         start_from : int, optional
             The index to start retrieving engine actions from. If not provided, the default value will be used.
         page_size : int, optional
-            The maximum number of engine actions to retrieve in a single request. If not provided, the default global maximum paging size will be used.
+            The maximum number of engine actions to retrieve in a single request. If not provided, the default global
+            maximum paging size will be used.
 
         Returns
         -------
         list of dict | str
-            A list of dictionaries representing the retrieved engine actions, or "no actions" if no engine actions were found with the given name.
+            A list of dictionaries representing the retrieved engine actions, or "no actions" if no engine actions were
+             found with the given name.
         Raises:
         ------
         InvalidParameterException
         PropertyServerException
         UserNotAuthorizedException
 
         Notes
@@ -600,24 +602,27 @@
         There are no wildcards supported on this request.
 
         Parameters
         ----------
         name : str
             The name of the engine action to retrieve.
         server : str, optional
-            The name of the server to retrieve the engine action from. If not provided, the default server specified in the instance will be used.
+            The name of the server to retrieve the engine action from. If not provided, the default server specified in
+            the instance will be used.
         start_from : int, optional
             The index to start retrieving engine actions from. If not provided, the default value will be used.
         page_size : int, optional
-            The maximum number of engine actions to retrieve in a single request. If not provided, the default global maximum paging size will be used.
+            The maximum number of engine actions to retrieve in a single request. If not provided, the default global
+             maximum paging size will be used.
 
         Returns
         -------
         list of dict | str
-            A list of dictionaries representing the retrieved engine actions, or "no actions" if no engine actions were found with the given name.
+            A list of dictionaries representing the retrieved engine actions, or "no actions" if no engine actions were
+            found with the given name.
         Raises:
         ------
         InvalidParameterException
         PropertyServerException
         UserNotAuthorizedException
 
         Notes
@@ -741,17 +746,17 @@
         response = loop.run_until_complete(
             self._async_find_engine_actions(search_string, server, starts_with,
                                             ends_with, ignore_case, start_from,
                                             page_size)
         )
         return response
 
-#
-# Governance action processes
-#
+    #
+    # Governance action processes
+    #
 
     async def _async_get_governance_action_process_by_guid(self, process_guid: str, server: str = None) -> dict | str:
         """ Retrieve the governance action process metadata element with the supplied unique identifier. Async Version.
 
             Parameters:
             ----------
                 process_guid: str
@@ -859,33 +864,35 @@
                this exception is raised with details from the response content.
                PropertyServerException: If the API response indicates a server side error.
                UserNotAuthorizedException:
 
        """
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
-            self._async_get_gov_action_process_graph(process_guid, server)
+            self._async_gov_action_process_graph(process_guid, server)
         )
         return response
 
     async def _async_get_gov_action_processes_by_name(self, name: str, server: str = None, start_from: int = None,
                                                       page_size: int = max_paging_size) -> list | str:
         """ Retrieve the list of governance action process metadata elements with a matching qualified or display name.
             There are no wildcards supported on this request. Async Version.
 
            Parameters
            ----------
            name : str
                The name of the engine action to retrieve.
            server : str, optional
-               The name of the server to retrieve the engine action from. If not provided, the default server specified in the instance will be used.
+               The name of the server to retrieve the engine action from. If not provided, the default server specified
+               in the instance will be used.
            start_from : int, optional
                The index to start retrieving engine actions from. If not provided, the default value will be used.
            page_size : int, optional
-               The maximum number of engine actions to retrieve in a single request. If not provided, the default global maximum paging size will be used.
+               The maximum number of engine actions to retrieve in a single request. If not provided, the default
+               global maximum paging size will be used.
 
            Returns
            -------
            list of dict | str
                A list of dictionaries representing the retrieved engine actions,
                or "no actions" if no engine actions were found with the given name.
            Raises:
@@ -912,19 +919,21 @@
             There are no wildcards supported on this request.
 
            Parameters
            ----------
            name : str
                The name of the engine action to retrieve.
            server : str, optional
-               The name of the server to retrieve the engine action from. If not provided, the default server specified in the instance will be used.
+               The name of the server to retrieve the engine action from. If not provided, the default server specified
+               in the instance will be used.
            start_from : int, optional
                The index to start retrieving engine actions from. If not provided, the default value will be used.
            page_size : int, optional
-               The maximum number of engine actions to retrieve in a single request. If not provided, the default global maximum paging size will be used.
+               The maximum number of engine actions to retrieve in a single request. If not provided, the default global
+                maximum paging size will be used.
 
            Returns
            -------
            list of dict | str
                A list of dictionaries representing the retrieved engine actions,
                or "no actions" if no engine actions were found with the given name.
            Raises:
@@ -1037,16 +1046,16 @@
         InvalidParameterException
         PropertyServerException
         UserNotAuthorizedException
         """
 
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
-            self._async_get_gov_action_processes(search_string, server, starts_with, ends_with, ignore_case,
-                                                 start_from, page_size)
+            self._async_find_gov_action_processes(search_string, server, starts_with, ends_with, ignore_case,
+                                                  start_from, page_size)
         )
         return response
 
     async def _async_initiate_gov_action_process(self, action_type_qualified_name: str, request_source_guids: [str],
                                                  action_targets: list, start_time: datetime, request_parameters: dict,
                                                  orig_service_name: str, orig_engine_name: str,
                                                  server: str = None) -> str:
@@ -1113,14 +1122,16 @@
             - time to start the process
         request_parameters: [str]
             - parameters passed into the process
         orig_service_name: str
             - unique name of the requesting governance service (if initiated by a governance engine)
         orig_engine_name: str
             - optional unique name of the governance engine (if initiated by a governance engine).
+        server: str, optional
+            - if not specified, the server from the class instance will be used
 
         Returns
         -------
         Unique id (guid) of the newly started governance engine process
 
         Raises
         ------
@@ -1198,15 +1209,16 @@
             There are no wildcards supported on this request. Async version.
 
                 Parameters:
                 ----------
                     action_type_name: str
                       The name of the governance action type to retrieve.
                     server: str, optional
-                        The name of the server. If None, will use the default server specified in the instance will be used.
+                        The name of the server. If None, will use the default server specified in the instance
+                        will be used.
                 Returns:
                 -------
                     dict: The JSON representation of the governance action type element.
 
                 Raises:
                 ------
                     InvalidParameterException: If the API response indicates an error (non-200 status code),
@@ -1365,16 +1377,18 @@
         response = loop.run_until_complete(
             self._async_find_gov_action_types(search_string, server, starts_with, ends_with,
                                               ignore_case, start_from, page_size)
         )
         return response
 
     async def _async_initiate_gov_action_type(self, action_type_qualified_name: str, request_source_guids: [str],
-                                              action_targets: list, start_time: datetime= None, request_parameters: dict= None,
-                                              orig_service_name: str= None, orig_engine_name: str = None, server: str = None) -> str:
+                                              action_targets: list, start_time: datetime = None,
+                                              request_parameters: dict = None,
+                                              orig_service_name: str = None, orig_engine_name: str = None,
+                                              server: str = None) -> str:
         """ Using the named governance action type as a template, initiate an engine action. Async version.
 
         Parameters
         ----------
         action_type_qualified_name: str
             - unique name for the governance process
         request_source_guids: [str]
@@ -1385,14 +1399,16 @@
             - time to start the process
         request_parameters: [str]
             - parameters passed into the process
         orig_service_name: str
             - unique name of the requesting governance service (if initiated by a governance engine)
         orig_engine_name: str
             - optional unique name of the governance engine (if initiated by a governance engine).
+        server : str, optional
+            - The name of the server. If None, will use the default server specified in the instance will be used.
 
         Returns
         -------
         Unique id (guid) of the newly started governance engine process
 
         Raises
         ------
@@ -1435,14 +1451,16 @@
             - time to start the process
         request_parameters: [str]
             - parameters passed into the process
         orig_service_name: str
             - unique name of the requesting governance service (if initiated by a governance engine)
         orig_engine_name: str
             - optional unique name of the governance engine (if initiated by a governance engine).
+        server : str, optional
+            - The name of the server. If None, will use the default server specified in the instance will be used.
 
         Returns
         -------
         Unique id (guid) of the newly started governance engine process
 
         Raises
         ------
@@ -1454,26 +1472,26 @@
         response = loop.run_until_complete(
             self._async_initiate_gov_action_type(action_type_qualified_name, request_source_guids,
                                                  action_targets, start_time, request_parameters,
                                                  orig_service_name, orig_engine_name, server)
         )
         return response
 
-    async def _async_initiate_postgres_server_survey(self, postgres_server_guid: str,  server: str = None )-> str:
+    async def _async_initiate_postgres_server_survey(self, postgres_server_guid: str, server: str = None) -> str:
         server = self.server_name if server is None else server
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-types/"
                f"initiate")
 
         body = {
             "class": "InitiateGovernanceActionTypeRequestBody",
             "governanceActionTypeQualifiedName": "Egeria:GovernanceActionType:2adeb8f1-0f59-4970-b6f2-6cc25d4d2402survey-postgres-server",
             "actionTargets": [{
-                "class" : "NewActionTarget",
-                "actionTargetName" : "serverToSurvey",
-                "actionTargetGUID" : postgres_server_guid
+                "class": "NewActionTarget",
+                "actionTargetName": "serverToSurvey",
+                "actionTargetGUID": postgres_server_guid
             }]
         }
         response = await self._async_make_request("POST", url, body)
         return response.json().get("guid", "Action not initiated")
         # Create/Retrieve the Postgres Server Element
 
         # Run the survey using the information and return the engine action to monitor
@@ -1503,15 +1521,15 @@
         }
         response = await self._async_make_request("POST", url, body)
         return response.json().get("guid", "Action not initiated")
 
     def initiate_file_folder_survey(self, file_folder_guid: str, server: str = None) -> str:
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
-            self._async_initiate_file_folder_survey( file_folder_guid, server)
+            self._async_initiate_file_folder_survey(file_folder_guid, server)
         )
         return response
 
     async def _async_initiate_kafka_server_survey(self, kafka_server_guid: str, server: str = None) -> str:
         server = self.server_name if server is None else server
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-types/"
                f"initiate")
@@ -1532,22 +1550,21 @@
     def initiate_kafka_server_survey(self, kafka_server_guid: str, server: str = None) -> str:
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_initiate_file_folder_survey(kafka_server_guid, server)
         )
         return response
 
-    async def run_gov_action_postgres_server_survey(self, postgres_server: str, host_name: str, port: str,):
+    async def run_gov_action_postgres_server_survey(self, postgres_server: str, host_name: str, port: str, ):
         pass
         # New combo process to do
         # run a process the creates the postgres server catalog entry, runs the server survey
         # creates a survey report
         # adds a to-do list element when done
 
-
     async def _async_initiate_engine_action(self, qualified_name: str, domain_identifier: int, display_name: str,
                                             description: str, request_source_guids: str, action_targets: str,
                                             received_guards: [str], start_time: datetime, gov_engine_name: str,
                                             request_type: str, request_parameters: dict, process_name: str,
                                             request_src_name: str = None, originator_svc_name: str = None,
                                             originator_eng_name: str = None, server: str = None) -> str:
         """ Create an engine action in the metadata store that will trigger the governance service associated with
@@ -1924,16 +1941,16 @@
                                        this exception is raised with details from the response content.
             PropertyServerException: If the API response indicates a server side error.
             UserNotAuthorizedException:
             """
 
         loop = asyncio.get_event_loop()
         loop.run_until_complete(
-            self._async_add_catalog_target(integ_connector_guid, metadata_element_guid,
-                                           server)
+            self._async_remove_catalog_target(integ_connector_guid, metadata_element_guid,
+                                              server)
         )
         return
 
     #
     #   Get information about technologies
     #
 
@@ -2077,15 +2094,15 @@
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_get_technology_type_detail(type_name, server)
         )
         return response
 
     async def _async_find_technology_types(self, search_string: str = "*", server: str = None, start_from: int = 0,
-                                           page_size: int = max_paging_size, starts_with: bool=False,
+                                           page_size: int = max_paging_size, starts_with: bool = False,
                                            ends_with: bool = False, ignore_case: bool = True) -> list | str:
         """ Retrieve the list of technology types that contain the search string. Async version.
 
             Parameters:
             ----------
             type_name: str
                 The technology type we are looking for.
@@ -2123,27 +2140,27 @@
         """
         server = self.server_name if server is None else server
 
         starts_with_s = str(starts_with).lower()
         ends_with_s = str(ends_with).lower()
         ignore_case_s = str(ignore_case).lower()
         validate_name(search_string)
-        if search_string== "*":
+        if search_string == "*":
             search_string = ""
 
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/technology-types/"
                f"by-search-string?startFrom={start_from}&pageSize={page_size}&startsWith={starts_with_s}&"
                f"endsWith={ends_with_s}&ignoreCase={ignore_case_s}")
         body = {"string": search_string}
 
         response = await self._async_make_request("POST", url, body)
         return response.json().get("elements", "no tech found")
 
     def find_technology_types(self, type_name: str = "*", server: str = None, start_from: int = 0,
-                              page_size: int = max_paging_size, starts_with: bool=False,
+                              page_size: int = max_paging_size, starts_with: bool = False,
                               ends_with: bool = False, ignore_case: bool = True) -> list | str:
         """ Retrieve the list of technology types that contain the search string. Async version.
 
             Parameters:
             ----------
             type_name: str
                 The technology type we are looking for.
@@ -2164,25 +2181,25 @@
             -----
             For more information see: https://egeria-project.org/concepts/deployed-implementation-type
         """
 
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_find_technology_types(type_name, server, start_from,
-                                              page_size, starts_with,ends_with, ignore_case)
+                                              page_size, starts_with, ends_with, ignore_case)
         )
         return response
 
     async def _async_get_all_technology_types(self, server: str = None, start_from: int = 0,
                                               page_size: int = max_paging_size) -> list | str:
         return await self._async_find_technology_types("*", server, start_from, page_size)
 
     def get_all_technology_types(self, server: str = None, start_from: int = 0,
                                  page_size: int = max_paging_size) -> list | str:
         return self.find_technology_types("*", server, start_from, page_size)
 
 
 if __name__ == "__main__":
     p = AutomatedCuration("meow", "https://127.0.0.1:9443", "garygeeke", verify_flag=False)
-    response = p.get_active_service_list_for_server()
-    out = response.json()["result"]
+    response = p.get_active_engine_actions()
+    out = response.json()
     print(out)
```

### Comparing `pyegeria-0.3.2/src/pyegeria/core_omag_server_config.py` & `pyegeria-0.3.3/src/pyegeria/core_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/full_omag_server_config.py` & `pyegeria-0.3.3/src/pyegeria/full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/glossary_omvs.py` & `pyegeria-0.3.3/src/pyegeria/glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/gov_engine.py` & `pyegeria-0.3.3/src/pyegeria/gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/governance_author.py` & `pyegeria-0.3.3/src/pyegeria/governance_author.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/my_profile_omvs.py` & `pyegeria-0.3.3/src/pyegeria/my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/platform_services.py` & `pyegeria-0.3.3/src/pyegeria/platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/registered_info.py` & `pyegeria-0.3.3/src/pyegeria/registered_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 
 This module allows users to query the available (registered) capabilities of Egeria. Detailed information is returned
 to provide both insight and understanding in how to use these capabilities. For example, when configuring an Egeria
 integration service, it is important to know what companion service it depends on so that you can make sure the
 companion service is also configured and running.
 
 """
+import json
+from rich.console import Console
+from rich import print, print_json
+
 import pandas as pd
 from tabulate import tabulate
 
-from .utils import wrap_text
+from pyegeria.utils import wrap_text
 
-from ._client import Client
+from pyegeria._client import Client
 
 
 class RegisteredInfo(Client):
     """ Client to discover Egeria services and capabilities
 
     Attributes:
     ----------
@@ -38,14 +42,17 @@
     -------
         list_registered_svcs(self, kind: str = None, fmt: str = 'json', skinny: bool = True, wrap_len: int = 30)
             -> list | str
             Returns information about the different kinds of services as either JSON or a printable table.
 
         list_severity_definitions(self, fmt: str = 'json', skinny: bool = True, wrap_len: int = 30) -> list | str
             Returns a list of severity definitions for an OMAG Server used by the audit services.
+
+        list_asset_types(self, server: str = None) -> list | str
+            Lists the defined asset types.
     """
 
     admin_command_root: str
 
     def __init__(
             self,
             platform_url: str,
@@ -89,37 +96,37 @@
                If the response code is not 200.
            PropertyServerException:
                Raised by the server when an issue arises in processing a valid request
            NotAuthorizedException:
                The principle specified by the user_id does not have authorization for the requested action
 
            """
-        if kind is None or kind is "help":
+        if kind is None or kind == "help":
             return ("""
             The kinds of services that you can get more information include:
                 all.....................lists all registered services
                 access-services.........lists all registered access services
                 common-services.........lists all registered common services
                 engine-services.........lists all registered engine services
                 governance-services.....lists all registered governance services
                 integration-services....lists all registered integration services
                 view-services...........lists all registered view services
                 
                 Pass in a parameter from the left-hand column into the function to 
                 get more details on the specified service category.
             """)
-        if kind is "all":
+        if kind == "all":
             url = f"{self.admin_command_root}"
         else:
             url = f"{self.admin_command_root}/{kind}"
         response = self.make_request("GET", url)
 
-        if fmt is 'json':
+        if fmt == 'json':
             return response.json().get("services", "No services found")
-        elif fmt is 'table':
+        elif fmt == 'table':
             df = pd.DataFrame(response.json().get("services", []))
             if skinny:
                 df = df.drop(columns=['serviceId', 'serviceDevelopmentStatus'])
             return tabulate(wrap_text(df, wrap_len=wrap_len), headers='keys', tablefmt='psql')
 
     def list_severity_definitions(self, fmt: str = 'json', skinny: bool = True, wrap_len: int = 30) -> list | str:
         """ Get the registered severities for the OMAG Server
@@ -151,14 +158,42 @@
               The principle specified by the user_id does not have authorization for the requested action
 
         """
         url = (f"{self.platform_url}/servers/{self.server_name}/open-metadata/repository-services"
                f"/users/{self.user_id}/audit-log/severity-definitions"
                )
         response = self.make_request("GET", url)
-        if fmt is 'json':
+        if fmt == 'json':
             return response.json().get("severities", "No severities found")
-        elif fmt is 'table':
+        elif fmt == 'table':
             df = pd.DataFrame(response.json().get("severities", []))
             if skinny:
                 df = df.drop(columns=['ordinal'])
             return tabulate(wrap_text(df, wrap_len=wrap_len), headers='keys', tablefmt='psql')
+
+    def list_asset_types(self, server: str = None) -> list | str:
+        """ Get the registered severities for the OMAG Server
+
+          Parameters
+          ----------
+           server: str, optional, default = None
+
+          Returns
+          -------
+          dict | str
+              Returns a list of the asset types.
+
+          Raises
+          ------
+          InvalidParameterException
+              If the response code is not 200.
+          PropertyServerException:
+              Raised by the server when an issue arises in processing a valid request
+          NotAuthorizedException:
+              The principle specified by the user_id does not have authorization for the requested action
+
+        """
+        server = self.server_name if server is None else server
+        url = f"{self.platform_url}/servers/{self.server_name}/api/open-metadata/asset-catalog/assets/types"
+
+        response = self.make_request("GET", url)
+        return response.json().get('types', 'no types found')
```

### Comparing `pyegeria-0.3.2/src/pyegeria/server_operations.py` & `pyegeria-0.3.3/src/pyegeria/server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria/utils.py` & `pyegeria-0.3.3/src/pyegeria/utils.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/src/pyegeria.egg-info/PKG-INFO` & `pyegeria-0.3.3/src/pyegeria.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.2/src/pyegeria.egg-info/SOURCES.txt` & `pyegeria-0.3.3/src/pyegeria.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/pyegeria/__init__.py
 src/pyegeria/_client.py
 src/pyegeria/_exceptions.py
 src/pyegeria/_globals.py
 src/pyegeria/_validators.py
 src/pyegeria/automated_curation_omvs.py
 src/pyegeria/core_omag_server_config.py
+src/pyegeria/exceptions.py
 src/pyegeria/full_omag_server_config.py
 src/pyegeria/glossary_omvs.py
 src/pyegeria/gov_engine.py
 src/pyegeria/governance_author.py
 src/pyegeria/my_profile_omvs.py
 src/pyegeria/platform_services.py
 src/pyegeria/registered_info.py
```

### Comparing `pyegeria-0.3.2/tests/test_automated_curation_omvs.py` & `pyegeria-0.3.3/tests/test_automated_curation_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_automated_curation_omvs_cray.py` & `pyegeria-0.3.3/tests/test_automated_curation_omvs_cray.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_client.py` & `pyegeria-0.3.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_core_omag_server_config.py` & `pyegeria-0.3.3/tests/test_core_omag_server_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 InvalidParameterException,
                 PropertyServerException,
                 UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
-    def test_configure_all_access_services_good(self, server:str = good_server_1):
+    def test_configure_all_access_services_good(self, server:str = good_server_3):
         try:
             o_client = CoreServerConfig(
                 server, self.good_platform1_url,
                 self.good_user_1)
             o_client.configure_all_access_services()
             print(f"\n\n\t Server {server} has all access services configured")
             assert True
```

### Comparing `pyegeria-0.3.2/tests/test_full_omag_server_config.py` & `pyegeria-0.3.3/tests/test_full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_glossary_omvs.py` & `pyegeria-0.3.3/tests/test_glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_gov_engine.py` & `pyegeria-0.3.3/tests/test_gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_my_profile_omvs.py` & `pyegeria-0.3.3/tests/test_my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_platform_services.py` & `pyegeria-0.3.3/tests/test_platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_registered_info.py` & `pyegeria-0.3.3/tests/test_registered_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 This module is for testing the core OMAG config class and methods
 The routines assume that pytest is being used as the test tool and framework.
 
 A running Egeria environment is needed to run these tests.
 
 """
+import json
 import pytest
 from rich import print as rprint
 from rich.console import Console
 from rich.table import Table
 
 from pyegeria._exceptions import (
     InvalidParameterException,
@@ -24,24 +25,24 @@
 from pyegeria.registered_info import RegisteredInfo
 
 disable_ssl_warnings = True
 
 
 class TestRegisteredInfoServices:
     good_platform1_url = "https://127.0.0.1:9443"
-    good_platform2_url = "https://127.0.0.1:9444"
+    good_platform2_url = "https://cray.local:9443"
     bad_platform1_url = "https://localhost:9443"
 
     good_user_1 = "garygeeke"
     good_user_2 = "erinoverview"
     bad_user_1 = "eviledna"
     bad_user_2 = ""
 
     good_server_1 = "simple-metadata-store"
-    good_server_2 = "cocoMDS2"
+    good_server_2 = "view-server"
     good_server_3 = "active-metadata-store"
     bad_server_1 = "coco"
     bad_server_2 = ""
 
     @pytest.mark.parametrize(
         "service_kind",
         [
@@ -122,8 +123,31 @@
 
         except (
                 InvalidParameterException,
                 PropertyServerException,
                 UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
+            assert False, "Invalid request"
+
+    def test_list_asset_types(self):
+        user = self.good_user_2
+        try:
+            r_client = RegisteredInfo(self.good_platform1_url, user, "secret",
+                                      server_name =self.good_server_2,)
+            token = r_client.create_egeria_bearer_token(user, "secret")
+            response = r_client.list_asset_types()
+
+            assert type(response) is list, "No services found"
+            if type(response) is list:
+                print(f"\n\nAsset types are: \n\n")
+                print(json.dumps(response, indent=4))
+            else:
+                print(f"\n\n{response}: \n\n")
+
+        except (
+                InvalidParameterException,
+                PropertyServerException,
+                UserNotAuthorizedException
+        ) as e:
+            print_exception_response(e)
             assert False, "Invalid request"
```

### Comparing `pyegeria-0.3.2/tests/test_server_operations.py` & `pyegeria-0.3.3/tests/test_server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_util_exp.py` & `pyegeria-0.3.3/tests/test_util_exp.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.2/tests/test_validators.py` & `pyegeria-0.3.3/tests/test_validators.py`

 * *Files identical despite different names*

