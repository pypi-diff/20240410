# Comparing `tmp/lusid_drive_sdk-2.0.9.tar.gz` & `tmp/lusid_drive_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_drive_sdk-2.0.9.tar", max compression
+gzip compressed data, was "lusid_drive_sdk-2.1.1.tar", max compression
```

## Comparing `lusid_drive_sdk-2.0.9.tar` & `lusid_drive_sdk-2.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     7241 2023-12-19 14:51:15.304728 lusid_drive_sdk-2.0.9/README.md
--rw-r--r--   0        0        0     2077 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/__init__.py
--rw-r--r--   0        0        0      271 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/__init__.py
--rw-r--r--   0        0        0     7516 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/application_metadata_api.py
--rw-r--r--   0        0        0    46851 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/files_api.py
--rw-r--r--   0        0        0    65918 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/folders_api.py
--rw-r--r--   0        0        0    10285 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/search_api.py
--rw-r--r--   0        0        0    30511 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api_client.py
--rw-r--r--   0        0        0      852 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/api_response.py
--rw-r--r--   0        0        0    14436 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/configuration.py
--rw-r--r--   0        0        0     5336 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/exceptions.py
--rw-r--r--   0        0        0      288 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/__init__.py
--rw-r--r--   0        0        0    30461 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client.py
--rw-r--r--   0        0        0     9614 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8000 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_configuration.py
--rw-r--r--   0        0        0     6856 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12704 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/rest.py
--rw-r--r--   0        0        0    11570 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/retry.py
--rw-r--r--   0        0        0     1653 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3883 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     1349 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/__init__.py
--rw-r--r--   0        0        0     3888 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_action.py
--rw-r--r--   0        0        0     4831 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2064 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/action_id.py
--rw-r--r--   0        0        0     2703 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/create_folder.py
--rw-r--r--   0        0        0     3171 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/id_selector_definition.py
--rw-r--r--   0        0        0     3096 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2256 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/link.py
--rw-r--r--   0        0        0     3851 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4687 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     4150 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/paged_resource_list_of_storage_object.py
--rw-r--r--   0        0        0     4243 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     3105 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/search_body.py
--rw-r--r--   0        0        0     6063 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/storage_object.py
--rw-r--r--   0        0        0     2714 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/update_file.py
--rw-r--r--   0        0        0     2719 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/update_folder.py
--rw-r--r--   0        0        0        0 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/py.typed
--rw-r--r--   0        0        0    10023 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/rest.py
--rw-r--r--   0        0        0      835 2023-12-19 14:51:15.304728 lusid_drive_sdk-2.0.9/pyproject.toml
--rw-r--r--   0        0        0     8269 1970-01-01 00:00:00.000000 lusid_drive_sdk-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0     9387 2024-04-10 10:42:10.646849 lusid_drive_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     3128 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/api/__init__.py
+-rw-r--r--   0        0        0     7519 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/api/application_metadata_api.py
+-rw-r--r--   0        0        0    46857 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/api/files_api.py
+-rw-r--r--   0        0        0    65924 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/api/folders_api.py
+-rw-r--r--   0        0        0    10291 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/api/search_api.py
+-rw-r--r--   0        0        0    30761 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/api_response.py
+-rw-r--r--   0        0        0    14436 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/configuration.py
+-rw-r--r--   0        0        0     5336 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/exceptions.py
+-rw-r--r--   0        0        0      578 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/__init__.py
+-rw-r--r--   0        0        0    30625 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/api_client.py
+-rw-r--r--   0        0        0     9832 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8082 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6784 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12704 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/rest.py
+-rw-r--r--   0        0        0    11570 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3883 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     1757 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/models/__init__.py
+-rw-r--r--   0        0        0     3891 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4834 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2067 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/action_id.py
+-rw-r--r--   0        0        0     2706 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/create_folder.py
+-rw-r--r--   0        0        0     3174 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3099 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2259 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/link.py
+-rw-r--r--   0        0        0     3854 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4690 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     4153 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/paged_resource_list_of_storage_object.py
+-rw-r--r--   0        0        0     4246 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     3108 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/search_body.py
+-rw-r--r--   0        0        0     6066 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/storage_object.py
+-rw-r--r--   0        0        0     2717 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/update_file.py
+-rw-r--r--   0        0        0     2722 2024-04-10 10:42:10.643849 lusid_drive_sdk-2.1.1/lusid_drive/models/update_folder.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:42:10.644849 lusid_drive_sdk-2.1.1/lusid_drive/py.typed
+-rw-r--r--   0        0        0    10154 2024-04-10 10:42:10.645849 lusid_drive_sdk-2.1.1/lusid_drive/rest.py
+-rw-r--r--   0        0        0      834 2024-04-10 10:42:10.646849 lusid_drive_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10414 1970-01-01 00:00:00.000000 lusid_drive_sdk-2.1.1/PKG-INFO
```

### Comparing `lusid_drive_sdk-2.0.9/README.md` & `lusid_drive_sdk-2.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-drive-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.602
-- Package version: 2.0.9
+- API version: 0.1.627
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -43,29 +43,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the lusid_drive application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_LUSID_DRIVE_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_LUSID_DRIVE_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to lusid_drive via a proxy, by setting `FBN_PROXY_ADDRESS`. 
+If your proxy has basic auth enabled, you must akso supply `FBN_PROXY_USERNAME` and `FBN_PROXY_PASSWORD`
+
+### Secrets file
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set in a `secrets.json` file in the same folder as your script.
+
+``` 
+{
+    "api":
+    {
+        "tokenUrl":"<your-token-url>",
+        "lusid_driveUrl":"<FINBOURNE-application-url>",
+        "username":"<your-username>",
+        "password":"<your-password>",
+        "clientId":"<your-client-id>",
+        "clientSecret":"<your-client-secret>",
+    }
+}
+```
+
+To use a long lived Personal Access Token, you must provide a `secrets.json` with the following variables:
+``` 
+{
+    "api":
+    {
+        "lusid_driveUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to lusid_drive via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "lusid_driveUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    },
+    "proxy":
+    {
+        "address":"<your-proxy-address>",
+        "username":"<your-proxy-username>",
+        "password":"<your-proxy-password>"
+    }
+}
+```
+
+### Using the SDK
+
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
 import lusid_drive
