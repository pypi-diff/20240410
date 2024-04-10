# Comparing `tmp/mypy-boto3-connect-1.34.67.tar.gz` & `tmp/mypy-boto3-connect-1.34.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.34.67.tar", last modified: Wed Mar 20 19:32:19 2024, max compression
+gzip compressed data, was "mypy-boto3-connect-1.34.82.tar", last modified: Wed Apr 10 19:19:35 2024, max compression
```

## Comparing `mypy-boto3-connect-1.34.67.tar` & `mypy-boto3-connect-1.34.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:32:19.949769 mypy-boto3-connect-1.34.67/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-03-20 19:32:19.949769 mypy-boto3-connect-1.34.67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:32:19.945769 mypy-boto3-connect-1.34.67/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   187084 2024-03-20 19:31:55.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   187081 2024-03-20 19:31:54.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30419 2024-03-20 19:31:56.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    30419 2024-03-20 19:31:56.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    65203 2024-03-20 19:31:56.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    65148 2024-03-20 19:31:55.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   221058 2024-03-20 19:32:01.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   221058 2024-03-20 19:31:59.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:32:19.945769 mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-03-20 19:32:19.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-20 19:32:19.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:32:19.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:32:19.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-20 19:32:19.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 19:32:19.000000 mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 19:32:19.949769 mypy-boto3-connect-1.34.67/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-20 19:31:53.000000 mypy-boto3-connect-1.34.67/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187084 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187081 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30510 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30510 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    65203 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65148 2024-04-10 19:19:10.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   221361 2024-04-10 19:19:14.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   221361 2024-04-10 19:19:13.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:08.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20551 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 19:19:35.000000 mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:35.321250 mypy-boto3-connect-1.34.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-10 19:19:07.000000 mypy-boto3-connect-1.34.82/setup.py
```

### Comparing `mypy-boto3-connect-1.34.67/LICENSE` & `mypy-boto3-connect-1.34.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/PKG-INFO` & `mypy-boto3-connect-1.34.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.34.67
-Summary: Type annotations for boto3.Connect 1.34.67 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.Connect 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect)](https://pepy.tech/project/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.34.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-connect-1.34.67/README.md` & `mypy-boto3-connect-1.34.82/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect)](https://pepy.tech/project/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.34.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/__init__.py` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/__init__.pyi` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/__main__.py` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.34.67\n"
-        "Version:         1.34.67\n"
+        "Type annotations for boto3.Connect 1.34.82\n"
+        "Version:         1.34.82\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.67")
+    print("1.34.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/client.py` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/client.pyi` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/literals.py` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 ActionTypeType = Literal[
     "ASSIGN_CONTACT_CATEGORY",
     "CREATE_CASE",
     "CREATE_TASK",
     "END_ASSOCIATED_TASKS",
     "GENERATE_EVENTBRIDGE_EVENT",
     "SEND_NOTIFICATION",
+    "SUBMIT_AUTO_EVALUATION",
     "UPDATE_CASE",
 ]
 AgentAvailabilityTimerType = Literal["TIME_SINCE_LAST_ACTIVITY", "TIME_SINCE_LAST_INBOUND"]
 AgentStatusStateType = Literal["DISABLED", "ENABLED"]
 AgentStatusTypeType = Literal["CUSTOM", "OFFLINE", "ROUTABLE"]
 ArtifactStatusType = Literal["APPROVED", "IN_PROGRESS", "REJECTED"]
 BehaviorTypeType = Literal["ROUTE_ANY_CHANNEL", "ROUTE_CURRENT_CHANNEL_ONLY"]
@@ -822,14 +823,15 @@
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
@@ -842,24 +844,26 @@
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
```

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/literals.pyi` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 ActionTypeType = Literal[
     "ASSIGN_CONTACT_CATEGORY",
     "CREATE_CASE",
     "CREATE_TASK",
     "END_ASSOCIATED_TASKS",
     "GENERATE_EVENTBRIDGE_EVENT",
     "SEND_NOTIFICATION",
+    "SUBMIT_AUTO_EVALUATION",
     "UPDATE_CASE",
 ]
 AgentAvailabilityTimerType = Literal["TIME_SINCE_LAST_ACTIVITY", "TIME_SINCE_LAST_INBOUND"]
 AgentStatusStateType = Literal["DISABLED", "ENABLED"]
 AgentStatusTypeType = Literal["CUSTOM", "OFFLINE", "ROUTABLE"]
 ArtifactStatusType = Literal["APPROVED", "IN_PROGRESS", "REJECTED"]
 BehaviorTypeType = Literal["ROUTE_ANY_CHANNEL", "ROUTE_CURRENT_CHANNEL_ONLY"]
