# Comparing `tmp/finbourne_insights_sdk-2.0.9.tar.gz` & `tmp/finbourne_insights_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_insights_sdk-2.0.9.tar", max compression
+gzip compressed data, was "finbourne_insights_sdk-2.1.1.tar", max compression
```

## Comparing `finbourne_insights_sdk-2.0.9.tar` & `finbourne_insights_sdk-2.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    10647 2024-02-22 10:34:34.037325 finbourne_insights_sdk-2.0.9/README.md
--rw-r--r--   0        0        0     3697 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/__init__.py
--rw-r--r--   0        0        0      395 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/__init__.py
--rw-r--r--   0        0        0    24453 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/access_evaluations_api.py
--rw-r--r--   0        0        0     7547 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/application_metadata_api.py
--rw-r--r--   0        0        0    24163 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/auditing_api.py
--rw-r--r--   0        0        0    35942 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/requests_api.py
--rw-r--r--   0        0        0    36142 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/vendor_logs_api.py
--rw-r--r--   0        0        0    30813 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/api_client.py
--rw-r--r--   0        0        0      852 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/api_response.py
--rw-r--r--   0        0        0    14459 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/configuration.py
--rw-r--r--   0        0        0     5339 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/exceptions.py
--rw-r--r--   0        0        0      302 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/__init__.py
--rw-r--r--   0        0        0    30684 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client.py
--rw-r--r--   0        0        0     9803 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8117 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_configuration.py
--rw-r--r--   0        0        0     6812 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/rest.py
--rw-r--r--   0        0        0    11577 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     2789 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/__init__.py
--rw-r--r--   0        0        0     3912 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_action.py
--rw-r--r--   0        0        0     4855 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_resource.py
--rw-r--r--   0        0        0    11912 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_evaluation_log.py
--rw-r--r--   0        0        0     2067 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/action_id.py
--rw-r--r--   0        0        0     3753 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data.py
--rw-r--r--   0        0        0     2216 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data_summary.py
--rw-r--r--   0        0        0     3448 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry.py
--rw-r--r--   0        0        0     2093 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry_note.py
--rw-r--r--   0        0        0     2776 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process.py
--rw-r--r--   0        0        0     3036 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process_summary.py
--rw-r--r--   0        0        0     2116 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/bucket.py
--rw-r--r--   0        0        0     2516 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/create_audit_entry.py
--rw-r--r--   0        0        0     2594 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/histogram.py
--rw-r--r--   0        0        0     3181 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/id_selector_definition.py
--rw-r--r--   0        0        0     3106 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2259 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/link.py
--rw-r--r--   0        0        0     3854 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4690 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3209 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/problem_details.py
--rw-r--r--   0        0        0     5507 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/request.py
--rw-r--r--   0        0        0     8265 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/request_log.py
--rw-r--r--   0        0        0     2371 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource.py
--rw-r--r--   0        0        0     4260 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4200 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_audit_process_summary.py
--rw-r--r--   0        0        0     4735 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
--rw-r--r--   0        0        0     4635 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
--rw-r--r--   0        0        0     4624 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
--rw-r--r--   0        0        0     5045 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/response.py
--rw-r--r--   0        0        0     2910 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/scrollable_collection_of_audit_entry.py
--rw-r--r--   0        0        0     4517 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_log.py
--rw-r--r--   0        0        0     2794 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_request.py
--rw-r--r--   0        0        0     2820 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_response.py
--rw-r--r--   0        0        0        0 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/py.typed
--rw-r--r--   0        0        0    10033 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/rest.py
--rw-r--r--   0        0        0      872 2024-02-22 10:34:34.037325 finbourne_insights_sdk-2.0.9/pyproject.toml
--rw-r--r--   0        0        0    11701 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0    10629 2024-04-10 10:43:04.484893 finbourne_insights_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     5228 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/__init__.py
+-rw-r--r--   0        0        0      526 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/__init__.py
+-rw-r--r--   0        0        0    24459 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/access_evaluations_api.py
+-rw-r--r--   0        0        0     7550 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/application_metadata_api.py
+-rw-r--r--   0        0        0    24169 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/auditing_api.py
+-rw-r--r--   0        0        0    35948 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/requests_api.py
+-rw-r--r--   0        0        0    36148 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api/vendor_logs_api.py
+-rw-r--r--   0        0        0    30813 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/api_response.py
+-rw-r--r--   0        0        0    14459 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/configuration.py
+-rw-r--r--   0        0        0     5339 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/__init__.py
+-rw-r--r--   0        0        0    30684 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client.py
+-rw-r--r--   0        0        0     9902 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8117 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6812 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2024-04-10 10:43:04.482894 finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     3641 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/__init__.py
+-rw-r--r--   0        0        0     3915 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4858 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_resource.py
+-rw-r--r--   0        0        0    11915 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_evaluation_log.py
+-rw-r--r--   0        0        0     2070 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/action_id.py
+-rw-r--r--   0        0        0     3756 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data.py
+-rw-r--r--   0        0        0     2219 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data_summary.py
+-rw-r--r--   0        0        0     3451 2024-04-10 10:43:04.478894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry.py
+-rw-r--r--   0        0        0     2096 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry_note.py
+-rw-r--r--   0        0        0     2779 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process.py
+-rw-r--r--   0        0        0     3039 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process_summary.py
+-rw-r--r--   0        0        0     2119 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/bucket.py
+-rw-r--r--   0        0        0     2519 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/create_audit_entry.py
+-rw-r--r--   0        0        0     2597 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/histogram.py
+-rw-r--r--   0        0        0     3184 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3109 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2262 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/link.py
+-rw-r--r--   0        0        0     3857 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4693 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3212 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/problem_details.py
+-rw-r--r--   0        0        0     5510 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/request.py
+-rw-r--r--   0        0        0     8268 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/request_log.py
+-rw-r--r--   0        0        0     2374 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource.py
+-rw-r--r--   0        0        0     4263 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4203 2024-04-10 10:43:04.479894 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_audit_process_summary.py
+-rw-r--r--   0        0        0     4738 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
+-rw-r--r--   0        0        0     4638 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
+-rw-r--r--   0        0        0     4627 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
+-rw-r--r--   0        0        0     5048 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/response.py
+-rw-r--r--   0        0        0     2913 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/scrollable_collection_of_audit_entry.py
+-rw-r--r--   0        0        0     4520 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_log.py
+-rw-r--r--   0        0        0     2797 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_request.py
+-rw-r--r--   0        0        0     2823 2024-04-10 10:43:04.480893 finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_response.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/py.typed
+-rw-r--r--   0        0        0    10164 2024-04-10 10:43:04.481893 finbourne_insights_sdk-2.1.1/finbourne_insights/rest.py
+-rw-r--r--   0        0        0      871 2024-04-10 10:43:04.484893 finbourne_insights_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11682 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.1.1/PKG-INFO
```

### Comparing `finbourne_insights_sdk-2.0.9/README.md` & `finbourne_insights_sdk-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.759
-- Package version: 2.0.9
+- API version: 0.0.764
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -56,16 +56,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_FINBOURNE_INSIGHTS_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_FINBOURNE_INSIGHTS_API_URL,
 FBN_ACCESS_TOKEN
 ```
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/api/access_evaluations_api.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/api/access_evaluations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field, StrictStr, conint, constr, validator
+from pydantic.v1 import Field, StrictStr, conint, constr, validator
 
 from typing import Optional
 
 from finbourne_insights.models.access_evaluation_log import AccessEvaluationLog
 from finbourne_insights.models.resource_list_with_histogram_of_access_evaluation_log import ResourceListWithHistogramOfAccessEvaluationLog
 
 from finbourne_insights.api_client import ApiClient
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/api/application_metadata_api.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/api/application_metadata_api.py`

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
 
 from finbourne_insights.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 
 from finbourne_insights.api_client import ApiClient
 from finbourne_insights.api_response import ApiResponse
 from finbourne_insights.exceptions import (  # noqa: F401
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/api/auditing_api.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/api/auditing_api.py`

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
-from pydantic import Field, StrictInt, StrictStr
+from pydantic.v1 import Field, StrictInt, StrictStr
 
 from typing import Optional
 
 from finbourne_insights.models.audit_entry import AuditEntry
 from finbourne_insights.models.create_audit_entry import CreateAuditEntry
 from finbourne_insights.models.resource_list_of_audit_process_summary import ResourceListOfAuditProcessSummary
 from finbourne_insights.models.scrollable_collection_of_audit_entry import ScrollableCollectionOfAuditEntry
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/api/requests_api.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/api/requests_api.py`

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
-from pydantic import Field, StrictStr, conint, constr, validator
+from pydantic.v1 import Field, StrictStr, conint, constr, validator
 
 from typing import Optional
 
 from finbourne_insights.models.request import Request
 from finbourne_insights.models.request_log import RequestLog
 from finbourne_insights.models.resource_list_with_histogram_of_request_log import ResourceListWithHistogramOfRequestLog
 from finbourne_insights.models.response import Response
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/api/vendor_logs_api.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/api/vendor_logs_api.py`

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
-from pydantic import Field, StrictStr, conint, constr, validator
+from pydantic.v1 import Field, StrictStr, conint, constr, validator
 
 from typing import Optional
 
 from finbourne_insights.models.resource_list_with_histogram_of_vendor_log import ResourceListWithHistogramOfVendorLog
 from finbourne_insights.models.vendor_log import VendorLog
 from finbourne_insights.models.vendor_request import VendorRequest
 from finbourne_insights.models.vendor_response import VendorResponse
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/api_client.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/api_response.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/configuration.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_insights-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.759\n"\
+               "Version of the API: 0.0.764\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/exceptions.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client_factory.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_client_factory.py`

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

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_configuration.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/configuration_loaders.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/proxy_config.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/refreshing_token.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/rest.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/retry.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/socket_keep_alive.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/tcp_keep_alive_connector.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_action.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_action.py`

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
 from finbourne_insights.models.action_id import ActionId
 from finbourne_insights.models.id_selector_definition import IdSelectorDefinition
 from finbourne_insights.models.link import Link
 
 class AccessControlledAction(BaseModel):
     """
     AccessControlledAction
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_resource.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_insights.models.access_controlled_action import AccessControlledAction
 from finbourne_insights.models.identifier_part_schema import IdentifierPartSchema
 from finbourne_insights.models.link import Link
 
 class AccessControlledResource(BaseModel):
     """
     AccessControlledResource
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_evaluation_log.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/access_evaluation_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist, constr, validator
 from finbourne_insights.models.link import Link
 
 class AccessEvaluationLog(BaseModel):
     """
     Holds logged information about an access check performed on an API.  # noqa: E501
     """
     timestamp: datetime = Field(..., description="The timestamp of the access evaluation.")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/action_id.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/action_id.py`

 * *Files 1% similar despite different names*

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

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data.py`

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
 from finbourne_insights.models.resource import Resource
 
 class AuditData(BaseModel):
     """
     AuditData
     """
     action: constr(strict=True, max_length=64, min_length=0) = Field(...)
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data_summary.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_data_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, StrictInt
+from pydantic.v1 import BaseModel, StrictInt
 
 class AuditDataSummary(BaseModel):
     """
     AuditDataSummary
     """
     count: Optional[StrictInt] = None
     categories: Optional[Dict[str, StrictInt]] = None
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_insights.models.audit_data import AuditData
 from finbourne_insights.models.audit_entry_note import AuditEntryNote
 from finbourne_insights.models.audit_process import AuditProcess
 
 class AuditEntry(BaseModel):
     """
     AuditEntry
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry_note.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_entry_note.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class AuditEntryNote(BaseModel):
     """
     AuditEntryNote
     """
     user_id: constr(strict=True, min_length=1) = Field(..., alias="userId")
     text: constr(strict=True, min_length=1) = Field(...)
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictBool, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, constr
 
 class AuditProcess(BaseModel):
     """
     AuditProcess
     """
     name: constr(strict=True, max_length=128, min_length=0) = Field(...)
     run_id: constr(strict=True, min_length=1) = Field(..., alias="runId")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process_summary.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/audit_process_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_insights.models.audit_data import AuditData
 from finbourne_insights.models.audit_data_summary import AuditDataSummary
 from finbourne_insights.models.audit_process import AuditProcess
 
 class AuditProcessSummary(BaseModel):
     """
     AuditProcessSummary
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/bucket.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt
+from pydantic.v1 import BaseModel, Field, StrictInt
 
 class Bucket(BaseModel):
     """
     A single histogram bucket.  # noqa: E501
     """
     start_time: Optional[datetime] = Field(None, alias="startTime", description="The bucket's start time as a DateTimeOffset.")
     item_count: Optional[StrictInt] = Field(None, alias="itemCount", description="The number of items in the bucket.")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/create_audit_entry.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/create_audit_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 from finbourne_insights.models.audit_data import AuditData
 from finbourne_insights.models.audit_process import AuditProcess
 
 class CreateAuditEntry(BaseModel):
     """
     Details to create an audit entry  # noqa: E501
     """
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/histogram.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_insights.models.bucket import Bucket
 
 class Histogram(BaseModel):
     """
     A histogram showing an item's count in buckets of equal timespans.  # noqa: E501
     """
     buckets: Optional[conlist(Bucket)] = Field(None, description="An ordered list of the histogram buckets.")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/id_selector_definition.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_insights.models.action_id import ActionId
 
 class IdSelectorDefinition(BaseModel):
     """
     IdSelectorDefinition
     """
     identifier: Dict[str, StrictStr] = Field(...)
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/identifier_part_schema.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt, conlist, constr
 from finbourne_insights.models.link import Link
 
 class IdentifierPartSchema(BaseModel):
     """
     IdentifierPartSchema
     """
     index: StrictInt = Field(...)
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/link.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/link.py`

 * *Files 1% similar despite different names*

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

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_problem_details.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_problem_details.py`

 * *Files 1% similar despite different names*

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

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_validation_problem_details.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/lusid_validation_problem_details.py`

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

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/problem_details.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/problem_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic.v1 import BaseModel, StrictInt, StrictStr
 
 class ProblemDetails(BaseModel):
     """
     ProblemDetails
     """
     type: Optional[StrictStr] = None
     title: Optional[StrictStr] = None
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/request.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
 from finbourne_insights.models.link import Link
 
 class Request(BaseModel):
     """
     DTO of Finbourne.AspNetCore.Http.TrackingEntry.RequestInformation.  # noqa: E501
     """
     headers: Optional[Dict[str, conlist(StrictStr)]] = Field(None, description="The headers")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/request_log.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/request_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist, constr
 from finbourne_insights.models.link import Link
 
 class RequestLog(BaseModel):
     """
     Holds logged information about a request performed on an API.  # noqa: E501
     """
     timestamp: datetime = Field(..., description="The timestamp of the request.")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, constr
+from pydantic.v1 import BaseModel, constr
 
 class Resource(BaseModel):
     """
     Resource
     """
     type: Optional[constr(strict=True, max_length=64, min_length=0)] = None
     identifier: Optional[constr(strict=True, max_length=128, min_length=0)] = None
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_access_controlled_resource.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_access_controlled_resource.py`

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
 from finbourne_insights.models.access_controlled_resource import AccessControlledResource
 from finbourne_insights.models.link import Link
 
 class ResourceListOfAccessControlledResource(BaseModel):
     """
     ResourceListOfAccessControlledResource
     """
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_audit_process_summary.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_of_audit_process_summary.py`

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
 from finbourne_insights.models.audit_process_summary import AuditProcessSummary
 from finbourne_insights.models.link import Link
 
 class ResourceListOfAuditProcessSummary(BaseModel):
     """
     ResourceListOfAuditProcessSummary
     """
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py`

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
 from finbourne_insights.models.access_evaluation_log import AccessEvaluationLog
 from finbourne_insights.models.histogram import Histogram
 from finbourne_insights.models.link import Link
 
 class ResourceListWithHistogramOfAccessEvaluationLog(BaseModel):
     """
     ResourceList with additional aggregation data about the values.  # noqa: E501
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_request_log.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_request_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from finbourne_insights.models.histogram import Histogram
 from finbourne_insights.models.link import Link
 from finbourne_insights.models.request_log import RequestLog
 
 class ResourceListWithHistogramOfRequestLog(BaseModel):
     """
     ResourceList with additional aggregation data about the values.  # noqa: E501
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from finbourne_insights.models.histogram import Histogram
 from finbourne_insights.models.link import Link
 from finbourne_insights.models.vendor_log import VendorLog
 
 class ResourceListWithHistogramOfVendorLog(BaseModel):
     """
     ResourceList with additional aggregation data about the values.  # noqa: E501
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/response.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
 from finbourne_insights.models.link import Link
 
 class Response(BaseModel):
     """
     DTO of Finbourne.AspNetCore.Http.TrackingEntry.ResponseInformation.  # noqa: E501
     """
     headers: Optional[Dict[str, conlist(StrictStr)]] = Field(None, description="The headers")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/scrollable_collection_of_audit_entry.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/scrollable_collection_of_audit_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, StrictStr, conlist
+from pydantic.v1 import BaseModel, StrictStr, conlist
 from finbourne_insights.models.audit_entry import AuditEntry
 
 class ScrollableCollectionOfAuditEntry(BaseModel):
     """
     ScrollableCollectionOfAuditEntry
     """
     data: Optional[conlist(AuditEntry)] = None
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_log.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictFloat, StrictInt, conlist, constr
 from finbourne_insights.models.link import Link
 
 class VendorLog(BaseModel):
     """
     Holds logged information about a request made to an external vendor.  # noqa: E501
     """
     id: constr(strict=True, min_length=1) = Field(..., description="The identifier of a log entry.")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_request.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_request.py`

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
 from finbourne_insights.models.link import Link
 
 class VendorRequest(BaseModel):
     """
     Details of a request made to a vendor service.  # noqa: E501
     """
     id: constr(strict=True, min_length=1) = Field(..., description="The ID of the log.")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_response.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/models/vendor_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_insights.models.link import Link
 
 class VendorResponse(BaseModel):
     """
     Details of a response to a request made to a vendor service.  # noqa: E501
     """
     id: constr(strict=True, min_length=1) = Field(..., description="The ID of the log.")
```

### Comparing `finbourne_insights_sdk-2.0.9/finbourne_insights/rest.py` & `finbourne_insights_sdk-2.1.1/finbourne_insights/rest.py`

 * *Files 4% similar despite different names*

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

### Comparing `finbourne_insights_sdk-2.0.9/pyproject.toml` & `finbourne_insights_sdk-2.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-insights-sdk"
-version = "2.0.9"
+version = "2.1.1"
 description = "FINBOURNE Insights API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/insights-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Insights API", "finbourne-insights-sdk"]
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

### Comparing `finbourne_insights_sdk-2.0.9/PKG-INFO` & `finbourne_insights_sdk-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-insights-sdk
-Version: 2.0.9
+Version: 2.1.1
 Summary: FINBOURNE Insights API
 Home-page: https://github.com/finbourne/insights-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Insights API,finbourne-insights-sdk
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
 Project-URL: Repository, https://github.com/finbourne/insights-sdk-python
 Description-Content-Type: text/markdown
 
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.759
-- Package version: 2.0.9
+- API version: 0.0.764
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -82,16 +82,15 @@
 
 ``` 
 FBN_TOKEN_URL,
 FBN_FINBOURNE_INSIGHTS_API_URL,
 FBN_USERNAME,
 FBN_PASSWORD,
 FBN_CLIENT_ID,
-FBN_CLIENT_SECRET,
-FBN_ACCESS_TOKEN
+FBN_CLIENT_SECRET
 ```
 
 To use a long lived Personal Access Token, you must provide the following environment variables:
 ``` 
 FBN_FINBOURNE_INSIGHTS_API_URL,
 FBN_ACCESS_TOKEN
 ```
```

