# Comparing `tmp/mypy-boto3-rekognition-1.34.20.tar.gz` & `tmp/mypy-boto3-rekognition-1.34.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.34.20.tar", last modified: Tue Jan 16 20:32:46 2024, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.34.82.tar", last modified: Wed Apr 10 19:19:36 2024, max compression
```

## Comparing `mypy-boto3-rekognition-1.34.20.tar` & `mypy-boto3-rekognition-1.34.82.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.780973 mypy-boto3-rekognition-1.34.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-01-16 20:32:46.780973 mypy-boto3-rekognition-1.34.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.776972 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59371 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    59368 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-01-16 20:32:15.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-01-16 20:32:15.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    90429 2024-01-16 20:32:17.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    90429 2024-01-16 20:32:16.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.776972 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-01-16 20:32:46.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-16 20:32:46.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:46.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:46.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-16 20:32:46.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-16 20:32:46.000000 mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 20:32:46.780973 mypy-boto3-rekognition-1.34.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-16 20:32:14.000000 mypy-boto3-rekognition-1.34.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.385251 mypy-boto3-rekognition-1.34.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-10 19:19:36.385251 mypy-boto3-rekognition-1.34.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.385251 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59371 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59368 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-04-10 19:19:20.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    90505 2024-04-10 19:19:22.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90505 2024-04-10 19:19:21.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:36.385251 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-10 19:19:36.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-10 19:19:36.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:36.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:36.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:36.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 19:19:36.000000 mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:36.385251 mypy-boto3-rekognition-1.34.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-10 19:19:19.000000 mypy-boto3-rekognition-1.34.82/setup.py
```

### Comparing `mypy-boto3-rekognition-1.34.20/LICENSE` & `mypy-boto3-rekognition-1.34.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/PKG-INFO` & `mypy-boto3-rekognition-1.34.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.34.20
-Summary: Type annotations for boto3.Rekognition 1.34.20 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.82
+Summary: Type annotations for boto3.Rekognition 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rekognition-1.34.20/README.md` & `mypy-boto3-rekognition-1.34.82/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/__main__.py` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Rekognition 1.34.20\nVersion:         1.34.20\nBuilder version:"
-        " 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Rekognition 1.34.82\n"
+        "Version:         1.34.82\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.20")
+    print("1.34.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,15 @@
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
@@ -283,14 +284,15 @@
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
@@ -308,14 +310,15 @@
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
@@ -328,24 +331,26 @@
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
@@ -406,15 +411,14 @@
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
@@ -594,14 +598,15 @@
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

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,15 @@
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
@@ -283,14 +284,15 @@
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
@@ -308,14 +310,15 @@
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
@@ -328,24 +331,26 @@
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
@@ -406,15 +411,14 @@
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
@@ -594,14 +598,15 @@
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

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
     "ConnectedHomeSettingsTypeDef",
-    "ModerationLabelTypeDef",
     "ContentTypeTypeDef",
+    "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
@@ -409,18 +409,18 @@
         "FaceId": NotRequired[str],
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
 UnsuccessfulFaceAssociationTypeDef = TypedDict(
     "UnsuccessfulFaceAssociationTypeDef",
     {
         "FaceId": NotRequired[str],
         "UserId": NotRequired[str],
@@ -522,28 +522,28 @@
 ConnectedHomeSettingsTypeDef = TypedDict(
     "ConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
         "MinConfidence": NotRequired[float],
     },
 )
-ModerationLabelTypeDef = TypedDict(
-    "ModerationLabelTypeDef",
+ContentTypeTypeDef = TypedDict(
+    "ContentTypeTypeDef",
     {
         "Confidence": NotRequired[float],
         "Name": NotRequired[str],
-        "ParentName": NotRequired[str],
-        "TaxonomyLevel": NotRequired[int],
     },
 )
-ContentTypeTypeDef = TypedDict(
-    "ContentTypeTypeDef",
+ModerationLabelTypeDef = TypedDict(
+    "ModerationLabelTypeDef",
     {
         "Confidence": NotRequired[float],
         "Name": NotRequired[str],
+        "ParentName": NotRequired[str],
+        "TaxonomyLevel": NotRequired[int],
     },
 )
 OutputConfigTypeDef = TypedDict(
     "OutputConfigTypeDef",
     {
         "S3Bucket": NotRequired[str],
         "S3KeyPrefix": NotRequired[str],
@@ -1635,14 +1635,15 @@
     "ContentModerationDetectionTypeDef",
     {
         "Timestamp": NotRequired[int],
         "ModerationLabel": NotRequired[ModerationLabelTypeDef],
         "StartTimestampMillis": NotRequired[int],
         "EndTimestampMillis": NotRequired[int],
         "DurationMillis": NotRequired[int],
+        "ContentTypes": NotRequired[List[ContentTypeTypeDef]],
     },
 )
 CopyProjectVersionRequestRequestTypeDef = TypedDict(
     "CopyProjectVersionRequestRequestTypeDef",
     {
         "SourceProjectArn": str,
         "SourceProjectVersionArn": str,
```

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
     "ConnectedHomeSettingsTypeDef",
