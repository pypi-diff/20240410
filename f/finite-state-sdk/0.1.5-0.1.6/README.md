# Comparing `tmp/finite_state_sdk-0.1.5.tar.gz` & `tmp/finite_state_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finite_state_sdk-0.1.5.tar", max compression
+gzip compressed data, was "finite_state_sdk-0.1.6.tar", max compression
```

## Comparing `finite_state_sdk-0.1.5.tar` & `finite_state_sdk-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-09-20 20:35:28.671382 finite_state_sdk-0.1.5/LICENSE
--rw-r--r--   0        0        0     2053 2023-12-13 14:36:56.605409 finite_state_sdk-0.1.5/README.md
--rw-r--r--   0        0        0    89311 2024-02-07 21:22:14.873313 finite_state_sdk-0.1.5/finite_state_sdk/__init__.py
--rw-r--r--   0        0        0    24653 2024-02-06 20:51:19.435601 finite_state_sdk-0.1.5/finite_state_sdk/queries.py
--rw-r--r--   0        0        0     2633 2023-12-13 19:05:20.733977 finite_state_sdk-0.1.5/finite_state_sdk/token_cache.py
--rw-r--r--   0        0        0     1204 2024-02-07 21:27:55.717182 finite_state_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 finite_state_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-03-29 20:05:40.406290 finite_state_sdk-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2053 2024-03-29 20:05:40.406388 finite_state_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0    95617 2024-04-10 18:42:22.531582 finite_state_sdk-0.1.6/finite_state_sdk/__init__.py
+-rw-r--r--   0        0        0    24623 2024-04-10 18:42:22.532040 finite_state_sdk-0.1.6/finite_state_sdk/queries.py
+-rw-r--r--   0        0        0     2634 2024-04-10 18:42:22.532375 finite_state_sdk-0.1.6/finite_state_sdk/token_cache.py
+-rw-r--r--   0        0        0     3051 2024-04-10 19:16:33.477428 finite_state_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 finite_state_sdk-0.1.6/PKG-INFO
```

### Comparing `finite_state_sdk-0.1.5/LICENSE` & `finite_state_sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.5/README.md` & `finite_state_sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.5/finite_state_sdk/__init__.py` & `finite_state_sdk-0.1.6/finite_state_sdk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,47 @@
 import json
+from enum import Enum
+
 import requests
 import time
 from warnings import warn
 import finite_state_sdk.queries as queries
 
 API_URL = 'https://platform.finitestate.io/api/v1/graphql'
 AUDIENCE = "https://platform.finitestate.io/api/v1/graphql"
 TOKEN_URL = "https://platform.finitestate.io/api/v1/auth/token"
 
 
-def create_artifact(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_version_id=None, artifact_name=None, product_id=None):
+class UploadMethod(Enum):
+    """
+    Enumeration class representing different upload methods.
+
+    Attributes:
+        WEB_APP_UI: Upload method via web application UI.
+        API: Upload method via API.
+        GITHUB_INTEGRATION: Upload method via GitHub integration.
+        AZURE_DEVOPS_INTEGRATION: Upload method via Azure DevOps integration.
+
+    To use any value from this enumeration, use UploadMethod.<attribute> i.e. finite_state_sdk.UploadMethod.WEB_APP_UI
+    """
+    WEB_APP_UI = "WEB_APP_UI"
+    API = "API"
+    GITHUB_INTEGRATION = "GITHUB_INTEGRATION"
+    AZURE_DEVOPS_INTEGRATION = "AZURE_DEVOPS_INTEGRATION"
+
+
+def create_artifact(
+    token,
+    organization_context,
+    business_unit_id=None,
+    created_by_user_id=None,
+    asset_version_id=None,
+    artifact_name=None,
+    product_id=None,
+):
     """
     Create a new Artifact.
     This is an advanced method - you are probably looking for create_new_asset_version_and_upload_test_results or create_new_asset_version_and_upload_binary.
     Please see the examples in the Github repository for more information:
     - https://github.com/FiniteStateInc/finite-state-sdk-python/blob/main/examples/upload_test_results.py
     - https://github.com/FiniteStateInc/finite-state-sdk-python/blob/main/examples/uploading_a_binary.py
 
@@ -168,15 +196,23 @@
     if product_id is not None:
         variables["input"]["ctx"]["products"] = product_id
 
     response = send_graphql_query(token, organization_context, graphql_query, variables)
     return response['data']
 
 
-def create_asset_version(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, asset_version_name=None, product_id=None):
+def create_asset_version(
+    token,
+    organization_context,
+    business_unit_id=None,
+    created_by_user_id=None,
+    asset_id=None,
+    asset_version_name=None,
+    product_id=None,
+):
     """
     Create a new Asset Version.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -246,15 +282,26 @@
     if product_id is not None:
         variables["input"]["ctx"]["products"] = product_id
 
     response = send_graphql_query(token, organization_context, graphql_query, variables)
     return response['data']
 
 
