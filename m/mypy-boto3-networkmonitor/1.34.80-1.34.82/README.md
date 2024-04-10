# Comparing `tmp/mypy-boto3-networkmonitor-1.34.80.tar.gz` & `tmp/mypy-boto3-networkmonitor-1.34.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-networkmonitor-1.34.80.tar", last modified: Mon Apr  8 19:18:12 2024, max compression
+gzip compressed data, was "mypy-boto3-networkmonitor-1.34.82.tar", last modified: Wed Apr 10 19:19:35 2024, max compression
```

## Comparing `mypy-boto3-networkmonitor-1.34.80.tar` & `mypy-boto3-networkmonitor-1.34.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 19:18:12.000000 mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:18:12.725873 mypy-boto3-networkmonitor-1.34.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-08 19:18:01.000000 mypy-boto3-networkmonitor-1.34.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.717250 mypy-boto3-networkmonitor-1.34.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:19:14.000000 mypy-boto3-networkmonitor-1.34.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-10 19:19:35.717250 mypy-boto3-networkmonitor-1.34.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-10 19:19:14.000000 mypy-boto3-networkmonitor-1.34.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.713250 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 19:19:14.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 19:19:14.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:15.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-10 19:19:16.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-10 19:19:16.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:19:14.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:35.713250 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-10 19:19:35.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-10 19:19:35.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:35.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:35.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:19:35.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 19:19:35.000000 mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:35.717250 mypy-boto3-networkmonitor-1.34.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-10 19:19:14.000000 mypy-boto3-networkmonitor-1.34.82/setup.py
```

### Comparing `mypy-boto3-networkmonitor-1.34.80/LICENSE` & `mypy-boto3-networkmonitor-1.34.82/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/PKG-INFO` & `mypy-boto3-networkmonitor-1.34.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-networkmonitor
-Version: 1.34.80
-Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-networkmonitor)](https://pepy.tech/project/mypy-boto3-networkmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchNetworkMonitor 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
+[boto3.CloudWatchNetworkMonitor 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-networkmonitor-1.34.80/README.md` & `mypy-boto3-networkmonitor-1.34.82/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-networkmonitor)](https://pepy.tech/project/mypy-boto3-networkmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchNetworkMonitor 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
+[boto3.CloudWatchNetworkMonitor 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.py` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__init__.pyi` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/__main__.py` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80\n"
-        "Version:         1.34.80\n"
+        "Type annotations for boto3.CloudWatchNetworkMonitor 1.34.82\n"
+        "Version:         1.34.82\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.80")
+    print("1.34.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.py` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client.delete_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/client/#delete_monitor)
         """
 
     def delete_probe(self, *, monitorName: str, probeId: str) -> Dict[str, Any]:
         """
-        Deletes the specified monitor.
+        Deletes the specified probe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client.delete_probe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/client/#delete_probe)
         """
 
     def generate_presigned_url(
         self,
```

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/client.pyi` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client.delete_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/client/#delete_monitor)
         """
 
     def delete_probe(self, *, monitorName: str, probeId: str) -> Dict[str, Any]:
         """
-        Deletes the specified monitor.
+        Deletes the specified probe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client.delete_probe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/client/#delete_probe)
         """
 
     def generate_presigned_url(
         self,
```

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.py` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/literals.pyi` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.py` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/paginator.pyi` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.py` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor/type_defs.pyi` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/PKG-INFO` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-networkmonitor
-Version: 1.34.80
-Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.82
+Summary: Type annotations for boto3.CloudWatchNetworkMonitor 1.34.82 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-networkmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-networkmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_networkmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-networkmonitor)](https://pepy.tech/project/mypy-boto3-networkmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchNetworkMonitor 1.34.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
+[boto3.CloudWatchNetworkMonitor 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-networkmonitor-1.34.80/mypy_boto3_networkmonitor.egg-info/SOURCES.txt` & `mypy-boto3-networkmonitor-1.34.82/mypy_boto3_networkmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-networkmonitor-1.34.80/setup.py` & `mypy-boto3-networkmonitor-1.34.82/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-networkmonitor",
-    version="1.34.80",
+    version="1.34.82",
     packages=["mypy_boto3_networkmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CloudWatchNetworkMonitor 1.34.80 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CloudWatchNetworkMonitor 1.34.82 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

