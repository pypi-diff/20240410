# Comparing `tmp/lusid_configuration_sdk-2.0.9.tar.gz` & `tmp/lusid_configuration_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_configuration_sdk-2.0.9.tar", max compression
+gzip compressed data, was "lusid_configuration_sdk-2.1.1.tar", max compression
```

## Comparing `lusid_configuration_sdk-2.0.9.tar` & `lusid_configuration_sdk-2.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     9255 2024-02-01 16:09:12.248072 lusid_configuration_sdk-2.0.9/README.md
--rw-r--r--   0        0        0     2940 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/__init__.py
--rw-r--r--   0        0        0      212 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/api/__init__.py
--rw-r--r--   0        0        0     7563 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/api/application_metadata_api.py
--rw-r--r--   0        0        0   138071 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/api/configuration_sets_api.py
--rw-r--r--   0        0        0    30832 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/api_client.py
--rw-r--r--   0        0        0      852 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/api_response.py
--rw-r--r--   0        0        0    14483 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/configuration.py
--rw-r--r--   0        0        0     5351 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/exceptions.py
--rw-r--r--   0        0        0      304 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/__init__.py
--rw-r--r--   0        0        0    30704 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client.py
--rw-r--r--   0        0        0     9813 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8032 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_configuration.py
--rw-r--r--   0        0        0     6888 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12712 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/rest.py
--rw-r--r--   0        0        0    11578 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3891 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     2207 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/__init__.py
--rw-r--r--   0        0        0     3927 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_action.py
--rw-r--r--   0        0        0     4870 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2079 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/action_id.py
--rw-r--r--   0        0        0     4736 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item.py
--rw-r--r--   0        0        0     3480 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item_summary.py
--rw-r--r--   0        0        0     5223 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set.py
--rw-r--r--   0        0        0     3090 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set_summary.py
--rw-r--r--   0        0        0     4233 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_item.py
--rw-r--r--   0        0        0     2826 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_set.py
--rw-r--r--   0        0        0     3194 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/id_selector_definition.py
--rw-r--r--   0        0        0     3119 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2271 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/link.py
--rw-r--r--   0        0        0     3866 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4702 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3408 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/personal_access_token.py
--rw-r--r--   0        0        0     2086 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_id.py
--rw-r--r--   0        0        0     4274 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4189 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_item.py
--rw-r--r--   0        0        0     4177 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set.py
--rw-r--r--   0        0        0     4262 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set_summary.py
--rw-r--r--   0        0        0     2778 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_item.py
--rw-r--r--   0        0        0     2307 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_set.py
--rw-r--r--   0        0        0        0 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/py.typed
--rw-r--r--   0        0        0    10046 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/rest.py
--rw-r--r--   0        0        0      905 2024-02-01 16:09:12.248072 lusid_configuration_sdk-2.0.9/pyproject.toml
--rw-r--r--   0        0        0    10345 1970-01-01 00:00:00.000000 lusid_configuration_sdk-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11457 2024-04-10 10:43:05.976283 lusid_configuration_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     4232 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api/__init__.py
+-rw-r--r--   0        0        0     7566 2024-04-10 10:43:05.972283 lusid_configuration_sdk-2.1.1/lusid_configuration/api/application_metadata_api.py
+-rw-r--r--   0        0        0   138077 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api/configuration_sets_api.py
+-rw-r--r--   0        0        0    30832 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api_response.py
+-rw-r--r--   0        0        0    14483 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/configuration.py
+-rw-r--r--   0        0        0     5351 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/exceptions.py
+-rw-r--r--   0        0        0      602 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/__init__.py
+-rw-r--r--   0        0        0    30704 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client.py
+-rw-r--r--   0        0        0     9912 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8122 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6816 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12712 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/rest.py
+-rw-r--r--   0        0        0    11578 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3891 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     2879 2024-04-10 10:43:05.972283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/__init__.py
+-rw-r--r--   0        0        0     3930 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4873 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2082 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/action_id.py
+-rw-r--r--   0        0        0     4739 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item.py
+-rw-r--r--   0        0        0     3483 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item_summary.py
+-rw-r--r--   0        0        0     5226 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set.py
+-rw-r--r--   0        0        0     3093 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set_summary.py
+-rw-r--r--   0        0        0     4236 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_item.py
+-rw-r--r--   0        0        0     2829 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_set.py
+-rw-r--r--   0        0        0     3197 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3122 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2274 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/link.py
+-rw-r--r--   0        0        0     3869 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4705 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3411 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/personal_access_token.py
+-rw-r--r--   0        0        0     2089 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_id.py
+-rw-r--r--   0        0        0     4277 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4192 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_item.py
+-rw-r--r--   0        0        0     4180 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set.py
+-rw-r--r--   0        0        0     4265 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set_summary.py
+-rw-r--r--   0        0        0     2781 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_item.py
+-rw-r--r--   0        0        0     2310 2024-04-10 10:43:05.972283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_set.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/py.typed
+-rw-r--r--   0        0        0    10177 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/rest.py
+-rw-r--r--   0        0        0      904 2024-04-10 10:43:05.977283 lusid_configuration_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12546 1970-01-01 00:00:00.000000 lusid_configuration_sdk-2.1.1/PKG-INFO
```

### Comparing `lusid_configuration_sdk-2.0.9/README.md` & `lusid_configuration_sdk-2.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-configuration-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.492
-- Package version: 2.0.9
+- API version: 0.1.518
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -43,29 +43,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the lusid_configuration application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_LUSID_CONFIGURATION_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_LUSID_CONFIGURATION_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to lusid_configuration via a proxy, by setting `FBN_PROXY_ADDRESS`. 
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
+        "lusid_configurationUrl":"<FINBOURNE-application-url>",
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
+        "lusid_configurationUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to lusid_configuration via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "lusid_configurationUrl":"<FINBOURNE-application-url>",
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
 import lusid_configuration
