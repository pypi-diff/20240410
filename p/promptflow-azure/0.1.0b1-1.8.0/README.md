# Comparing `tmp/promptflow_azure-0.1.0b1-py3-none-any.whl.zip` & `tmp/promptflow_azure-1.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 604500 bytes, number of entries: 91
+Zip file size: 668890 bytes, number of entries: 97
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 promptflow/azure/__init__.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/__init__.py
 -rw-r--r--  2.0 unx     3566 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/_connection.py
 -rw-r--r--  2.0 unx     9458 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/_flow.py
 -rw-r--r--  2.0 unx    18636 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/_run.py
+-rw-r--r--  2.0 unx      289 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/_user_agent.py
 -rw-r--r--  2.0 unx      594 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/_utils.py
--rw-r--r--  2.0 unx     5099 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/entry.py
+-rw-r--r--  2.0 unx     5971 b- defN 80-Jan-01 00:00 promptflow/azure/_cli/entry.py
 -rw-r--r--  2.0 unx      484 b- defN 80-Jan-01 00:00 promptflow/azure/_constants/__init__.py
 -rw-r--r--  2.0 unx      382 b- defN 80-Jan-01 00:00 promptflow/azure/_constants/_component.py
 -rw-r--r--  2.0 unx     1049 b- defN 80-Jan-01 00:00 promptflow/azure/_constants/_flow.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 promptflow/azure/_entities/__init__.py
 -rw-r--r--  2.0 unx    10394 b- defN 80-Jan-01 00:00 promptflow/azure/_entities/_flow.py
 -rw-r--r--  2.0 unx     2010 b- defN 80-Jan-01 00:00 promptflow/azure/_entities/_workspace_connection_spec.py
 -rw-r--r--  2.0 unx     1642 b- defN 80-Jan-01 00:00 promptflow/azure/_load_functions.py
 -rw-r--r--  2.0 unx     1808 b- defN 80-Jan-01 00:00 promptflow/azure/_ml/__init__.py
--rw-r--r--  2.0 unx    15590 b- defN 80-Jan-01 00:00 promptflow/azure/_pf_client.py
+-rw-r--r--  2.0 unx    15804 b- defN 80-Jan-01 00:00 promptflow/azure/_pf_client.py
 -rw-r--r--  2.0 unx     2721 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/README.md
 -rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/__init__.py
 -rw-r--r--  2.0 unx      755 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/__init__.py
 -rw-r--r--  2.0 unx     6459 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/_azure_machine_learning_designer_service_client.py
 -rw-r--r--  2.0 unx     2366 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/_configuration.py
 -rw-r--r--  2.0 unx     1712 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/_patch.py
 -rw-r--r--  2.0 unx     1095 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/_vendor.py
@@ -59,35 +60,40 @@
 -rw-r--r--  2.0 unx   125755 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/operations/_flows_operations.py
 -rw-r--r--  2.0 unx    10194 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/operations/_flows_provider_operations.py
 -rw-r--r--  2.0 unx    25009 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/operations/_tools_operations.py
 -rw-r--r--  2.0 unx    23026 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/operations/_trace_sessions_operations.py
 -rw-r--r--  2.0 unx       26 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow/py.typed
 -rw-r--r--  2.0 unx    27483 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/flow_service_caller.py
 -rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/service_caller_factory.py
+-rw-r--r--  2.0 unx   862524 b- defN 80-Jan-01 00:00 promptflow/azure/_restclient/swagger.json
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 promptflow/azure/_schemas/__init__.py
 -rw-r--r--  2.0 unx     1751 b- defN 80-Jan-01 00:00 promptflow/azure/_schemas/_flow_schema.py
 -rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/__init__.py
+-rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/blob/__init__.py
+-rw-r--r--  2.0 unx     5489 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/blob/client.py
 -rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/__init__.py
--rw-r--r--  2.0 unx     3727 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/client.py
--rw-r--r--  2.0 unx     3228 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/collection.py
+-rw-r--r--  2.0 unx     3810 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/client.py
+-rw-r--r--  2.0 unx     3556 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/collection.py
 -rw-r--r--  2.0 unx      662 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/cosmosdb_utils.py
--rw-r--r--  2.0 unx     2163 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/span.py
--rw-r--r--  2.0 unx    10428 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/summary.py
+-rw-r--r--  2.0 unx     3161 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/span.py
+-rw-r--r--  2.0 unx    10996 b- defN 80-Jan-01 00:00 promptflow/azure/_storage/cosmosdb/summary.py
+-rw-r--r--  2.0 unx      289 b- defN 80-Jan-01 00:00 promptflow/azure/_user_agent.py
 -rw-r--r--  2.0 unx      319 b- defN 80-Jan-01 00:00 promptflow/azure/_utils/__init__.py
 -rw-r--r--  2.0 unx     3080 b- defN 80-Jan-01 00:00 promptflow/azure/_utils/_tracing.py
 -rw-r--r--  2.0 unx     2206 b- defN 80-Jan-01 00:00 promptflow/azure/_utils/_url_utils.py
 -rw-r--r--  2.0 unx     1231 b- defN 80-Jan-01 00:00 promptflow/azure/_utils/general.py
+-rw-r--r--  2.0 unx      297 b- defN 80-Jan-01 00:00 promptflow/azure/_version.py
 -rw-r--r--  2.0 unx      399 b- defN 80-Jan-01 00:00 promptflow/azure/operations/__init__.py
--rw-r--r--  2.0 unx     2459 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_arm_connection_operations.py
--rw-r--r--  2.0 unx    17342 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_artifact_utilities.py
+-rw-r--r--  2.0 unx     3702 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_arm_connection_operations.py
+-rw-r--r--  2.0 unx    17351 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_artifact_utilities.py
 -rw-r--r--  2.0 unx    14378 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_async_run_downloader.py
 -rw-r--r--  2.0 unx     3837 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_connection_operations.py
 -rw-r--r--  2.0 unx     9139 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_fileshare_storeage_helper.py
--rw-r--r--  2.0 unx    28112 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_flow_operations.py
--rw-r--r--  2.0 unx    47347 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_run_operations.py
+-rw-r--r--  2.0 unx    28114 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_flow_operations.py
+-rw-r--r--  2.0 unx    47326 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_run_operations.py
 -rw-r--r--  2.0 unx     1710 b- defN 80-Jan-01 00:00 promptflow/azure/operations/_trace_operations.py
 -rw-r--r--  2.0 unx      283 b- defN 80-Jan-01 00:00 promptflow/azure/resources/component_spec_template.yaml