-def create_new_asset_version_artifact_and_test_for_upload(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, version=None, product_id=None, test_type=None, artifact_description=None):
+def create_new_asset_version_artifact_and_test_for_upload(
+    token,
+    organization_context,
+    business_unit_id=None,
+    created_by_user_id=None,
+    asset_id=None,
+    version=None,
+    product_id=None,
+    test_type=None,
+    artifact_description=None,
+    upload_method: UploadMethod = UploadMethod.API,
+):
     """
     Creates the entities needed for uploading a file for Binary Analysis or test results from a third party scanner to an existing Asset. This will create a new Asset Version, Artifact, and Test.
     This method is used by the upload_file_for_binary_analysis and upload_test_results_file methods, which are generally easier to use for basic use cases.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
@@ -270,14 +317,17 @@
             Version to create the asset version for.
         product_id (str, optional):
             Product ID to create the entities for. If not provided, the default product will be used.
         test_type (str, required):
             Test type to create the test for. Must be one of "finite_state_binary_analysis" or of the list of supported third party test types. For the full list, see the API documenation.
         artifact_description (str, optional):
             Description to use for the artifact. Examples inlcude "Firmware", "Source Code Repository". This will be appended to the default Artifact description. If none is provided, the default Artifact description will be used.
+        upload_method (UploadMethod, optional):
+            The method of uploading the test results. Default is UploadMethod.API.
+
 
     Raises:
         ValueError: Raised if asset_id or version are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         str: The Test ID of the newly created test that is used for uploading the file.
@@ -309,53 +359,78 @@
 
         if not business_unit_id:
             raise ValueError("Business Unit ID is required and could not be retrieved from the existing asset")
         if not created_by_user_id:
             raise ValueError("Created By User ID is required and could not be retrieved from the existing asset")
 
     # create the asset version
-    response = create_asset_version(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, asset_version_name=version)
+    response = create_asset_version(token, organization_context, business_unit_id=business_unit_id,
+                                    created_by_user_id=created_by_user_id, asset_id=asset_id,
+                                    asset_version_name=version)
     # get the asset version ID
     asset_version_id = response['createAssetVersion']['id']
 
     # create the test
     if test_type == "finite_state_binary_analysis":
         # create the artifact
         if not artifact_description:
             artifact_description = "Binary"
         binary_artifact_name = f"{asset_name} {version} - {artifact_description}"
-        response = create_artifact(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_version_id=asset_version_id, artifact_name=binary_artifact_name, product_id=asset_product_ids)
+        response = create_artifact(token, organization_context, business_unit_id=business_unit_id,
+                                   created_by_user_id=created_by_user_id, asset_version_id=asset_version_id,
+                                   artifact_name=binary_artifact_name, product_id=asset_product_ids)
 
         # get the artifact ID
         binary_artifact_id = response['createArtifact']['id']
 
         # create the test
         test_name = f"{asset_name} {version} - Finite State Binary Analysis"
-        response = create_test_as_binary_analysis(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=binary_artifact_id, product_id=asset_product_ids, test_name=test_name)
+        response = create_test_as_binary_analysis(token, organization_context, business_unit_id=business_unit_id,
+                                                  created_by_user_id=created_by_user_id, asset_id=asset_id,
+                                                  artifact_id=binary_artifact_id, product_id=asset_product_ids,
+                                                  test_name=test_name, upload_method=upload_method)
         test_id = response['createTest']['id']
         return test_id
 
     else:
         # create the artifact
         if not artifact_description:
             artifact_description = "Unspecified Artifact"
         artifact_name = f"{asset_name} {version} - {artifact_description}"
-        response = create_artifact(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_version_id=asset_version_id, artifact_name=artifact_name, product_id=asset_product_ids)
+        response = create_artifact(token, organization_context, business_unit_id=business_unit_id,
+                                   created_by_user_id=created_by_user_id, asset_version_id=asset_version_id,
+                                   artifact_name=artifact_name, product_id=asset_product_ids)
 
         # get the artifact ID
         binary_artifact_id = response['createArtifact']['id']
 
         # create the test
         test_name = f"{asset_name} {version} - {test_type}"
-        response = create_test_as_third_party_scanner(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=binary_artifact_id, product_id=asset_product_ids, test_name=test_name, test_type=test_type)
+        response = create_test_as_third_party_scanner(token, organization_context, business_unit_id=business_unit_id,
+                                                      created_by_user_id=created_by_user_id, asset_id=asset_id,
+                                                      artifact_id=binary_artifact_id, product_id=asset_product_ids,
+                                                      test_name=test_name, test_type=test_type,
+                                                      upload_method=upload_method)
         test_id = response['createTest']['id']
         return test_id
 
 
-def create_new_asset_version_and_upload_binary(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, version=None, file_path=None, product_id=None, artifact_description=None, quick_scan=False):
+def create_new_asset_version_and_upload_binary(
+    token,
+    organization_context,
+    business_unit_id=None,
+    created_by_user_id=None,
+    asset_id=None,
+    version=None,
+    file_path=None,
+    product_id=None,
+    artifact_description=None,
+    quick_scan=False,
+    upload_method: UploadMethod = UploadMethod.API,
+):
     """
     Creates a new Asset Version for an existing asset, and uploads a binary file for Finite State Binary Analysis.
     By default, this uses the existing Business Unit and Created By User for the Asset. If you need to change these, you can provide the IDs for them.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
@@ -373,14 +448,16 @@
             Local path to the file to upload.
         product_id (str, optional):
             Product ID to create the asset version for. If not provided, the existing Product for the Asset will be used, if it exists.
         artifact_description (str, optional):
             Description of the artifact. If not provided, the default is "Firmware Binary".
         quick_scan (bool, optional):
             If True, will upload the file for quick scan. Defaults to False (Full Scan). For details about Quick Scan vs Full Scan, please see the API documentation.
+        upload_method (UploadMethod, optional):
+            The method of uploading the test results. Default is UploadMethod.API.
 
     Raises:
         ValueError: Raised if asset_id, version, or file_path are not provided.
         Exception: Raised if any of the queries fail.
 
     Returns:
         dict: The response from the GraphQL query, a createAssetVersion Object.
@@ -391,22 +468,37 @@
         raise ValueError("Version is required")
     if not file_path:
         raise ValueError("File path is required")
 
     # create the asset version and binary test
     if not artifact_description:
         artifact_description = "Firmware Binary"
-    binary_test_id = create_new_asset_version_artifact_and_test_for_upload(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, version=version, product_id=product_id, test_type="finite_state_binary_analysis", artifact_description=artifact_description)
+    binary_test_id = create_new_asset_version_artifact_and_test_for_upload(
+        token,
+        organization_context,
+        business_unit_id=business_unit_id,
+        created_by_user_id=created_by_user_id,
+        asset_id=asset_id,
+        version=version,
+        product_id=product_id,
+        test_type="finite_state_binary_analysis",
+        artifact_description=artifact_description,
+        upload_method=upload_method,
+    )
 
     # upload file for binary test
-    response = upload_file_for_binary_analysis(token, organization_context, test_id=binary_test_id, file_path=file_path, quick_scan=quick_scan)
+    response = upload_file_for_binary_analysis(token, organization_context, test_id=binary_test_id, file_path=file_path,
+                                               quick_scan=quick_scan)
     return response
 
 
