# Comparing `tmp/mypy-boto3-qconnect-1.34.23.tar.gz` & `tmp/mypy-boto3-qconnect-1.34.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qconnect-1.34.23.tar", last modified: Fri Jan 19 20:47:11 2024, max compression
+gzip compressed data, was "mypy-boto3-qconnect-1.34.82.tar", last modified: Wed Apr 10 19:19:36 2024, max compression
```

## Comparing `mypy-boto3-qconnect-1.34.23.tar` & `mypy-boto3-qconnect-1.34.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 20:47:11.631491 mypy-boto3-qconnect-1.34.23/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-01-19 20:47:11.631491 mypy-boto3-qconnect-1.34.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 20:47:11.631491 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33764 2024-01-19 20:46:59.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33761 2024-01-19 20:46:59.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-01-19 20:46:59.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-01-19 20:46:59.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-01-19 20:46:59.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-01-19 20:46:59.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    48864 2024-01-19 20:47:00.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    48864 2024-01-19 20:47:00.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 20:47:11.631491 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-01-19 20:47:11.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-19 20:47:11.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 20:47:11.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 20:47:11.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-19 20:47:11.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-19 20:47:11.000000 mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 20:47:11.631491 mypy-boto3-qconnect-1.34.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-01-19 20:46:58.000000 mypy-boto3-qconnect-1.34.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.045251 mypy-boto3-qconnect-1.34.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-04-10 19:19:36.045251 mypy-boto3-qconnect-1.34.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.045251 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34396 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34393 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-10 19:19:17.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-10 19:19:17.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    50166 2024-04-10 19:19:17.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50166 2024-04-10 19:19:17.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.045251 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-04-10 19:19:36.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-10 19:19:36.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:36.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:36.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:36.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 19:19:36.000000 mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:36.045251 mypy-boto3-qconnect-1.34.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-10 19:19:16.000000 mypy-boto3-qconnect-1.34.82/setup.py
```

### Comparing `mypy-boto3-qconnect-1.34.23/LICENSE` & `mypy-boto3-qconnect-1.34.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qconnect-1.34.23/PKG-INFO` & `mypy-boto3-qconnect-1.34.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qconnect
-Version: 1.34.23
-Summary: Type annotations for boto3.QConnect 1.34.23 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.82
+Summary: Type annotations for boto3.QConnect 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-qconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qconnect)](https://pepy.tech/project/mypy-boto3-qconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QConnect 1.34.23](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
+[boto3.QConnect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
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
 [mypy-boto3-qconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qconnect-1.34.23/README.md` & `mypy-boto3-qconnect-1.34.82/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-qconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qconnect)](https://pepy.tech/project/mypy-boto3-qconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QConnect 1.34.23](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
+[boto3.QConnect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
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
 [mypy-boto3-qconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/__init__.py` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/__init__.pyi` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/__main__.py` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QConnect 1.34.23\nVersion:         1.34.23\nBuilder version:"
-        " 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.QConnect 1.34.82\n"
+        "Version:         1.34.82\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.23")
+    print("1.34.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/client.py` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,19 @@
     SearchExpressionTypeDef,
     SearchQuickResponsesResponseTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SourceConfigurationTypeDef,
     StartContentUploadResponseTypeDef,
     StartImportJobResponseTypeDef,
+    TagFilterTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
     UpdateQuickResponseResponseTypeDef,
+    UpdateSessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -183,15 +185,15 @@
         clientToken: str = ...,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         tags: Mapping[str, str] = ...,
         title: str = ...,
     ) -> CreateContentResponseTypeDef:
         """
-        Creates Amazon Q content.
+        Creates Amazon Q in Connect content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#create_content)
         """
 
     def create_knowledge_base(
         self,
@@ -225,27 +227,28 @@
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         shortcutKey: str = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateQuickResponseResponseTypeDef:
         """
-        Creates an Amazon Q quick response.
+        Creates an Amazon Q in Connect quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_quick_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#create_quick_response)
         """
 
     def create_session(
         self,
         *,
         assistantId: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
+        tagFilter: TagFilterTypeDef = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#create_session)
@@ -381,15 +384,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#get_quick_response)
         """
 
     def get_recommendations(
         self, *, assistantId: str, sessionId: str, maxResults: int = ..., waitTimeSeconds: int = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
-        Retrieves recommendations for the specified session.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.get_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#get_recommendations)
         """
 
     def get_session(self, *, assistantId: str, sessionId: str) -> GetSessionResponseTypeDef:
         """
@@ -501,15 +504,15 @@
         queryText: str,
         maxResults: int = ...,
         nextToken: str = ...,
         queryCondition: Sequence[QueryConditionTypeDef] = ...,
         sessionId: str = ...,
     ) -> QueryAssistantResponseTypeDef:
         """
-        Performs a manual search against the specified assistant.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.query_assistant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#query_assistant)
         """
 
     def remove_knowledge_base_template_uri(self, *, knowledgeBaseId: str) -> Dict[str, Any]:
         """
@@ -540,15 +543,17 @@
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> SearchQuickResponsesResponseTypeDef:
         """
-        Searches existing Amazon Q quick responses in an Amazon Q knowledge base.
+        Searches existing Amazon Q in Connect quick responses in an Amazon Q in Connect
+        knowledge
+        base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_quick_responses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#search_quick_responses)
         """
 
     def search_sessions(
         self,
@@ -582,15 +587,16 @@
         knowledgeBaseId: str,
         uploadId: str,
         clientToken: str = ...,
         externalSourceConfiguration: ExternalSourceConfigurationTypeDef = ...,
         metadata: Mapping[str, str] = ...,
     ) -> StartImportJobResponseTypeDef:
         """
-        Start an asynchronous job to import Amazon Q resources from an uploaded source
+        Start an asynchronous job to import Amazon Q in Connect resources from an
+        uploaded source
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.start_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#start_import_job)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
@@ -653,20 +659,35 @@
         name: str = ...,
         removeDescription: bool = ...,
         removeGroupingConfiguration: bool = ...,
         removeShortcutKey: bool = ...,
         shortcutKey: str = ...,
     ) -> UpdateQuickResponseResponseTypeDef:
         """
-        Updates an existing Amazon Q quick response.
+        Updates an existing Amazon Q in Connect quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_quick_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#update_quick_response)
         """
 
+    def update_session(
+        self,
+        *,
+        assistantId: str,
+        sessionId: str,
+        description: str = ...,
+        tagFilter: TagFilterTypeDef = ...,
+    ) -> UpdateSessionResponseTypeDef:
+        """
+        Updates a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#update_session)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_assistant_associations"]
     ) -> ListAssistantAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#get_paginator)
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/client.pyi` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,19 @@
     SearchExpressionTypeDef,
     SearchQuickResponsesResponseTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SourceConfigurationTypeDef,
     StartContentUploadResponseTypeDef,
     StartImportJobResponseTypeDef,
+    TagFilterTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
     UpdateQuickResponseResponseTypeDef,
+    UpdateSessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -180,15 +182,15 @@
         clientToken: str = ...,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         tags: Mapping[str, str] = ...,
         title: str = ...,
     ) -> CreateContentResponseTypeDef:
         """
-        Creates Amazon Q content.
+        Creates Amazon Q in Connect content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#create_content)
         """
 
     def create_knowledge_base(
         self,
@@ -222,27 +224,28 @@
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         shortcutKey: str = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateQuickResponseResponseTypeDef:
         """
-        Creates an Amazon Q quick response.
+        Creates an Amazon Q in Connect quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_quick_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#create_quick_response)
         """
 
     def create_session(
         self,
         *,
         assistantId: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
+        tagFilter: TagFilterTypeDef = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.create_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#create_session)
@@ -378,15 +381,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#get_quick_response)
         """
 
     def get_recommendations(
         self, *, assistantId: str, sessionId: str, maxResults: int = ..., waitTimeSeconds: int = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
-        Retrieves recommendations for the specified session.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.get_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#get_recommendations)
         """
 
     def get_session(self, *, assistantId: str, sessionId: str) -> GetSessionResponseTypeDef:
         """
@@ -498,15 +501,15 @@
         queryText: str,
         maxResults: int = ...,
         nextToken: str = ...,
         queryCondition: Sequence[QueryConditionTypeDef] = ...,
         sessionId: str = ...,
     ) -> QueryAssistantResponseTypeDef:
         """
-        Performs a manual search against the specified assistant.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.query_assistant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#query_assistant)
         """
 
     def remove_knowledge_base_template_uri(self, *, knowledgeBaseId: str) -> Dict[str, Any]:
         """
@@ -537,15 +540,17 @@
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> SearchQuickResponsesResponseTypeDef:
         """
-        Searches existing Amazon Q quick responses in an Amazon Q knowledge base.
+        Searches existing Amazon Q in Connect quick responses in an Amazon Q in Connect
+        knowledge
+        base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.search_quick_responses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#search_quick_responses)
         """
 
     def search_sessions(
         self,
@@ -579,15 +584,16 @@
         knowledgeBaseId: str,
         uploadId: str,
         clientToken: str = ...,
         externalSourceConfiguration: ExternalSourceConfigurationTypeDef = ...,
         metadata: Mapping[str, str] = ...,
     ) -> StartImportJobResponseTypeDef:
         """
-        Start an asynchronous job to import Amazon Q resources from an uploaded source
+        Start an asynchronous job to import Amazon Q in Connect resources from an
+        uploaded source
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.start_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#start_import_job)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
@@ -650,20 +656,35 @@
         name: str = ...,
         removeDescription: bool = ...,
         removeGroupingConfiguration: bool = ...,
         removeShortcutKey: bool = ...,
         shortcutKey: str = ...,
     ) -> UpdateQuickResponseResponseTypeDef:
         """
-        Updates an existing Amazon Q quick response.
+        Updates an existing Amazon Q in Connect quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_quick_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#update_quick_response)
         """
 
+    def update_session(
+        self,
+        *,
+        assistantId: str,
+        sessionId: str,
+        description: str = ...,
+        tagFilter: TagFilterTypeDef = ...,
+    ) -> UpdateSessionResponseTypeDef:
+        """
+        Updates a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.update_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#update_session)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_assistant_associations"]
     ) -> ListAssistantAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/client/#get_paginator)
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/literals.py` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
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
@@ -175,14 +176,15 @@
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
@@ -200,14 +202,15 @@
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
@@ -220,24 +223,26 @@
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
@@ -298,15 +303,14 @@
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
@@ -486,14 +490,15 @@
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
@@ -535,9 +540,17 @@
     "list_quick_responses",
     "query_assistant",
     "search_content",
     "search_quick_responses",
     "search_sessions",
 ]
 RegionName = Literal[
-    "ap-northeast-1", "ap-southeast-2", "eu-central-1", "eu-west-2", "us-east-1", "us-west-2"
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-west-2",
 ]
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/literals.pyi` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
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
@@ -175,14 +176,15 @@
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
@@ -200,14 +202,15 @@
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
@@ -220,24 +223,26 @@
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
@@ -298,15 +303,14 @@
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
@@ -486,14 +490,15 @@
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
@@ -535,9 +540,17 @@
     "list_quick_responses",
     "query_assistant",
     "search_content",
     "search_quick_responses",
     "search_sessions",
 ]
 RegionName = Literal[
-    "ap-northeast-1", "ap-southeast-2", "eu-central-1", "eu-west-2", "us-east-1", "us-west-2"
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-west-2",
+    "us-east-1",
+    "us-west-2",
 ]
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/paginator.py` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/paginator.pyi` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/type_defs.py` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "GroupingConfigurationTypeDef",
     "QuickResponseDataProviderTypeDef",
-    "CreateSessionRequestRequestTypeDef",
     "GenerativeReferenceTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteImportJobRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
     "DeleteQuickResponseRequestRequestTypeDef",
@@ -96,14 +95,15 @@
     "ListImportJobsRequestRequestTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListQuickResponsesRequestRequestTypeDef",
     "QuickResponseSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
+    "TagConditionTypeDef",
     "QueryConditionItemTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "QuickResponseContentProviderTypeDef",
     "QuickResponseFilterFieldTypeDef",
     "QuickResponseOrderFieldTypeDef",
     "QuickResponseQueryFieldTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
@@ -141,20 +141,20 @@
     "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListContentsRequestListContentsPaginateTypeDef",
     "ListImportJobsRequestListImportJobsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListQuickResponsesRequestListQuickResponsesPaginateTypeDef",
     "ListQuickResponsesResponseTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
+    "OrConditionTypeDef",
     "QueryConditionTypeDef",
     "RecommendationTriggerDataTypeDef",
     "QuickResponseContentsTypeDef",
     "QuickResponseSearchExpressionTypeDef",
     "SearchSessionsResponseTypeDef",
-    "SessionDataTypeDef",
     "KnowledgeBaseSummaryPaginatorTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
@@ -166,24 +166,23 @@
     "DataSummaryTypeDef",
     "DocumentTypeDef",
     "TextDataTypeDef",
     "SearchContentRequestRequestTypeDef",
     "SearchContentRequestSearchContentPaginateTypeDef",
     "SearchSessionsRequestRequestTypeDef",
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
+    "TagFilterTypeDef",
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "RecommendationTriggerTypeDef",
     "QuickResponseDataTypeDef",
     "QuickResponseSearchResultDataPaginatorTypeDef",
     "QuickResponseSearchResultDataTypeDef",
     "SearchQuickResponsesRequestRequestTypeDef",
     "SearchQuickResponsesRequestSearchQuickResponsesPaginateTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
     "ListKnowledgeBasesResponsePaginatorTypeDef",
     "CreateKnowledgeBaseResponseTypeDef",
     "GetKnowledgeBaseResponseTypeDef",
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "CreateAssistantAssociationResponseTypeDef",
     "GetAssistantAssociationResponseTypeDef",
@@ -191,25 +190,31 @@
     "ImportJobDataTypeDef",
     "ImportJobSummaryTypeDef",
     "StartImportJobRequestRequestTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "ContentDataDetailsTypeDef",
     "SourceContentDataDetailsTypeDef",
+    "CreateSessionRequestRequestTypeDef",
+    "SessionDataTypeDef",
+    "UpdateSessionRequestRequestTypeDef",
     "CreateQuickResponseResponseTypeDef",
     "GetQuickResponseResponseTypeDef",
     "UpdateQuickResponseResponseTypeDef",
     "SearchQuickResponsesResponsePaginatorTypeDef",
     "SearchQuickResponsesResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "StartImportJobResponseTypeDef",
     "ListImportJobsResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
     "DataDetailsTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
+    "UpdateSessionResponseTypeDef",
 )
 
 AppIntegrationsConfigurationPaginatorTypeDef = TypedDict(
     "AppIntegrationsConfigurationPaginatorTypeDef",
     {
         "appIntegrationArn": str,
         "objectFields": NotRequired[List[str]],
@@ -316,18 +321,18 @@
         "tags": NotRequired[Dict[str, str]],
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
 CreateContentRequestRequestTypeDef = TypedDict(
     "CreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
@@ -354,24 +359,14 @@
 )
 QuickResponseDataProviderTypeDef = TypedDict(
     "QuickResponseDataProviderTypeDef",
     {
         "content": NotRequired[str],
     },
 )
-CreateSessionRequestRequestTypeDef = TypedDict(
-    "CreateSessionRequestRequestTypeDef",
-    {
-        "assistantId": str,
-        "name": str,
-        "clientToken": NotRequired[str],
-        "description": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
-    },
-)
 GenerativeReferenceTypeDef = TypedDict(
     "GenerativeReferenceTypeDef",
     {
         "generationId": NotRequired[str],
         "modelId": NotRequired[str],
     },
 )
@@ -590,14 +585,21 @@
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
     },
 )
+TagConditionTypeDef = TypedDict(
+    "TagConditionTypeDef",
+    {
+        "key": str,
+        "value": NotRequired[str],
+    },
+)
 QueryConditionItemTypeDef = TypedDict(
     "QueryConditionItemTypeDef",
     {
         "comparator": Literal["EQUALS"],
         "field": Literal["RESULT_TYPE"],
         "value": str,
     },
@@ -961,14 +963,21 @@
     "NotifyRecommendationsReceivedResponseTypeDef",
     {
         "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
         "recommendationIds": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+OrConditionTypeDef = TypedDict(
+    "OrConditionTypeDef",
+    {
+        "andConditions": NotRequired[Sequence[TagConditionTypeDef]],
+        "tagCondition": NotRequired[TagConditionTypeDef],
+    },
+)
 QueryConditionTypeDef = TypedDict(
     "QueryConditionTypeDef",
     {
         "single": NotRequired[QueryConditionItemTypeDef],
     },
 )
 RecommendationTriggerDataTypeDef = TypedDict(
@@ -996,25 +1005,14 @@
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SessionDataTypeDef = TypedDict(
-    "SessionDataTypeDef",
-    {
-        "name": str,
-        "sessionArn": str,
-        "sessionId": str,
-        "description": NotRequired[str],
-        "integrationConfiguration": NotRequired[SessionIntegrationConfigurationTypeDef],
-        "tags": NotRequired[Dict[str, str]],
-    },
-)
 KnowledgeBaseSummaryPaginatorTypeDef = TypedDict(
     "KnowledgeBaseSummaryPaginatorTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
@@ -1195,14 +1193,22 @@
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+TagFilterTypeDef = TypedDict(
+    "TagFilterTypeDef",
+    {
+        "andConditions": NotRequired[Sequence[TagConditionTypeDef]],
+        "orConditions": NotRequired[Sequence[OrConditionTypeDef]],
+        "tagCondition": NotRequired[TagConditionTypeDef],
+    },
+)
 QueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
         "assistantId": str,
         "queryText": str,
         "queryCondition": NotRequired[Sequence[QueryConditionTypeDef]],
         "sessionId": NotRequired[str],
@@ -1318,28 +1324,14 @@
     {
         "knowledgeBaseId": str,
         "searchExpression": QuickResponseSearchExpressionTypeDef,
         "attributes": NotRequired[Mapping[str, str]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListKnowledgeBasesResponsePaginatorTypeDef = TypedDict(
     "ListKnowledgeBasesResponsePaginatorTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryPaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1472,14 +1464,46 @@
     {
         "id": str,
         "rankingData": RankingDataTypeDef,
         "textData": TextDataTypeDef,
         "type": Literal["KNOWLEDGE_CONTENT"],
     },
 )
+CreateSessionRequestRequestTypeDef = TypedDict(
+    "CreateSessionRequestRequestTypeDef",
+    {
+        "assistantId": str,
+        "name": str,
+        "clientToken": NotRequired[str],
+        "description": NotRequired[str],
+        "tagFilter": NotRequired[TagFilterTypeDef],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+SessionDataTypeDef = TypedDict(
+    "SessionDataTypeDef",
+    {
+        "name": str,
+        "sessionArn": str,
+        "sessionId": str,
+        "description": NotRequired[str],
+        "integrationConfiguration": NotRequired[SessionIntegrationConfigurationTypeDef],
+        "tagFilter": NotRequired[TagFilterTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
+UpdateSessionRequestRequestTypeDef = TypedDict(
+    "UpdateSessionRequestRequestTypeDef",
+    {
+        "assistantId": str,
+        "sessionId": str,
+        "description": NotRequired[str],
+        "tagFilter": NotRequired[TagFilterTypeDef],
+    },
+)
 CreateQuickResponseResponseTypeDef = TypedDict(
     "CreateQuickResponseResponseTypeDef",
     {
         "quickResponse": QuickResponseDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1555,7 +1579,28 @@
     "DataDetailsTypeDef",
     {
         "contentData": NotRequired[ContentDataDetailsTypeDef],
         "generativeData": NotRequired["GenerativeDataDetailsTypeDef"],
         "sourceContentData": NotRequired[SourceContentDataDetailsTypeDef],
     },
 )
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateSessionResponseTypeDef = TypedDict(
+    "UpdateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect/type_defs.pyi` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "GroupingConfigurationTypeDef",
     "QuickResponseDataProviderTypeDef",
-    "CreateSessionRequestRequestTypeDef",
     "GenerativeReferenceTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteImportJobRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
     "DeleteQuickResponseRequestRequestTypeDef",
@@ -96,14 +95,15 @@
     "ListImportJobsRequestRequestTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListQuickResponsesRequestRequestTypeDef",
     "QuickResponseSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
+    "TagConditionTypeDef",
     "QueryConditionItemTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "QuickResponseContentProviderTypeDef",
     "QuickResponseFilterFieldTypeDef",
     "QuickResponseOrderFieldTypeDef",
     "QuickResponseQueryFieldTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
@@ -141,20 +141,20 @@
     "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListContentsRequestListContentsPaginateTypeDef",
     "ListImportJobsRequestListImportJobsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListQuickResponsesRequestListQuickResponsesPaginateTypeDef",
     "ListQuickResponsesResponseTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
+    "OrConditionTypeDef",
     "QueryConditionTypeDef",
     "RecommendationTriggerDataTypeDef",
     "QuickResponseContentsTypeDef",
     "QuickResponseSearchExpressionTypeDef",
     "SearchSessionsResponseTypeDef",
-    "SessionDataTypeDef",
     "KnowledgeBaseSummaryPaginatorTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
@@ -166,24 +166,23 @@
     "DataSummaryTypeDef",
     "DocumentTypeDef",
     "TextDataTypeDef",
     "SearchContentRequestRequestTypeDef",
     "SearchContentRequestSearchContentPaginateTypeDef",
     "SearchSessionsRequestRequestTypeDef",
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
+    "TagFilterTypeDef",
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "RecommendationTriggerTypeDef",
     "QuickResponseDataTypeDef",
     "QuickResponseSearchResultDataPaginatorTypeDef",
     "QuickResponseSearchResultDataTypeDef",
     "SearchQuickResponsesRequestRequestTypeDef",
     "SearchQuickResponsesRequestSearchQuickResponsesPaginateTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
     "ListKnowledgeBasesResponsePaginatorTypeDef",
     "CreateKnowledgeBaseResponseTypeDef",
     "GetKnowledgeBaseResponseTypeDef",
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "CreateAssistantAssociationResponseTypeDef",
     "GetAssistantAssociationResponseTypeDef",
@@ -191,25 +190,31 @@
     "ImportJobDataTypeDef",
     "ImportJobSummaryTypeDef",
     "StartImportJobRequestRequestTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "ContentDataDetailsTypeDef",
     "SourceContentDataDetailsTypeDef",
+    "CreateSessionRequestRequestTypeDef",
+    "SessionDataTypeDef",
+    "UpdateSessionRequestRequestTypeDef",
     "CreateQuickResponseResponseTypeDef",
     "GetQuickResponseResponseTypeDef",
     "UpdateQuickResponseResponseTypeDef",
     "SearchQuickResponsesResponsePaginatorTypeDef",
     "SearchQuickResponsesResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "StartImportJobResponseTypeDef",
     "ListImportJobsResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
     "DataDetailsTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
+    "UpdateSessionResponseTypeDef",
 )
 
 AppIntegrationsConfigurationPaginatorTypeDef = TypedDict(
     "AppIntegrationsConfigurationPaginatorTypeDef",
     {
         "appIntegrationArn": str,
         "objectFields": NotRequired[List[str]],
@@ -316,18 +321,18 @@
         "tags": NotRequired[Dict[str, str]],
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
 CreateContentRequestRequestTypeDef = TypedDict(
     "CreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
@@ -354,24 +359,14 @@
 )
 QuickResponseDataProviderTypeDef = TypedDict(
     "QuickResponseDataProviderTypeDef",
     {
         "content": NotRequired[str],
     },
 )
-CreateSessionRequestRequestTypeDef = TypedDict(
-    "CreateSessionRequestRequestTypeDef",
-    {
-        "assistantId": str,
-        "name": str,
-        "clientToken": NotRequired[str],
-        "description": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
-    },
-)
 GenerativeReferenceTypeDef = TypedDict(
     "GenerativeReferenceTypeDef",
     {
         "generationId": NotRequired[str],
         "modelId": NotRequired[str],
     },
 )
@@ -590,14 +585,21 @@
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
     },
 )
+TagConditionTypeDef = TypedDict(
+    "TagConditionTypeDef",
+    {
+        "key": str,
+        "value": NotRequired[str],
+    },
+)
 QueryConditionItemTypeDef = TypedDict(
     "QueryConditionItemTypeDef",
     {
         "comparator": Literal["EQUALS"],
         "field": Literal["RESULT_TYPE"],
         "value": str,
     },
@@ -961,14 +963,21 @@
     "NotifyRecommendationsReceivedResponseTypeDef",
     {
         "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
         "recommendationIds": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+OrConditionTypeDef = TypedDict(
+    "OrConditionTypeDef",
+    {
+        "andConditions": NotRequired[Sequence[TagConditionTypeDef]],
+        "tagCondition": NotRequired[TagConditionTypeDef],
+    },
+)
 QueryConditionTypeDef = TypedDict(
     "QueryConditionTypeDef",
     {
         "single": NotRequired[QueryConditionItemTypeDef],
     },
 )
 RecommendationTriggerDataTypeDef = TypedDict(
@@ -996,25 +1005,14 @@
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SessionDataTypeDef = TypedDict(
-    "SessionDataTypeDef",
-    {
-        "name": str,
-        "sessionArn": str,
-        "sessionId": str,
-        "description": NotRequired[str],
-        "integrationConfiguration": NotRequired[SessionIntegrationConfigurationTypeDef],
-        "tags": NotRequired[Dict[str, str]],
-    },
-)
 KnowledgeBaseSummaryPaginatorTypeDef = TypedDict(
     "KnowledgeBaseSummaryPaginatorTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
@@ -1195,14 +1193,22 @@
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+TagFilterTypeDef = TypedDict(
+    "TagFilterTypeDef",
+    {
+        "andConditions": NotRequired[Sequence[TagConditionTypeDef]],
+        "orConditions": NotRequired[Sequence[OrConditionTypeDef]],
+        "tagCondition": NotRequired[TagConditionTypeDef],
+    },
+)
 QueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
         "assistantId": str,
         "queryText": str,
         "queryCondition": NotRequired[Sequence[QueryConditionTypeDef]],
         "sessionId": NotRequired[str],
@@ -1318,28 +1324,14 @@
     {
         "knowledgeBaseId": str,
         "searchExpression": QuickResponseSearchExpressionTypeDef,
         "attributes": NotRequired[Mapping[str, str]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListKnowledgeBasesResponsePaginatorTypeDef = TypedDict(
     "ListKnowledgeBasesResponsePaginatorTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryPaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1472,14 +1464,46 @@
     {
         "id": str,
         "rankingData": RankingDataTypeDef,
         "textData": TextDataTypeDef,
         "type": Literal["KNOWLEDGE_CONTENT"],
     },
 )
+CreateSessionRequestRequestTypeDef = TypedDict(
+    "CreateSessionRequestRequestTypeDef",
+    {
+        "assistantId": str,
+        "name": str,
+        "clientToken": NotRequired[str],
+        "description": NotRequired[str],
+        "tagFilter": NotRequired[TagFilterTypeDef],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+SessionDataTypeDef = TypedDict(
+    "SessionDataTypeDef",
+    {
+        "name": str,
+        "sessionArn": str,
+        "sessionId": str,
+        "description": NotRequired[str],
+        "integrationConfiguration": NotRequired[SessionIntegrationConfigurationTypeDef],
+        "tagFilter": NotRequired[TagFilterTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
+UpdateSessionRequestRequestTypeDef = TypedDict(
+    "UpdateSessionRequestRequestTypeDef",
+    {
+        "assistantId": str,
+        "sessionId": str,
+        "description": NotRequired[str],
+        "tagFilter": NotRequired[TagFilterTypeDef],
+    },
+)
 CreateQuickResponseResponseTypeDef = TypedDict(
     "CreateQuickResponseResponseTypeDef",
     {
         "quickResponse": QuickResponseDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1555,7 +1579,28 @@
     "DataDetailsTypeDef",
     {
         "contentData": NotRequired[ContentDataDetailsTypeDef],
         "generativeData": NotRequired["GenerativeDataDetailsTypeDef"],
         "sourceContentData": NotRequired[SourceContentDataDetailsTypeDef],
     },
 )
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateSessionResponseTypeDef = TypedDict(
+    "UpdateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/PKG-INFO` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qconnect
-Version: 1.34.23
-Summary: Type annotations for boto3.QConnect 1.34.23 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.82
+Summary: Type annotations for boto3.QConnect 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-qconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qconnect)](https://pepy.tech/project/mypy-boto3-qconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QConnect 1.34.23](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
+[boto3.QConnect 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
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
 [mypy-boto3-qconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qconnect-1.34.23/mypy_boto3_qconnect.egg-info/SOURCES.txt` & `mypy-boto3-qconnect-1.34.82/mypy_boto3_qconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qconnect-1.34.23/setup.py` & `mypy-boto3-qconnect-1.34.82/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qconnect",
-    version="1.34.23",
+    version="1.34.82",
     packages=["mypy_boto3_qconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.QConnect 1.34.23 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.QConnect 1.34.82 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