-from lusid_drive.rest import ApiException
+from lusid_drive.exceptions import ApiException
 from pprint import pprint
 
+import os
 from lusid_drive import (
-	  ApiClientFactory,
-	  ApplicationMetadataApi,
-	  EnvironmentVariablesConfigurationLoader,
-	  SecretsFileConfigurationLoader,
-	  ArgsConfigurationLoader
+    ApiClientFactory,
+    ApplicationMetadataApi,
+    EnvironmentVariablesConfigurationLoader,
+    SecretsFileConfigurationLoader,
+    ArgsConfigurationLoader
 )
 
 # Use the lusid_drive ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -90,15 +166,15 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = lusid_drive.ApplicationMetadataApi(api_client)
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
         # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/__init__.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,23 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     FINBOURNE Drive API
 
     FINBOURNE Technology  # noqa: E501
 
     Contact: info@finbourne.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-from __future__ import absolute_import
-
-# import apis into sdk package
-from lusid_drive.api.application_metadata_api import ApplicationMetadataApi
-from lusid_drive.api.files_api import FilesApi
-from lusid_drive.api.folders_api import FoldersApi
-from lusid_drive.api.search_api import SearchApi
-
-# import ApiClient
-from lusid_drive.api_client import ApiClient
-from lusid_drive.configuration import Configuration
-from lusid_drive.exceptions import OpenApiException
-from lusid_drive.exceptions import ApiTypeError
-from lusid_drive.exceptions import ApiValueError
-from lusid_drive.exceptions import ApiKeyError
-from lusid_drive.exceptions import ApiException
-# import models into sdk package
+# import models into model package
 from lusid_drive.models.access_controlled_action import AccessControlledAction
 from lusid_drive.models.access_controlled_resource import AccessControlledResource
 from lusid_drive.models.action_id import ActionId
 from lusid_drive.models.create_folder import CreateFolder
 from lusid_drive.models.id_selector_definition import IdSelectorDefinition
 from lusid_drive.models.identifier_part_schema import IdentifierPartSchema
 from lusid_drive.models.link import Link
@@ -43,9 +26,25 @@
 from lusid_drive.models.paged_resource_list_of_storage_object import PagedResourceListOfStorageObject
 from lusid_drive.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_drive.models.search_body import SearchBody
 from lusid_drive.models.storage_object import StorageObject
 from lusid_drive.models.update_file import UpdateFile
 from lusid_drive.models.update_folder import UpdateFolder
 