--rw-r--r--  2.0 unx     1440 b- defN 80-Jan-01 00:00 promptflow_azure-0.1.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 promptflow_azure-0.1.0b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 promptflow_azure-0.1.0b1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    10148 b- defN 16-Jan-01 00:00 promptflow_azure-0.1.0b1.dist-info/RECORD
-91 files, 4614182 bytes uncompressed, 587568 bytes compressed:  87.3%
+-rw-r--r--  2.0 unx     3051 b- defN 80-Jan-01 00:00 promptflow_azure-1.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 promptflow_azure-1.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 promptflow_azure-1.8.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    10698 b- defN 16-Jan-01 00:00 promptflow_azure-1.8.0.dist-info/RECORD
+97 files, 5489707 bytes uncompressed, 651082 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: promptflow/azure/_cli/_flow.py
 Comment: 
 
 Filename: promptflow/azure/_cli/_run.py
 Comment: 
 
+Filename: promptflow/azure/_cli/_user_agent.py
+Comment: 
+
 Filename: promptflow/azure/_cli/_utils.py
 Comment: 
 
 Filename: promptflow/azure/_cli/entry.py
 Comment: 
 
 Filename: promptflow/azure/_constants/__init__.py
@@ -186,23 +189,32 @@
 
 Filename: promptflow/azure/_restclient/flow_service_caller.py
 Comment: 
 
 Filename: promptflow/azure/_restclient/service_caller_factory.py
 Comment: 
 
+Filename: promptflow/azure/_restclient/swagger.json
+Comment: 
+
 Filename: promptflow/azure/_schemas/__init__.py
 Comment: 
 
 Filename: promptflow/azure/_schemas/_flow_schema.py
 Comment: 
 
 Filename: promptflow/azure/_storage/__init__.py
 Comment: 
 
+Filename: promptflow/azure/_storage/blob/__init__.py
+Comment: 
+
+Filename: promptflow/azure/_storage/blob/client.py
+Comment: 
+
 Filename: promptflow/azure/_storage/cosmosdb/__init__.py
 Comment: 
 
 Filename: promptflow/azure/_storage/cosmosdb/client.py
 Comment: 
 
 Filename: promptflow/azure/_storage/cosmosdb/collection.py
@@ -213,26 +225,32 @@
 
 Filename: promptflow/azure/_storage/cosmosdb/span.py
 Comment: 
 
 Filename: promptflow/azure/_storage/cosmosdb/summary.py
 Comment: 
 
+Filename: promptflow/azure/_user_agent.py
+Comment: 
+
 Filename: promptflow/azure/_utils/__init__.py
 Comment: 
 
 Filename: promptflow/azure/_utils/_tracing.py
 Comment: 
 
 Filename: promptflow/azure/_utils/_url_utils.py
 Comment: 
 
 Filename: promptflow/azure/_utils/general.py
 Comment: 
 
+Filename: promptflow/azure/_version.py
+Comment: 
+
 Filename: promptflow/azure/operations/__init__.py
 Comment: 
 
 Filename: promptflow/azure/operations/_arm_connection_operations.py
 Comment: 
 
 Filename: promptflow/azure/operations/_artifact_utilities.py
@@ -255,20 +273,20 @@
 
 Filename: promptflow/azure/operations/_trace_operations.py
 Comment: 
 
 Filename: promptflow/azure/resources/component_spec_template.yaml
 Comment: 
 
-Filename: promptflow_azure-0.1.0b1.dist-info/METADATA
+Filename: promptflow_azure-1.8.0.dist-info/METADATA
 Comment: 
 
-Filename: promptflow_azure-0.1.0b1.dist-info/WHEEL
+Filename: promptflow_azure-1.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: promptflow_azure-0.1.0b1.dist-info/entry_points.txt
+Filename: promptflow_azure-1.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: promptflow_azure-0.1.0b1.dist-info/RECORD
+Filename: promptflow_azure-1.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## promptflow/azure/_cli/entry.py

```diff
@@ -2,26 +2,33 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 # pylint: disable=wrong-import-position
 import json
 import time
 
 from promptflow._cli._pf.help import show_privacy_statement, show_welcome_message
-from promptflow._cli._user_agent import USER_AGENT
 from promptflow._cli._utils import _get_cli_activity_name, cli_exception_and_telemetry_handler, get_client_info_for_cli
+from promptflow.azure._cli._user_agent import USER_AGENT
 
 # Log the start time
 start_time = time.perf_counter()
 
 # E402 module level import not at top of file
 import argparse  # noqa: E402
 import logging  # noqa: E402
 import sys  # noqa: E402
 
-from promptflow._sdk._utils import get_promptflow_sdk_version, print_pf_version  # noqa: E402
+from promptflow._sdk._utils import (  # noqa: E402
+    get_promptflow_azure_version,
+    get_promptflow_core_version,
+    get_promptflow_devkit_version,
+    get_promptflow_sdk_version,
+    get_promptflow_tracing_version,
+    print_pf_version,
+)
 from promptflow._utils.logger_utils import get_cli_sdk_logger  # noqa: E402
 from promptflow._utils.user_agent_utils import setup_user_agent_to_operation_context  # noqa: E402
 from promptflow.azure._cli._flow import add_parser_flow, dispatch_flow_commands  # noqa: E402
 from promptflow.azure._cli._run import add_parser_run, dispatch_run_commands  # noqa: E402
 
 # get logger for CLI
 logger = get_cli_sdk_logger()
@@ -36,15 +43,15 @@
             for handler in logger.handlers:
                 handler.setLevel(logging.INFO)
         # --debug, enable debug logging
         if hasattr(args, "debug") and args.debug:
             for handler in logger.handlers:
                 handler.setLevel(logging.DEBUG)
         if args.version:
-            print_pf_version()
+            print_pf_version(with_azure=True)
         elif args.action == "run":
             dispatch_run_commands(args)
         elif args.action == "flow":
             dispatch_flow_commands(args)
     except KeyboardInterrupt as ex:
         logger.debug("Keyboard interrupt is captured.")
         raise ex
@@ -113,14 +120,30 @@
 
 
 def main():
     """Entrance of pf CLI."""
     command_args = sys.argv[1:]
     if len(command_args) == 1 and command_args[0] == "version":
         version_dict = {"promptflow": get_promptflow_sdk_version()}
+        # check tracing version
+        version_tracing = get_promptflow_tracing_version()
+        if version_tracing:
+            version_dict["promptflow-tracing"] = version_tracing
+        # check azure version
+        version_azure = get_promptflow_azure_version()
+        if version_azure:
+            version_dict["promptflow-azure"] = version_azure
+        # check core version
+        version_core = get_promptflow_core_version()
+        if version_core:
+            version_dict["promptflow-core"] = version_core
+        # check devkit version
+        version_devkit = get_promptflow_devkit_version()
+        if version_devkit:
+            version_dict["promptflow-devkit"] = version_devkit
         return json.dumps(version_dict, ensure_ascii=False, indent=2, sort_keys=True, separators=(",", ": ")) + "\n"
     if len(command_args) == 0:
         # print privacy statement & welcome message like azure-cli
         show_privacy_statement()
         show_welcome_message()
         command_args.append("-h")
     elif len(command_args) == 1:
```

