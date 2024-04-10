# Comparing `tmp/mypy-boto3-cleanrooms-1.34.78.tar.gz` & `tmp/mypy-boto3-cleanrooms-1.34.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanrooms-1.34.78.tar", last modified: Thu Apr  4 19:33:16 2024, max compression
+gzip compressed data, was "mypy-boto3-cleanrooms-1.34.82.tar", last modified: Wed Apr 10 19:19:34 2024, max compression
```

## Comparing `mypy-boto3-cleanrooms-1.34.78.tar` & `mypy-boto3-cleanrooms-1.34.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.504019 mypy-boto3-cleanrooms-1.34.78/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-04 19:33:16.504019 mypy-boto3-cleanrooms-1.34.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.500019 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53441 2024-04-04 19:32:18.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53438 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-04 19:32:18.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-04 19:32:18.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-04-04 19:32:18.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-04-04 19:32:18.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    70150 2024-04-04 19:32:19.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70150 2024-04-04 19:32:19.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.504019 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-04 19:33:16.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-04 19:33:16.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:16.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:16.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:16.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 19:33:16.000000 mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:16.504019 mypy-boto3-cleanrooms-1.34.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-04 19:32:17.000000 mypy-boto3-cleanrooms-1.34.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:34.977250 mypy-boto3-cleanrooms-1.34.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-10 19:19:34.977250 mypy-boto3-cleanrooms-1.34.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:34.977250 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53441 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53438 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    70944 2024-04-10 19:19:05.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70944 2024-04-10 19:19:05.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:34.977250 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-10 19:19:34.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-10 19:19:34.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:34.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:34.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:34.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 19:19:34.000000 mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:34.977250 mypy-boto3-cleanrooms-1.34.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-10 19:19:04.000000 mypy-boto3-cleanrooms-1.34.82/setup.py
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/LICENSE` & `mypy-boto3-cleanrooms-1.34.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/PKG-INFO` & `mypy-boto3-cleanrooms-1.34.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.34.78
-Summary: Type annotations for boto3.CleanRoomsService 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.CleanRoomsService 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/README.md` & `mypy-boto3-cleanrooms-1.34.82/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/__init__.py` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/__init__.pyi` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/__main__.py` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CleanRoomsService 1.34.78\n"
-        "Version:         1.34.78\n"
+        "Type annotations for boto3.CleanRoomsService 1.34.82\n"
+        "Version:         1.34.82\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.78")
+    print("1.34.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/client.py` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/client.pyi` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/literals.py` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 __all__ = (
     "AggregateFunctionNameType",
     "AggregationTypeType",
     "AnalysisFormatType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
+    "AnalysisTemplateValidationStatusType",
+    "AnalysisTemplateValidationTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
     "DifferentialPrivacyAggregationTypeType",
     "FilterableMemberStatusType",
     "JoinOperatorType",
     "JoinRequiredOptionType",
     "ListAnalysisTemplatesPaginatorName",
@@ -70,14 +72,16 @@
 )
 
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
 AnalysisFormatType = Literal["SQL"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
 AnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
+AnalysisTemplateValidationStatusType = Literal["INVALID", "UNABLE_TO_VALIDATE", "VALID"]
+AnalysisTemplateValidationTypeType = Literal["DIFFERENTIAL_PRIVACY"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
 DifferentialPrivacyAggregationTypeType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "STDDEV", "SUM"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
 JoinOperatorType = Literal["AND", "OR"]
 JoinRequiredOptionType = Literal["QUERY_RUNNER"]
 ListAnalysisTemplatesPaginatorName = Literal["list_analysis_templates"]
@@ -254,14 +258,15 @@
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
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/literals.pyi` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 __all__ = (
     "AggregateFunctionNameType",
     "AggregationTypeType",
     "AnalysisFormatType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
+    "AnalysisTemplateValidationStatusType",
+    "AnalysisTemplateValidationTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
     "DifferentialPrivacyAggregationTypeType",
     "FilterableMemberStatusType",
     "JoinOperatorType",
     "JoinRequiredOptionType",
     "ListAnalysisTemplatesPaginatorName",
@@ -70,14 +72,16 @@
 )
 
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
 AnalysisFormatType = Literal["SQL"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
 AnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
+AnalysisTemplateValidationStatusType = Literal["INVALID", "UNABLE_TO_VALIDATE", "VALID"]
+AnalysisTemplateValidationTypeType = Literal["DIFFERENTIAL_PRIVACY"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
 DifferentialPrivacyAggregationTypeType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "STDDEV", "SUM"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
 JoinOperatorType = Literal["AND", "OR"]
 JoinRequiredOptionType = Literal["QUERY_RUNNER"]
 ListAnalysisTemplatesPaginatorName = Literal["list_analysis_templates"]
@@ -254,14 +258,15 @@
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
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/paginator.py` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/paginator.pyi` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/type_defs.py` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
+    AnalysisTemplateValidationStatusType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     DifferentialPrivacyAggregationTypeType,
     FilterableMemberStatusType,
     JoinOperatorType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
@@ -54,14 +55,15 @@
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
     "AnalysisParameterTypeDef",
     "AnalysisRuleListTypeDef",
     "AnalysisSchemaTypeDef",
     "AnalysisSourceTypeDef",
     "AnalysisTemplateSummaryTypeDef",
+    "AnalysisTemplateValidationStatusReasonTypeDef",
     "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
     "BatchGetCollaborationAnalysisTemplateInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetSchemaAnalysisRuleErrorTypeDef",
     "SchemaAnalysisRuleRequestTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
@@ -145,17 +147,16 @@
     "UpdateAnalysisTemplateInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredAudienceModelAssociationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
-    "AnalysisTemplateTypeDef",
-    "CollaborationAnalysisTemplateTypeDef",
     "CreateAnalysisTemplateInputRequestTypeDef",
+    "AnalysisTemplateValidationStatusDetailTypeDef",
     "ListAnalysisTemplatesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "BatchGetSchemaAnalysisRuleInputRequestTypeDef",
     "ListCollaborationAnalysisTemplatesOutputTypeDef",
     "ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef",
     "GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef",
     "ListCollaborationPrivacyBudgetTemplatesOutputTypeDef",
@@ -199,19 +200,16 @@
     "ListSchemasOutputTypeDef",
     "MembershipPaymentConfigurationTypeDef",
     "MembershipProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "PaymentConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "SchemaStatusDetailTypeDef",
-    "CreateAnalysisTemplateOutputTypeDef",
-    "GetAnalysisTemplateOutputTypeDef",
-    "UpdateAnalysisTemplateOutputTypeDef",
-    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
-    "GetCollaborationAnalysisTemplateOutputTypeDef",
+    "AnalysisTemplateTypeDef",
+    "CollaborationAnalysisTemplateTypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "AnalysisRuleCustomTypeDef",
     "PrivacyImpactTypeDef",
     "PreviewPrivacyImpactInputRequestTypeDef",
     "PrivacyBudgetTypeDef",
@@ -224,14 +222,19 @@
     "MembershipSummaryTypeDef",
     "MembershipProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "MemberSpecificationTypeDef",
     "MemberSummaryTypeDef",
     "ProtectedQueryResultTypeDef",
     "SchemaTypeDef",
+    "CreateAnalysisTemplateOutputTypeDef",
+    "GetAnalysisTemplateOutputTypeDef",
+    "UpdateAnalysisTemplateOutputTypeDef",
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "PreviewPrivacyImpactOutputTypeDef",
     "CollaborationPrivacyBudgetSummaryTypeDef",
     "PrivacyBudgetSummaryTypeDef",
     "GetCollaborationPrivacyBudgetTemplateOutputTypeDef",
     "CreatePrivacyBudgetTemplateOutputTypeDef",
@@ -325,14 +328,20 @@
         "membershipArn": str,
         "membershipId": str,
         "collaborationArn": str,
         "collaborationId": str,
         "description": NotRequired[str],
     },
 )