-# import extensions into sdk package
-from lusid_drive.extensions import *
+
+__all__ = [
+    "AccessControlledAction",
+    "AccessControlledResource",
+    "ActionId",
+    "CreateFolder",
+    "IdSelectorDefinition",
+    "IdentifierPartSchema",
+    "Link",
+    "LusidProblemDetails",
+    "LusidValidationProblemDetails",
+    "PagedResourceListOfStorageObject",
+    "ResourceListOfAccessControlledResource",
+    "SearchBody",
+    "StorageObject",
+    "UpdateFile",
+    "UpdateFolder"
+]
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/api/application_metadata_api.py` & `lusid_drive_sdk-2.1.1/lusid_drive/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from lusid_drive.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 
 from lusid_drive.api_client import ApiClient
 from lusid_drive.api_response import ApiResponse
 from lusid_drive.exceptions import (  # noqa: F401
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/api/files_api.py` & `lusid_drive_sdk-2.1.1/lusid_drive/api/files_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBytes, StrictInt, StrictStr, constr, validator
+from pydantic.v1 import Field, StrictBytes, StrictInt, StrictStr, constr, validator
 
 from typing import Union
 
 from lusid_drive.models.storage_object import StorageObject
 from lusid_drive.models.update_file import UpdateFile
 
 from lusid_drive.api_client import ApiClient
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/api/folders_api.py` & `lusid_drive_sdk-2.1.1/lusid_drive/api/folders_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBool, StrictInt, StrictStr, conlist, constr, validator
+from pydantic.v1 import Field, StrictBool, StrictInt, StrictStr, conlist, constr, validator
 
 from typing import Optional
 
 from lusid_drive.models.create_folder import CreateFolder
 from lusid_drive.models.paged_resource_list_of_storage_object import PagedResourceListOfStorageObject
 from lusid_drive.models.storage_object import StorageObject
 from lusid_drive.models.update_folder import UpdateFolder
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/api/search_api.py` & `lusid_drive_sdk-2.1.1/lusid_drive/api/search_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictInt, StrictStr, conlist, constr, validator
+from pydantic.v1 import Field, StrictInt, StrictStr, conlist, constr, validator
 
 from typing import Optional
 
 from lusid_drive.models.paged_resource_list_of_storage_object import PagedResourceListOfStorageObject
 from lusid_drive.models.search_body import SearchBody
 
 from lusid_drive.api_client import ApiClient
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/api_client.py` & `lusid_drive_sdk-2.1.1/lusid_drive/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
         if query_params:
             query_params = self.sanitize_for_serialization(query_params)
             url_query = self.parameters_to_url_query(query_params,
                                                      collection_formats)
             url += "?" + url_query
 
         try:
+            # if returning http_data_only then we need to deserialise response.
+            _preload_content = True if _return_http_data_only else _preload_content
             # perform request and return response
             response_data = await self.request(
                 method, url,
                 query_params=query_params,
                 headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
@@ -256,16 +258,16 @@
               return_data = None
 
         if _return_http_data_only:
             return return_data
         else:
             return ApiResponse(status_code = response_data.status,
                            data = return_data,
-                           headers = response_data.getheaders(),
-                           raw_data = response_data.data)
+                           headers = response_data.getheaders() if _preload_content else response_data.headers,
+                           raw_data = response_data.data if _preload_content else response_data)
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/api_response.py` & `lusid_drive_sdk-2.1.1/lusid_drive/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/configuration.py` & `lusid_drive_sdk-2.1.1/lusid_drive/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_drive-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.602\n"\
+               "Version of the API: 0.1.627\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/exceptions.py` & `lusid_drive_sdk-2.1.1/lusid_drive/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,16 @@
         if query_params:
             query_params = self.sanitize_for_serialization(query_params)
             url_query = self.parameters_to_url_query(query_params,
                                                      collection_formats)
             url += "?" + url_query
 
         try:
+            # if returning http_data_only then we need to deserialise response.
+            _preload_content = True if _return_http_data_only else _preload_content
             # perform request and return response
             response_data = self.request(
                 method, url,
                 query_params=query_params,
                 headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client_factory.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/api_client_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,38 +180,43 @@
         An aiohttp.ClientSession, pass this to re-use 
         connections across different ApiFactories,
         by default None
         trace_configs: Optional[List[TraceConfig]], optional
         A list of aiohttp TraceConfigs, used to set up request tracing.
         by default None
         """
+        is_owner = True
         api_config = get_api_configuration(config_loaders=config_loaders)
         api_client_config = api_config.build_api_client_config(
             tcp_keep_alive=tcp_keep_alive,
             socket_options=socket_options,
             id_provider_response_handler=id_provider_response_handler
         )
         self.__api_client = ApiClient(
             configuration=api_client_config,
         )
         rc = self.__api_client.rest_client
         try:
             if client_session is not None:
                 connector = client_session.connector
+                is_owner = False
                 # by default take explicitly passed trace_config param
                 # otherwise copy from session.
                 trace_configs = trace_configs or client_session.trace_configs
             else:
                 connector = rc.pool_manager.connector
             if tcp_keep_alive:
                 connector = TcpKeepAliveConnector(connector=connector, socket_options=socket_options)
+            # dereference connector so existing session closes correctly
+            rc.pool_manager._connector = None
             rc.pool_manager = ClientSession(
                 connector=connector,
                 trust_env=True,
-                trace_configs=trace_configs
+                trace_configs=trace_configs,
+                connector_owner=is_owner
             )
         except AttributeError:
             logger.exception("client_session must be an aiohttp.ClientSession"
                              " object with an initialised TCP Connector")
         rest_client_wrapper = RetryingRestWrapperAsync
         wrapped_rest_client = rest_client_wrapper(rc)
         self.__api_client.rest_client = wrapped_rest_client
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_configuration.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/api_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import logging
 from typing import Optional, Union, Tuple, Any, Callable
 from lusid_drive.configuration import Configuration
 from lusid_drive.extensions.refreshing_token import RefreshingToken
 from lusid_drive.extensions.socket_keep_alive import keep_alive_socket_options
+from lusid_drive.extensions.proxy_config import ProxyConfig
 from requests import Response
 logger = logging.getLogger(__name__)
 
 
 class ApiConfiguration:
     def __init__(
         self,
@@ -15,15 +16,15 @@
         api_url=None,
         username=None,
         password=None,
         client_id=None,
         client_secret=None,
         app_name=None,
         certificate_filename=None,
-        proxy_config=None,
+        proxy_config:Optional[ProxyConfig]=None,
         access_token=None,
     ):
         """
         The configuration required to access LUSID, read more at https://support.finbourne.com/getting-started-with-apis-sdks
 
         :param str token_url: The token URL of the identity provider
         :param str api_url: The API URL for the LUSID client
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/configuration_loaders.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/configuration_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,15 @@
             if value is not None
         }
         config.update(loaded_config)
     proxy_address = config.pop("proxy_address", None)
     proxy_username = config.pop("proxy_username", None)
     proxy_password = config.pop("proxy_password", None)
     # If the proxy address is missing ensure that no proxy is used in the ApiConfiguration
-    if all(
-        (item is not None for item in (proxy_address, proxy_password, proxy_username))
-    ):
+    if proxy_address is not None:
         config["proxy_config"] = ProxyConfig(
             address=proxy_address, username=proxy_username, password=proxy_password
         )
     else:
         config["proxy_config"] = None
     # Create and return the ApiConfiguration
     return ApiConfiguration(**config)
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/proxy_config.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/proxy_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib3 import make_headers
-from typing import Any
+from typing import Dict
 
 
 class ProxyConfig:
     """
     This class is used to hold the proxy configuration details
     """
 
@@ -52,18 +52,21 @@
             index = self.address.index("://")
 
             proxy_url = f"{self.address[0:index + 3]}{self.username}:{self.password}@{self.address[index + 3:]}"
 
         return {"http": proxy_url, "https": proxy_url}
 
     @property
-    def headers(self) -> Any:
+    def headers(self) -> Dict[str, str]:
         """Return Proxy auth headers
 
         Returns
         -------
         Any
             Proxy auth headers
         """
-        return make_headers(
-            proxy_basic_auth=f"{self.__username}:{self.__password}"
-        )
+        if self.__username is not None and self.__password is not None:
+            return make_headers(
+                proxy_basic_auth=f"{self.__username}:{self.__password}"
+            )
+        else:
+            return {}
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/refreshing_token.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/rest.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/retry.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/socket_keep_alive.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/extensions/tcp_keep_alive_connector.py` & `lusid_drive_sdk-2.1.1/lusid_drive/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_action.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from lusid_drive.models.action_id import ActionId
 from lusid_drive.models.id_selector_definition import IdSelectorDefinition
 from lusid_drive.models.link import Link
 
 class AccessControlledAction(BaseModel):
     """
     AccessControlledAction
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_resource.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/access_controlled_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_drive.models.access_controlled_action import AccessControlledAction
 from lusid_drive.models.identifier_part_schema import IdentifierPartSchema
 from lusid_drive.models.link import Link
 
 class AccessControlledResource(BaseModel):
     """
     AccessControlledResource
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/action_id.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/action_id.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class ActionId(BaseModel):
     """
     ActionId
     """
     scope: constr(strict=True, max_length=100, min_length=3) = Field(...)
     activity: constr(strict=True, max_length=25, min_length=3) = Field(...)
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/create_folder.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/create_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class CreateFolder(BaseModel):
     """
     DTO representing the creation of a folder  # noqa: E501
     """
     path: constr(strict=True, max_length=512, min_length=1) = Field(..., description="Path of the created folder")
     name: constr(strict=True, max_length=50, min_length=1) = Field(..., description="Name of the created folder")
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/id_selector_definition.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_drive.models.action_id import ActionId
 
 class IdSelectorDefinition(BaseModel):
     """
     IdSelectorDefinition
     """
     identifier: Dict[str, StrictStr] = Field(...)
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/identifier_part_schema.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt, conlist, constr
 from lusid_drive.models.link import Link
 
 class IdentifierPartSchema(BaseModel):
     """
     IdentifierPartSchema
     """
     index: StrictInt = Field(...)
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/link.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/link.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class Link(BaseModel):
     """
     Link
     """
     relation: StrictStr = Field(...)
     href: StrictStr = Field(...)
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_problem_details.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/lusid_problem_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, constr
 
 class LusidProblemDetails(BaseModel):
     """
     LusidProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_validation_problem_details.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, constr
 
 class LusidValidationProblemDetails(BaseModel):
     """
     LusidValidationProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/paged_resource_list_of_storage_object.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/paged_resource_list_of_storage_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_drive.models.link import Link
 from lusid_drive.models.storage_object import StorageObject
 
 class PagedResourceListOfStorageObject(BaseModel):
     """
     PagedResourceListOfStorageObject
     """
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/resource_list_of_access_controlled_resource.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from lusid_drive.models.access_controlled_resource import AccessControlledResource
 from lusid_drive.models.link import Link
 
 class ResourceListOfAccessControlledResource(BaseModel):
     """
     ResourceListOfAccessControlledResource
     """
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/search_body.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/search_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class SearchBody(BaseModel):
     """
     DTO representing the search query  # noqa: E501
     """
     with_path: Optional[constr(strict=True, max_length=512, min_length=1)] = Field(None, alias="withPath", description="Optional path field to limit the search to result with a matching (case insensitive) path")
     name: constr(strict=True, max_length=256, min_length=1) = Field(..., description="Name of the file or folder to be searched")
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/storage_object.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/storage_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, constr, validator
 from lusid_drive.models.link import Link
 
 class StorageObject(BaseModel):
     """
     An object representation of a drive file or folder  # noqa: E501
     """
     id: constr(strict=True, max_length=40, min_length=30) = Field(..., description="File or folder identifier")
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/update_file.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/update_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class UpdateFile(BaseModel):
     """
     DTO representing the update of the name or path of a file  # noqa: E501
     """
     path: constr(strict=True, max_length=512, min_length=1) = Field(..., description="Path of the updated file")
     name: constr(strict=True, max_length=256, min_length=1) = Field(..., description="Name of the updated file")
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/models/update_folder.py` & `lusid_drive_sdk-2.1.1/lusid_drive/models/update_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class UpdateFolder(BaseModel):
     """
     DTO representing the update of the name or path of a file  # noqa: E501
     """
     path: constr(strict=True, max_length=512, min_length=1) = Field(..., description="Path of the updated folder")
     name: constr(strict=True, max_length=50, min_length=1) = Field(..., description="Name of the updated folder")
```

### Comparing `lusid_drive_sdk-2.0.9/lusid_drive/rest.py` & `lusid_drive_sdk-2.1.1/lusid_drive/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,18 @@
         # url already contains the URL query string
         # so reset query_params to empty dict
         query_params = {}
         timeout = _request_timeout or 5 * 60
 
         if 'Content-Type' not in headers:
             headers['Content-Type'] = 'application/json'
-
+        
+        for content in headers:
+            headers[content] = str(headers[content])
+            
         args = {
             "method": method,
             "url": url,
             "timeout": timeout,
             "headers": headers
         }
 
@@ -155,15 +158,15 @@
                     else:
                         data.add_field(k, v)
                 args["data"] = data
 
             # Pass a `bytes` parameter directly in the body to support
             # other content types than Json when `body` argument is provided
             # in serialized form
-            elif isinstance(body, bytes):
+            elif isinstance(body, str) or isinstance(body, bytes):
                 args["data"] = body
             else:
                 # Cannot generate the request from given parameters
                 msg = """Cannot prepare a request message for provided
                          arguments. Please check that your arguments match
                          declared content type."""
                 raise ApiException(status=0, reason=msg)
```

### Comparing `lusid_drive_sdk-2.0.9/pyproject.toml` & `lusid_drive_sdk-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-drive-sdk"
-version = "2.0.9"
+version = "2.1.1"
 description = "FINBOURNE Drive API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/drive-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Drive API", "lusid-drive-sdk"]
 packages = [
@@ -15,15 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 
 urllib3 = "^1.25.3"
 python-dateutil = "^2.8.2"
 requests = "^2"
 aiohttp = "^3.8.4"
-pydantic = "^1.10.5"
+pydantic = "^2.6.3"
 aenum = "^3.1.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0"
 flake8 = "^4.0.0"
 black = "^23.9.1"
```

### Comparing `lusid_drive_sdk-2.0.9/PKG-INFO` & `lusid_drive_sdk-2.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-drive-sdk
-Version: 2.0.9
+Version: 2.1.1
 Summary: FINBOURNE Drive API
 Home-page: https://github.com/finbourne/drive-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Drive API,lusid-drive-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aenum (>=3.1.11,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
 Project-URL: Repository, https://github.com/finbourne/drive-sdk-python
 Description-Content-Type: text/markdown
 
 # lusid-drive-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.602
-- Package version: 2.0.9
+- API version: 0.1.627
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -69,29 +69,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the lusid_drive application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_LUSID_DRIVE_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_LUSID_DRIVE_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to lusid_drive via a proxy, by setting `FBN_PROXY_ADDRESS`. 
+If your proxy has basic auth enabled, you must akso supply `FBN_PROXY_USERNAME` and `FBN_PROXY_PASSWORD`
+
+### Secrets file
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set in a `secrets.json` file in the same folder as your script.
+
+``` 
+{
+    "api":
+    {
+        "tokenUrl":"<your-token-url>",
+        "lusid_driveUrl":"<FINBOURNE-application-url>",
+        "username":"<your-username>",
+        "password":"<your-password>",
+        "clientId":"<your-client-id>",
+        "clientSecret":"<your-client-secret>",
+    }
+}
+```
+
+To use a long lived Personal Access Token, you must provide a `secrets.json` with the following variables:
+``` 
+{
+    "api":
+    {
+        "lusid_driveUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to lusid_drive via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "lusid_driveUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    },
+    "proxy":
+    {
+        "address":"<your-proxy-address>",
+        "username":"<your-proxy-username>",
+        "password":"<your-proxy-password>"
+    }
+}
+```
+
+### Using the SDK
+
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
 import lusid_drive
-from lusid_drive.rest import ApiException
+from lusid_drive.exceptions import ApiException
 from pprint import pprint
 
+import os
 from lusid_drive import (
-	  ApiClientFactory,
-	  ApplicationMetadataApi,
-	  EnvironmentVariablesConfigurationLoader,
-	  SecretsFileConfigurationLoader,
-	  ArgsConfigurationLoader
+    ApiClientFactory,
+    ApplicationMetadataApi,
+    EnvironmentVariablesConfigurationLoader,
+    SecretsFileConfigurationLoader,
+    ArgsConfigurationLoader
 )
 
 # Use the lusid_drive ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -116,15 +192,15 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = lusid_drive.ApplicationMetadataApi(api_client)
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
         # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
```

