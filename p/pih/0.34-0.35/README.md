# Comparing `tmp/pih-0.34.tar.gz` & `tmp/pih-0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.34.tar", last modified: Wed Apr 10 01:57:22 2024, max compression
+gzip compressed data, was "pih-0.35.tar", last modified: Wed Apr 10 02:46:43 2024, max compression
```

## Comparing `pih-0.34.tar` & `pih-0.35.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.595889 pih-0.34/
--rw-rw-rw-   0        0        0      247 2024-04-10 01:57:22.516696 pih-0.34/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:57:20.337723 pih-0.34/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.34/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:57:20.714803 pih-0.34/pih/collections/
--rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.34/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.34/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.34/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.34/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.084004 pih-0.34/pih/consts/
--rw-rw-rw-   0        0        0    25247 2024-04-10 01:56:44.000000 pih-0.34/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.34/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.34/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.34/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.34/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.34/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.34/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.34/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.34/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.34/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.34/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.34/pih/consts/password.py
--rw-rw-rw-   0        0        0    11359 2024-04-10 01:28:07.000000 pih-0.34/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.34/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.34/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.34/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.34/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.34/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.34/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.34/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.34/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.34/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.34/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   547826 2024-04-09 23:48:44.000000 pih-0.34/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.271491 pih-0.34/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.34/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.34/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.34/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.34/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.381901 pih-0.34/pih/tools/
--rw-rw-rw-   0        0        0    51367 2024-04-09 22:35:48.000000 pih-0.34/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.34/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.34/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:57:22.460022 pih-0.34/pih.egg-info/
--rw-rw-rw-   0        0        0      247 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-10 01:57:19.000000 pih-0.34/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:57:22.595889 pih-0.34/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.949484 pih-0.35/
+-rw-rw-rw-   0        0        0      247 2024-04-10 02:46:43.854689 pih-0.35/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:46:39.826676 pih-0.35/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.35/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:46:40.637106 pih-0.35/pih/collections/
+-rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.35/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.35/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.35/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.35/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:46:42.905287 pih-0.35/pih/consts/
+-rw-rw-rw-   0        0        0    25247 2024-04-10 02:45:39.000000 pih-0.35/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.35/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.35/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.35/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.35/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.35/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.35/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.35/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.35/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.35/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.35/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.35/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11367 2024-04-10 02:31:10.000000 pih-0.35/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.35/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.35/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.35/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.35/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.35/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.35/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.35/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.35/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.35/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.35/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   547808 2024-04-10 02:36:34.000000 pih-0.35/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.228216 pih-0.35/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.35/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.35/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.35/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.35/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.744271 pih-0.35/pih/tools/
+-rw-rw-rw-   0        0        0    51367 2024-04-09 22:35:48.000000 pih-0.35/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.35/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.35/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.807811 pih-0.35/pih.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-04-10 02:46:37.000000 pih-0.35/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-10 02:46:39.000000 pih-0.35/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:46:38.000000 pih-0.35/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 02:46:38.000000 pih-0.35/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-10 02:46:38.000000 pih-0.35/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:46:43.949484 pih-0.35/setup.cfg
```

### Comparing `pih-0.34/pih/collections/__init__.py` & `pih-0.35/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/collections/service.py` & `pih-0.35/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/console_api.py` & `pih-0.35/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/console_api_wrapper.py` & `pih-0.35/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/__init__.py` & `pih-0.35/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.34"
+VERSION: str = "0.35"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.34/pih/consts/ad.py` & `pih-0.35/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/addresses.py` & `pih-0.35/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/date_time.py` & `pih-0.35/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/errors.py` & `pih-0.35/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/events.py` & `pih-0.35/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/hosts.py` & `pih-0.35/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/names.py` & `pih-0.35/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/password.py` & `pih-0.35/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/paths.py` & `pih-0.35/pih/consts/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 class PATH_DATA_STORAGE:
     NAME: str = ".data"
     VALUE: str = os.path.join(PATH_FACADE.VALUE, NAME)
 
 
 class PATH_BUILD:
-    NAME: str = "build"
+    NAME: str = ".build"
     VALUE: str = os.path.join(PATH_FACADE.VALUE, NAME)
 
 
 class PATH_SCAN:
     NAME: str = "scan"
     VALUE: str = os.path.join(AD.PATH_ROOT, NAME)
 
@@ -145,15 +145,15 @@
 
 
 class PATH_SCAN_RESULT:
     NAME: str = "Результат"
     VALUE: str = os.path.join(PATH_SCAN.VALUE, NAME)
 
     @staticmethod
-    def get_path(type: DocumentTypes) -> str:
+    def get_path(type: DocumentTypes) -> str | None:
         if type == DocumentTypes.MEDICAL_DIRECTION:
             return os.path.join(PATH_SCAN_RESULT.VALUE, "Направления")
 
 
 class PATH_WS_816_SCAN:
 
     HOST: str = Hosts.WS816.NAME
```

### Comparing `pih-0.34/pih/consts/polibase.py` & `pih-0.35/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/service.py` & `pih-0.35/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/service_commands.py` & `pih-0.35/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/service_roles.py` & `pih-0.35/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/consts/settings.py` & `pih-0.35/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/pih.py` & `pih-0.35/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -7291,15 +7291,15 @@
                 if reverse:
                     return ListTool.not_empty_items(
                         j(
                             j(value.replace("\\", CONST.SPLITTER)).replace("/", CONST.SPLITTER)
                         ).split(CONST.SPLITTER)
                     )[0]
                 if use_default_domain and not value.endswith(AD.DOMAIN_MAIN):
-                    value = j((value, AD.DOMAIN_MAIN), AD.CONST.SPLITTER)
+                    value = jp((value, AD.DOMAIN_MAIN))
                 return ("" if value.startswith(host_start) else host_start) + value
 
             @staticmethod
             def host_name(value: str) -> str:
                 return value.split(".")[0]
 
             @staticmethod
```

### Comparing `pih-0.34/pih/rpc/__init__.py` & `pih-0.35/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.35/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.35/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/tools/__init__.py` & `pih-0.35/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/tools/service.py` & `pih-0.35/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih/widgets.py` & `pih-0.35/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.34/pih.egg-info/SOURCES.txt` & `pih-0.35/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