## promptflow/azure/_pf_client.py

```diff
@@ -1,32 +1,32 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 import os
 from os import PathLike
-from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 from azure.ai.ml import MLClient
 from azure.core.credentials import TokenCredential
 
 from promptflow._sdk._constants import MAX_SHOW_DETAILS_RESULTS
 from promptflow._sdk._errors import RunOperationParameterError
-from promptflow._sdk._user_agent import USER_AGENT
 from promptflow._sdk._utils import generate_yaml_entry
 from promptflow._sdk.entities import Run
 from promptflow._utils.user_agent_utils import ClientUserAgentUtil, setup_user_agent_to_operation_context
 from promptflow.azure._restclient.service_caller_factory import _FlowServiceCallerFactory
 from promptflow.azure.operations import RunOperations
 from promptflow.azure.operations._arm_connection_operations import ArmConnectionOperations
 from promptflow.azure.operations._connection_operations import ConnectionOperations
 from promptflow.azure.operations._flow_operations import FlowOperations
 from promptflow.azure.operations._trace_operations import TraceOperations
 from promptflow.exceptions import UserErrorException
 
+from ._user_agent import USER_AGENT
+
 
 class PFClient:
     """A client class to interact with Promptflow service.
 
     Use this client to manage promptflow resources, e.g. runs.
 
     :param credential: Credential to use for authentication, optional
@@ -195,14 +195,15 @@
         connections: dict = None,
         environment_variables: dict = None,
         name: str = None,
         display_name: str = None,
         tags: Dict[str, str] = None,
         resume_from: Union[str, Run] = None,
         code: Union[str, PathLike] = None,
+        init: Optional[dict] = None,
         **kwargs,
     ) -> Run:
         """Run flow against provided data or run.
 
         .. note:: at least one of data or run must be provided.
 
         .. admonition::
@@ -252,17 +253,22 @@
         :type display_name: str
         :param tags: Tags of the run.
         :type tags: Dict[str, str]
         :param resume_from: Create run resume from an existing run.
         :type resume_from: str
         :param code: Path to the code directory to run.
         :type code: Union[str, PathLike]
+        :param init: Initialization parameters for flex flow, only supported when flow is callable class.
+        :type init: dict
         :return: flow run info.
         :rtype: ~promptflow.entities.Run
         """
+        # TODO(3047273): support cloud run init
+        if init:
+            raise NotImplementedError("init is not supported for pfazure.")
         if resume_from:
             unsupported = {
                 k: v
                 for k, v in {
                     "flow": flow,
                     "data": data,
                     "run": run,
@@ -277,18 +283,16 @@
                 raise ValueError(
                     f"'resume_from' is not supported to be used with the with following parameters: {unsupported}. "
                 )
             resume_from = resume_from.name if isinstance(resume_from, Run) else resume_from
             return self.runs._create_by_resume_from(
                 resume_from=resume_from, name=name, display_name=display_name, tags=tags, **kwargs
             )
-
-        if code and not os.path.exists(code):
-            raise FileNotFoundError(f"code path {code} does not exist")
-        code = Path(code) if code else Path(os.getcwd())
+        if callable(flow):
+            raise UserErrorException(f"Providing callable {flow} as flow is not supported.")
         with generate_yaml_entry(entry=flow, code=code) as flow:
             run = Run(
                 name=name,
                 display_name=display_name,
                 tags=tags,
                 data=data,
                 column_mapping=column_mapping,
```

## promptflow/azure/_storage/cosmosdb/client.py

```diff
@@ -97,8 +97,9 @@
     token_client = CosmosClient(endpoint, token_dict)
     token_db = token_client.get_database_client(database_name)
     container_client = token_db.get_container_client(container_name)
     return container_client
 
 
 def _get_db_client_key(container_name: str, subscription_id: str, resource_group_name: str, workspace_name: str) -> str:
-    return f"{subscription_id}_{resource_group_name}_{workspace_name}_{container_name}"
+    # Azure name allow hyphens and underscores. User @ to avoid possible conflict.
+    return f"{subscription_id}@{resource_group_name}@{workspace_name}@{container_name}"
```

## promptflow/azure/_storage/cosmosdb/collection.py

```diff
@@ -5,16 +5,16 @@
 import time
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict
 
 from azure.cosmos import ContainerProxy
 
-from promptflow._constants import SpanAttributeFieldName, SpanFieldName, SpanResourceAttributesFieldName
-from promptflow._sdk._constants import CreatedByFieldName
+from promptflow._constants import SpanAttributeFieldName, SpanResourceAttributesFieldName, SpanResourceFieldName
+from promptflow._sdk._constants import TRACE_DEFAULT_COLLECTION, CreatedByFieldName
 from promptflow._sdk.entities._trace import Span
 from promptflow.azure._storage.cosmosdb.cosmosdb_utils import safe_create_cosmosdb_item
 
 
 @dataclass
 class Collection:
     id: str  # Collection id for cosmosDB query, usually hide from customer
@@ -35,25 +35,31 @@
     return f"{name}_{created_by[CreatedByFieldName.OBJECT_ID]}"
 
 
 class CollectionCosmosDB:
     def __init__(self, span: Span, is_cloud_trace: bool, created_by: Dict[str, Any]):
         self.span = span
         self.created_by = created_by
-        self.collection_name = span.session_id
         self.location = LocationType.CLOUD if is_cloud_trace else LocationType.LOCAL
-        resource_attributes = span._content.get(SpanFieldName.RESOURCE, None)
-        self.collection_id = (
-            resource_attributes[SpanResourceAttributesFieldName.COLLECTION_ID]
-            if is_cloud_trace
-            else generate_collection_id_by_name_and_created_by(self.collection_name, created_by)
+        resource_attributes = span.resource.get(SpanResourceFieldName.ATTRIBUTES, {})
+        self.collection_name = resource_attributes.get(
+            SpanResourceAttributesFieldName.COLLECTION, TRACE_DEFAULT_COLLECTION
         )
+        span_attributes = self.span.attributes
+        if SpanAttributeFieldName.BATCH_RUN_ID in span_attributes:
+            self.collection_id = span_attributes[SpanAttributeFieldName.BATCH_RUN_ID]
+        else:
+            self.collection_id = (
+                resource_attributes[SpanResourceAttributesFieldName.COLLECTION_ID]
+                if is_cloud_trace
+                else generate_collection_id_by_name_and_created_by(self.collection_name, created_by)
+            )
 
     def create_collection_if_not_exist(self, client: ContainerProxy):
-        span_attributes = self.span._content[SpanFieldName.ATTRIBUTES]
+        span_attributes = self.span.attributes
         # For batch run, ignore collection operation
         if SpanAttributeFieldName.BATCH_RUN_ID in span_attributes:
             return
 
         item = Collection(
             id=self.collection_id,
             partition_key=self.collection_id,
@@ -67,15 +73,15 @@
         # Update name if customer change flow display name
         patch_operations = [{"op": "replace", "path": "/name", "value": self.collection_name}]
         return client.patch_item(
             item=self.collection_id, partition_key=self.collection_id, patch_operations=patch_operations
         )
 
     def update_collection_updated_at_info(self, client: ContainerProxy):
-        span_attributes = self.span._content[SpanFieldName.ATTRIBUTES]
+        span_attributes = self.span.attributes
         # For batch run, ignore collection operation
         if SpanAttributeFieldName.BATCH_RUN_ID in span_attributes:
             return
 
         patch_operations = [{"op": "replace", "path": "/updated_at", "value": int(time.time())}]
         return client.patch_item(
             item=self.collection_id, partition_key=self.collection_id, patch_operations=patch_operations
```

