# Comparing `tmp/lusid_configuration_sdk-2.1.1.tar.gz` & `tmp/lusid_configuration_sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_configuration_sdk-2.1.1.tar", max compression
+gzip compressed data, was "lusid_configuration_sdk-2.1.2.tar", max compression
```

## Comparing `lusid_configuration_sdk-2.1.1.tar` & `lusid_configuration_sdk-2.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11457 2024-04-10 10:43:05.976283 lusid_configuration_sdk-2.1.1/README.md
--rw-r--r--   0        0        0     4232 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/__init__.py
--rw-r--r--   0        0        0      284 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api/__init__.py
--rw-r--r--   0        0        0     7566 2024-04-10 10:43:05.972283 lusid_configuration_sdk-2.1.1/lusid_configuration/api/application_metadata_api.py
--rw-r--r--   0        0        0   138077 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api/configuration_sets_api.py
--rw-r--r--   0        0        0    30832 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api_client.py
--rw-r--r--   0        0        0      852 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/api_response.py
--rw-r--r--   0        0        0    14483 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/configuration.py
--rw-r--r--   0        0        0     5351 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/exceptions.py
--rw-r--r--   0        0        0      602 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/__init__.py
--rw-r--r--   0        0        0    30704 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client.py
--rw-r--r--   0        0        0     9912 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8122 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_configuration.py
--rw-r--r--   0        0        0     6816 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12712 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/rest.py
--rw-r--r--   0        0        0    11578 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3891 2024-04-10 10:43:05.974283 lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     2879 2024-04-10 10:43:05.972283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/__init__.py
--rw-r--r--   0        0        0     3930 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_action.py
--rw-r--r--   0        0        0     4873 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2082 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/action_id.py
--rw-r--r--   0        0        0     4739 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item.py
--rw-r--r--   0        0        0     3483 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item_summary.py
--rw-r--r--   0        0        0     5226 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set.py
--rw-r--r--   0        0        0     3093 2024-04-10 10:43:05.970283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set_summary.py
--rw-r--r--   0        0        0     4236 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_item.py
--rw-r--r--   0        0        0     2829 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_set.py
--rw-r--r--   0        0        0     3197 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/id_selector_definition.py
--rw-r--r--   0        0        0     3122 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2274 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/link.py
--rw-r--r--   0        0        0     3869 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4705 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3411 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/personal_access_token.py
--rw-r--r--   0        0        0     2089 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_id.py
--rw-r--r--   0        0        0     4277 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4192 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_item.py
--rw-r--r--   0        0        0     4180 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set.py
--rw-r--r--   0        0        0     4265 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set_summary.py
--rw-r--r--   0        0        0     2781 2024-04-10 10:43:05.971283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_item.py
--rw-r--r--   0        0        0     2310 2024-04-10 10:43:05.972283 lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_set.py
--rw-r--r--   0        0        0        0 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/py.typed
--rw-r--r--   0        0        0    10177 2024-04-10 10:43:05.973283 lusid_configuration_sdk-2.1.1/lusid_configuration/rest.py
--rw-r--r--   0        0        0      904 2024-04-10 10:43:05.977283 lusid_configuration_sdk-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    12546 1970-01-01 00:00:00.000000 lusid_configuration_sdk-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11457 2024-04-10 12:35:32.220610 lusid_configuration_sdk-2.1.2/README.md
+-rw-r--r--   0        0        0     4232 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/api/__init__.py
+-rw-r--r--   0        0        0     7566 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/api/application_metadata_api.py
+-rw-r--r--   0        0        0   138077 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/api/configuration_sets_api.py
+-rw-r--r--   0        0        0    30832 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/api_response.py
+-rw-r--r--   0        0        0    14483 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/configuration.py
+-rw-r--r--   0        0        0     5351 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/exceptions.py
+-rw-r--r--   0        0        0      602 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/__init__.py
+-rw-r--r--   0        0        0    30704 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/api_client.py
+-rw-r--r--   0        0        0     9912 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8122 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6816 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12712 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/rest.py
+-rw-r--r--   0        0        0    11578 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3891 2024-04-10 12:35:32.218610 lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     2879 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/__init__.py
+-rw-r--r--   0        0        0     3930 2024-04-10 12:35:32.214610 lusid_configuration_sdk-2.1.2/lusid_configuration/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4873 2024-04-10 12:35:32.214610 lusid_configuration_sdk-2.1.2/lusid_configuration/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2082 2024-04-10 12:35:32.215611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/action_id.py
+-rw-r--r--   0        0        0     4739 2024-04-10 12:35:32.215611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_item.py
+-rw-r--r--   0        0        0     3483 2024-04-10 12:35:32.215611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_item_summary.py
+-rw-r--r--   0        0        0     5226 2024-04-10 12:35:32.215611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_set.py
+-rw-r--r--   0        0        0     3093 2024-04-10 12:35:32.215611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_set_summary.py
+-rw-r--r--   0        0        0     4236 2024-04-10 12:35:32.215611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/create_configuration_item.py
+-rw-r--r--   0        0        0     2829 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/create_configuration_set.py
+-rw-r--r--   0        0        0     3197 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3122 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2274 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/link.py
+-rw-r--r--   0        0        0     3869 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4705 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3411 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/personal_access_token.py
+-rw-r--r--   0        0        0     2089 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_id.py
+-rw-r--r--   0        0        0     4277 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4192 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_configuration_item.py
+-rw-r--r--   0        0        0     4180 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_configuration_set.py
+-rw-r--r--   0        0        0     4265 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_configuration_set_summary.py
+-rw-r--r--   0        0        0     2781 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/update_configuration_item.py
+-rw-r--r--   0        0        0     2310 2024-04-10 12:35:32.216611 lusid_configuration_sdk-2.1.2/lusid_configuration/models/update_configuration_set.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/py.typed
+-rw-r--r--   0        0        0    10177 2024-04-10 12:35:32.217610 lusid_configuration_sdk-2.1.2/lusid_configuration/rest.py
+-rw-r--r--   0        0        0      904 2024-04-10 12:35:32.220610 lusid_configuration_sdk-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12546 1970-01-01 00:00:00.000000 lusid_configuration_sdk-2.1.2/PKG-INFO
```

### Comparing `lusid_configuration_sdk-2.1.1/README.md` & `lusid_configuration_sdk-2.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-configuration-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.518
-- Package version: 2.1.1
+- API version: 0.1.519
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/__init__.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/api/application_metadata_api.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/api/configuration_sets_api.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/api/configuration_sets_api.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/api_client.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/api_response.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/configuration.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_configuration-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.518\n"\
+               "Version of the API: 0.1.519\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/exceptions.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/__init__.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_client_factory.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/api_configuration.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/configuration_loaders.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/proxy_config.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/refreshing_token.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/rest.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/retry.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/socket_keep_alive.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/extensions/tcp_keep_alive_connector.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/__init__.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_action.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/access_controlled_resource.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/action_id.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_item_summary.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_item_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/configuration_set_summary.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/configuration_set_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_item.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/create_configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/create_configuration_set.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/create_configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/id_selector_definition.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/identifier_part_schema.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/link.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_problem_details.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/lusid_validation_problem_details.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/personal_access_token.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_id.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_access_controlled_resource.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_item.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/resource_list_of_configuration_set_summary.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/resource_list_of_configuration_set_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_item.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/update_configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/models/update_configuration_set.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/models/update_configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/lusid_configuration/rest.py` & `lusid_configuration_sdk-2.1.2/lusid_configuration/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.1.1/pyproject.toml` & `lusid_configuration_sdk-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-configuration-sdk"
-version = "2.1.1"
+version = "2.1.2"
 description = "FINBOURNE ConfigurationService API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/configuration-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE ConfigurationService API", "lusid-configuration-sdk"]
 packages = [
```

### Comparing `lusid_configuration_sdk-2.1.1/PKG-INFO` & `lusid_configuration_sdk-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-configuration-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: FINBOURNE ConfigurationService API
 Home-page: https://github.com/finbourne/configuration-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE ConfigurationService API,lusid-configuration-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-configuration-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.518
-- Package version: 2.1.1
+- API version: 0.1.519
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```