-def create_new_asset_version_and_upload_test_results(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, version=None, file_path=None, product_id=None, test_type=None, artifact_description=""):
+def create_new_asset_version_and_upload_test_results(token, organization_context, business_unit_id=None,
+                                                     created_by_user_id=None, asset_id=None, version=None,
+                                                     file_path=None, product_id=None, test_type=None,
+                                                     artifact_description="", upload_method: UploadMethod = UploadMethod.API):
     """
     Creates a new Asset Version for an existing asset, and uploads test results for that asset version.
     By default, this uses the existing Business Unit and Created By User for the Asset. If you need to change these, you can provide the IDs for them.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
@@ -424,14 +516,16 @@
             Path to the test results file to upload.
         product_id (str, optional):
             Product ID to create the asset version for. If not provided, the existing Product for the Asset will be used.
         test_type (str, required):
             Test type. This must be one of the list of supported third party scanner types. For the full list of supported third party scanner types, see the Finite State API documentation.
         artifact_description (str, optional):
             Description of the artifact being scanned (e.g. "Source Code Repository", "Container Image"). If not provided, the default artifact description will be used.
+        upload_method (UploadMethod, optional):
+            The method of uploading the test results. Default is UploadMethod.API.
 
     Raises:
         ValueError: If the asset_id, version, or file_path are not provided.
         Exception: If the test_type is not a supported third party scanner type, or if the query fails.
 
     Returns:
         dict: The response from the GraphQL query, a createAssetVersion Object.
@@ -442,22 +536,29 @@
         raise ValueError("Version is required")
     if not file_path:
         raise ValueError("File path is required")
     if not test_type:
         raise ValueError("Test type is required")
 
     # create the asset version and test
-    test_id = create_new_asset_version_artifact_and_test_for_upload(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, version=version, product_id=product_id, test_type=test_type, artifact_description=artifact_description)
+    test_id = create_new_asset_version_artifact_and_test_for_upload(token, organization_context,
+                                                                    business_unit_id=business_unit_id,
+                                                                    created_by_user_id=created_by_user_id,
+                                                                    asset_id=asset_id, version=version,
+                                                                    product_id=product_id, test_type=test_type,
+                                                                    artifact_description=artifact_description,
+                                                                    upload_method=upload_method)
 
     # upload test results file
     response = upload_test_results_file(token, organization_context, test_id=test_id, file_path=file_path)
     return response
 
 
-def create_product(token, organization_context, business_unit_id=None, created_by_user_id=None, product_name=None, product_description=None, vendor_id=None, vendor_name=None):
+def create_product(token, organization_context, business_unit_id=None, created_by_user_id=None, product_name=None,
+                   product_description=None, vendor_id=None, vendor_name=None):
     """
     Create a new Product.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -488,15 +589,15 @@
     if not created_by_user_id:
         raise ValueError("Created by user ID is required")
     if not product_name:
         raise ValueError("Product name is required")
 
     graphql_query = '''
     mutation CreateProductMutation($input: CreateProductInput!) {
-		createProduct(input: $input) {
+        createProduct(input: $input) {
             id
             name
             vendor {
                 name
             }
             group {
                 id
@@ -505,15 +606,15 @@
             createdBy {
                 id
                 email
             }
             ctx {
                 businessUnit
             }
-		}
+        }
     }
     '''
 
     # Product name, business unit context, and creating user are required
     variables = {
         "input": {
             "name": product_name,
@@ -541,15 +642,16 @@
         }
 
     response = send_graphql_query(token, organization_context, graphql_query, variables)
 
     return response['data']
 
 
-def create_test(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, artifact_id=None, test_name=None, product_id=None, test_type=None, tools=[]):
+def create_test(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None,
+                artifact_id=None, test_name=None, product_id=None, test_type=None, tools=[], upload_method: UploadMethod = UploadMethod.API):
     """
     Create a new Test object for uploading files.
     This is an advanced method - you are probably looking for create_new_asset_version_and_upload_test_results or create_new_asset_version_and_upload_binary.
     Please see the examples in the Github repository for more information:
     - https://github.com/FiniteStateInc/finite-state-sdk-python/blob/main/examples/upload_test_results.py
     - https://github.com/FiniteStateInc/finite-state-sdk-python/blob/main/examples/uploading_a_binary.py
 
@@ -570,14 +672,16 @@
             The name of the Test being created.
         product_id (str, optional):
             Product ID to associate the Test with. If not specified, the Test will not be associated with a product.
         test_type (str, required):
             The type of test being created. Valid values are "cyclonedx" and "finite_state_binary_analysis".
         tools (list, optional):
             List of Tool objects used to perform the test. Each Tool object is a dict that should have a "name" and "description" field. This is used to describe the actual scanner that was used to perform the test.
+        upload_method (UploadMethod, required):
+            The method of uploading the test results.
 
     Raises:
         ValueError: Raised if business_unit_id, created_by_user_id, asset_id, artifact_id, test_name, or test_type are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         dict: createTest Object
@@ -621,14 +725,15 @@
                 email
             }
             ctx {
                 asset
                 products
                 businessUnits
             }
+            uploadMethod
         }
     }
     '''
 
     # Asset name, business unit context, and creating user are required
     variables = {
         "input": {
@@ -636,26 +741,29 @@
             "createdBy": created_by_user_id,
             "artifactUnderTest": artifact_id,
             "testResultFileFormat": test_type,
             "ctx": {
                 "asset": asset_id,
                 "businessUnits": [business_unit_id]
             },
-            "tools": tools
+            "tools": tools,
+            "uploadMethod": upload_method.value
         }
     }
 
     if product_id is not None:
         variables["input"]["ctx"]["products"] = product_id
 
     response = send_graphql_query(token, organization_context, graphql_query, variables)
     return response['data']
 
 
-def create_test_as_binary_analysis(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, artifact_id=None, test_name=None, product_id=None):
+def create_test_as_binary_analysis(token, organization_context, business_unit_id=None, created_by_user_id=None,
+                                   asset_id=None, artifact_id=None, test_name=None, product_id=None,
+                                   upload_method: UploadMethod = UploadMethod.API):
     """
     Create a new Test object for uploading files for Finite State Binary Analysis.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -668,32 +776,38 @@
             Asset ID to associate the Test with.
         artifact_id (str, required):
             Artifact ID to associate the Test with.
         test_name (str, required):
             The name of the Test being created.
         product_id (str, optional):
             Product ID to associate the Test with. If not specified, the Test will not be associated with a product.
+        upload_method (UploadMethod, optional):
+            The method of uploading the test results. Default is UploadMethod.API.
 
     Raises:
         ValueError: Raised if business_unit_id, created_by_user_id, asset_id, artifact_id, or test_name are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         dict: createTest Object
     """
     tools = [
         {
             "description": "SBOM and Vulnerability Analysis from Finite State Binary SCA and Binary SAST.",
             "name": "Finite State Binary Analysis"
         }
     ]
-    return create_test(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=artifact_id, test_name=test_name, product_id=product_id, test_type="finite_state_binary_analysis", tools=tools)
+    return create_test(token, organization_context, business_unit_id=business_unit_id,
+                       created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=artifact_id,
+                       test_name=test_name, product_id=product_id, test_type="finite_state_binary_analysis",
+                       tools=tools, upload_method=upload_method)
 
 
-def create_test_as_cyclone_dx(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, artifact_id=None, test_name=None, product_id=None):
+def create_test_as_cyclone_dx(token, organization_context, business_unit_id=None, created_by_user_id=None,
+                              asset_id=None, artifact_id=None, test_name=None, product_id=None, upload_method: UploadMethod = UploadMethod.API):
     """
     Create a new Test object for uploading CycloneDX files.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -706,26 +820,32 @@
             Asset ID to associate the Test with.
         artifact_id (str, required):
             Artifact ID to associate the Test with.
         test_name (str, required):
             The name of the Test being created.
         product_id (str, optional):
             Product ID to associate the Test with. If not specified, the Test will not be associated with a product.
+        upload_method (UploadMethod, optional):
+            The method of uploading the test results. Default is UploadMethod.API.
 
     Raises:
         ValueError: Raised if business_unit_id, created_by_user_id, asset_id, artifact_id, or test_name are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         dict: createTest Object
     """
-    return create_test(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=artifact_id, test_name=test_name, product_id=product_id, test_type="cyclonedx")
+    return create_test(token, organization_context, business_unit_id=business_unit_id,
+                       created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=artifact_id,
+                       test_name=test_name, product_id=product_id, test_type="cyclonedx", upload_method=upload_method)
 
 
-def create_test_as_third_party_scanner(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None, artifact_id=None, test_name=None, product_id=None, test_type=None):
+def create_test_as_third_party_scanner(token, organization_context, business_unit_id=None, created_by_user_id=None,
+                                       asset_id=None, artifact_id=None, test_name=None, product_id=None, test_type=None,
+                                       upload_method: UploadMethod = UploadMethod.API):
     """
     Create a new Test object for uploading Third Party Scanner files.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -740,26 +860,31 @@
             Artifact ID to associate the Test with.
         test_name (str, required):
             The name of the Test being created.
         product_id (str, optional):
             Product ID to associate the Test with. If not specified, the Test will not be associated with a product.
         test_type (str, required):
             Test type of the scanner which indicates the output file format from the scanner. Valid values are "cyclonedx" and others. For the full list see the API documentation.
+        upload_method (UploadMethod, optional):
+            The method of uploading the test results. Default is UploadMethod.API.
 
     Raises:
         ValueError: Raised if business_unit_id, created_by_user_id, asset_id, artifact_id, or test_name are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         dict: createTest Object
     """
-    return create_test(token, organization_context, business_unit_id=business_unit_id, created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=artifact_id, test_name=test_name, product_id=product_id, test_type=test_type)
+    return create_test(token, organization_context, business_unit_id=business_unit_id,
+                       created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=artifact_id,
+                       test_name=test_name, product_id=product_id, test_type=test_type, upload_method=upload_method)
 
 
-def download_asset_version_report(token, organization_context, asset_version_id=None, report_type=None, report_subtype=None, output_filename=None, verbose=False):
+def download_asset_version_report(token, organization_context, asset_version_id=None, report_type=None,
+                                  report_subtype=None, output_filename=None, verbose=False):
     """
     Download a report for a specific asset version and save it to a local file. This is a blocking call, and can sometimes take minutes to return if the report is very large.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -780,15 +905,16 @@
     Raises:
         ValueError: Raised if required parameters are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         None
     """
-    url = generate_report_download_url(token, organization_context, asset_version_id=asset_version_id, report_type=report_type, report_subtype=report_subtype, verbose=verbose)
+    url = generate_report_download_url(token, organization_context, asset_version_id=asset_version_id,
+                                       report_type=report_type, report_subtype=report_subtype, verbose=verbose)
 
     # Send an HTTP GET request to the URL
     response = requests.get(url)
 
     # Check if the request was successful (status code 200)
     if response.status_code == 200:
         # Open a local file in binary write mode and write the content to it
@@ -798,15 +924,16 @@
             file.write(response.content)
             if verbose:
                 print(f'Wrote file to {output_filename}')
     else:
         raise Exception(f"Failed to download the file. Status code: {response.status_code}")
 
 
-def download_product_report(token, organization_context, product_id=None, report_type=None, report_subtype=None, output_filename=None, verbose=False):
+def download_product_report(token, organization_context, product_id=None, report_type=None, report_subtype=None,
+                            output_filename=None, verbose=False):
     """
     Download a report for a specific product and save it to a local file. This is a blocking call, and can sometimes take minutes to return if the report is very large.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -819,15 +946,16 @@
             The type of report to download. Based on available reports for the `report_type` specified
             Valid values for CSV are "ALL_FINDINGS".
         output_filename (str, optional):
             The local filename to save the report to. If not provided, the report will be saved to a file named "report.csv" or "report.pdf" in the current directory based on the report type.
         verbose (bool, optional):
             If True, will print additional information to the console. Defaults to False.
     """
-    url = generate_report_download_url(token, organization_context, product_id=product_id, report_type=report_type, report_subtype=report_subtype, verbose=verbose)
+    url = generate_report_download_url(token, organization_context, product_id=product_id, report_type=report_type,
+                                       report_subtype=report_subtype, verbose=verbose)
 
     # Send an HTTP GET request to the URL
     response = requests.get(url)
 
     # Check if the request was successful (status code 200)
     if response.status_code == 200:
         # Open a local file in binary write mode and write the content to it
@@ -837,15 +965,16 @@
             file.write(response.content)
             if verbose:
                 print(f'Wrote file to {output_filename}')
     else:
         raise Exception(f"Failed to download the file. Status code: {response.status_code}")
 
 
-def download_sbom(token, organization_context, sbom_type="CYCLONEDX", sbom_subtype="SBOM_ONLY", asset_version_id=None, output_filename="sbom.json", verbose=False):
+def download_sbom(token, organization_context, sbom_type="CYCLONEDX", sbom_subtype="SBOM_ONLY", asset_version_id=None,
+                  output_filename="sbom.json", verbose=False):
     """
     Download an SBOM for an Asset Version and save it to a local file. This is a blocking call, and can sometimes take minutes to return if the SBOM is very large.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
@@ -864,15 +993,16 @@
     Raises:
         ValueError: Raised if required parameters are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         None
     """
-    url = generate_sbom_download_url(token, organization_context, sbom_type=sbom_type, sbom_subtype=sbom_subtype, asset_version_id=asset_version_id, verbose=verbose)
+    url = generate_sbom_download_url(token, organization_context, sbom_type=sbom_type, sbom_subtype=sbom_subtype,
+                                     asset_version_id=asset_version_id, verbose=verbose)
 
     # Send an HTTP GET request to the URL
     response = requests.get(url)
 
     # Check if the request was successful (status code 200)
     if response.status_code == 200:
         # Open a local file in binary write mode and write the content to it
@@ -927,15 +1057,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of Artifact Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_ARTIFACTS['query'], queries.ALL_ARTIFACTS['variables'](artifact_id, business_unit_id), 'allAssets')
+    return get_all_paginated_results(token, organization_context, queries.ALL_ARTIFACTS['query'],
+                                     queries.ALL_ARTIFACTS['variables'](artifact_id, business_unit_id), 'allAssets')
 
 
 def get_all_assets(token, organization_context, asset_id=None, business_unit_id=None):
     """
     Gets all assets in the organization. Uses pagination to get all results.
 
     Args:
@@ -950,15 +1081,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of Asset Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_ASSETS['query'], queries.ALL_ASSETS['variables'](asset_id, business_unit_id), 'allAssets')
+    return get_all_paginated_results(token, organization_context, queries.ALL_ASSETS['query'],
+                                     queries.ALL_ASSETS['variables'](asset_id, business_unit_id), 'allAssets')
 
 
 def get_all_asset_versions(token, organization_context):
     """
     Get all asset versions in the organization. Uses pagination to get all results.
 
     Args:
@@ -969,15 +1101,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of AssetVersion Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_ASSET_VERSIONS['query'], queries.ALL_ASSET_VERSIONS['variables'], 'allAssetVersions')
+    return get_all_paginated_results(token, organization_context, queries.ALL_ASSET_VERSIONS['query'],
+                                     queries.ALL_ASSET_VERSIONS['variables'], 'allAssetVersions')
 
 
 def get_all_asset_versions_for_product(token, organization_context, product_id):
     """
     Get all asset versions for a product. Uses pagination to get all results.
 
     Args:
@@ -987,15 +1120,16 @@
             Organization context. This is provided by the Finite State API management. It looks like "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx".
         product_id (str):
             The Product ID to get asset versions for
 
     Returns:
         list: List of AssetVersion Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ONE_PRODUCT_ALL_ASSET_VERSIONS['query'], queries.ONE_PRODUCT_ALL_ASSET_VERSIONS['variables'](product_id), 'allProducts')
+    return get_all_paginated_results(token, organization_context, queries.ONE_PRODUCT_ALL_ASSET_VERSIONS['query'],
+                                     queries.ONE_PRODUCT_ALL_ASSET_VERSIONS['variables'](product_id), 'allProducts')
 
 
 def get_all_business_units(token, organization_context):
     """
     Get all business units in the organization. NOTE: The return type here is Group. Uses pagination to get all results.
 
     Args:
@@ -1006,15 +1140,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of Group Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_BUSINESS_UNITS['query'], queries.ALL_BUSINESS_UNITS['variables'], 'allGroups')
+    return get_all_paginated_results(token, organization_context, queries.ALL_BUSINESS_UNITS['query'],
+                                     queries.ALL_BUSINESS_UNITS['variables'], 'allGroups')
 
 
 def get_all_organizations(token, organization_context):
     """
     Get all organizations available to the user. For most users there is only one organization. Uses pagination to get all results.
 
     Args:
