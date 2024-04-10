# Comparing `tmp/pih-0.36.tar.gz` & `tmp/pih-0.36.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.36.tar", last modified: Wed Apr 10 04:32:35 2024, max compression
+gzip compressed data, was "pih-0.36.1.tar", last modified: Wed Apr 10 09:23:31 2024, max compression
```

## Comparing `pih-0.36.tar` & `pih-0.36.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.527765 pih-0.36/
--rw-rw-rw-   0        0        0      247 2024-04-10 04:32:35.495490 pih-0.36/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 04:32:33.380135 pih-0.36/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 04:32:33.739010 pih-0.36/pih/collections/
--rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.073670 pih-0.36/pih/consts/
--rw-rw-rw-   0        0        0    25247 2024-04-10 04:31:49.000000 pih-0.36/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36/pih/consts/password.py
--rw-rw-rw-   0        0        0    11367 2024-04-10 03:41:38.000000 pih-0.36/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.36/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   547796 2024-04-10 04:26:59.000000 pih-0.36/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.292564 pih-0.36/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.417371 pih-0.36/pih/tools/
--rw-rw-rw-   0        0        0    51367 2024-04-09 22:35:48.000000 pih-0.36/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-10 04:32:35.464239 pih-0.36/pih.egg-info/
--rw-rw-rw-   0        0        0      247 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-10 04:32:32.000000 pih-0.36/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 04:32:35.543491 pih-0.36/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.833505 pih-0.36.1/
+-rw-rw-rw-   0        0        0      249 2024-04-10 09:23:31.801938 pih-0.36.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 09:23:29.431079 pih-0.36.1/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.1/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:23:30.057101 pih-0.36.1/pih/collections/
+-rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.1/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.1/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.1/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.1/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.409246 pih-0.36.1/pih/consts/
+-rw-rw-rw-   0        0        0    25249 2024-04-10 09:22:43.000000 pih-0.36.1/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.1/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.1/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.1/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.1/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.1/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36.1/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.1/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.1/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.1/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.1/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.1/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11367 2024-04-10 03:41:38.000000 pih-0.36.1/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.36.1/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.1/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.1/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.1/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.1/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.1/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36.1/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.1/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.1/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.1/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   547912 2024-04-10 06:39:42.000000 pih-0.36.1/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.583170 pih-0.36.1/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.1/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.1/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.1/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.1/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.708192 pih-0.36.1/pih/tools/
+-rw-rw-rw-   0        0        0    51419 2024-04-10 09:08:04.000000 pih-0.36.1/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.1/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.1/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.755064 pih-0.36.1/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 09:23:31.849141 pih-0.36.1/setup.cfg
```

### Comparing `pih-0.36/pih/collections/__init__.py` & `pih-0.36.1/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/collections/service.py` & `pih-0.36.1/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/console_api.py` & `pih-0.36.1/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/console_api_wrapper.py` & `pih-0.36.1/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/__init__.py` & `pih-0.36.1/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.36"
+VERSION: str = "0.36.1"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.36/pih/consts/ad.py` & `pih-0.36.1/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/addresses.py` & `pih-0.36.1/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/date_time.py` & `pih-0.36.1/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/errors.py` & `pih-0.36.1/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/events.py` & `pih-0.36.1/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/hosts.py` & `pih-0.36.1/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/names.py` & `pih-0.36.1/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/password.py` & `pih-0.36.1/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/paths.py` & `pih-0.36.1/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/polibase.py` & `pih-0.36.1/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/service.py` & `pih-0.36.1/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/service_commands.py` & `pih-0.36.1/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/service_roles.py` & `pih-0.36.1/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/consts/settings.py` & `pih-0.36.1/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/pih.py` & `pih-0.36.1/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -4352,15 +4352,15 @@
                         "Предзапись"
                         if value.pin == POLIBASE.PRERECORDING_PIN
                         else value.pin
                     ),
                     value,
                 ),
             )