@@ -822,14 +823,15 @@
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
@@ -842,24 +844,26 @@
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
```

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/paginator.py` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/paginator.pyi` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/type_defs.py` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,14 +384,15 @@
     "UrlReferenceTypeDef",
     "ReferenceTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReplicateInstanceRequestRequestTypeDef",
     "TagSearchConditionTypeDef",
     "ResumeContactRecordingRequestRequestTypeDef",
     "ResumeContactRequestRequestTypeDef",
+    "SubmitAutoEvaluationActionDefinitionTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SortTypeDef",
     "SearchPredefinedAttributesRequestRequestTypeDef",
     "TagSetTypeDef",
     "SecurityProfileSearchSummaryTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "VocabularySummaryTypeDef",
@@ -3084,14 +3085,20 @@
     "ResumeContactRequestRequestTypeDef",
     {
         "ContactId": str,
         "InstanceId": str,
         "ContactFlowId": NotRequired[str],
     },
 )
+SubmitAutoEvaluationActionDefinitionTypeDef = TypedDict(
+    "SubmitAutoEvaluationActionDefinitionTypeDef",
+    {
+        "EvaluationFormId": str,
+    },
+)
 SearchAvailablePhoneNumbersRequestRequestTypeDef = TypedDict(
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     {
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": NotRequired[str],
         "InstanceId": NotRequired[str],
@@ -6543,14 +6550,15 @@
         "TaskAction": NotRequired[TaskActionDefinitionTypeDef],
         "EventBridgeAction": NotRequired[EventBridgeActionDefinitionTypeDef],
         "AssignContactCategoryAction": NotRequired[Mapping[str, Any]],
         "SendNotificationAction": NotRequired[SendNotificationActionDefinitionTypeDef],
         "CreateCaseAction": NotRequired[CreateCaseActionDefinitionTypeDef],
         "UpdateCaseAction": NotRequired[UpdateCaseActionDefinitionTypeDef],
         "EndAssociatedTasksAction": NotRequired[Mapping[str, Any]],
+        "SubmitAutoEvaluationAction": NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],
     },
 )
 GetCurrentUserDataResponseTypeDef = TypedDict(
     "GetCurrentUserDataResponseTypeDef",
     {
         "NextToken": str,
         "UserDataList": List[UserDataTypeDef],
```

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect/type_defs.pyi` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -384,14 +384,15 @@
     "UrlReferenceTypeDef",
     "ReferenceTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReplicateInstanceRequestRequestTypeDef",
     "TagSearchConditionTypeDef",
     "ResumeContactRecordingRequestRequestTypeDef",
     "ResumeContactRequestRequestTypeDef",
+    "SubmitAutoEvaluationActionDefinitionTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SortTypeDef",
     "SearchPredefinedAttributesRequestRequestTypeDef",
     "TagSetTypeDef",
     "SecurityProfileSearchSummaryTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "VocabularySummaryTypeDef",
@@ -3084,14 +3085,20 @@
     "ResumeContactRequestRequestTypeDef",
     {
         "ContactId": str,
         "InstanceId": str,
         "ContactFlowId": NotRequired[str],
     },
 )
+SubmitAutoEvaluationActionDefinitionTypeDef = TypedDict(
+    "SubmitAutoEvaluationActionDefinitionTypeDef",
+    {
+        "EvaluationFormId": str,
+    },
+)
 SearchAvailablePhoneNumbersRequestRequestTypeDef = TypedDict(
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     {
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": NotRequired[str],
         "InstanceId": NotRequired[str],
@@ -6543,14 +6550,15 @@
         "TaskAction": NotRequired[TaskActionDefinitionTypeDef],
         "EventBridgeAction": NotRequired[EventBridgeActionDefinitionTypeDef],
         "AssignContactCategoryAction": NotRequired[Mapping[str, Any]],
         "SendNotificationAction": NotRequired[SendNotificationActionDefinitionTypeDef],
         "CreateCaseAction": NotRequired[CreateCaseActionDefinitionTypeDef],
         "UpdateCaseAction": NotRequired[UpdateCaseActionDefinitionTypeDef],
         "EndAssociatedTasksAction": NotRequired[Mapping[str, Any]],
+        "SubmitAutoEvaluationAction": NotRequired[SubmitAutoEvaluationActionDefinitionTypeDef],
     },
 )
 GetCurrentUserDataResponseTypeDef = TypedDict(
     "GetCurrentUserDataResponseTypeDef",
     {
         "NextToken": str,
         "UserDataList": List[UserDataTypeDef],
```

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.34.67
-Summary: Type annotations for boto3.Connect 1.34.67 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.Connect 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect)](https://pepy.tech/project/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.34.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-connect-1.34.67/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy-boto3-connect-1.34.82/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.34.67/setup.py` & `mypy-boto3-connect-1.34.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.34.67",
+    version="1.34.82",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Connect 1.34.67 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Connect 1.34.82 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