## promptflow/azure/_storage/cosmosdb/span.py

```diff
@@ -1,19 +1,22 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
+import json
 from typing import Any, Dict
 
-from promptflow._constants import SpanFieldName
+from azure.cosmos.container import ContainerProxy
+from azure.storage.blob import ContainerClient
+
+from promptflow._constants import SpanContextFieldName, SpanEventFieldName, SpanFieldName
 from promptflow._sdk.entities._trace import Span as SpanEntity
 
 
 class Span:
-
     name: str = None
     context: dict = None
     kind: str = None
     parent_id: str = None
     start_time: str = None
     end_time: str = None
     status: dict = None
@@ -21,42 +24,62 @@
     events: list = None
     links: list = None
     resource: dict = None
     id: str = None
     partition_key: str = None
     collection_id: str = None
     created_by: dict = None
+    external_event_data_uris: list = None
 
     def __init__(self, span: SpanEntity, collection_id: str, created_by: dict) -> None:
         self.name = span.name
-        self.context = span._content[SpanFieldName.CONTEXT]
-        self.kind = span._content[SpanFieldName.KIND]
-        self.parent_id = span.parent_span_id
-        self.start_time = span._content[SpanFieldName.START_TIME]
-        self.end_time = span._content[SpanFieldName.END_TIME]
-        self.status = span._content[SpanFieldName.STATUS]
-        self.attributes = span._content[SpanFieldName.ATTRIBUTES]
-        self.events = span._content[SpanFieldName.EVENTS]
-        self.links = span._content[SpanFieldName.LINKS]
-        self.resource = span._content[SpanFieldName.RESOURCE]
-        self.partition_key = span.session_id
+        self.context = span.context
+        self.kind = span.kind
+        self.parent_id = span.parent_id
+        self.start_time = span.start_time.isoformat()
+        self.end_time = span.end_time.isoformat()
+        self.status = span.status
+        self.attributes = span.attributes
+        self.events = span.events
+        self.links = span.links
+        self.resource = span.resource
+        self.partition_key = collection_id
         self.collection_id = collection_id
         self.id = span.span_id
         self.created_by = created_by
+        self.external_event_data_uris = []
 
-    def persist(self, client):
+    def persist(self, cosmos_client: ContainerProxy, blob_container_client: ContainerClient, blob_base_uri: str):
         if self.id is None or self.partition_key is None or self.resource is None:
             return
 
         resource_attributes = self.resource.get(SpanFieldName.ATTRIBUTES, None)
         if resource_attributes is None:
             return
 
+        if self.events and blob_container_client is not None and blob_base_uri is not None:
+            self._persist_events(blob_container_client, blob_base_uri)
+
         from azure.cosmos.exceptions import CosmosResourceExistsError
 
         try:
-            return client.create_item(body=self.to_dict())
+            return cosmos_client.create_item(body=self.to_dict())
         except CosmosResourceExistsError:
-            return None
+            return
 
     def to_dict(self) -> Dict[str, Any]:
         return {k: v for k, v in self.__dict__.items() if v}
+
+    def _persist_events(self, blob_container_client: ContainerClient, blob_base_uri: str):
+        for idx, event in enumerate(self.events):
+            event_data = json.dumps(event)
+            blob_client = blob_container_client.get_blob_client(self._event_path(idx))
+            blob_client.upload_blob(event_data)
+
+            event[SpanEventFieldName.ATTRIBUTES] = {}
+            self.external_event_data_uris.append(f"{blob_base_uri}{self._event_path(idx)}")
+
+    EVENT_PATH_PREFIX = ".promptflow/.trace"
+
+    def _event_path(self, idx: int) -> str:
+        trace_id = self.context[SpanContextFieldName.TRACE_ID]
+        return f"{self.EVENT_PATH_PREFIX}/{self.collection_id}/{trace_id}/{self.id}/{idx}"
```

## promptflow/azure/_storage/cosmosdb/summary.py