-            
+
         @staticmethod
         def polibase_person_answered(who: PolibasePerson, answer: str) -> None:
             PIH.EVENT.send(
                 Events.POLIBASE_PERSON_ANSWERED,
                 (
                     who.pin,
                     who.telephoneNumber,
@@ -5109,14 +5109,15 @@
 
             @staticmethod
             def start(
                 service_role_or_description: ServiceRoles | ServiceDescriptionBase,
                 check_if_started: bool = False,
                 ipih_install: bool = True,
                 pih_install: bool = True,
+                package_install: bool = True,
                 show_output: bool = True,
             ) -> bool | None:
                 service_description: ServiceDescription = EnumTool.get(
                     service_role_or_description
                 )
                 host_is_linux: bool | None = None
                 host: str | None = service_description.host
@@ -5178,24 +5179,25 @@
                             host=host,
                             show_output=show_output,
                         )
                     package_name: str = PIH.PATH.FACADE.DITRIBUTIVE.NAME(
                         service_description.standalone_name  # type: ignore
                     )
                     if as_standalone:
-                        version_list: list[str] = PIH.UPDATER.versions(package_name)
-                        if nn(version):
-                            if version not in version_list:
-                                version = one(version_list)
-                        PIH.UPDATER.install_package(
-                            name=package_name,
-                            version=version,
-                            host=host,
-                            show_output=show_output,
-                        )
+                        if package_install:
+                            version_list: list[str] = PIH.UPDATER.versions(package_name)
+                            if nn(version):
+                                if version not in version_list:
+                                    version = one(version_list)
+                            PIH.UPDATER.install_package(
+                                name=package_name,
+                                version=version,
+                                host=host,
+                                show_output=show_output,
+                            )
                     else:
                         PIH.UPDATER.uninstall_package(
                             name=package_name,
                             version=None,
                             host=host,
                             show_output=show_output,
                         )
@@ -5230,24 +5232,26 @@
                                     host_is_linux=host_is_linux,
                                 )
                             else:
                                 file_path = PIH.PATH.join(
                                     service_description.service_path, service_file  # type: ignore
                                 )
                         command_list.append(file_path)
-                        command_list.append(j((CONST.ARGUMENT_PREFIX, CONST.ISOLATED_ARG_NAME)))
+                        command_list.append(
+                            j((CONST.ARGUMENT_PREFIX, CONST.ISOLATED_ARG_NAME))
+                        )
                         command_list.append("0")
                         if ne(parameters):
                             if isinstance(parameters, (list, tuple)):
                                 for parameter_item in parameters:
                                     command_list.append(parameter_item)
                             elif isinstance(parameters, dict):
                                 for parameter_item in parameters:
                                     command_list.append(
-                                        j((ARGUMENT_PREFIX, parameter_item))
+                                        j((CONST.ARGUMENT_PREFIX, parameter_item))
                                     )
                                     command_list.append(parameters[parameter_item])
                             else:
                                 command_list.append(parameter_item)
                         if not host_is_linux or n(host_is_linux):
                             command_list = (
                                 list(
@@ -6141,21 +6145,19 @@
 
             @staticmethod
             def get(
                 name: str | None = None, section: Sections | str | None = None
             ) -> StorageVariableHolder | list[StorageVariableHolder] | None:
                 section = section or PIH.DATA.VARIABLE.Sections.VARIABLE
                 section_name: str | None = EnumTool.get(section)
-                data: strdict | list[strdict] | None = (
-                    PIH.RESULT.DATA_STORAGE.value(
-                        name,
-                        None if n(name) else StorageVariableHolder,
-                        section_name,
-                    ).data
-                )
+                data: strdict | list[strdict] | None = PIH.RESULT.DATA_STORAGE.value(
+                    name,
+                    None if n(name) else StorageVariableHolder,
+                    section_name,
+                ).data
 
                 def convert(
                     value_holder: StorageVariableHolder | None,
                 ) -> StorageVariableHolder | None:
                     if e(value_holder):
                         return value_holder
                     if value_holder.section == EnumTool.get(
@@ -7287,15 +7289,17 @@
                 if n(value):
                     return None
                 value = value.lower()
                 host_start: str = r"\\"
                 if reverse:
                     return ListTool.not_empty_items(
                         j(
-                            j(value.replace("\\", CONST.SPLITTER)).replace("/", CONST.SPLITTER)
+                            j(value.replace("\\", CONST.SPLITTER)).replace(
+                                "/", CONST.SPLITTER
+                            )
                         ).split(CONST.SPLITTER)
                     )[0]
                 if use_default_domain and not value.endswith(AD.DOMAIN_MAIN):
                     value = jp((value, AD.DOMAIN_MAIN))
                 return ("" if value.startswith(host_start) else host_start) + value
 
             @staticmethod
@@ -8408,15 +8412,16 @@
                     if exclude_private_files
                     else result
                 )
 
                 def sort_function(value: File) -> str:
                     title_list: list[str] = lw(value.title).split(CONST.SPLITTER)
                     return j(
-                        [title_list[0]] + [title_list[-1]] + title_list[1:-1], CONST.SPLITTER
+                        [title_list[0]] + [title_list[-1]] + title_list[1:-1],
+                        CONST.SPLITTER,
                     )
 
                 return ResultTool.sort(sort_function, result)
 
             @staticmethod
             def execute(
                 file_search_request: str,
@@ -9074,15 +9079,17 @@
                 )
                 start_date = DateTimeTool.begin_date(start_date or now)
                 end_date = DateTimeTool.end_date(end_date or now)
 
                 def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str:
                     return DataTool.check_not_none(
                         entity,
-                        lambda: entity.TimeVal.split(DATE_TIME.CONST.SPLITTER)[not date],
+                        lambda: entity.TimeVal.split(DATE_TIME.CONST.SPLITTER)[
+                            not date
+                        ],
                     )
 
                 result_data: dict = {}
                 full_name_by_tab_number_map: dict = {}
                 result_data = defaultdict(
                     lambda: defaultdict(lambda: defaultdict(list))
                 )
@@ -9377,19 +9384,15 @@
                 return PIH.RESULT.MARK.temporary_mark_owner(
                     PIH.RESULT.MARK.by_tab_number(value).data
                 )
 
         class POLIBASE:
             @staticmethod
             def _person_pin(value: PolibasePerson | int) -> int:
-                return (
-                    value.pin
-                    if isinstance(value, PolibasePerson)
-                    else value
-                )
+                return value.pin if isinstance(value, PolibasePerson) else value
 
             @staticmethod
             def bonus_information(
                 who: PolibasePerson | int, test: bool | None = None
             ) -> Result[BonusInformation]:
                 result: BonusInformation = BonusInformation()
 
@@ -9652,17 +9655,15 @@
                 if e(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error(
                         "идентификационным номером", value
                     )
                 return result
 
             @staticmethod
-            def execute(
-                query: str, test: bool | None = None
-            ) -> Result[list[strdict]]:
+            def execute(query: str, test: bool | None = None) -> Result[list[strdict]]:
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(
                         ServiceCommands.execute_polibase_query, (query, test)
                     ),
                 )
 
             @staticmethod
@@ -12883,33 +12884,32 @@
                 return PIH.EXECUTOR.start_windows_service(name, computer_name)
 
             @staticmethod
             def stop_windows_service(name: str, computer_name: str) -> bool | None:
                 return PIH.EXECUTOR.stop_windows_service(name, computer_name)
 
         class DOOR:
-            
+
             @staticmethod
             def operation(name: str, operation_name: str) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.door_operation,
                         (name, operation_name),
                     )
                 )
