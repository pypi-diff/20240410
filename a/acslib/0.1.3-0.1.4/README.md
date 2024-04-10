# Comparing `tmp/acslib-0.1.3.tar.gz` & `tmp/acslib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acslib-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acslib-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acslib-0.1.3.tar` & `acslib-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      163 2023-10-24 15:48:19.427776 acslib-0.1.3/.coveragerc
--rw-r--r--   0        0        0      104 2023-10-24 15:48:19.423776 acslib-0.1.3/.dockerignore
--rw-r--r--   0        0        0      292 2023-10-24 15:48:19.431776 acslib-0.1.3/.editorconfig
--rw-r--r--   0        0        0     5737 2023-10-24 15:48:19.443776 acslib-0.1.3/.github/workflows/dev.yml
--rw-r--r--   0        0        0     3216 2023-10-24 15:48:19.443776 acslib-0.1.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1352 2023-10-24 15:48:19.435776 acslib-0.1.3/.gitignore
--rw-r--r--   0        0        0       81 2023-10-24 15:48:19.439777 acslib-0.1.3/.isort.cfg
--rw-r--r--   0        0        0      875 2023-10-24 15:48:19.423776 acslib-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      118 2023-10-24 15:48:19.411776 acslib-0.1.3/AUTHORS.md
--rw-r--r--   0        0        0      212 2023-10-24 15:57:17.064897 acslib-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      473 2023-10-24 15:48:19.423776 acslib-0.1.3/Dockerfile
--rw-r--r--   0        0        0       59 2023-10-24 15:48:19.431776 acslib-0.1.3/HISTORY.md
--rw-r--r--   0        0        0     1089 2023-10-24 15:57:17.060897 acslib-0.1.3/LICENSE
--rw-r--r--   0        0        0      589 2024-03-19 14:18:21.790000 acslib-0.1.3/Makefile
--rw-r--r--   0        0        0     4455 2024-04-05 19:22:19.372551 acslib-0.1.3/README.md
--rw-r--r--   0        0        0      188 2024-03-19 14:18:28.694065 acslib-0.1.3/acslib/__init__.py
--rw-r--r--   0        0        0      218 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/base/__init__.py
--rw-r--r--   0        0        0      266 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/base/acs.py
--rw-r--r--   0        0        0      173 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/base/config.py
--rw-r--r--   0        0        0     6294 2024-03-19 14:18:28.694065 acslib-0.1.3/acslib/base/connection.py
--rw-r--r--   0        0        0      277 2024-03-04 18:42:56.581079 acslib-0.1.3/acslib/base/search.py
--rw-r--r--   0        0        0     6113 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/base/status.py
--rw-r--r--   0        0        0      322 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/__init__.py
--rw-r--r--   0        0        0      595 2024-03-19 14:18:28.694065 acslib-0.1.3/acslib/ccure/base.py
--rw-r--r--   0        0        0     2916 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/ccure/config.py
--rw-r--r--   0        0        0     7444 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/connection.py
--rw-r--r--   0        0        0    13405 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/crud.py
--rw-r--r--   0        0        0     1015 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/endpoints.py
--rw-r--r--   0        0        0     7648 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/filters.py
--rw-r--r--   0        0        0       36 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/ccure/tests/__init__.py
--rw-r--r--   0        0        0     1839 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/ccure/tests/conftest.py
--rw-r--r--   0        0        0     1821 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/tests/test_base.py
--rw-r--r--   0        0        0     2800 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/ccure/tests/test_config.py
--rw-r--r--   0        0        0     2111 2024-01-11 18:55:00.490990 acslib-0.1.3/acslib/ccure/tests/test_connection.py
--rw-r--r--   0        0        0     2524 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/tests/test_search.py
--rw-r--r--   0        0        0     1138 2024-04-05 19:22:19.372551 acslib-0.1.3/acslib/ccure/types.py
--rw-r--r--   0        0        0       11 2023-10-24 15:48:19.451777 acslib-0.1.3/docs/api.md
--rw-r--r--   0        0        0       41 2023-10-24 15:48:19.451777 acslib-0.1.3/docs/authors.md
--rw-r--r--   0        0        0       46 2023-10-24 15:48:19.447776 acslib-0.1.3/docs/contributing.md
--rw-r--r--   0        0        0       41 2023-10-24 15:48:19.455777 acslib-0.1.3/docs/history.md
--rw-r--r--   0        0        0       42 2023-10-24 15:48:19.447776 acslib-0.1.3/docs/index.md
--rw-r--r--   0        0        0     1188 2023-10-24 15:48:19.455777 acslib-0.1.3/docs/installation.md
--rw-r--r--   0        0        0       87 2023-10-24 15:48:19.451777 acslib-0.1.3/docs/usage.md
--rw-r--r--   0        0        0       20 2023-10-24 15:48:19.431776 acslib-0.1.3/envrc_sample
--rw-r--r--   0        0        0     1949 2023-10-24 15:48:19.419776 acslib-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0     1918 2024-04-05 19:22:19.376551 acslib-0.1.3/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
--rw-r--r--   0        0        0     2314 2024-04-05 19:22:19.376551 acslib-0.1.3/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
--rw-r--r--   0        0        0    12624 2024-04-05 19:22:19.376551 acslib-0.1.3/notebooks/encode_investigation.ipynb
--rw-r--r--   0        0        0     2644 2024-04-05 19:27:54.047419 acslib-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      219 2024-01-11 18:55:00.490990 acslib-0.1.3/pytest.ini
--rw-r--r--   0        0        0      926 2024-03-19 14:18:21.794000 acslib-0.1.3/requirements/base/base.txt
--rw-r--r--   0        0        0     4618 2024-03-19 14:18:21.794000 acslib-0.1.3/requirements/dev/dev.txt
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 acslib-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-04-10 13:51:14.379070 acslib-0.1.4/.coveragerc
+-rw-r--r--   0        0        0      104 2024-04-10 13:51:14.379070 acslib-0.1.4/.dockerignore
+-rw-r--r--   0        0        0      292 2024-04-10 13:51:14.379070 acslib-0.1.4/.editorconfig
+-rw-r--r--   0        0        0      296 2024-04-10 13:51:14.379070 acslib-0.1.4/.github/pr_template.md
+-rw-r--r--   0        0        0     9158 2024-04-10 13:51:14.379070 acslib-0.1.4/.github/workflows/test_publish_release..yml
+-rw-r--r--   0        0        0     1388 2024-04-10 13:51:14.379070 acslib-0.1.4/.gitignore
+-rw-r--r--   0        0        0       81 2024-04-10 13:51:14.379070 acslib-0.1.4/.isort.cfg
+-rw-r--r--   0        0        0      875 2024-04-10 13:51:14.379070 acslib-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      118 2024-04-10 13:51:14.379070 acslib-0.1.4/AUTHORS.md
+-rw-r--r--   0        0        0      212 2024-04-10 13:51:14.379070 acslib-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      473 2024-04-10 13:51:14.379070 acslib-0.1.4/Dockerfile
+-rw-r--r--   0        0        0       59 2024-04-10 13:51:14.379070 acslib-0.1.4/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-04-10 13:51:14.379070 acslib-0.1.4/LICENSE
+-rw-r--r--   0        0        0      589 2024-04-10 13:51:14.379070 acslib-0.1.4/Makefile
+-rw-r--r--   0        0        0     4455 2024-04-10 13:51:14.379070 acslib-0.1.4/README.md
+-rw-r--r--   0        0        0      188 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/acs.py
+-rw-r--r--   0        0        0      172 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/config.py
+-rw-r--r--   0        0        0     6294 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/connection.py
+-rw-r--r--   0        0        0      272 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/search.py
+-rw-r--r--   0        0        0     6113 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/status.py
+-rw-r--r--   0        0        0      322 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/base.py
+-rw-r--r--   0        0        0     2923 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/config.py
+-rw-r--r--   0        0        0     7444 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/connection.py
+-rw-r--r--   0        0        0    13405 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/crud.py
+-rw-r--r--   0        0        0     1015 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/endpoints.py
+-rw-r--r--   0        0        0     7674 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/filters.py
+-rw-r--r--   0        0        0       36 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/conftest.py
+-rw-r--r--   0        0        0     2037 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_base.py
+-rw-r--r--   0        0        0     2801 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_config.py
+-rw-r--r--   0        0        0     2111 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_connection.py
+-rw-r--r--   0        0        0     2588 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_search.py
+-rw-r--r--   0        0        0     1138 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/types.py
+-rw-r--r--   0        0        0       11 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/api.md
+-rw-r--r--   0        0        0       41 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/authors.md
+-rw-r--r--   0        0        0       46 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/contributing.md
+-rw-r--r--   0        0        0       41 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/history.md
+-rw-r--r--   0        0        0       42 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/index.md
+-rw-r--r--   0        0        0     1188 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/installation.md
+-rw-r--r--   0        0        0       87 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/usage.md
+-rw-r--r--   0        0        0       20 2024-04-10 13:51:14.379070 acslib-0.1.4/envrc_sample
+-rw-r--r--   0        0        0     1949 2024-04-10 13:51:14.379070 acslib-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0     1918 2024-04-10 13:51:14.379070 acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
+-rw-r--r--   0        0        0     2314 2024-04-10 13:51:14.379070 acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
+-rw-r--r--   0        0        0    12624 2024-04-10 13:51:14.379070 acslib-0.1.4/notebooks/encode_investigation.ipynb
+-rw-r--r--   0        0        0     2699 2024-04-10 13:51:14.379070 acslib-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-10 13:51:14.379070 acslib-0.1.4/pytest.ini
+-rw-r--r--   0        0        0      926 2024-04-10 13:51:14.379070 acslib-0.1.4/requirements/base/base.txt
+-rw-r--r--   0        0        0     4618 2024-04-10 13:51:14.379070 acslib-0.1.4/requirements/dev/dev.txt
+-rw-r--r--   0        0        0     6040 1970-01-01 00:00:00.000000 acslib-0.1.4/PKG-INFO
```

### Comparing `acslib-0.1.3/.gitignore` & `acslib-0.1.4/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -97,9 +97,11 @@
 .idea/
 .envrc
 
 # mkdocs
 site/
 .history/
 
