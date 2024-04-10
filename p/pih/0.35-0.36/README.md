# Comparing `tmp/pih-0.35.tar.gz` & `tmp/pih-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.35.tar", last modified: Wed Apr 10 02:46:43 2024, max compression
+gzip compressed data, was "pih-0.36.tar", last modified: Wed Apr 10 04:32:35 2024, max compression
```

## Comparing `pih-0.35.tar` & `pih-0.36.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.949484 pih-0.35/
--rw-rw-rw-   0        0        0      247 2024-04-10 02:46:43.854689 pih-0.35/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:46:39.826676 pih-0.35/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.35/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:46:40.637106 pih-0.35/pih/collections/
--rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.35/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.35/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.35/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.35/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:46:42.905287 pih-0.35/pih/consts/
--rw-rw-rw-   0        0        0    25247 2024-04-10 02:45:39.000000 pih-0.35/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.35/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.35/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.35/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.35/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.35/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.35/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.35/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.35/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.35/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.35/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.35/pih/consts/password.py
--rw-rw-rw-   0        0        0    11367 2024-04-10 02:31:10.000000 pih-0.35/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.35/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.35/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.35/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.35/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.35/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.35/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.35/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.35/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.35/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.35/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   547808 2024-04-10 02:36:34.000000 pih-0.35/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.228216 pih-0.35/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.35/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.35/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.35/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.35/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.744271 pih-0.35/pih/tools/
--rw-rw-rw-   0        0        0    51367 2024-04-09 22:35:48.000000 pih-0.35/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.35/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.35/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:46:43.807811 pih-0.35/pih.egg-info/
--rw-rw-rw-   0        0        0      247 2024-04-10 02:46:37.000000 pih-0.35/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-10 02:46:39.000000 pih-0.35/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:46:38.000000 pih-0.35/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 02:46:38.000000 pih-0.35/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-10 02:46:38.000000 pih-0.35/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:46:43.949484 pih-0.35/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.527765 pih-0.36/
+-rw-rw-rw-   0        0        0      247 2024-04-10 04:32:35.495490 pih-0.36/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 04:32:33.380135 pih-0.36/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:32:33.739010 pih-0.36/pih/collections/
+-rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.073670 pih-0.36/pih/consts/
+-rw-rw-rw-   0        0        0    25247 2024-04-10 04:31:49.000000 pih-0.36/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11367 2024-04-10 03:41:38.000000 pih-0.36/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.36/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   547796 2024-04-10 04:26:59.000000 pih-0.36/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.292564 pih-0.36/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.417371 pih-0.36/pih/tools/
+-rw-rw-rw-   0        0        0    51367 2024-04-09 22:35:48.000000 pih-0.36/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.464239 pih-0.36/pih.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 04:32:35.543491 pih-0.36/setup.cfg
```

### Comparing `pih-0.35/pih/collections/__init__.py` & `pih-0.36/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/collections/service.py` & `pih-0.36/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/console_api.py` & `pih-0.36/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/console_api_wrapper.py` & `pih-0.36/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/__init__.py` & `pih-0.36/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.35"
+VERSION: str = "0.36"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.35/pih/consts/ad.py` & `pih-0.36/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/addresses.py` & `pih-0.36/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/date_time.py` & `pih-0.36/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/errors.py` & `pih-0.36/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/events.py` & `pih-0.36/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/hosts.py` & `pih-0.36/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/names.py` & `pih-0.36/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/password.py` & `pih-0.36/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/paths.py` & `pih-0.36/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/polibase.py` & `pih-0.36/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/service.py` & `pih-0.36/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/service_commands.py` & `pih-0.36/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/service_roles.py` & `pih-0.36/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/consts/settings.py` & `pih-0.36/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/pih.py` & `pih-0.36/pih/pih.py`

 * *Files 1% similar despite different names*

```diff
@@ -942,15 +942,15 @@
         return self.arg_parser.parse_args().__getattribute__(name)
 
     def isolated_arg(self) -> str | None:
         return self.named_arg(CONST.ISOLATED_ARG_NAME)
 
     def add_arg(self, *args, **kwargs) -> bool:
         try:
-            self.arg_parser.add_argument(j((ARGUMENT_PREFIX, args[0])), **kwargs)
+            self.arg_parser.add_argument(j((CONST.ARGUMENT_PREFIX, args[0])), **kwargs)
         except ArgumentError as _:
             return False
         return True
 
     def add_isolated_arg(self) -> bool:
         return self.add_arg(
             CONST.ISOLATED_ARG_NAME,
@@ -1423,15 +1423,15 @@
         self.green(f"Service name: {information.name}")
         with self.make_indent(1):
             if information.standalone:
                 self.magenta("Standalone")
             if information.isolated:
                 self.blue("Isolated")
             self.value("Version", information.version)
-            self.value("Host", PIH.DATA.FORMAT.donain(information.host))
+            self.value("Host", PIH.DATA.FORMAT.domain(information.host))
             self.value("Port", information.port)
             self.value("PID process", information.pid)
 
     def free_marks(
         self,
         show_guest_marks: bool,
         use_index: bool = False,
@@ -2610,15 +2610,15 @@
             code: Any = None,
         ) -> Any:
             return RPC.create_error(context or RPC.context, message, code)
 
         @staticmethod
         def service_host_is_unchangeable(value: str) -> None:
             PIH.output.error(
-                f"Sorry, but service can't be start, cause service host is unchangeble.\n You are trying to start service on {PIH.DATA.FORMAT.donain(PIH.SYS.host())}, but service must be started on {PIH.DATA.FORMAT.donain(value)}"
+                f"Sorry, but service can't be start, cause service host is unchangeble.\n You are trying to start service on {PIH.DATA.FORMAT.domain(PIH.SYS.host())}, but service must be started on {PIH.DATA.FORMAT.domain(value)}"
             )
 
         @staticmethod
         def create_header(details: str) -> str:
             return j(
                 (
                     nl(),
@@ -5568,16 +5568,16 @@
             service_role_or_description: ServiceRoles | ServiceDescriptionBase,
         ) -> str:
             service_description: ServiceDescriptionBase | None = (
                 ServiceRoleTool.service_description(service_role_or_description)
             )
             if isinstance(service_description, ServiceDescription):
                 if ne(service_description.port):
-                    return PIH.DATA.FORMAT.donain(service_description.host)
-            return PIH.DATA.FORMAT.donain(
+                    return PIH.DATA.FORMAT.domain(service_description.host)
+            return PIH.DATA.FORMAT.domain(
                 (
                     PIH.SERVICE.get_information(service_role_or_description)
                     or ServiceDescriptionBase()
                 ).host
                 or service_description.host
             )
 
@@ -7095,36 +7095,36 @@
                                 )  # type: ignore
                             ),
                         )
                     )  # type: ignore
                 )
 
             class BACKUP:
-                CONST.SPLITTER: str = "::"
+                SPLITTER: str = "::"
 
                 @staticmethod
                 def job_full_name(name: str, source: str, destination: str) -> str:
                     return j(
-                        (source, destination, name), PIH.DATA.FORMAT.BACKUP.CONST.SPLITTER
+                        (source, destination, name), PIH.DATA.FORMAT.BACKUP.SPLITTER
                     )
 
                 @staticmethod
                 def job_status_name(name: str, source: str, destination: str) -> str:
                     return j(
                         (
                             "robocopy_job_status",
                             PIH.DATA.FORMAT.BACKUP.job_full_name(
                                 name, source, destination
                             ),
                         ),
-                        PIH.DATA.FORMAT.BACKUP.CONST.SPLITTER,
+                        PIH.DATA.FORMAT.BACKUP.SPLITTER,
                     )
 
             @staticmethod
-            def donain(value: str) -> str:
+            def domain(value: str) -> str:
                 return if_else(
                     value.endswith(AD.DOMAIN_DNS),
                     value,
                     lambda: j((value, AD.DOMAIN_DNS), "."),
                 )
 
             @staticmethod
```

### Comparing `pih-0.35/pih/rpc/__init__.py` & `pih-0.36/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.36/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.36/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/tools/__init__.py` & `pih-0.36/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/tools/service.py` & `pih-0.36/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih/widgets.py` & `pih-0.36/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.35/pih.egg-info/SOURCES.txt` & `pih-0.36/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