@@ -1025,15 +1160,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of Organization Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_ORGANIZATIONS['query'], queries.ALL_ORGANIZATIONS['variables'], 'allOrganizations')
+    return get_all_paginated_results(token, organization_context, queries.ALL_ORGANIZATIONS['query'],
+                                     queries.ALL_ORGANIZATIONS['variables'], 'allOrganizations')
 
 
 def get_all_paginated_results(token, organization_context, query, variables=None, field=None, limit=None):
     """
     Get all results from a paginated GraphQL query
 
     Args:
@@ -1115,15 +1251,16 @@
 
     Returns:
         list: List of Product Objects
 
     .. deprecated:: 0.1.4. Use get_products instead.
     """
     warn('`get_all_products` is deprecated. Use: `get_products instead`', DeprecationWarning, stacklevel=2)
-    return get_all_paginated_results(token, organization_context, queries.ALL_PRODUCTS['query'], queries.ALL_PRODUCTS['variables'], 'allProducts')
+    return get_all_paginated_results(token, organization_context, queries.ALL_PRODUCTS['query'],
+                                     queries.ALL_PRODUCTS['variables'], 'allProducts')
 
 
 def get_all_users(token, organization_context):
     """
     Get all users in the organization. Uses pagination to get all results.
 
     Args:
@@ -1134,15 +1271,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of User Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_USERS['query'], queries.ALL_USERS['variables'], 'allUsers')
+    return get_all_paginated_results(token, organization_context, queries.ALL_USERS['query'],
+                                     queries.ALL_USERS['variables'], 'allUsers')
 
 
 def get_artifact_context(token, organization_context, artifact_id):
     """
     Get the context for a single artifact. This is typically used for querying for existing context, which is used for role based access control. This is not used for creating new artifacts.
 
     Args:
@@ -1153,15 +1291,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         dict: Artifact Context Object
     """
-    artifact = get_all_paginated_results(token, organization_context, queries.ALL_ARTIFACTS['query'], queries.ALL_ARTIFACTS['variables'](artifact_id, None), 'allAssets')
+    artifact = get_all_paginated_results(token, organization_context, queries.ALL_ARTIFACTS['query'],
+                                         queries.ALL_ARTIFACTS['variables'](artifact_id, None), 'allAssets')
 
     return artifact[0]['ctx']
 
 
 def get_assets(token, organization_context, asset_id=None, business_unit_id=None):
     """
     Gets assets in the organization. Uses pagination to get all results.
@@ -1178,15 +1317,16 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of Asset Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_ASSETS['query'], queries.ALL_ASSETS['variables'](asset_id, business_unit_id), 'allAssets')
+    return get_all_paginated_results(token, organization_context, queries.ALL_ASSETS['query'],
+                                     queries.ALL_ASSETS['variables'](asset_id, business_unit_id), 'allAssets')
 
 
 def get_asset_versions(token, organization_context, asset_version_id=None, asset_id=None, business_unit_id=None):
     """
     Gets asset versions in the organization. Uses pagination to get all results.
 
     Args:
@@ -1203,15 +1343,19 @@
 
     Raises:
         Exception: Raised if the query fails.
 
     Returns:
         list: List of AssetVersion Objects
     """
-    return get_all_paginated_results(token, organization_context, queries.ALL_ASSET_VERSIONS['query'], queries.ALL_ASSET_VERSIONS['variables'](asset_version_id=asset_version_id, asset_id=asset_id, business_unit_id=business_unit_id), 'allAssetVersions')
+    return get_all_paginated_results(token, organization_context, queries.ALL_ASSET_VERSIONS['query'],
+                                     queries.ALL_ASSET_VERSIONS['variables'](asset_version_id=asset_version_id,
+                                                                             asset_id=asset_id,
+                                                                             business_unit_id=business_unit_id),
+                                     'allAssetVersions')
 
 
 def get_auth_token(client_id, client_secret, token_url=TOKEN_URL, audience=AUDIENCE):
     """
     Get an auth token for use with the API using CLIENT_ID and CLIENT_SECRET
 
     Args:
@@ -1246,15 +1390,16 @@
         auth_token = response.json()['access_token']
     else:
         raise Exception(f"Error: {response.status_code} - {response.text}")
 
     return auth_token
 
 
-def get_findings(token, organization_context, asset_version_id=None, finding_id=None, category=None, status=None, severity=None, count=False, limit=None):
+def get_findings(token, organization_context, asset_version_id=None, finding_id=None, category=None, status=None,
+                 severity=None, count=False, limit=None):
     """
     Gets all the Findings for an Asset Version. Uses pagination to get all results.
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string.
         organization_context (str):
             Organization context. This is provided by the Finite State API management. It looks like "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx".
@@ -1278,17 +1423,25 @@
         Exception: Raised if the query fails, required parameters are not specified, or parameters are incompatible.
 
     Returns:
         list: List of Finding Objects
     """
 
     if count:
-        return send_graphql_query(token, organization_context, queries.GET_FINDINGS_COUNT['query'], queries.GET_FINDINGS_COUNT['variables'](asset_version_id=asset_version_id, finding_id=finding_id, category=category, status=status, severity=severity, limit=limit))["data"]["_allFindingsMeta"]
+        return send_graphql_query(token, organization_context, queries.GET_FINDINGS_COUNT['query'],
+                                  queries.GET_FINDINGS_COUNT['variables'](asset_version_id=asset_version_id,
+                                                                          finding_id=finding_id, category=category,
+                                                                          status=status, severity=severity,
+                                                                          limit=limit))["data"]["_allFindingsMeta"]
     else:
-        return get_all_paginated_results(token, organization_context, queries.GET_FINDINGS['query'], queries.GET_FINDINGS['variables'](asset_version_id=asset_version_id, finding_id=finding_id, category=category, status=status, severity=severity, limit=limit), 'allFindings', limit=limit)
+        return get_all_paginated_results(token, organization_context, queries.GET_FINDINGS['query'],
+                                         queries.GET_FINDINGS['variables'](asset_version_id=asset_version_id,
+                                                                           finding_id=finding_id, category=category,
+                                                                           status=status, severity=severity,
+                                                                           limit=limit), 'allFindings', limit=limit)
 
 
 def get_product_asset_versions(token, organization_context, product_id=None):
     """
     Gets all the asset versions for a product.
     Args:
         token (str):
@@ -1301,15 +1454,16 @@
         Exception: Raised if the query fails, required parameters are not specified, or parameters are incompatible.
     Returns:
         list: List of AssetVersion Objects
     """
     if not product_id:
         raise Exception("Product ID is required")
 
-    return get_all_paginated_results(token, organization_context, queries.GET_PRODUCT_ASSET_VERSIONS['query'], queries.GET_PRODUCT_ASSET_VERSIONS['variables'](product_id), 'allProducts')
+    return get_all_paginated_results(token, organization_context, queries.GET_PRODUCT_ASSET_VERSIONS['query'],
+                                     queries.GET_PRODUCT_ASSET_VERSIONS['variables'](product_id), 'allProducts')
 
 
 def get_products(token, organization_context, product_id=None, business_unit_id=None) -> list:
     """
     Gets all the products for the specified business unit.
     Args:
         token (str):
@@ -1322,18 +1476,22 @@
             Business Unit ID to get products for. If not provided, will get all products in the organization.
     Raises:
         Exception: Raised if the query fails, required parameters are not specified, or parameters are incompatible.
     Returns:
         list: List of Product Objects
     """
 
-    return get_all_paginated_results(token, organization_context, queries.GET_PRODUCTS['query'], queries.GET_PRODUCTS['variables'](product_id=product_id, business_unit_id=business_unit_id), 'allProducts')
+    return get_all_paginated_results(token, organization_context, queries.GET_PRODUCTS['query'],
+                                     queries.GET_PRODUCTS['variables'](product_id=product_id,
+                                                                       business_unit_id=business_unit_id),
+                                     'allProducts')
 
 
-def generate_report_download_url(token, organization_context, asset_version_id=None, product_id=None, report_type=None, report_subtype=None, verbose=False) -> str:
+def generate_report_download_url(token, organization_context, asset_version_id=None, product_id=None, report_type=None,
+                                 report_subtype=None, verbose=False) -> str:
     """
     Blocking call: Initiates generation of a report, and returns a pre-signed URL for downloading the report.
     This may take several minutes to complete, depending on the size of the report.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