+# repo pulled in for CI/CD
+actions/
 
 Access Control Systems
```

### Comparing `acslib-0.1.3/.pre-commit-config.yaml` & `acslib-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/LICENSE` & `acslib-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/Makefile` & `acslib-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/README.md` & `acslib-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/base/connection.py` & `acslib-0.1.4/acslib/base/connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/base/status.py` & `acslib-0.1.4/acslib/base/status.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/ccure/base.py` & `acslib-0.1.4/acslib/ccure/base.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/ccure/config.py` & `acslib-0.1.4/acslib/ccure/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from acslib.base import ACSConfig, ACSConfigException
+from acslib.base.config import ACSConfig, ACSConfigException
 from acslib.ccure.endpoints import V2Endpoints
 
 
 class CcureConfig(ACSConfig):
     """
     CcureConfig returns an object that implements the ACSConfig interface.
     It expects the following variables to be set either in the environment or passed as kwargs:
```

### Comparing `acslib-0.1.3/acslib/ccure/connection.py` & `acslib-0.1.4/acslib/ccure/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from numbers import Number
 
 from acslib.base import (
     ACSConnection,
-    ACSRequestException,
     ACSRequestData,
+    ACSRequestException,
     ACSRequestResponse,
-    status
+    status,
 )
 from acslib.base.connection import ACSRequestMethod
 from acslib.ccure.config import CcureConfigFactory
 
 
 class CcureConnection(ACSConnection):
     def __init__(self, **kwargs):
@@ -149,15 +149,14 @@
                 request_data=ACSRequestData(url=version_url),
             ).json
             self.logger.debug(f"CCure webservice version: {response.get('webServiceVersion')}")
             self.logger.debug(f"CCure app server version: {response.get('appServerVersion')}")
         except ACSRequestException as e:
             self.logger.debug(f"Could not get CCure api version number: {e}")
 
-
     @staticmethod
     def encode_data(data: dict) -> str:
         """
         Encode a dictionary of form data as a string for requests
 
         Parameters:
             data: form data for the request