```diff
@@ -6,17 +6,18 @@
 
 from azure.cosmos import ContainerProxy
 
 from promptflow._constants import (
     OK_LINE_RUN_STATUS,
     RUNNING_LINE_RUN_STATUS,
     SpanAttributeFieldName,
-    SpanFieldName,
+    SpanResourceAttributesFieldName,
     SpanStatusFieldName,
 )
+from promptflow._sdk._constants import TRACE_DEFAULT_COLLECTION
 from promptflow._sdk._utils import json_loads_parse_const_as_str
 from promptflow._sdk.entities._trace import Span
 from promptflow.azure._storage.cosmosdb.cosmosdb_utils import safe_create_cosmosdb_item
 
 
 @dataclass
 class SummaryLine:
@@ -70,22 +71,23 @@
 
 
 class Summary:
     def __init__(self, span: Span, collection_id: str, created_by: typing.Dict, logger: logging.Logger) -> None:
         self.span = span
         self.created_by = created_by
         self.logger = logger
+        self.session_id = self.span.resource.get(SpanResourceAttributesFieldName.COLLECTION, TRACE_DEFAULT_COLLECTION)
         self.collection_id = collection_id
 
     def persist(self, client: ContainerProxy):
-        if self.span.parent_span_id:
+        if self.span.parent_id:
             # For non root span, write a placeholder item to LineSummary table.
             self._persist_running_item(client)
             return
-        attributes = self.span._content[SpanFieldName.ATTRIBUTES]
+        attributes = self.span.attributes
 
         # Persist root span as a line run.
         self._persist_line_run(client)
 
         if (
             SpanAttributeFieldName.LINE_RUN_ID not in attributes
             and SpanAttributeFieldName.BATCH_RUN_ID not in attributes
@@ -101,40 +103,40 @@
             and SpanAttributeFieldName.LINE_NUMBER in attributes
         ):
             self._insert_evaluation_with_retry(client)
 
     # When there is the first span for line run, write placeholder item to LineSummary table.
     def _persist_running_item(self, client: ContainerProxy):
         trace_id = self.span.trace_id
-        session_id = self.span.session_id
+        session_id = self.session_id
 
         item = SummaryLine(
             id=trace_id,
-            partition_key=session_id,
+            partition_key=self.collection_id,
             session_id=session_id,
             trace_id=trace_id,
             status=RUNNING_LINE_RUN_STATUS,
             collection_id=self.collection_id,
             created_by=self.created_by,
-            start_time=self.span._content[SpanFieldName.START_TIME],
+            start_time=self.span.start_time.isoformat(),
         )
-        attributes: dict = self.span._content[SpanFieldName.ATTRIBUTES]
+        attributes: dict = self.span.attributes
         if SpanAttributeFieldName.LINE_RUN_ID in attributes:
             item.line_run_id = attributes[SpanAttributeFieldName.LINE_RUN_ID]
         elif SpanAttributeFieldName.BATCH_RUN_ID in attributes and SpanAttributeFieldName.LINE_NUMBER in attributes:
             item.batch_run_id = attributes[SpanAttributeFieldName.BATCH_RUN_ID]
             item.line_number = attributes[SpanAttributeFieldName.LINE_NUMBER]
         safe_create_cosmosdb_item(client, item)
 
     def _persist_line_run(self, client: ContainerProxy):
-        attributes: dict = self.span._content[SpanFieldName.ATTRIBUTES]
+        attributes: dict = self.span.attributes
 
-        session_id = self.span.session_id
-        start_time = self.span._content[SpanFieldName.START_TIME]
-        end_time = self.span._content[SpanFieldName.END_TIME]
+        session_id = self.session_id
+        start_time = self.span.start_time.isoformat()
+        end_time = self.span.end_time.isoformat()
 
         # Span's original format don't include latency, so we need to calculate it.
         # Convert ISO 8601 formatted strings to datetime objects
         start_time_date = datetime.datetime.fromisoformat(start_time.replace("Z", "+00:00"))
         end_time_date = datetime.datetime.fromisoformat(end_time.replace("Z", "+00:00"))
         latency = (end_time_date - start_time_date).total_seconds()
         # calculate `cumulative_token_count`
@@ -148,24 +150,24 @@
                 "prompt": prompt_token_count,
                 "total": total_token_count,
             }
         else:
             cumulative_token_count = None
         item = SummaryLine(
             id=self.span.trace_id,  # trace id is unique for LineSummary container
-            partition_key=session_id,
+            partition_key=self.collection_id,
             session_id=session_id,
             trace_id=self.span.trace_id,
             collection_id=self.collection_id,
             root_span_id=self.span.span_id,
             inputs=json_loads_parse_const_as_str(attributes.get(SpanAttributeFieldName.INPUTS, "{}")),
             outputs=json_loads_parse_const_as_str(attributes.get(SpanAttributeFieldName.OUTPUT, "{}")),
             start_time=start_time,
             end_time=end_time,
-            status=self.span._content[SpanFieldName.STATUS][SpanStatusFieldName.STATUS_CODE],
+            status=self.span.status[SpanStatusFieldName.STATUS_CODE],
             latency=latency,
             name=self.span.name,
             kind=attributes[SpanAttributeFieldName.SPAN_TYPE],
             cumulative_token_count=cumulative_token_count,
             created_by=self.created_by,
         )
         if SpanAttributeFieldName.LINE_RUN_ID in attributes:
@@ -189,23 +191,21 @@
             except InsertEvaluationsRetriableException as e:
                 if attempt == 2:  # If this is the last attempt, ignore and just return
                     self.logger.error(f"Error while inserting evaluation: {e}")
                     return
                 time.sleep(1)
 
     def _insert_evaluation(self, client: ContainerProxy):
-        attributes: dict = self.span._content[SpanFieldName.ATTRIBUTES]
-        partition_key = self.span.session_id
-        name = self.span.name
+        attributes: dict = self.span.attributes
         item = LineEvaluation(
             trace_id=self.span.trace_id,
             root_span_id=self.span.span_id,
             collection_id=self.collection_id,
             outputs=json_loads_parse_const_as_str(attributes.get(SpanAttributeFieldName.OUTPUT, "{}")),
-            name=name,
+            name=self.span.name,
             created_by=self.created_by,
         )
 
         # None is the default value for the field.
         referenced_line_run_id = attributes.get(SpanAttributeFieldName.REFERENCED_LINE_RUN_ID, None)
         referenced_batch_run_id = attributes.get(SpanAttributeFieldName.REFERENCED_BATCH_RUN_ID, None)
         line_number = attributes.get(SpanAttributeFieldName.LINE_NUMBER, None)
@@ -215,32 +215,40 @@
             "c.line_run_id = @line_run_id AND c.batch_run_id = @batch_run_id AND c.line_number = @line_number"
         )
         parameters = [
             {"name": "@line_run_id", "value": referenced_line_run_id},
             {"name": "@batch_run_id", "value": referenced_batch_run_id},
             {"name": "@line_number", "value": line_number},
         ]
-        query_results = list(client.query_items(query=query, parameters=parameters, partition_key=partition_key))
+        # Don't use partition key for query, we can't know the partition key of main run in all scenarios.
+        query_results = list(client.query_items(query=query, parameters=parameters, enable_cross_partition_query=True))
 
         if query_results:
             current_status = query_results[0].get("status", "")
             if current_status != OK_LINE_RUN_STATUS:
                 raise InsertEvaluationsRetriableException(
                     f"Main run status is {current_status}, cannot patch evaluation now."
                 )
             main_id = query_results[0]["id"]
+            main_partition_key = query_results[0]["partition_key"]
         else:
             raise InsertEvaluationsRetriableException(f"Cannot find main run by parameter {parameters}.")
 
         if SpanAttributeFieldName.LINE_RUN_ID in attributes:
             item.line_run_id = attributes[SpanAttributeFieldName.LINE_RUN_ID]
+            key = self.span.name
         else:
-            item.batch_run_id = attributes[SpanAttributeFieldName.BATCH_RUN_ID]
+            batch_run_id = attributes[SpanAttributeFieldName.BATCH_RUN_ID]
+            item.batch_run_id = batch_run_id
             item.line_number = line_number
+            # Use the batch run id, instead of the name, as the key in the evaluations dictionary.
+            # Customers may execute the same evaluation flow multiple times for a batch run.
+            # We should be able to save all evaluations, as customers use batch runs in a critical manner.
+            key = batch_run_id
 
-        patch_operations = [{"op": "add", "path": f"/evaluations/{name}", "value": asdict(item)}]
+        patch_operations = [{"op": "add", "path": f"/evaluations/{key}", "value": asdict(item)}]
         self.logger.info(f"Insert evaluation for LineSummary main_id: {main_id}")
-        return client.patch_item(item=main_id, partition_key=partition_key, patch_operations=patch_operations)
+        return client.patch_item(item=main_id, partition_key=main_partition_key, patch_operations=patch_operations)
 
 
 class InsertEvaluationsRetriableException(Exception):
     pass
```