+AnalysisTemplateValidationStatusReasonTypeDef = TypedDict(
+    "AnalysisTemplateValidationStatusReasonTypeDef",
+    {
+        "message": str,
+    },
+)
 BatchGetCollaborationAnalysisTemplateErrorTypeDef = TypedDict(
     "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
@@ -1097,63 +1106,34 @@
         "dimensionColumns": List[str],
         "scalarFunctions": List[ScalarFunctionsType],
         "outputConstraints": List[AggregationConstraintTypeDef],
         "joinRequired": NotRequired[Literal["QUERY_RUNNER"]],
         "allowedJoinOperators": NotRequired[List[JoinOperatorType]],
     },
 )
-AnalysisTemplateTypeDef = TypedDict(
-    "AnalysisTemplateTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "collaborationId": str,
-        "collaborationArn": str,
-        "membershipId": str,
-        "membershipArn": str,
-        "name": str,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "schema": AnalysisSchemaTypeDef,
-        "format": Literal["SQL"],
-        "source": AnalysisSourceTypeDef,
-        "description": NotRequired[str],
-        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
-    },
-)
-CollaborationAnalysisTemplateTypeDef = TypedDict(
-    "CollaborationAnalysisTemplateTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "collaborationId": str,
-        "collaborationArn": str,
-        "creatorAccountId": str,
-        "name": str,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "schema": AnalysisSchemaTypeDef,
-        "format": Literal["SQL"],
-        "source": AnalysisSourceTypeDef,
-        "description": NotRequired[str],
-        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
-    },
-)
 CreateAnalysisTemplateInputRequestTypeDef = TypedDict(
     "CreateAnalysisTemplateInputRequestTypeDef",
     {
         "membershipIdentifier": str,
         "name": str,
         "format": Literal["SQL"],
         "source": AnalysisSourceTypeDef,
         "description": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
         "analysisParameters": NotRequired[Sequence[AnalysisParameterTypeDef]],
     },
 )