```

### Comparing `acslib-0.1.3/acslib/ccure/crud.py` & `acslib-0.1.4/acslib/ccure/crud.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/ccure/endpoints.py` & `acslib-0.1.4/acslib/ccure/endpoints.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/ccure/filters.py` & `acslib-0.1.4/acslib/ccure/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         self.term_operator = term_operator.value
         #: List of properties from CCURE to be included in the CCURE response
         self.display_properties = []
 
     def _compile_term(self, term) -> str:
         """Get all parts of the query for one search term"""
         fields = [(field_name, lookup(term)) for field_name, lookup in self.filter_fields.items()]
-        field_queries = [f"{field_name} {self.term_operator} '{lookup}'" for field_name, lookup in fields]
+        field_queries = [
+            f"{field_name} {self.term_operator} '{lookup}'" for field_name, lookup in fields
+        ]
         return f"({self.inner_bool.join(field_queries)})"
 
     def update_display_properties(self, properties: list[str]):
         if not isinstance(properties, list):
             raise TypeError("Properties must be a list of strings")
         self.display_properties += properties
 
@@ -86,15 +88,15 @@
 
     def __init__(
         self,
         lookups: Optional[dict[str, callable]] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
-        display_properties: Optional[list[str]] = None
+        display_properties: Optional[list[str]] = None,
     ):
         self.filter_fields = lookups or PERSONNEL_LOOKUP_FIELDS
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["FirstName", "MiddleName", "LastName", "ObjectID"]
         if display_properties is not None:
@@ -118,15 +120,15 @@
 
     def __init__(
         self,
         lookups: Optional[dict[str, callable]] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
-        display_properties: Optional[list[str]] = None
+        display_properties: Optional[list[str]] = None,
     ):
         self.filter_fields = lookups or CLEARANCE_LOOKUP_FIELDS
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["Name"]
         if display_properties is not None:
@@ -150,15 +152,15 @@
 
     def __init__(
         self,
         lookups: Optional[dict[str, callable]] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
-        display_properties: Optional[list[str]] = None
+        display_properties: Optional[list[str]] = None,
     ):
         self.filter_fields = lookups or CREDENTIAL_LOOKUP_FIELDS
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["Name"]
         if display_properties is not None:
@@ -182,15 +184,15 @@
 
     def __init__(
         self,
         lookups: Optional[dict[str, callable]] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
-        display_properties: Optional[list[str]] = None
+        display_properties: Optional[list[str]] = None,
     ):
         self.filter_fields = lookups or CREDENTIAL_LOOKUP_FIELDS
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
         self.display_properties = ["Name"]
         if display_properties is not None:
```

### Comparing `acslib-0.1.3/acslib/ccure/tests/conftest.py` & `acslib-0.1.4/acslib/ccure/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/ccure/tests/test_base.py` & `acslib-0.1.4/acslib/ccure/tests/test_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,49 +7,52 @@
 from acslib.ccure.filters import PersonnelFilter, SearchTypes
 
 
 def test_default_ccure_acs(env_config, caplog):
     """Default picks up env vars."""
     ccure = CcureACS()
     assert ccure.config.base_url == "https://example.com/ccure"
-    assert ccure.logger.name == "acslib.ccure.base"
-    assert "acslib.ccure.base" in caplog.text
+    assert ccure.logger.name == "acslib.ccure.connection"
+    assert "acslib.ccure.connection" in caplog.text
 
 
 def test_user_supplied_logger(env_config, caplog):
     """."""
     import logging
 
     cc_conn = CcureConnection(logger=logging.getLogger("test"))
     ccure = CcureACS(connection=cc_conn)
     assert ccure.logger.name == "test"