## promptflow/azure/operations/_arm_connection_operations.py

```diff
@@ -6,14 +6,16 @@
 from azure.ai.ml._scope_dependent_operations import (
     OperationConfig,
     OperationsContainer,
     OperationScope,
     _ScopeDependentOperations,
 )
 
+from promptflow._sdk._errors import ConnectionClassNotFoundError
+from promptflow._sdk.entities._connection import CustomConnection, _Connection
 from promptflow.azure._restclient.flow_service_caller import FlowServiceCaller
 from promptflow.core._connection_provider._workspace_connection_provider import WorkspaceConnectionProvider
 from promptflow.core._errors import OpenURLFailedUserError
 
 
 class ArmConnectionOperations(_ScopeDependentOperations):
     """ArmConnectionOperations.
@@ -39,16 +41,37 @@
         self._provider = WorkspaceConnectionProvider(
             self._operation_scope.subscription_id,
             self._operation_scope.resource_group_name,
             self._operation_scope.workspace_name,
             self._credential,
         )
 
+    @classmethod
+    def _convert_core_connection_to_sdk_connection(cls, core_conn):
+        # TODO: Refine this and connection operation ones to (devkit) _Connection._from_core_object
+        sdk_conn_mapping = _Connection.SUPPORTED_TYPES
+        sdk_conn_cls = sdk_conn_mapping.get(core_conn.type)
+        if sdk_conn_cls is None:
+            raise ConnectionClassNotFoundError(
+                f"Correspond sdk connection type not found for core connection type: {core_conn.type!r}, "
+                f"please re-install the 'promptflow' package."
+            )
+        common_args = {
+            "name": core_conn.name,
+            "module": core_conn.module,
+            "expiry_time": core_conn.expiry_time,
+            "created_date": core_conn.created_date,
+            "last_modified_date": core_conn.last_modified_date,
+        }
+        if sdk_conn_cls is CustomConnection:
+            return sdk_conn_cls(configs=core_conn.configs, secrets=core_conn.secrets, **common_args)
+        return sdk_conn_cls(**dict(core_conn), **common_args)
+
     def get(self, name, **kwargs):
-        return self._provider.get(name)
+        return self._convert_core_connection_to_sdk_connection(self._provider.get(name))
 
     @classmethod
     def _direct_get(cls, name, subscription_id, resource_group_name, workspace_name, credential):
         """
         This method is added for local pf_client with workspace provider to ensure we only require limited
         permission(workspace/list secrets). As create azure pf_client requires workspace read permission.
         """
```

## promptflow/azure/operations/_artifact_utilities.py

```diff
@@ -39,15 +39,16 @@
 from azure.ai.ml.entities._credentials import AccountKeyConfiguration
 from azure.ai.ml.entities._datastore._constants import WORKSPACE_BLOB_STORE
 from azure.ai.ml.exceptions import ErrorTarget, ValidationException
 from azure.ai.ml.operations._datastore_operations import DatastoreOperations
 from azure.storage.blob import BlobSasPermissions, generate_blob_sas
 from azure.storage.filedatalake import FileSasPermissions, generate_file_sas
 
-from ..._utils.logger_utils import LoggerFactory
+from promptflow._utils.logger_utils import LoggerFactory
+
 from ._fileshare_storeage_helper import FlowFileStorageClient
 
 module_logger = LoggerFactory.get_logger(__name__)
 
 
 def _get_datastore_name(*, datastore_name: Optional[str] = WORKSPACE_BLOB_STORE) -> str:
     datastore_name = WORKSPACE_BLOB_STORE if not datastore_name else datastore_name
```

## promptflow/azure/operations/_flow_operations.py

```diff
@@ -204,15 +204,15 @@
         logger.info(f"Flow updated successfully:\n{json.dumps(flow_dict, indent=4)}")
 
         return updated_flow
 
     @staticmethod
     def _validate_flow_creation_parameters(source, flow_display_name=None, flow_type=None, **kwargs):
         """Validate the parameters for flow creation operation."""
-        from promptflow._sdk.entities._flow import FlexFlow
+        from promptflow._sdk.entities._flows import FlexFlow
         from promptflow.client import load_flow as load_local_flow
 
         # validate the source folder
         logger.info("Validating flow source.")
         if not Path(source, DAG_FILE_NAME).exists():
             raise UserErrorException(
                 f"Flow source must be a directory with flow definition yaml '{DAG_FILE_NAME}'. "
@@ -252,15 +252,15 @@
             kwargs["tags"] = tags
 
         return flow, flow_display_name, flow_type, kwargs
 
     @staticmethod
     def _validate_flow_schema(source, display_name=None, type=None, **kwargs):
         """Validate the flow schema."""
-        from promptflow._sdk.entities._flow import Flow
+        from promptflow._sdk.entities._flows import Flow
 
         params_override = copy.deepcopy(kwargs)
         if display_name is not None:
             params_override["display_name"] = display_name
         if type is not None:
             params_override["type"] = type
```

## promptflow/azure/operations/_run_operations.py

```diff
@@ -42,20 +42,15 @@
     ListViewType,
     RunDataKeys,
     RunHistoryKeys,
     RunStatus,
 )
 from promptflow._sdk._errors import InvalidRunStatusError, RunNotFoundError, RunOperationParameterError
 from promptflow._sdk._telemetry import ActivityType, WorkspaceTelemetryMixin, monitor_operation
-from promptflow._sdk._utils import (
-    incremental_print,
-    is_multi_container_enabled,
-    is_remote_uri,
-    print_red_error,
-)
+from promptflow._sdk._utils import incremental_print, is_multi_container_enabled, is_remote_uri, print_red_error
 from promptflow._sdk.entities import Run
 from promptflow._utils.async_utils import async_run_allowing_running_loop
 from promptflow._utils.logger_utils import get_cli_sdk_logger
 from promptflow._utils.utils import in_jupyter_notebook
 from promptflow.azure._constants._flow import AUTOMATIC_RUNTIME, AUTOMATIC_RUNTIME_NAME, CLOUD_RUNS_PAGE_SIZE
 from promptflow.azure._load_functions import load_flow
 from promptflow.azure._restclient.flow_service_caller import FlowServiceCaller
@@ -1020,15 +1015,15 @@
             enable_multi_container=is_multi_container_enabled(),
         )
         return rest_obj
 
     @monitor_operation(activity_name="pfazure.runs.resume", activity_type=ActivityType.PUBLICAPI)
     def _create_by_resume_from(self, resume_from: str, **kwargs):
         """Create a run by specify resume_from to an existing run."""
-        stream = kwargs.get("stream", False)
+        stream = kwargs.pop("stream", False)
         run_name = self._service_caller.resume_bulk_run(
             subscription_id=self._operation_scope.subscription_id,
             resource_group_name=self._operation_scope.resource_group_name,
             workspace_name=self._operation_scope.workspace_name,
             body=self._build_resume_request_rest_object(resume_from=resume_from, **kwargs),
         )
```

