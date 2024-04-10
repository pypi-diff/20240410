# Comparing `tmp/mypy-boto3-supplychain-1.34.18.tar.gz` & `tmp/mypy-boto3-supplychain-1.34.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-supplychain-1.34.18.tar", last modified: Fri Jan 12 21:05:17 2024, max compression
+gzip compressed data, was "mypy-boto3-supplychain-1.34.82.tar", last modified: Wed Apr 10 19:19:36 2024, max compression
```

## Comparing `mypy-boto3-supplychain-1.34.18.tar` & `mypy-boto3-supplychain-1.34.82.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:05:17.771044 mypy-boto3-supplychain-1.34.18/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-01-12 21:05:17.771044 mypy-boto3-supplychain-1.34.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:05:17.771044 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:05:17.771044 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-01-12 21:05:17.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-12 21:05:17.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 21:05:17.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 21:05:17.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-12 21:05:17.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-12 21:05:17.000000 mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 21:05:17.771044 mypy-boto3-supplychain-1.34.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-12 21:05:02.000000 mypy-boto3-supplychain-1.34.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.741251 mypy-boto3-supplychain-1.34.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-04-10 19:19:36.741251 mypy-boto3-supplychain-1.34.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.737251 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.741251 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-04-10 19:19:36.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-10 19:19:36.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:36.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:36.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:36.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 19:19:36.000000 mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:36.741251 mypy-boto3-supplychain-1.34.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-10 19:19:22.000000 mypy-boto3-supplychain-1.34.82/setup.py
```

### Comparing `mypy-boto3-supplychain-1.34.18/LICENSE` & `mypy-boto3-supplychain-1.34.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-supplychain-1.34.18/PKG-INFO` & `mypy-boto3-supplychain-1.34.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-supplychain
-Version: 1.34.18
-Summary: Type annotations for boto3.SupplyChain 1.34.18 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.82
+Summary: Type annotations for boto3.SupplyChain 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-supplychain.svg?color=blue)](https://pypi.org/project/mypy-boto3-supplychain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-supplychain)](https://pepy.tech/project/mypy-boto3-supplychain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SupplyChain 1.34.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
+[boto3.SupplyChain 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-supplychain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-supplychain-1.34.18/README.md` & `mypy-boto3-supplychain-1.34.82/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-supplychain.svg?color=blue)](https://pypi.org/project/mypy-boto3-supplychain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-supplychain)](https://pepy.tech/project/mypy-boto3-supplychain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SupplyChain 1.34.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
+[boto3.SupplyChain 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-supplychain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/__main__.py` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SupplyChain 1.34.18\nVersion:         1.34.18\nBuilder version:"
-        " 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.SupplyChain 1.34.82\n"
+        "Version:         1.34.82\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.18")
+    print("1.34.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/client.py` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,20 @@
     ```
 """
 
 from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import DataIntegrationEventTypeType
 from .type_defs import (
     CreateBillOfMaterialsImportJobResponseTypeDef,
     GetBillOfMaterialsImportJobResponseTypeDef,
+    SendDataIntegrationEventResponseTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("SupplyChainClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
@@ -109,7 +112,24 @@
     ) -> GetBillOfMaterialsImportJobResponseTypeDef:
         """
         Get status and details of a BillOfMaterialsImportJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.get_bill_of_materials_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/client/#get_bill_of_materials_import_job)
         """
+
+    def send_data_integration_event(
+        self,
+        *,
+        instanceId: str,
+        eventType: DataIntegrationEventTypeType,
+        data: str,
+        eventGroupId: str,
+        eventTimestamp: TimestampTypeDef = ...,
+        clientToken: str = ...,
+    ) -> SendDataIntegrationEventResponseTypeDef:
+        """
+        Send transactional data events with real-time data for analysis or monitoring.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.send_data_integration_event)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/client/#send_data_integration_event)
+        """
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/client.pyi` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,20 @@
     ```
 """
 
 from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import DataIntegrationEventTypeType
 from .type_defs import (
     CreateBillOfMaterialsImportJobResponseTypeDef,
     GetBillOfMaterialsImportJobResponseTypeDef,
+    SendDataIntegrationEventResponseTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("SupplyChainClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
@@ -106,7 +109,24 @@
     ) -> GetBillOfMaterialsImportJobResponseTypeDef:
         """
         Get status and details of a BillOfMaterialsImportJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.get_bill_of_materials_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/client/#get_bill_of_materials_import_job)
         """
+
+    def send_data_integration_event(
+        self,
+        *,
+        instanceId: str,
+        eventType: DataIntegrationEventTypeType,
+        data: str,
+        eventGroupId: str,
+        eventTimestamp: TimestampTypeDef = ...,
+        clientToken: str = ...,
+    ) -> SendDataIntegrationEventResponseTypeDef:
+        """
+        Send transactional data events with real-time data for analysis or monitoring.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.send_data_integration_event)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/client/#send_data_integration_event)
+        """
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/literals.py` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/literals.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,20 +17,38 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ConfigurationJobStatusType",
+    "DataIntegrationEventTypeType",
     "SupplyChainServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
 ConfigurationJobStatusType = Literal["FAILED", "IN_PROGRESS", "NEW", "QUEUED", "SUCCESS"]
+DataIntegrationEventTypeType = Literal[
+    "scn.data.forecast",
+    "scn.data.inboundorder",
+    "scn.data.inboundorderline",
+    "scn.data.inboundorderlineschedule",
+    "scn.data.inventorylevel",
+    "scn.data.outboundorderline",
+    "scn.data.outboundshipment",
+    "scn.data.processheader",
+    "scn.data.processoperation",
+    "scn.data.processproduct",
+    "scn.data.reservation",
+    "scn.data.shipment",
+    "scn.data.shipmentstop",
+    "scn.data.shipmentstoporder",
+    "scn.data.supplyplan",
+]
 SupplyChainServiceName = Literal["supplychain"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -50,14 +68,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -68,14 +87,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -93,14 +113,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -113,24 +134,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -191,15 +214,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -379,14 +401,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/literals.pyi` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/literals.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -17,20 +17,38 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ConfigurationJobStatusType",
+    "DataIntegrationEventTypeType",
     "SupplyChainServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
 ConfigurationJobStatusType = Literal["FAILED", "IN_PROGRESS", "NEW", "QUEUED", "SUCCESS"]
+DataIntegrationEventTypeType = Literal[
+    "scn.data.forecast",
+    "scn.data.inboundorder",
+    "scn.data.inboundorderline",
+    "scn.data.inboundorderlineschedule",
+    "scn.data.inventorylevel",
+    "scn.data.outboundorderline",
+    "scn.data.outboundshipment",
+    "scn.data.processheader",
+    "scn.data.processoperation",
+    "scn.data.processproduct",
+    "scn.data.reservation",
+    "scn.data.shipment",
+    "scn.data.shipmentstop",
+    "scn.data.shipmentstoporder",
+    "scn.data.supplyplan",
+]
 SupplyChainServiceName = Literal["supplychain"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -50,14 +68,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -68,14 +87,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -93,14 +113,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -113,24 +134,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -191,15 +214,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -379,14 +401,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/type_defs.py` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     from mypy_boto3_supplychain.type_defs import BillOfMaterialsImportJobTypeDef
 
     data: BillOfMaterialsImportJobTypeDef = ...
     ```
 """
 
 import sys
-from typing import Dict
+from datetime import datetime
+from typing import Dict, Union
 
-from .literals import ConfigurationJobStatusType
+from .literals import ConfigurationJobStatusType, DataIntegrationEventTypeType
 
 if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
@@ -27,16 +28,19 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "BillOfMaterialsImportJobTypeDef",
     "CreateBillOfMaterialsImportJobRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetBillOfMaterialsImportJobRequestRequestTypeDef",
+    "TimestampTypeDef",
     "CreateBillOfMaterialsImportJobResponseTypeDef",
     "GetBillOfMaterialsImportJobResponseTypeDef",
+    "SendDataIntegrationEventResponseTypeDef",
+    "SendDataIntegrationEventRequestRequestTypeDef",
 )
 
 BillOfMaterialsImportJobTypeDef = TypedDict(
     "BillOfMaterialsImportJobTypeDef",
     {
         "instanceId": str,
         "jobId": str,
@@ -53,34 +57,53 @@
         "clientToken": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 GetBillOfMaterialsImportJobRequestRequestTypeDef = TypedDict(
     "GetBillOfMaterialsImportJobRequestRequestTypeDef",
     {
         "instanceId": str,
         "jobId": str,
     },
 )
+TimestampTypeDef = Union[datetime, str]
 CreateBillOfMaterialsImportJobResponseTypeDef = TypedDict(
     "CreateBillOfMaterialsImportJobResponseTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetBillOfMaterialsImportJobResponseTypeDef = TypedDict(
     "GetBillOfMaterialsImportJobResponseTypeDef",
     {
         "job": BillOfMaterialsImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SendDataIntegrationEventResponseTypeDef = TypedDict(
+    "SendDataIntegrationEventResponseTypeDef",
+    {
+        "eventId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+SendDataIntegrationEventRequestRequestTypeDef = TypedDict(
+    "SendDataIntegrationEventRequestRequestTypeDef",
+    {
+        "instanceId": str,
+        "eventType": DataIntegrationEventTypeType,
+        "data": str,
+        "eventGroupId": str,
+        "eventTimestamp": NotRequired[TimestampTypeDef],
+        "clientToken": NotRequired[str],
+    },
+)
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain/type_defs.pyi` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     from mypy_boto3_supplychain.type_defs import BillOfMaterialsImportJobTypeDef
 
     data: BillOfMaterialsImportJobTypeDef = ...
     ```
 """
 
 import sys
-from typing import Dict
+from datetime import datetime
+from typing import Dict, Union
 
-from .literals import ConfigurationJobStatusType
+from .literals import ConfigurationJobStatusType, DataIntegrationEventTypeType
 
 if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
@@ -27,16 +28,19 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "BillOfMaterialsImportJobTypeDef",
     "CreateBillOfMaterialsImportJobRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetBillOfMaterialsImportJobRequestRequestTypeDef",
+    "TimestampTypeDef",
     "CreateBillOfMaterialsImportJobResponseTypeDef",
     "GetBillOfMaterialsImportJobResponseTypeDef",
+    "SendDataIntegrationEventResponseTypeDef",
+    "SendDataIntegrationEventRequestRequestTypeDef",
 )
 
 BillOfMaterialsImportJobTypeDef = TypedDict(
     "BillOfMaterialsImportJobTypeDef",
     {
         "instanceId": str,
         "jobId": str,
@@ -53,34 +57,53 @@
         "clientToken": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 GetBillOfMaterialsImportJobRequestRequestTypeDef = TypedDict(
     "GetBillOfMaterialsImportJobRequestRequestTypeDef",
     {
         "instanceId": str,
         "jobId": str,
     },
 )
+TimestampTypeDef = Union[datetime, str]
 CreateBillOfMaterialsImportJobResponseTypeDef = TypedDict(
     "CreateBillOfMaterialsImportJobResponseTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetBillOfMaterialsImportJobResponseTypeDef = TypedDict(
     "GetBillOfMaterialsImportJobResponseTypeDef",
     {
         "job": BillOfMaterialsImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SendDataIntegrationEventResponseTypeDef = TypedDict(
+    "SendDataIntegrationEventResponseTypeDef",
+    {
+        "eventId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+SendDataIntegrationEventRequestRequestTypeDef = TypedDict(
+    "SendDataIntegrationEventRequestRequestTypeDef",
+    {
+        "instanceId": str,
+        "eventType": DataIntegrationEventTypeType,
+        "data": str,
+        "eventGroupId": str,
+        "eventTimestamp": NotRequired[TimestampTypeDef],
+        "clientToken": NotRequired[str],
+    },
+)
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/PKG-INFO` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-supplychain
-Version: 1.34.18
-Summary: Type annotations for boto3.SupplyChain 1.34.18 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.82
+Summary: Type annotations for boto3.SupplyChain 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-supplychain.svg?color=blue)](https://pypi.org/project/mypy-boto3-supplychain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-supplychain)](https://pepy.tech/project/mypy-boto3-supplychain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SupplyChain 1.34.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
+[boto3.SupplyChain 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-supplychain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-supplychain-1.34.18/mypy_boto3_supplychain.egg-info/SOURCES.txt` & `mypy-boto3-supplychain-1.34.82/mypy_boto3_supplychain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-supplychain-1.34.18/setup.py` & `mypy-boto3-supplychain-1.34.82/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-supplychain",
-    version="1.34.18",
+    version="1.34.82",
     packages=["mypy_boto3_supplychain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.SupplyChain 1.34.18 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.SupplyChain 1.34.82 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