+AnalysisTemplateValidationStatusDetailTypeDef = TypedDict(
+    "AnalysisTemplateValidationStatusDetailTypeDef",
+    {
+        "type": Literal["DIFFERENTIAL_PRIVACY"],
+        "status": AnalysisTemplateValidationStatusType,
+        "reasons": NotRequired[List[AnalysisTemplateValidationStatusReasonTypeDef]],
+    },
+)
 ListAnalysisTemplatesOutputTypeDef = TypedDict(
     "ListAnalysisTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "analysisTemplateSummaries": List[AnalysisTemplateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1526,48 +1506,51 @@
     {
         "status": SchemaStatusType,
         "reasons": NotRequired[List[SchemaStatusReasonTypeDef]],
         "analysisRuleType": NotRequired[AnalysisRuleTypeType],
         "configurations": NotRequired[List[Literal["DIFFERENTIAL_PRIVACY"]]],
     },
 )
-CreateAnalysisTemplateOutputTypeDef = TypedDict(
-    "CreateAnalysisTemplateOutputTypeDef",
-    {
-        "analysisTemplate": AnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetAnalysisTemplateOutputTypeDef = TypedDict(
-    "GetAnalysisTemplateOutputTypeDef",
-    {
-        "analysisTemplate": AnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateAnalysisTemplateOutputTypeDef = TypedDict(
-    "UpdateAnalysisTemplateOutputTypeDef",
-    {
-        "analysisTemplate": AnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-BatchGetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
-    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+AnalysisTemplateTypeDef = TypedDict(
+    "AnalysisTemplateTypeDef",
     {
-        "collaborationAnalysisTemplates": List[CollaborationAnalysisTemplateTypeDef],
-        "errors": List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "membershipId": str,
+        "membershipArn": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+        "description": NotRequired[str],
+        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
+        "validations": NotRequired[List[AnalysisTemplateValidationStatusDetailTypeDef]],
     },
 )
-GetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
-    "GetCollaborationAnalysisTemplateOutputTypeDef",
+CollaborationAnalysisTemplateTypeDef = TypedDict(
+    "CollaborationAnalysisTemplateTypeDef",
     {
-        "collaborationAnalysisTemplate": CollaborationAnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "creatorAccountId": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+        "description": NotRequired[str],
+        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
+        "validations": NotRequired[List[AnalysisTemplateValidationStatusDetailTypeDef]],
     },
 )
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1763,14 +1746,50 @@
         "createTime": datetime,
         "updateTime": datetime,
         "type": Literal["TABLE"],
         "schemaStatusDetails": List[SchemaStatusDetailTypeDef],
         "analysisMethod": NotRequired[Literal["DIRECT_QUERY"]],
     },
 )
+CreateAnalysisTemplateOutputTypeDef = TypedDict(
+    "CreateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateAnalysisTemplateOutputTypeDef = TypedDict(
+    "UpdateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+BatchGetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplates": List[CollaborationAnalysisTemplateTypeDef],
+        "errors": List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplate": CollaborationAnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
         "list": NotRequired[AnalysisRuleListTypeDef],
         "aggregation": NotRequired[AnalysisRuleAggregationTypeDef],
         "custom": NotRequired[AnalysisRuleCustomTypeDef],
     },
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms/type_defs.pyi` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
+    AnalysisTemplateValidationStatusType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     DifferentialPrivacyAggregationTypeType,
     FilterableMemberStatusType,
     JoinOperatorType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
@@ -54,14 +55,15 @@
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
     "AnalysisParameterTypeDef",
     "AnalysisRuleListTypeDef",
     "AnalysisSchemaTypeDef",
     "AnalysisSourceTypeDef",
     "AnalysisTemplateSummaryTypeDef",
+    "AnalysisTemplateValidationStatusReasonTypeDef",
     "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
     "BatchGetCollaborationAnalysisTemplateInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetSchemaAnalysisRuleErrorTypeDef",
     "SchemaAnalysisRuleRequestTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
@@ -145,17 +147,16 @@
     "UpdateAnalysisTemplateInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredAudienceModelAssociationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
-    "AnalysisTemplateTypeDef",
-    "CollaborationAnalysisTemplateTypeDef",
     "CreateAnalysisTemplateInputRequestTypeDef",
+    "AnalysisTemplateValidationStatusDetailTypeDef",
     "ListAnalysisTemplatesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "BatchGetSchemaAnalysisRuleInputRequestTypeDef",
     "ListCollaborationAnalysisTemplatesOutputTypeDef",
     "ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef",
     "GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef",
     "ListCollaborationPrivacyBudgetTemplatesOutputTypeDef",
@@ -199,19 +200,16 @@
     "ListSchemasOutputTypeDef",
     "MembershipPaymentConfigurationTypeDef",
     "MembershipProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "PaymentConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "SchemaStatusDetailTypeDef",
-    "CreateAnalysisTemplateOutputTypeDef",
-    "GetAnalysisTemplateOutputTypeDef",
-    "UpdateAnalysisTemplateOutputTypeDef",
-    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
-    "GetCollaborationAnalysisTemplateOutputTypeDef",
+    "AnalysisTemplateTypeDef",
+    "CollaborationAnalysisTemplateTypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "AnalysisRuleCustomTypeDef",
     "PrivacyImpactTypeDef",
     "PreviewPrivacyImpactInputRequestTypeDef",
     "PrivacyBudgetTypeDef",
@@ -224,14 +222,19 @@
     "MembershipSummaryTypeDef",
     "MembershipProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "MemberSpecificationTypeDef",
     "MemberSummaryTypeDef",
     "ProtectedQueryResultTypeDef",
     "SchemaTypeDef",
+    "CreateAnalysisTemplateOutputTypeDef",
+    "GetAnalysisTemplateOutputTypeDef",
+    "UpdateAnalysisTemplateOutputTypeDef",
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "PreviewPrivacyImpactOutputTypeDef",
     "CollaborationPrivacyBudgetSummaryTypeDef",
     "PrivacyBudgetSummaryTypeDef",
     "GetCollaborationPrivacyBudgetTemplateOutputTypeDef",
     "CreatePrivacyBudgetTemplateOutputTypeDef",
@@ -325,14 +328,20 @@
         "membershipArn": str,
         "membershipId": str,
         "collaborationArn": str,
         "collaborationId": str,
         "description": NotRequired[str],
     },
 )
+AnalysisTemplateValidationStatusReasonTypeDef = TypedDict(
+    "AnalysisTemplateValidationStatusReasonTypeDef",
+    {
+        "message": str,
+    },
+)
 BatchGetCollaborationAnalysisTemplateErrorTypeDef = TypedDict(
     "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
@@ -1097,63 +1106,34 @@
         "dimensionColumns": List[str],
         "scalarFunctions": List[ScalarFunctionsType],
         "outputConstraints": List[AggregationConstraintTypeDef],
         "joinRequired": NotRequired[Literal["QUERY_RUNNER"]],
         "allowedJoinOperators": NotRequired[List[JoinOperatorType]],
     },
 )
-AnalysisTemplateTypeDef = TypedDict(
-    "AnalysisTemplateTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "collaborationId": str,
-        "collaborationArn": str,
-        "membershipId": str,
-        "membershipArn": str,
-        "name": str,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "schema": AnalysisSchemaTypeDef,
-        "format": Literal["SQL"],
-        "source": AnalysisSourceTypeDef,
-        "description": NotRequired[str],
-        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
-    },
-)
-CollaborationAnalysisTemplateTypeDef = TypedDict(
-    "CollaborationAnalysisTemplateTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "collaborationId": str,
-        "collaborationArn": str,
-        "creatorAccountId": str,
-        "name": str,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "schema": AnalysisSchemaTypeDef,
-        "format": Literal["SQL"],
-        "source": AnalysisSourceTypeDef,
-        "description": NotRequired[str],
-        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
-    },
-)
 CreateAnalysisTemplateInputRequestTypeDef = TypedDict(
     "CreateAnalysisTemplateInputRequestTypeDef",
     {
         "membershipIdentifier": str,
         "name": str,
         "format": Literal["SQL"],
         "source": AnalysisSourceTypeDef,
         "description": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
         "analysisParameters": NotRequired[Sequence[AnalysisParameterTypeDef]],
     },
 )
+AnalysisTemplateValidationStatusDetailTypeDef = TypedDict(
+    "AnalysisTemplateValidationStatusDetailTypeDef",
+    {
+        "type": Literal["DIFFERENTIAL_PRIVACY"],
+        "status": AnalysisTemplateValidationStatusType,
+        "reasons": NotRequired[List[AnalysisTemplateValidationStatusReasonTypeDef]],
+    },
+)
 ListAnalysisTemplatesOutputTypeDef = TypedDict(
     "ListAnalysisTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "analysisTemplateSummaries": List[AnalysisTemplateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1526,48 +1506,51 @@
     {
         "status": SchemaStatusType,
         "reasons": NotRequired[List[SchemaStatusReasonTypeDef]],
         "analysisRuleType": NotRequired[AnalysisRuleTypeType],
         "configurations": NotRequired[List[Literal["DIFFERENTIAL_PRIVACY"]]],
     },
 )
-CreateAnalysisTemplateOutputTypeDef = TypedDict(
-    "CreateAnalysisTemplateOutputTypeDef",
-    {
-        "analysisTemplate": AnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetAnalysisTemplateOutputTypeDef = TypedDict(
-    "GetAnalysisTemplateOutputTypeDef",
-    {
-        "analysisTemplate": AnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateAnalysisTemplateOutputTypeDef = TypedDict(
-    "UpdateAnalysisTemplateOutputTypeDef",
-    {
-        "analysisTemplate": AnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-BatchGetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
-    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+AnalysisTemplateTypeDef = TypedDict(
+    "AnalysisTemplateTypeDef",
     {
-        "collaborationAnalysisTemplates": List[CollaborationAnalysisTemplateTypeDef],
-        "errors": List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "membershipId": str,
+        "membershipArn": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+        "description": NotRequired[str],
+        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
+        "validations": NotRequired[List[AnalysisTemplateValidationStatusDetailTypeDef]],
     },
 )
-GetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
-    "GetCollaborationAnalysisTemplateOutputTypeDef",
+CollaborationAnalysisTemplateTypeDef = TypedDict(
+    "CollaborationAnalysisTemplateTypeDef",
     {
-        "collaborationAnalysisTemplate": CollaborationAnalysisTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "creatorAccountId": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+        "description": NotRequired[str],
+        "analysisParameters": NotRequired[List[AnalysisParameterTypeDef]],
+        "validations": NotRequired[List[AnalysisTemplateValidationStatusDetailTypeDef]],
     },
 )
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1763,14 +1746,50 @@
         "createTime": datetime,
         "updateTime": datetime,
         "type": Literal["TABLE"],
         "schemaStatusDetails": List[SchemaStatusDetailTypeDef],
         "analysisMethod": NotRequired[Literal["DIRECT_QUERY"]],
     },
 )
+CreateAnalysisTemplateOutputTypeDef = TypedDict(
+    "CreateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateAnalysisTemplateOutputTypeDef = TypedDict(
+    "UpdateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+BatchGetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplates": List[CollaborationAnalysisTemplateTypeDef],
+        "errors": List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplate": CollaborationAnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
         "list": NotRequired[AnalysisRuleListTypeDef],
         "aggregation": NotRequired[AnalysisRuleAggregationTypeDef],
         "custom": NotRequired[AnalysisRuleCustomTypeDef],
     },
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/PKG-INFO` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.34.78
-Summary: Type annotations for boto3.CleanRoomsService 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.CleanRoomsService 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cleanrooms-1.34.78/mypy_boto3_cleanrooms.egg-info/SOURCES.txt` & `mypy-boto3-cleanrooms-1.34.82/mypy_boto3_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.34.78/setup.py` & `mypy-boto3-cleanrooms-1.34.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cleanrooms",
-    version="1.34.78",
+    version="1.34.82",
     packages=["mypy_boto3_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CleanRoomsService 1.34.78 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CleanRoomsService 1.34.82 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