## Comparing `promptflow_azure-0.1.0b1.dist-info/RECORD` & `promptflow_azure-1.8.0.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 promptflow/azure/__init__.py,sha256=DXMuDEOZou8lLpsV8qLGB3-UVjP8TU2NGHukdn90dFA,320
 promptflow/azure/_cli/__init__.py,sha256=vV8bhHRJHrJVbMOhR8jvnWF0_ZwCRQiSsUwf0X04gtg,262
 promptflow/azure/_cli/_connection.py,sha256=9-LX7vgDk_-D_HzsTCCNTtoISRcVUpH-QWWnnrSJZRE,3566
 promptflow/azure/_cli/_flow.py,sha256=dRDoAhwx2XFyUUQ-4mFHsdG7Gm_eS3cDldS7BrWIM64,9458
 promptflow/azure/_cli/_run.py,sha256=Mzl525Wp2tMGUiFYW9h2zpKptvILtTqI_k_ESO3fNDQ,18636
+promptflow/azure/_cli/_user_agent.py,sha256=RgKLrKmEQexShi5dale0h-hjUNTzBYmZLFmiCMRBX1g,289
 promptflow/azure/_cli/_utils.py,sha256=qDKtl20zHdPSs3X1hmvY_vxoU8eIL9W4MbCMSsUgfBs,594
-promptflow/azure/_cli/entry.py,sha256=Q3H3j6pFVmOYJC-f32qYzZdT08CaXJc1a5Xry5TXBwg,5099
+promptflow/azure/_cli/entry.py,sha256=RpSeBzqPmmx0Wgued3JNHRT6gbGcK8MBEIXCODowObo,5971
 promptflow/azure/_constants/__init__.py,sha256=No7kGvzn7Etf-QW5uW3RYFPAQDsPqcmZ7Unad5E3sDc,484
 promptflow/azure/_constants/_component.py,sha256=y-2KrsyXNqMWHg7rspbGlHOtAlpeJycHHeUsxnCl-bk,382
 promptflow/azure/_constants/_flow.py,sha256=M6RPiSpFXifboPXrju7KH6AIV_d5BLqvVgI-ndMcphk,1049
 promptflow/azure/_entities/__init__.py,sha256=vV8bhHRJHrJVbMOhR8jvnWF0_ZwCRQiSsUwf0X04gtg,262
 promptflow/azure/_entities/_flow.py,sha256=10eT4SxxmUCRQmsBiLRLzhUI0K-ngoRTWYVKlGxEf5I,10394
 promptflow/azure/_entities/_workspace_connection_spec.py,sha256=UAiPSewCi3KLHgv7A2wrNHCaIm0XVzazBEmST6wQOBw,2010
 promptflow/azure/_load_functions.py,sha256=qSIqPI1lY7j6cqaa6kqlg9vLaurnsfU6B9UN0qpRTXw,1642
 promptflow/azure/_ml/__init__.py,sha256=d2t86QOXH94DKsmHaC1aBQDKagmmYf7RcbYyg7ElNA0,1808
-promptflow/azure/_pf_client.py,sha256=wl222Cd3v15AsozvC_rj_o2JjHYhrwzqDJRzvBCq2R0,15590
+promptflow/azure/_pf_client.py,sha256=PuWHTeJWs0gC7I8S8-_-3twVAv84R3PwuHLrQfoR3l0,15804
 promptflow/azure/_restclient/README.md,sha256=VLnGY9D99O2t6jZ6oRbtUdy2AF1xNI2bBc1wmPQKCt8,2721
 promptflow/azure/_restclient/__init__.py,sha256=Yx1Iq2GNKQ5lYxTotvPwkPL4u0cm6YVxUe-iVbu1clI,180
 promptflow/azure/_restclient/flow/__init__.py,sha256=rNVzNp6TQKYt3Syh9sTJz4yRXomFbqrG-7Yjcdt9dmA,755
 promptflow/azure/_restclient/flow/_azure_machine_learning_designer_service_client.py,sha256=3lcdAXLtNp6jrKVj1rbNG5uC2xbcSOjj4nbm8egsDL8,6459
 promptflow/azure/_restclient/flow/_configuration.py,sha256=ccggZoi-rt7evku_2YFJ0-PJ6eGTE1XRcM3rr1THLQg,2366
 promptflow/azure/_restclient/flow/_patch.py,sha256=lvAtbb_xS2NvERfbdsc0Ct3yXlJN6NfkMfxHDtHAdmQ,1712
 promptflow/azure/_restclient/flow/_vendor.py,sha256=r93qWxRCXCvJo9F0j27BjH9O4MdRyae2hSOyQWBK-Yc,1095
@@ -58,34 +59,39 @@
 promptflow/azure/_restclient/flow/operations/_flows_operations.py,sha256=yOX7f01b4MRoxCkgzBjmfuE71Ddsw9sgfYLOmem0WZ8,125755
 promptflow/azure/_restclient/flow/operations/_flows_provider_operations.py,sha256=exAhnWqryovuquiy_aAXN2QD07aBXsT0jqBFyrdqHcE,10194
 promptflow/azure/_restclient/flow/operations/_tools_operations.py,sha256=CRkEEu86gAOpu3F_gRTWoNs0eMjKDQV4SWnXIJbWBpE,25009
 promptflow/azure/_restclient/flow/operations/_trace_sessions_operations.py,sha256=nb4Lyl_rhq66Po6DxLC6YOdDcPuiWCd3V7UxB0N2eKI,23026
 promptflow/azure/_restclient/flow/py.typed,sha256=dcrsqJrcYfTX-ckLFJMTaj6mD8aDe2u0tkQG-ZYxnEg,26
 promptflow/azure/_restclient/flow_service_caller.py,sha256=EJ-JooyhLlL2S8PGo2GBkmn4OuRBx0FREAoKvdv5BbQ,27483
 promptflow/azure/_restclient/service_caller_factory.py,sha256=fxtlEybv2o9HYIxuTkWDkZdWh5lhSb0SoCbO7QuGciA,1081
+promptflow/azure/_restclient/swagger.json,sha256=7mVk2r_2gzB-tBNwm9IXnXGB4xdCRZaH7kPIziu3_6A,862524
 promptflow/azure/_schemas/__init__.py,sha256=vV8bhHRJHrJVbMOhR8jvnWF0_ZwCRQiSsUwf0X04gtg,262
 promptflow/azure/_schemas/_flow_schema.py,sha256=FnuzuleBmJaeCo3tRW4FSZsXCnZFkb3eNOkkI66M7ls,1751
 promptflow/azure/_storage/__init__.py,sha256=Yx1Iq2GNKQ5lYxTotvPwkPL4u0cm6YVxUe-iVbu1clI,180
