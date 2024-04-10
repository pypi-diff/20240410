# Comparing `tmp/mypy-boto3-workspaces-thin-client-1.34.64.tar.gz` & `tmp/mypy-boto3-workspaces-thin-client-1.34.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-thin-client-1.34.64.tar", last modified: Fri Mar 15 19:34:24 2024, max compression
+gzip compressed data, was "mypy-boto3-workspaces-thin-client-1.34.82.tar", last modified: Wed Apr 10 19:19:37 2024, max compression
```

## Comparing `mypy-boto3-workspaces-thin-client-1.34.64.tar` & `mypy-boto3-workspaces-thin-client-1.34.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:34:24.789255 mypy-boto3-workspaces-thin-client-1.34.64/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-03-15 19:34:24.789255 mypy-boto3-workspaces-thin-client-1.34.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:34:24.789255 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-03-15 19:34:11.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14740 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-03-15 19:34:11.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-03-15 19:34:11.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-15 19:34:11.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-15 19:34:11.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-03-15 19:34:12.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-03-15 19:34:12.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:34:24.789255 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-03-15 19:34:24.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-15 19:34:24.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 19:34:24.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 19:34:24.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-15 19:34:24.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-15 19:34:24.000000 mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 19:34:24.789255 mypy-boto3-workspaces-thin-client-1.34.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-15 19:34:10.000000 mypy-boto3-workspaces-thin-client-1.34.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:37.069251 mypy-boto3-workspaces-thin-client-1.34.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-10 19:19:37.069251 mypy-boto3-workspaces-thin-client-1.34.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:37.069251 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-04-10 19:19:23.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-04-10 19:19:23.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:37.069251 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-10 19:19:37.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-10 19:19:37.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:37.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:37.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:37.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 19:19:37.000000 mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:37.069251 mypy-boto3-workspaces-thin-client-1.34.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-10 19:19:22.000000 mypy-boto3-workspaces-thin-client-1.34.82/setup.py
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/LICENSE` & `mypy-boto3-workspaces-thin-client-1.34.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/PKG-INFO` & `mypy-boto3-workspaces-thin-client-1.34.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-thin-client
-Version: 1.34.64
-Summary: Type annotations for boto3.WorkSpacesThinClient 1.34.64 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.WorkSpacesThinClient 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-thin-client)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-thin-client)](https://pepy.tech/project/mypy-boto3-workspaces-thin-client)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesThinClient 1.34.64](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
+[boto3.WorkSpacesThinClient 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/README.md` & `mypy-boto3-workspaces-thin-client-1.34.82/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-thin-client)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-thin-client)](https://pepy.tech/project/mypy-boto3-workspaces-thin-client)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesThinClient 1.34.64](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
+[boto3.WorkSpacesThinClient 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/__init__.py` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/__init__.pyi` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/__main__.py` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpacesThinClient 1.34.64\n"
-        "Version:         1.34.64\n"
+        "Type annotations for boto3.WorkSpacesThinClient 1.34.82\n"
+        "Version:         1.34.82\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.64")
+    print("1.34.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/client.py` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -43,35 +43,31 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("WorkSpacesThinClientClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
-    InternalServiceException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class WorkSpacesThinClientClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client/client/)
     """
 
     meta: ClientMeta
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/client.pyi` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,32 +43,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("WorkSpacesThinClientClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
-    InternalServiceException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class WorkSpacesThinClientClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client/client/)
     """
 
     meta: ClientMeta
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/literals.py` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
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
@@ -149,24 +150,26 @@
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

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/literals.pyi` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
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
@@ -149,24 +150,26 @@
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

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/paginator.py` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/paginator.pyi` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/type_defs.py` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
 __all__ = (
     "MaintenanceWindowTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeregisterDeviceRequestRequestTypeDef",
-    "EmbeddedTagTypeDef",
+    "DeviceSummaryTypeDef",
+    "DeviceTypeDef",
     "MaintenanceWindowPaginatorTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetSoftwareSetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
@@ -59,29 +60,27 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "SoftwareTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceRequestRequestTypeDef",
     "UpdateSoftwareSetRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "UpdateEnvironmentRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "DeviceSummaryTypeDef",
-    "DeviceTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTypeDef",
+    "UpdateEnvironmentRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListDevicesResponseTypeDef",
+    "UpdateDeviceResponseTypeDef",
+    "GetDeviceResponseTypeDef",
     "EnvironmentSummaryPaginatorTypeDef",
     "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListSoftwareSetsRequestListSoftwareSetsPaginateTypeDef",
     "ListSoftwareSetsResponseTypeDef",
     "SoftwareSetTypeDef",
-    "ListDevicesResponseTypeDef",
-    "UpdateDeviceResponseTypeDef",
-    "GetDeviceResponseTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponsePaginatorTypeDef",
     "GetSoftwareSetResponseTypeDef",
 )
@@ -126,19 +125,58 @@
     "DeregisterDeviceRequestRequestTypeDef",
     {
         "id": str,
         "targetDeviceStatus": NotRequired[TargetDeviceStatusType],
         "clientToken": NotRequired[str],
     },
 )
-EmbeddedTagTypeDef = TypedDict(
-    "EmbeddedTagTypeDef",
+DeviceSummaryTypeDef = TypedDict(
+    "DeviceSummaryTypeDef",
     {
-        "resourceArn": NotRequired[str],
-        "internalId": NotRequired[str],
+        "id": NotRequired[str],
+        "serialNumber": NotRequired[str],
+        "name": NotRequired[str],
+        "model": NotRequired[str],
+        "environmentId": NotRequired[str],
+        "status": NotRequired[DeviceStatusType],
+        "currentSoftwareSetId": NotRequired[str],
+        "desiredSoftwareSetId": NotRequired[str],
+        "pendingSoftwareSetId": NotRequired[str],
+        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
+        "lastConnectedAt": NotRequired[datetime],
+        "lastPostureAt": NotRequired[datetime],
+        "createdAt": NotRequired[datetime],
+        "updatedAt": NotRequired[datetime],
+        "arn": NotRequired[str],
+    },
+)
+DeviceTypeDef = TypedDict(
+    "DeviceTypeDef",
+    {
+        "id": NotRequired[str],
+        "serialNumber": NotRequired[str],
+        "name": NotRequired[str],
+        "model": NotRequired[str],
+        "environmentId": NotRequired[str],
+        "status": NotRequired[DeviceStatusType],
+        "currentSoftwareSetId": NotRequired[str],
+        "currentSoftwareSetVersion": NotRequired[str],
+        "desiredSoftwareSetId": NotRequired[str],
+        "pendingSoftwareSetId": NotRequired[str],
+        "pendingSoftwareSetVersion": NotRequired[str],
+        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
+        "softwareSetComplianceStatus": NotRequired[DeviceSoftwareSetComplianceStatusType],
+        "softwareSetUpdateStatus": NotRequired[SoftwareSetUpdateStatusType],
+        "lastConnectedAt": NotRequired[datetime],
+        "lastPostureAt": NotRequired[datetime],
+        "createdAt": NotRequired[datetime],
+        "updatedAt": NotRequired[datetime],
+        "arn": NotRequired[str],
+        "kmsKeyArn": NotRequired[str],
+        "tags": NotRequired[Dict[str, str]],
     },
 )
 MaintenanceWindowPaginatorTypeDef = TypedDict(
     "MaintenanceWindowPaginatorTypeDef",
     {
         "type": NotRequired[MaintenanceWindowTypeType],
         "startTimeHour": NotRequired[int],
@@ -261,81 +299,14 @@
         "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
         "desiredSoftwareSetId": NotRequired[str],
         "kmsKeyArn": NotRequired[str],
         "clientToken": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
     },
 )
-UpdateEnvironmentRequestRequestTypeDef = TypedDict(
-    "UpdateEnvironmentRequestRequestTypeDef",
-    {
-        "id": str,
-        "name": NotRequired[str],
-        "desktopArn": NotRequired[str],
-        "desktopEndpoint": NotRequired[str],
-        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
-        "maintenanceWindow": NotRequired[MaintenanceWindowTypeDef],
-        "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
-        "desiredSoftwareSetId": NotRequired[str],
-    },
-)
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DeviceSummaryTypeDef = TypedDict(
-    "DeviceSummaryTypeDef",
-    {
-        "id": NotRequired[str],
-        "serialNumber": NotRequired[str],
-        "name": NotRequired[str],
-        "model": NotRequired[str],
-        "environmentId": NotRequired[str],
-        "status": NotRequired[DeviceStatusType],
-        "currentSoftwareSetId": NotRequired[str],
-        "desiredSoftwareSetId": NotRequired[str],
-        "pendingSoftwareSetId": NotRequired[str],
-        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
-        "lastConnectedAt": NotRequired[datetime],
-        "lastPostureAt": NotRequired[datetime],
-        "createdAt": NotRequired[datetime],
-        "updatedAt": NotRequired[datetime],
-        "arn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
-    },
-)
-DeviceTypeDef = TypedDict(
-    "DeviceTypeDef",
-    {
-        "id": NotRequired[str],
-        "serialNumber": NotRequired[str],
-        "name": NotRequired[str],
-        "model": NotRequired[str],
-        "environmentId": NotRequired[str],
-        "status": NotRequired[DeviceStatusType],
-        "currentSoftwareSetId": NotRequired[str],
-        "currentSoftwareSetVersion": NotRequired[str],
-        "desiredSoftwareSetId": NotRequired[str],
-        "pendingSoftwareSetId": NotRequired[str],
-        "pendingSoftwareSetVersion": NotRequired[str],
-        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
-        "softwareSetComplianceStatus": NotRequired[DeviceSoftwareSetComplianceStatusType],
-        "softwareSetUpdateStatus": NotRequired[SoftwareSetUpdateStatusType],
-        "lastConnectedAt": NotRequired[datetime],
-        "lastPostureAt": NotRequired[datetime],
-        "createdAt": NotRequired[datetime],
-        "updatedAt": NotRequired[datetime],
-        "arn": NotRequired[str],
-        "kmsKeyArn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
-    },
-)
 EnvironmentSummaryTypeDef = TypedDict(
     "EnvironmentSummaryTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
         "desktopArn": NotRequired[str],
         "desktopEndpoint": NotRequired[str],
@@ -345,15 +316,14 @@
         "maintenanceWindow": NotRequired[MaintenanceWindowTypeDef],
         "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
         "desiredSoftwareSetId": NotRequired[str],
         "pendingSoftwareSetId": NotRequired[str],
         "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
         "arn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
     },
 )
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -369,15 +339,57 @@
         "pendingSoftwareSetId": NotRequired[str],
         "pendingSoftwareSetVersion": NotRequired[str],
         "softwareSetComplianceStatus": NotRequired[EnvironmentSoftwareSetComplianceStatusType],
         "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
         "arn": NotRequired[str],
         "kmsKeyArn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
+UpdateEnvironmentRequestRequestTypeDef = TypedDict(
+    "UpdateEnvironmentRequestRequestTypeDef",
+    {
+        "id": str,
+        "name": NotRequired[str],
+        "desktopArn": NotRequired[str],
+        "desktopEndpoint": NotRequired[str],
+        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
+        "maintenanceWindow": NotRequired[MaintenanceWindowTypeDef],
+        "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
+        "desiredSoftwareSetId": NotRequired[str],
+    },
+)
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListDevicesResponseTypeDef = TypedDict(
+    "ListDevicesResponseTypeDef",
+    {
+        "devices": List[DeviceSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateDeviceResponseTypeDef = TypedDict(
+    "UpdateDeviceResponseTypeDef",
+    {
+        "device": DeviceSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "device": DeviceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 EnvironmentSummaryPaginatorTypeDef = TypedDict(
     "EnvironmentSummaryPaginatorTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -389,15 +401,14 @@
         "maintenanceWindow": NotRequired[MaintenanceWindowPaginatorTypeDef],
         "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
         "desiredSoftwareSetId": NotRequired[str],
         "pendingSoftwareSetId": NotRequired[str],
         "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
         "arn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
     },
 )
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
@@ -428,36 +439,15 @@
         "id": NotRequired[str],
         "version": NotRequired[str],
         "releasedAt": NotRequired[datetime],
         "supportedUntil": NotRequired[datetime],
         "validationStatus": NotRequired[SoftwareSetValidationStatusType],
         "software": NotRequired[List[SoftwareTypeDef]],
         "arn": NotRequired[str],
-    },
-)
-ListDevicesResponseTypeDef = TypedDict(
-    "ListDevicesResponseTypeDef",
-    {
-        "devices": List[DeviceSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateDeviceResponseTypeDef = TypedDict(
-    "UpdateDeviceResponseTypeDef",
-    {
-        "device": DeviceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "device": DeviceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": NotRequired[Dict[str, str]],
     },
 )
 CreateEnvironmentResponseTypeDef = TypedDict(
     "CreateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client/type_defs.pyi` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
 __all__ = (
     "MaintenanceWindowTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeregisterDeviceRequestRequestTypeDef",
-    "EmbeddedTagTypeDef",
+    "DeviceSummaryTypeDef",
+    "DeviceTypeDef",
     "MaintenanceWindowPaginatorTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetSoftwareSetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
@@ -59,29 +60,27 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "SoftwareTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceRequestRequestTypeDef",
     "UpdateSoftwareSetRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "UpdateEnvironmentRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "DeviceSummaryTypeDef",
-    "DeviceTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTypeDef",
+    "UpdateEnvironmentRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListDevicesResponseTypeDef",
+    "UpdateDeviceResponseTypeDef",
+    "GetDeviceResponseTypeDef",
     "EnvironmentSummaryPaginatorTypeDef",
     "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListSoftwareSetsRequestListSoftwareSetsPaginateTypeDef",
     "ListSoftwareSetsResponseTypeDef",
     "SoftwareSetTypeDef",
-    "ListDevicesResponseTypeDef",
-    "UpdateDeviceResponseTypeDef",
-    "GetDeviceResponseTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponsePaginatorTypeDef",
     "GetSoftwareSetResponseTypeDef",
 )
@@ -126,19 +125,58 @@
     "DeregisterDeviceRequestRequestTypeDef",
     {
         "id": str,
         "targetDeviceStatus": NotRequired[TargetDeviceStatusType],
         "clientToken": NotRequired[str],
     },
 )
-EmbeddedTagTypeDef = TypedDict(
-    "EmbeddedTagTypeDef",
+DeviceSummaryTypeDef = TypedDict(
+    "DeviceSummaryTypeDef",
     {
-        "resourceArn": NotRequired[str],
-        "internalId": NotRequired[str],
+        "id": NotRequired[str],
+        "serialNumber": NotRequired[str],
+        "name": NotRequired[str],
+        "model": NotRequired[str],
+        "environmentId": NotRequired[str],
+        "status": NotRequired[DeviceStatusType],
+        "currentSoftwareSetId": NotRequired[str],
+        "desiredSoftwareSetId": NotRequired[str],
+        "pendingSoftwareSetId": NotRequired[str],
+        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
+        "lastConnectedAt": NotRequired[datetime],
+        "lastPostureAt": NotRequired[datetime],
+        "createdAt": NotRequired[datetime],
+        "updatedAt": NotRequired[datetime],
+        "arn": NotRequired[str],
+    },
+)
+DeviceTypeDef = TypedDict(
+    "DeviceTypeDef",
+    {
+        "id": NotRequired[str],
+        "serialNumber": NotRequired[str],
+        "name": NotRequired[str],
+        "model": NotRequired[str],
+        "environmentId": NotRequired[str],
+        "status": NotRequired[DeviceStatusType],
+        "currentSoftwareSetId": NotRequired[str],
+        "currentSoftwareSetVersion": NotRequired[str],
+        "desiredSoftwareSetId": NotRequired[str],
+        "pendingSoftwareSetId": NotRequired[str],
+        "pendingSoftwareSetVersion": NotRequired[str],
+        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
+        "softwareSetComplianceStatus": NotRequired[DeviceSoftwareSetComplianceStatusType],
+        "softwareSetUpdateStatus": NotRequired[SoftwareSetUpdateStatusType],
+        "lastConnectedAt": NotRequired[datetime],
+        "lastPostureAt": NotRequired[datetime],
+        "createdAt": NotRequired[datetime],
+        "updatedAt": NotRequired[datetime],
+        "arn": NotRequired[str],
+        "kmsKeyArn": NotRequired[str],
+        "tags": NotRequired[Dict[str, str]],
     },
 )
 MaintenanceWindowPaginatorTypeDef = TypedDict(
     "MaintenanceWindowPaginatorTypeDef",
     {
         "type": NotRequired[MaintenanceWindowTypeType],
         "startTimeHour": NotRequired[int],
@@ -261,81 +299,14 @@
         "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
         "desiredSoftwareSetId": NotRequired[str],
         "kmsKeyArn": NotRequired[str],
         "clientToken": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
     },
 )
-UpdateEnvironmentRequestRequestTypeDef = TypedDict(
-    "UpdateEnvironmentRequestRequestTypeDef",
-    {
-        "id": str,
-        "name": NotRequired[str],
-        "desktopArn": NotRequired[str],
-        "desktopEndpoint": NotRequired[str],
-        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
-        "maintenanceWindow": NotRequired[MaintenanceWindowTypeDef],
-        "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
-        "desiredSoftwareSetId": NotRequired[str],
-    },
-)
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DeviceSummaryTypeDef = TypedDict(
-    "DeviceSummaryTypeDef",
-    {
-        "id": NotRequired[str],
-        "serialNumber": NotRequired[str],
-        "name": NotRequired[str],
-        "model": NotRequired[str],
-        "environmentId": NotRequired[str],
-        "status": NotRequired[DeviceStatusType],
-        "currentSoftwareSetId": NotRequired[str],
-        "desiredSoftwareSetId": NotRequired[str],
-        "pendingSoftwareSetId": NotRequired[str],
-        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
-        "lastConnectedAt": NotRequired[datetime],
-        "lastPostureAt": NotRequired[datetime],
-        "createdAt": NotRequired[datetime],
-        "updatedAt": NotRequired[datetime],
-        "arn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
-    },
-)
-DeviceTypeDef = TypedDict(
-    "DeviceTypeDef",
-    {
-        "id": NotRequired[str],
-        "serialNumber": NotRequired[str],
-        "name": NotRequired[str],
-        "model": NotRequired[str],
-        "environmentId": NotRequired[str],
-        "status": NotRequired[DeviceStatusType],
-        "currentSoftwareSetId": NotRequired[str],
-        "currentSoftwareSetVersion": NotRequired[str],
-        "desiredSoftwareSetId": NotRequired[str],
-        "pendingSoftwareSetId": NotRequired[str],
-        "pendingSoftwareSetVersion": NotRequired[str],
-        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
-        "softwareSetComplianceStatus": NotRequired[DeviceSoftwareSetComplianceStatusType],
-        "softwareSetUpdateStatus": NotRequired[SoftwareSetUpdateStatusType],
-        "lastConnectedAt": NotRequired[datetime],
-        "lastPostureAt": NotRequired[datetime],
-        "createdAt": NotRequired[datetime],
-        "updatedAt": NotRequired[datetime],
-        "arn": NotRequired[str],
-        "kmsKeyArn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
-    },
-)
 EnvironmentSummaryTypeDef = TypedDict(
     "EnvironmentSummaryTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
         "desktopArn": NotRequired[str],
         "desktopEndpoint": NotRequired[str],
@@ -345,15 +316,14 @@
         "maintenanceWindow": NotRequired[MaintenanceWindowTypeDef],
         "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
         "desiredSoftwareSetId": NotRequired[str],
         "pendingSoftwareSetId": NotRequired[str],
         "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
         "arn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
     },
 )
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -369,15 +339,57 @@
         "pendingSoftwareSetId": NotRequired[str],
         "pendingSoftwareSetVersion": NotRequired[str],
         "softwareSetComplianceStatus": NotRequired[EnvironmentSoftwareSetComplianceStatusType],
         "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
         "arn": NotRequired[str],
         "kmsKeyArn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
+UpdateEnvironmentRequestRequestTypeDef = TypedDict(
+    "UpdateEnvironmentRequestRequestTypeDef",
+    {
+        "id": str,
+        "name": NotRequired[str],
+        "desktopArn": NotRequired[str],
+        "desktopEndpoint": NotRequired[str],
+        "softwareSetUpdateSchedule": NotRequired[SoftwareSetUpdateScheduleType],
+        "maintenanceWindow": NotRequired[MaintenanceWindowTypeDef],
+        "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
+        "desiredSoftwareSetId": NotRequired[str],
+    },
+)
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListDevicesResponseTypeDef = TypedDict(
+    "ListDevicesResponseTypeDef",
+    {
+        "devices": List[DeviceSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateDeviceResponseTypeDef = TypedDict(
+    "UpdateDeviceResponseTypeDef",
+    {
+        "device": DeviceSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "device": DeviceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 EnvironmentSummaryPaginatorTypeDef = TypedDict(
     "EnvironmentSummaryPaginatorTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -389,15 +401,14 @@
         "maintenanceWindow": NotRequired[MaintenanceWindowPaginatorTypeDef],
         "softwareSetUpdateMode": NotRequired[SoftwareSetUpdateModeType],
         "desiredSoftwareSetId": NotRequired[str],
         "pendingSoftwareSetId": NotRequired[str],
         "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
         "arn": NotRequired[str],
-        "tags": NotRequired[EmbeddedTagTypeDef],
     },
 )
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
@@ -428,36 +439,15 @@
         "id": NotRequired[str],
         "version": NotRequired[str],
         "releasedAt": NotRequired[datetime],
         "supportedUntil": NotRequired[datetime],
         "validationStatus": NotRequired[SoftwareSetValidationStatusType],
         "software": NotRequired[List[SoftwareTypeDef]],
         "arn": NotRequired[str],
-    },
-)
-ListDevicesResponseTypeDef = TypedDict(
-    "ListDevicesResponseTypeDef",
-    {
-        "devices": List[DeviceSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateDeviceResponseTypeDef = TypedDict(
-    "UpdateDeviceResponseTypeDef",
-    {
-        "device": DeviceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "device": DeviceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": NotRequired[Dict[str, str]],
     },
 )
 CreateEnvironmentResponseTypeDef = TypedDict(
     "CreateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/PKG-INFO` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-thin-client
-Version: 1.34.64
-Summary: Type annotations for boto3.WorkSpacesThinClient 1.34.64 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.WorkSpacesThinClient 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-thin-client.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-thin-client)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_thin_client/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-thin-client)](https://pepy.tech/project/mypy-boto3-workspaces-thin-client)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesThinClient 1.34.64](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
+[boto3.WorkSpacesThinClient 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/mypy_boto3_workspaces_thin_client.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-thin-client-1.34.82/mypy_boto3_workspaces_thin_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-thin-client-1.34.64/setup.py` & `mypy-boto3-workspaces-thin-client-1.34.82/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces-thin-client",
-    version="1.34.64",
+    version="1.34.82",
     packages=["mypy_boto3_workspaces_thin_client"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.WorkSpacesThinClient 1.34.64 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.WorkSpacesThinClient 1.34.82 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