@@ -1365,56 +1523,63 @@
     if report_type not in ["CSV", "PDF"]:
         raise Exception(f"Report Type {report_type} not supported")
 
     if report_type == "CSV":
         if report_subtype not in ["ALL_FINDINGS", "ALL_COMPONENTS", "EXPLOIT_INTELLIGENCE"]:
             raise Exception(f"Report Subtype {report_subtype} not supported")
 
-        mutation = queries.LAUNCH_REPORT_EXPORT['mutation'](asset_version_id=asset_version_id, product_id=product_id, report_type=report_type, report_subtype=report_subtype)
-        variables = queries.LAUNCH_REPORT_EXPORT['variables'](asset_version_id=asset_version_id, product_id=product_id, report_type=report_type, report_subtype=report_subtype)
+        mutation = queries.LAUNCH_REPORT_EXPORT['mutation'](asset_version_id=asset_version_id, product_id=product_id,
+                                                            report_type=report_type, report_subtype=report_subtype)
+        variables = queries.LAUNCH_REPORT_EXPORT['variables'](asset_version_id=asset_version_id, product_id=product_id,
+                                                              report_type=report_type, report_subtype=report_subtype)
 
         response_data = send_graphql_query(token, organization_context, mutation, variables)
         if verbose:
             print(f'Response Data: {json.dumps(response_data, indent=4)}')
 
         # get exportJobId from the result
         if asset_version_id:
             export_job_id = response_data['data']['launchArtifactCSVExport']['exportJobId']
         elif product_id:
             export_job_id = response_data['data']['launchProductCSVExport']['exportJobId']
         else:
-            raise Exception("Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
+            raise Exception(
+                "Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
 
         if verbose:
             print(f'Export Job ID: {export_job_id}')
 
     if report_type == "PDF":
         if report_subtype not in ["RISK_SUMMARY"]:
             raise Exception(f"Report Subtype {report_subtype} not supported")
 
-        mutation = queries.LAUNCH_REPORT_EXPORT['mutation'](asset_version_id=asset_version_id, product_id=product_id, report_type=report_type, report_subtype=report_subtype)
-        variables = queries.LAUNCH_REPORT_EXPORT['variables'](asset_version_id=asset_version_id, product_id=product_id, report_type=report_type, report_subtype=report_subtype)
+        mutation = queries.LAUNCH_REPORT_EXPORT['mutation'](asset_version_id=asset_version_id, product_id=product_id,
+                                                            report_type=report_type, report_subtype=report_subtype)
+        variables = queries.LAUNCH_REPORT_EXPORT['variables'](asset_version_id=asset_version_id, product_id=product_id,
+                                                              report_type=report_type, report_subtype=report_subtype)
 
         response_data = send_graphql_query(token, organization_context, mutation, variables)
         if verbose:
             print(f'Response Data: {json.dumps(response_data, indent=4)}')
 
         # get exportJobId from the result
         if asset_version_id:
             export_job_id = response_data['data']['launchArtifactPdfExport']['exportJobId']
         elif product_id:
             export_job_id = response_data['data']['launchProductPdfExport']['exportJobId']
         else:
-            raise Exception("Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
+            raise Exception(
+                "Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
 
         if verbose:
             print(f'Export Job ID: {export_job_id}')
 
     if not export_job_id:
-        raise Exception("Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
+        raise Exception(
+            "Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
 
     # poll the API until the export job is complete
     sleep_time = 10
     total_time = 0
     if verbose:
         print(f'Polling every {sleep_time} seconds for export job to complete')
 
@@ -1431,19 +1596,21 @@
 
         if verbose:
             print(f'Response Data: {json.dumps(response_data, indent=4)}')
 
         if response_data['data']['generateExportDownloadPresignedUrl']['status'] == 'COMPLETED':
             if response_data['data']['generateExportDownloadPresignedUrl']['downloadLink']:
                 if verbose:
-                    print(f'Export Job Complete. Download URL: {response_data["data"]["generateExportDownloadPresignedUrl"]["downloadLink"]}')
+                    print(
+                        f'Export Job Complete. Download URL: {response_data["data"]["generateExportDownloadPresignedUrl"]["downloadLink"]}')
                 return response_data['data']['generateExportDownloadPresignedUrl']['downloadLink']
 
 
-def generate_sbom_download_url(token, organization_context, sbom_type=None, sbom_subtype=None, asset_version_id=None, verbose=False) -> str:
+def generate_sbom_download_url(token, organization_context, sbom_type=None, sbom_subtype=None, asset_version_id=None,
+                               verbose=False) -> str:
     """
     Blocking call: Initiates generation of an SBOM for the asset_version_id, and return a pre-signed URL for downloading the SBOM.
     This may take several minutes to complete, depending on the size of SBOM.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
@@ -1505,15 +1672,16 @@
 
         # get exportJobId from the result
         export_job_id = response_data['data']['launchSpdxExport']['exportJobId']
         if verbose:
             print(f'Export Job ID: {export_job_id}')
 
     if not export_job_id:
-        raise Exception("Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
+        raise Exception(
+            "Error: Export Job ID not found - this should not happen, please contact your Finite State representative")
 
     # poll the API until the export job is complete
     sleep_time = 10
     total_time = 0
     if verbose:
         print(f'Polling every {sleep_time} seconds for export job to complete')
     while True:
@@ -1529,15 +1697,16 @@
 
         if verbose:
             print(f'Response Data: {json.dumps(response_data, indent=4)}')
 
         if response_data['data']['generateExportDownloadPresignedUrl']['status'] == "COMPLETED":
             if response_data['data']['generateExportDownloadPresignedUrl']['downloadLink']:
                 if verbose:
-                    print(f'Export Job Complete. Download URL: {response_data["data"]["generateExportDownloadPresignedUrl"]["downloadLink"]}')
+                    print(
+                        f'Export Job Complete. Download URL: {response_data["data"]["generateExportDownloadPresignedUrl"]["downloadLink"]}')
                 return response_data['data']['generateExportDownloadPresignedUrl']['downloadLink']
 
 
 def get_software_components(token, organization_context, asset_version_id=None, type=None) -> list:
     """
     Gets all the Software Components for an Asset Version. Uses pagination to get all results.
     Args:
@@ -1553,18 +1722,22 @@
         Exception: Raised if the query fails, required parameters are not specified, or parameters are incompatible.
     Returns:
         list: List of Software Component Objects
     """
     if not asset_version_id:
         raise Exception("Asset Version ID is required")
 
-    return get_all_paginated_results(token, organization_context, queries.GET_SOFTWARE_COMPONENTS['query'], queries.GET_SOFTWARE_COMPONENTS['variables'](asset_version_id=asset_version_id, type=type), 'allSoftwareComponentInstances')
+    return get_all_paginated_results(token, organization_context, queries.GET_SOFTWARE_COMPONENTS['query'],
+                                     queries.GET_SOFTWARE_COMPONENTS['variables'](asset_version_id=asset_version_id,
+                                                                                  type=type),
+                                     'allSoftwareComponentInstances')
 
 
-def search_sbom(token, organization_context, name=None, version=None, asset_version_id=None, search_method='EXACT', case_sensitive=False) -> list:
+def search_sbom(token, organization_context, name=None, version=None, asset_version_id=None, search_method='EXACT',
+                case_sensitive=False) -> list:
     """
     Searches the SBOM of a specific asset version or the entire organization for matching software components.
     Search Methods: EXACT or CONTAINS
     An exact match will return only the software component whose name matches the name exactly.
     A contains match will return all software components whose name contains the search string.
 
     Args:
@@ -1662,15 +1835,16 @@
 
     if version:
         if search_method == 'EXACT':
             variables["filter"]["version"] = version
         elif search_method == 'CONTAINS':
             variables["filter"]["version_contains"] = version
 
-    records = get_all_paginated_results(token, organization_context, query, variables=variables, field="allSoftwareComponentInstances")
+    records = get_all_paginated_results(token, organization_context, query, variables=variables,
+                                        field="allSoftwareComponentInstances")
 
     return records
 
 
 def send_graphql_query(token, organization_context, query, variables=None):
     """
     Send a GraphQL query to the API
@@ -1710,15 +1884,16 @@
             raise Exception(f"Error: {thejson['errors']}")
 
         return thejson
     else:
         raise Exception(f"Error: {response.status_code} - {response.text}")
 
 
-def update_finding_statuses(token, organization_context, user_id=None, finding_ids=None, status=None, justification=None, response=None, comment=None):
+def update_finding_statuses(token, organization_context, user_id=None, finding_ids=None, status=None,
+                            justification=None, response=None, comment=None):
     """
     Updates the status of a findings or multiple findings. This is a blocking call.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string.
         organization_context (str):
@@ -1747,20 +1922,23 @@
         raise ValueError("User ID is required")
     if not finding_ids:
         raise ValueError("Finding ID is required")
     if not status:
         raise ValueError("Status is required")
 
     mutation = queries.UPDATE_FINDING_STATUSES['mutation']
-    variables = queries.UPDATE_FINDING_STATUSES['variables'](user_id=user_id, finding_ids=finding_ids, status=status, justification=justification, response=response, comment=comment)
+    variables = queries.UPDATE_FINDING_STATUSES['variables'](user_id=user_id, finding_ids=finding_ids, status=status,
+                                                             justification=justification, response=response,
+                                                             comment=comment)
 
     return send_graphql_query(token, organization_context, mutation, variables)
 
 
-def upload_file_for_binary_analysis(token, organization_context, test_id=None, file_path=None, chunk_size=1024 * 1024 * 1024 * 5, quick_scan=False):
+def upload_file_for_binary_analysis(token, organization_context, test_id=None, file_path=None,
+                                    chunk_size=1024 * 1024 * 1024 * 5, quick_scan=False):
     """
     Upload a file for Binary Analysis. Will automatically chunk the file into chunks and upload each chunk. Chunk size defaults to 5GB.
     NOTE: This is NOT for uploading third party scanner results. Use upload_test_results_file for that.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
```

### Comparing `finite_state_sdk-0.1.5/finite_state_sdk/queries.py` & `finite_state_sdk-0.1.6/finite_state_sdk/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import json
-
 """
 GraphQL queries for the Finite State Platform
 """
 
 ALL_BUSINESS_UNITS = {
     "query": """
     query GetBusinessUnits(
@@ -323,15 +321,15 @@
 query GenerateExportDownloadPresignedUrl($exportId: ID!) {
   generateExportDownloadPresignedUrl(exportId: $exportId) {
     downloadLink
     status
   }
 }
 """,
-    "variables": lambda export_id: { "exportId": export_id }
+    "variables": lambda export_id: {"exportId": export_id}
 }
 
 
 GET_PRODUCT_ASSET_VERSIONS = {
     "query": """
 query GetProductAssetVersions(
     $filter: ProductFilter!,
@@ -943,18 +941,18 @@
     elif status == "NOT_AFFECTED":
         if response is not None:
             raise Exception("response pertains to status AFFECTED. Specify justification instead.")
 
     return {
         "ids": finding_ids,
         "updateStatusInput": {
-                "comment": comment,
-                "status": status,
-                "justification": justification,
-                "responses": response
+            "comment": comment,
+            "status": status,
+            "justification": justification,
+            "responses": response
         },
         "userId": user_id
     }
 
 
 UPDATE_FINDING_STATUSES = {
     "mutation": """
@@ -972,8 +970,8 @@
     "ALL_BUSINESS_UNITS",
     "ALL_USERS",
     "ALL_ORGANIZATIONS",
     "ALL_ASSET_VERSIONS",
     "ALL_ARTIFACTS",
     "ALL_PRODUCTS",
     "ONE_PRODUCT_ALL_ASSET_VERSIONS"
-]
+]
```

### Comparing `finite_state_sdk-0.1.5/finite_state_sdk/token_cache.py` & `finite_state_sdk-0.1.6/finite_state_sdk/token_cache.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
         else:
             return self.token
 
     def invalidate_token(self):
         self.token = None
         if os.path.exists(self.token_file):
             os.remove(self.token_file)
-            self.token = None
+            self.token = None
```