+promptflow/azure/_storage/blob/__init__.py,sha256=Yx1Iq2GNKQ5lYxTotvPwkPL4u0cm6YVxUe-iVbu1clI,180
+promptflow/azure/_storage/blob/client.py,sha256=ZBh8hIVuK06XyVEYV5fnpYXniiJurV5KIL0YthYTkwY,5489
 promptflow/azure/_storage/cosmosdb/__init__.py,sha256=Yx1Iq2GNKQ5lYxTotvPwkPL4u0cm6YVxUe-iVbu1clI,180
-promptflow/azure/_storage/cosmosdb/client.py,sha256=RAmLvJwiXCcxjcFEdSeR5emQpI-BuB4yFhzVRZzS5nc,3727
-promptflow/azure/_storage/cosmosdb/collection.py,sha256=8RvzlCbu5yfSKk-AJ0iqWTjdFoP9XlQJe7TmnP-UCFg,3228
+promptflow/azure/_storage/cosmosdb/client.py,sha256=jSToG5sBtAL8aiFEld8pX5gIBnmsq_jGlmkUt4KebcI,3810
+promptflow/azure/_storage/cosmosdb/collection.py,sha256=Itm1aAsOAuEBHX3t6fqzRwVrMKIG629ioAT-ontpYzc,3556
 promptflow/azure/_storage/cosmosdb/cosmosdb_utils.py,sha256=bCEQq5dwoaOatkwagop7b5YpAt1_S7k0szZqMoa6C2Q,662
-promptflow/azure/_storage/cosmosdb/span.py,sha256=HZoAL3cgR1GbIwBxV4gZxnJSD0eEOOjvzxfMFgjssaI,2163
-promptflow/azure/_storage/cosmosdb/summary.py,sha256=bmXfCJAYhjyxuwX92Zy-GRaV18Ko7NyIiflSRFTQ9Vo,10428
+promptflow/azure/_storage/cosmosdb/span.py,sha256=YPOemrqzabp1SHiOPU6JzQM_cOL04XvuxhRdWGh7HRs,3161
+promptflow/azure/_storage/cosmosdb/summary.py,sha256=FDjaX6ClrgACy8_LNz1krAOHncTGUT9GGDsr73Bk0hw,10996
+promptflow/azure/_user_agent.py,sha256=BFegaEjmBdwJgahlEmWtSSTFIvzLzJCRUAGzsfaiOBY,289
 promptflow/azure/_utils/__init__.py,sha256=8h08DkAnJHuwcGENoGcuADtRBaCzIFEVEXErUuXDG10,319
 promptflow/azure/_utils/_tracing.py,sha256=u4R-0iw2BapfZNSwZbXgaVVm_czufv_xLwgtmzv2rWc,3080
 promptflow/azure/_utils/_url_utils.py,sha256=9nw4C2SmiOZTBpScSwJtzGdjNGSvsLNKTbTGuT4bYlM,2206
 promptflow/azure/_utils/general.py,sha256=MrpQpVpbQyJJiU1rX74T6TpYOqFdmHWj4A404nVyxnw,1231
+promptflow/azure/_version.py,sha256=Ir3b-xvk_y0X1AXxzoFh2hFNiD56d4pylsStFeoc5RU,297
 promptflow/azure/operations/__init__.py,sha256=mNPyBqFBhj5gDmRFfQ5eIyKEmuYZlfIR7g7risFbVf4,399
-promptflow/azure/operations/_arm_connection_operations.py,sha256=o8CaUOlL_bb0IN7iXWu-rDVgjWf8n_xHEmDsdAeqFyg,2459
-promptflow/azure/operations/_artifact_utilities.py,sha256=4cGHl6SwNdCARLUetwmn8qkH_t1k6uJ26WKXTuNFNf8,17342
+promptflow/azure/operations/_arm_connection_operations.py,sha256=_CVd9swrdDFhnhA9egQiJMV6PZyRbbf08xvpbo41p3o,3702
+promptflow/azure/operations/_artifact_utilities.py,sha256=aKIMKClrn2jMD8KfSgAL_OHVSNrn7M-_gWNHOQtKlRQ,17351
 promptflow/azure/operations/_async_run_downloader.py,sha256=7bSiYaLjdUTS5qQ6E7tFkB2Ru_dI24fAPsohVxoQLSc,14378
 promptflow/azure/operations/_connection_operations.py,sha256=77EZMFnlL5gxjXS5FHCDChC1qZmgHiGMK3NKJ0XNLEU,3837
 promptflow/azure/operations/_fileshare_storeage_helper.py,sha256=8S7QzW8vvf-Mhid5teF9mGD99GKBOabSeAgoaWx-MZw,9139
-promptflow/azure/operations/_flow_operations.py,sha256=UXsKYOmzH06dCdxycgxv2euumEtx-4KB4TEyHrzYrgc,28112
-promptflow/azure/operations/_run_operations.py,sha256=SfocM0OXrk6YUpFF-qrZxEZNk-URCiqlpT3Wzpy_ke8,47347
+promptflow/azure/operations/_flow_operations.py,sha256=WvGeQizQyu5eiSxjTwARWDCWsXlR-CyGDyZcqDLyMXs,28114
+promptflow/azure/operations/_run_operations.py,sha256=9ZSJs0lPOfhZXxg-CbKzoQdccNE2fwX8fKvaZL_2nos,47326
 promptflow/azure/operations/_trace_operations.py,sha256=l9xVmgTVWatQxGUsQdZStCvOJRF-UiHXumOVw-EMrbc,1710
 promptflow/azure/resources/component_spec_template.yaml,sha256=ii_xnSU52Gi3RofkGNElxWA-UZgBC1dhqg3cjVI5RBw,283
-promptflow_azure-0.1.0b1.dist-info/METADATA,sha256=gUDPH3MvSSuZOvbyvEfgFn8VM4shySK1PdaCCBNWUxU,1440
-promptflow_azure-0.1.0b1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-promptflow_azure-0.1.0b1.dist-info/entry_points.txt,sha256=EtwYpjxuk_qoQ89XrW1zc92TICNpi_GFpOkYYFP7-_Q,60
-promptflow_azure-0.1.0b1.dist-info/RECORD,,
+promptflow_azure-1.8.0.dist-info/METADATA,sha256=_wHXu7X-uZErTdLtaByVZAGXG9oIWdOc97omPi5TYkg,3051
+promptflow_azure-1.8.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+promptflow_azure-1.8.0.dist-info/entry_points.txt,sha256=EtwYpjxuk_qoQ89XrW1zc92TICNpi_GFpOkYYFP7-_Q,60
+promptflow_azure-1.8.0.dist-info/RECORD,,
```