-from lusid_configuration.rest import ApiException
+from lusid_configuration.exceptions import ApiException
 from pprint import pprint
 
+import os
 from lusid_configuration import (
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
 
 # Use the lusid_configuration ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -90,15 +166,15 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = lusid_configuration.ApplicationMetadataApi(api_client)
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
         # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/__init__.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
     Contact: info@finbourne.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-from __future__ import absolute_import
-
-# import apis into sdk package
-from lusid_configuration.api.application_metadata_api import ApplicationMetadataApi
-from lusid_configuration.api.configuration_sets_api import ConfigurationSetsApi
-
-# import ApiClient
-from lusid_configuration.api_client import ApiClient
-from lusid_configuration.configuration import Configuration
-from lusid_configuration.exceptions import OpenApiException
-from lusid_configuration.exceptions import ApiTypeError
-from lusid_configuration.exceptions import ApiValueError
-from lusid_configuration.exceptions import ApiKeyError
-from lusid_configuration.exceptions import ApiException
-# import models into sdk package
+# import models into model package
 from lusid_configuration.models.access_controlled_action import AccessControlledAction
 from lusid_configuration.models.access_controlled_resource import AccessControlledResource
 from lusid_configuration.models.action_id import ActionId
 from lusid_configuration.models.configuration_item import ConfigurationItem
 from lusid_configuration.models.configuration_item_summary import ConfigurationItemSummary
 from lusid_configuration.models.configuration_set import ConfigurationSet
 from lusid_configuration.models.configuration_set_summary import ConfigurationSetSummary
@@ -48,9 +33,32 @@
 from lusid_configuration.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_configuration.models.resource_list_of_configuration_item import ResourceListOfConfigurationItem
 from lusid_configuration.models.resource_list_of_configuration_set import ResourceListOfConfigurationSet
 from lusid_configuration.models.resource_list_of_configuration_set_summary import ResourceListOfConfigurationSetSummary
 from lusid_configuration.models.update_configuration_item import UpdateConfigurationItem
 from lusid_configuration.models.update_configuration_set import UpdateConfigurationSet
 
-# import extensions into sdk package
-from lusid_configuration.extensions import *
+
+__all__ = [
+    "AccessControlledAction",
+    "AccessControlledResource",
+    "ActionId",
+    "ConfigurationItem",
+    "ConfigurationItemSummary",
+    "ConfigurationSet",
+    "ConfigurationSetSummary",
+    "CreateConfigurationItem",
+    "CreateConfigurationSet",
+    "IdSelectorDefinition",
+    "IdentifierPartSchema",
+    "Link",
+    "LusidProblemDetails",
+    "LusidValidationProblemDetails",
+    "PersonalAccessToken",
+    "ResourceId",
+    "ResourceListOfAccessControlledResource",
+    "ResourceListOfConfigurationItem",
+    "ResourceListOfConfigurationSet",
+    "ResourceListOfConfigurationSetSummary",
+    "UpdateConfigurationItem",
+    "UpdateConfigurationSet"
+]
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/api/application_metadata_api.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from lusid_configuration.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 
 from lusid_configuration.api_client import ApiClient
 from lusid_configuration.api_response import ApiResponse
 from lusid_configuration.exceptions import (  # noqa: F401
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/api/configuration_sets_api.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/api/configuration_sets_api.py`

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
-from pydantic import Field, StrictBool, StrictStr, constr, validator
+from pydantic.v1 import Field, StrictBool, StrictStr, constr, validator
 
 from typing import Optional
 
 from lusid_configuration.models.configuration_item import ConfigurationItem
 from lusid_configuration.models.configuration_set import ConfigurationSet
 from lusid_configuration.models.create_configuration_item import CreateConfigurationItem
 from lusid_configuration.models.create_configuration_set import CreateConfigurationSet
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/api_client.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/api_response.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/configuration.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_configuration-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.492\n"\
+               "Version of the API: 0.1.518\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/exceptions.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client_factory.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,40 +180,43 @@
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
             # dereference connector so existing session closes correctly
             rc.pool_manager._connector = None
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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_configuration.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import logging
 from typing import Optional, Union, Tuple, Any, Callable
 from lusid_configuration.configuration import Configuration
 from lusid_configuration.extensions.refreshing_token import RefreshingToken
 from lusid_configuration.extensions.socket_keep_alive import keep_alive_socket_options
+from lusid_configuration.extensions.proxy_config import ProxyConfig
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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/configuration_loaders.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/configuration_loaders.py`

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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/proxy_config.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/proxy_config.py`

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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/refreshing_token.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/rest.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/retry.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/socket_keep_alive.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/tcp_keep_alive_connector.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_action.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from lusid_configuration.models.action_id import ActionId
 from lusid_configuration.models.id_selector_definition import IdSelectorDefinition
 from lusid_configuration.models.link import Link
 
 class AccessControlledAction(BaseModel):
     """
     AccessControlledAction
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_resource.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_resource.py`

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
 from lusid_configuration.models.access_controlled_action import AccessControlledAction
 from lusid_configuration.models.identifier_part_schema import IdentifierPartSchema
 from lusid_configuration.models.link import Link
 
 class AccessControlledResource(BaseModel):
     """
     AccessControlledResource
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/action_id.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/action_id.py`

 * *Files 5% similar despite different names*

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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist, constr
 from lusid_configuration.models.link import Link
 
 class ConfigurationItem(BaseModel):
     """
     The full version of the configuration item  # noqa: E501
     """
     created_at: datetime = Field(..., alias="createdAt", description="The date referring to the creation date of the configuration item")
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item_summary.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, conlist, constr
 from lusid_configuration.models.link import Link
 
 class ConfigurationItemSummary(BaseModel):
     """
     A single configuration object  # noqa: E501
     """
     key: constr(strict=True, min_length=1) = Field(..., description="The key which identifies the configuration item")
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid_configuration.models.configuration_item_summary import ConfigurationItemSummary
 from lusid_configuration.models.link import Link
 from lusid_configuration.models.resource_id import ResourceId
 
 class ConfigurationSet(BaseModel):
     """
     The full version of the configuration set  # noqa: E501
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set_summary.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from lusid_configuration.models.link import Link
 from lusid_configuration.models.resource_id import ResourceId
 
 class ConfigurationSetSummary(BaseModel):
     """
     A group of configuration items  # noqa: E501
     """
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_item.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, constr, validator
 
 class CreateConfigurationItem(BaseModel):
     """
     The information required to create a configuration item  # noqa: E501
     """
     key: constr(strict=True, max_length=256, min_length=1) = Field(..., description="The key of the new configuration item")
     value: constr(strict=True, max_length=2000000, min_length=1) = Field(..., description="The value of the new configuration item                The maximum size for secrets is 4KB and for text values is 2MB")
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_set.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 from lusid_configuration.models.resource_id import ResourceId
 
 class CreateConfigurationSet(BaseModel):
     """
     The information required to create a new configuration set  # noqa: E501
     """
     id: ResourceId = Field(...)
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/id_selector_definition.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/id_selector_definition.py`

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
 from lusid_configuration.models.action_id import ActionId
 
 class IdSelectorDefinition(BaseModel):
     """
     IdSelectorDefinition
     """
     identifier: Dict[str, StrictStr] = Field(...)
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/identifier_part_schema.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/identifier_part_schema.py`

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
 from lusid_configuration.models.link import Link
 
 class IdentifierPartSchema(BaseModel):
     """
     IdentifierPartSchema
     """
     index: StrictInt = Field(...)
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/link.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/link.py`

 * *Files 4% similar despite different names*

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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_problem_details.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_problem_details.py`

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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_validation_problem_details.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_validation_problem_details.py`

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

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/personal_access_token.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/personal_access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from lusid_configuration.models.link import Link
 
 class PersonalAccessToken(BaseModel):
     """
     Representation of a Personal Access Token under a Configuration Item format.  # noqa: E501
     """
     value: constr(strict=True, min_length=1) = Field(..., description="Value of the Personal Access Token.")
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_id.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class ResourceId(BaseModel):
     """
     Identifiers of an entity  # noqa: E501
     """
     scope: constr(strict=True, max_length=512, min_length=1) = Field(..., description="The scope used to identify an entity")
     code: constr(strict=True, max_length=512, min_length=1) = Field(..., description="The code used to identify an entity")
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_access_controlled_resource.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_access_controlled_resource.py`

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
 from lusid_configuration.models.access_controlled_resource import AccessControlledResource
 from lusid_configuration.models.link import Link
 
 class ResourceListOfAccessControlledResource(BaseModel):
     """
     ResourceListOfAccessControlledResource
     """
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_item.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_item.py`

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
 from lusid_configuration.models.configuration_item import ConfigurationItem
 from lusid_configuration.models.link import Link
 
 class ResourceListOfConfigurationItem(BaseModel):
     """
     ResourceListOfConfigurationItem
     """
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set.py`

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
 from lusid_configuration.models.configuration_set import ConfigurationSet
 from lusid_configuration.models.link import Link
 
 class ResourceListOfConfigurationSet(BaseModel):
     """
     ResourceListOfConfigurationSet
     """
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set_summary.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set_summary.py`

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
 from lusid_configuration.models.configuration_set_summary import ConfigurationSetSummary
 from lusid_configuration.models.link import Link
 
 class ResourceListOfConfigurationSetSummary(BaseModel):
     """
     ResourceListOfConfigurationSetSummary
     """
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_item.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class UpdateConfigurationItem(BaseModel):
     """
     The information required to update a configuration item  # noqa: E501
     """
     value: constr(strict=True, max_length=2000000, min_length=1) = Field(..., description="The new value of the configuration item")
     description: Optional[constr(strict=True, max_length=255, min_length=0)] = Field(None, description="The new description of the configuration item")
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_set.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class UpdateConfigurationSet(BaseModel):
     """
     The information required to update a configuration set  # noqa: E501
     """
     description: Optional[constr(strict=True, max_length=255, min_length=0)] = Field(None, description="The new description of the configuration set")
     __properties = ["description"]
```

### Comparing `lusid_configuration_sdk-2.0.9/lusid_configuration/rest.py` & `lusid_configuration_sdk-2.1.1/lusid_configuration/rest.py`

 * *Files 8% similar despite different names*

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

### Comparing `lusid_configuration_sdk-2.0.9/pyproject.toml` & `lusid_configuration_sdk-2.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-configuration-sdk"
-version = "2.0.9"
+version = "2.1.1"
 description = "FINBOURNE ConfigurationService API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/configuration-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE ConfigurationService API", "lusid-configuration-sdk"]
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

### Comparing `lusid_configuration_sdk-2.0.9/PKG-INFO` & `lusid_configuration_sdk-2.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-configuration-sdk
-Version: 2.0.9
+Version: 2.1.1
 Summary: FINBOURNE ConfigurationService API
 Home-page: https://github.com/finbourne/configuration-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE ConfigurationService API,lusid-configuration-sdk
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
 Project-URL: Repository, https://github.com/finbourne/configuration-sdk-python
 Description-Content-Type: text/markdown
 
 # lusid-configuration-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.492
-- Package version: 2.0.9
+- API version: 0.1.518
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -69,29 +69,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the lusid_configuration application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_LUSID_CONFIGURATION_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_LUSID_CONFIGURATION_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to lusid_configuration via a proxy, by setting `FBN_PROXY_ADDRESS`. 
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
+        "lusid_configurationUrl":"<FINBOURNE-application-url>",
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
+        "lusid_configurationUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to lusid_configuration via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "lusid_configurationUrl":"<FINBOURNE-application-url>",
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
 import lusid_configuration
-from lusid_configuration.rest import ApiException
+from lusid_configuration.exceptions import ApiException
 from pprint import pprint
 
+import os
 from lusid_configuration import (
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
 
 # Use the lusid_configuration ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -116,15 +192,15 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = lusid_configuration.ApplicationMetadataApi(api_client)
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
         # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
```