-    "ModerationLabelTypeDef",
     "ContentTypeTypeDef",
+    "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
@@ -409,18 +409,18 @@
         "FaceId": NotRequired[str],
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
 UnsuccessfulFaceAssociationTypeDef = TypedDict(
     "UnsuccessfulFaceAssociationTypeDef",
     {
         "FaceId": NotRequired[str],
         "UserId": NotRequired[str],
@@ -522,28 +522,28 @@
 ConnectedHomeSettingsTypeDef = TypedDict(
     "ConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
         "MinConfidence": NotRequired[float],
     },
 )
-ModerationLabelTypeDef = TypedDict(
-    "ModerationLabelTypeDef",
+ContentTypeTypeDef = TypedDict(
+    "ContentTypeTypeDef",
     {
         "Confidence": NotRequired[float],
         "Name": NotRequired[str],
-        "ParentName": NotRequired[str],
-        "TaxonomyLevel": NotRequired[int],
     },
 )
-ContentTypeTypeDef = TypedDict(
-    "ContentTypeTypeDef",
+ModerationLabelTypeDef = TypedDict(
+    "ModerationLabelTypeDef",
     {
         "Confidence": NotRequired[float],
         "Name": NotRequired[str],
+        "ParentName": NotRequired[str],
+        "TaxonomyLevel": NotRequired[int],
     },
 )
 OutputConfigTypeDef = TypedDict(
     "OutputConfigTypeDef",
     {
         "S3Bucket": NotRequired[str],
         "S3KeyPrefix": NotRequired[str],
@@ -1635,14 +1635,15 @@
     "ContentModerationDetectionTypeDef",
     {
         "Timestamp": NotRequired[int],
         "ModerationLabel": NotRequired[ModerationLabelTypeDef],
         "StartTimestampMillis": NotRequired[int],
         "EndTimestampMillis": NotRequired[int],
         "DurationMillis": NotRequired[int],
+        "ContentTypes": NotRequired[List[ContentTypeTypeDef]],
     },
 )
 CopyProjectVersionRequestRequestTypeDef = TypedDict(
     "CopyProjectVersionRequestRequestTypeDef",
     {
         "SourceProjectArn": str,
         "SourceProjectVersionArn": str,
```

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/PKG-INFO` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.34.20
-Summary: Type annotations for boto3.Rekognition 1.34.20 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.82
+Summary: Type annotations for boto3.Rekognition 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rekognition-1.34.20/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.34.82/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.34.20/setup.py` & `mypy-boto3-rekognition-1.34.82/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.34.20",
+    version="1.34.82",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Rekognition 1.34.20 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.Rekognition 1.34.82 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