-                
+
             @staticmethod
             def open(name: str) -> bool:
                 return PIH.ACTION.DOOR.operation(name, "open")
-                
+
             @staticmethod
             def close(name: str) -> bool:
                 return PIH.ACTION.DOOR.operation(name, "close")
 
-
         class MARK:
 
             @staticmethod
             def create(
                 full_name: FullName,
                 person_division_id: int,
                 tab_number: str,
@@ -12973,17 +12973,15 @@
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_statistics_chart, (type.name,)
                     )
                 )
 
             @staticmethod
-            def save_xlsx(
-                title: str, result: Result[list[strdict]], path: str
-            ) -> bool:
+            def save_xlsx(title: str, result: Result[list[strdict]], path: str) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.save_xlsx,
                         (title, result.fields.list, result.data, path),
                     )
                 )
 
@@ -13002,15 +13000,17 @@
                 tab_number: str,
                 pc: LoginPasswordPair | None,
                 polibase: LoginPasswordPair | None,
                 email: LoginPasswordPair,
             ) -> bool:
                 locale.setlocale(locale.LC_ALL, "ru_RU")
                 date_now = datetime.now().date()
-                date_now_string = js((date_now.day, calendar.month_name[date_now.month], date_now.year))
+                date_now_string = js(
+                    (date_now.day, calendar.month_name[date_now.month], date_now.year)
+                )
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_user_document,
                         (
                             path,
                             date_now_string,
                             ADDRESSES.SITE_ADDRESS,
```

### Comparing `pih-0.36/pih/rpc/__init__.py` & `pih-0.36.1/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.36.1/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.36.1/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/tools/__init__.py` & `pih-0.36.1/pih/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 
 def nna(value: Any) -> Any:
     return value
 
 def nnd(value: Any) -> dict:
     return value
 
+def nnt(value: T | None) -> T:
+    return value
+
 def nns(value: Any) -> str:
     return value
 
 def nnb(value: Any) -> bytes:
     return value
 
 def nni(value: Any) -> int:
```

### Comparing `pih-0.36/pih/tools/service.py` & `pih-0.36.1/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih/widgets.py` & `pih-0.36.1/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.36/pih.egg-info/SOURCES.txt` & `pih-0.36.1/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