-    assert "test:base" in caplog.text
+    assert "test:connection" in caplog.text
 
 
+@pytest.mark.skip(reason="ccure search no longer works this way")
 def test_default_ccure_search(env_config, personnel_response, caplog):
     ccure = CcureACS()
     with patch(
         "acslib.ccure.base.CcureACS._search_people", return_value=personnel_response
     ) as mock_search:
         ccure.search(search_type=SearchTypes.PERSONNEL, terms=["test"])
         mock_search.assert_called_with(["test"])
     assert "Searching for personnel" in caplog.text
 
 
+@pytest.mark.skip(reason="ccure search no longer works this way")
 def test_ccure_search_with_filter(env_config, personnel_response, caplog):
     ccure = CcureACS()
     filter = PersonnelFilter()
     with patch(
         "acslib.ccure.base.CcureACS._search_people", return_value=personnel_response
     ) as mock_search:
         ccure.search(search_type=SearchTypes.PERSONNEL, terms=["test"], search_filter=filter)
         mock_search.assert_called_with(["test"], filter)
     assert "Searching for personnel" in caplog.text
 
 
+@pytest.mark.skip(reason="ccure search no longer works this way")
 def test_invalid_search_type(env_config):
     class NewTypes(Enum):
         NEW = "new"
         PERSONNEL = "personnel"
 
     ccure = CcureACS()
     with pytest.raises(ValueError):
```

### Comparing `acslib-0.1.3/acslib/ccure/tests/test_config.py` & `acslib-0.1.4/acslib/ccure/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 import pytest
 
 from acslib.base import ACSConfigException
 from acslib.ccure.config import CcureConfigFactory
 
 
 def test_ccure_config_with_kwargs(config):
```

### Comparing `acslib-0.1.3/acslib/ccure/tests/test_connection.py` & `acslib-0.1.4/acslib/ccure/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/acslib/ccure/tests/test_search.py` & `acslib-0.1.4/acslib/ccure/tests/test_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,45 +4,50 @@
 from acslib.ccure.filters import (
     FUZZ,
     LFUZZ,
     NFUZZ,
     PERSONNEL_LOOKUP_FIELDS,
     CLEARANCE_LOOKUP_FIELDS,
     RFUZZ,
+    ClearanceFilter,
     PersonnelFilter,
-    ClearanceFilter
 )
 
 
 def test_default_instance():
     personnel_filter = PersonnelFilter()
     assert personnel_filter.filter_fields == PERSONNEL_LOOKUP_FIELDS
-    assert personnel_filter.outer_bool == "AND"
-    assert personnel_filter.inner_bool == "OR"
+    assert personnel_filter.outer_bool == " AND "
+    assert personnel_filter.inner_bool == " OR "
     assert personnel_filter.term_operator == "LIKE"
-    assert personnel_filter.display_properties == ["FirstName", "MiddleName", "LastName"]
+    assert personnel_filter.display_properties == [
+        "FirstName",
+        "MiddleName",
+        "LastName",
+        "ObjectID",
+    ]
 
     clearance_filter = ClearanceFilter()
     assert clearance_filter.filter_fields == CLEARANCE_LOOKUP_FIELDS
-    assert clearance_filter.outer_bool == "AND"
-    assert clearance_filter.inner_bool == "OR"
+    assert clearance_filter.outer_bool == " AND "
+    assert clearance_filter.inner_bool == " OR "
     assert clearance_filter.term_operator == "LIKE"
     assert clearance_filter.display_properties == ["Name"]
 
 
 def test_custom_instance():
     filter = PersonnelFilter(
         lookups={"Text1": NFUZZ, "Tex14": NFUZZ},
         outer_bool=BooleanOperators.OR,
         inner_bool=BooleanOperators.AND,
         term_operator=TermOperators.EQUALS,
     )
     assert filter.filter_fields == {"Text1": NFUZZ, "Tex14": NFUZZ}
-    assert filter.outer_bool == "OR"
-    assert filter.inner_bool == "AND"
+    assert filter.outer_bool == " OR "
+    assert filter.inner_bool == " AND "
     assert filter.term_operator == "="
 
 
 def test_single_search_term():
     filter = PersonnelFilter()
     search = filter.filter(["test"])
     assert search == "(FirstName LIKE '%test%' OR LastName LIKE '%test%')"
@@ -62,15 +67,15 @@
         == "(FirstName LIKE '%test%' OR LastName LIKE '%test%') AND (FirstName LIKE '%test2%' OR LastName LIKE '%test2%')"
     )
 
 
 def test_update_display_properties():
     filter = PersonnelFilter()
     filter.update_display_properties(["EmailAddress"])
-    assert len(filter.display_properties) == 4
+    assert len(filter.display_properties) == 5
     assert "EmailAddress" in filter.display_properties
 
 
 def test_update_display_properties_not_list():
     filter = PersonnelFilter()
     with pytest.raises(TypeError):
         filter.update_display_properties("EmailAddress")
```

### Comparing `acslib-0.1.3/acslib/ccure/types.py` & `acslib-0.1.4/acslib/ccure/types.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/docs/installation.md` & `acslib-0.1.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/mkdocs.yml` & `acslib-0.1.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint` & `acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb` & `acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/notebooks/encode_investigation.ipynb` & `acslib-0.1.4/notebooks/encode_investigation.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/pyproject.toml` & `acslib-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["flit_core>=3.2, <4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "acslib"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name="Jeremy Gibson", email="jmgibso3@ncsu.edu" },
+    { name="Luc Sanchez", email="lgsanche@ncsu.edu" },
     { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
 ]
 description = "A library for interacting with Access Control Systems like Genetec or Ccure9k"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 
@@ -51,17 +52,17 @@
 [tool.black]
 target-version = ["py310"]
 line-length = 100
 include = '\.pyi?$'
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F", "W", "I001"]
+select = ["E", "F", "W"]
 src = ["acslib"]
-ignore = ["E501"]
+ignore = ["E501", "F401"]
 fix = true
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
```

### Comparing `acslib-0.1.3/requirements/base/base.txt` & `acslib-0.1.4/requirements/base/base.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/requirements/dev/dev.txt` & `acslib-0.1.4/requirements/dev/dev.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.3/PKG-INFO` & `acslib-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: acslib
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for interacting with Access Control Systems like Genetec or Ccure9k
-Author-email: Jeremy Gibson <jmgibso3@ncsu.edu>, Ryan Semmler <rsemmle@ncsu.edu>
+Author-email: Jeremy Gibson <jmgibso3@ncsu.edu>, Luc Sanchez <lgsanche@ncsu.edu>, Ryan Semmler <rsemmle@ncsu.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0
 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0, <5.0.0 ; extra == "dev"
 Requires-Dist: pytest-mock>=3.10.0, <4.0.0 ; extra == "dev"
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: acslib Version: 0.1.3 Summary: A library for
+Metadata-Version: 2.1 Name: acslib Version: 0.1.4 Summary: A library for
 interacting with Access Control Systems like Genetec or Ccure9k Author-email:
 Jeremy Gibson
+ncsu.edu>, Luc Sanchez
 ncsu.edu>, Ryan Semmler
 ncsu.edu> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev" Requires-Dist: pytest-
 cov>=4.0.0, <5.0.0 ; extra == "dev" Requires-Dist: pytest-mock>=3.10.0, <4.0.0
 ; extra == "dev" Requires-Dist: coverage[toml]>=6.2 ; extra == "dev" Requires-
 Dist: black>=23.3.0, <24.0.0 ; extra == "dev" Requires-Dist: ruff==0.1.1 ;
```

